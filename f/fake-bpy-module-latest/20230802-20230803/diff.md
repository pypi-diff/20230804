# Comparing `tmp/fake-bpy-module-latest-20230802.tar.gz` & `tmp/fake-bpy-module-latest-20230803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230802.tar", last modified: Wed Aug  2 06:26:09 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230803.tar", last modified: Thu Aug  3 06:27:20 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230802.tar` & `fake-bpy-module-latest-20230803.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-08-02 06:23:27.000000 fake-bpy-module-latest-20230802/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-08-02 06:23:22.000000 fake-bpy-module-latest-20230802/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-08-02 06:23:35.000000 fake-bpy-module-latest-20230802/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-08-02 06:23:35.000000 fake-bpy-module-latest-20230802/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-08-02 06:23:36.000000 fake-bpy-module-latest-20230802/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-08-02 06:23:37.000000 fake-bpy-module-latest-20230802/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-02 06:23:35.000000 fake-bpy-module-latest-20230802/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-08-02 06:23:32.000000 fake-bpy-module-latest-20230802/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-02 06:23:37.000000 fake-bpy-module-latest-20230802/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-02 06:23:32.000000 fake-bpy-module-latest-20230802/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-08-02 06:23:35.000000 fake-bpy-module-latest-20230802/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-02 06:23:32.000000 fake-bpy-module-latest-20230802/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-08-02 06:23:37.000000 fake-bpy-module-latest-20230802/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-02 06:23:34.000000 fake-bpy-module-latest-20230802/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_operators/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-08-02 06:23:37.000000 fake-bpy-module-latest-20230802/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-02 06:23:32.000000 fake-bpy-module-latest-20230802/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 06:23:32.000000 fake-bpy-module-latest-20230802/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-08-02 06:23:34.000000 fake-bpy-module-latest-20230802/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-02 06:23:34.000000 fake-bpy-module-latest-20230802/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   100551 2023-08-02 06:23:34.000000 fake-bpy-module-latest-20230802/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-08-02 06:23:39.000000 fake-bpy-module-latest-20230802/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-08-02 06:24:46.000000 fake-bpy-module-latest-20230802/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-02 06:23:39.000000 fake-bpy-module-latest-20230802/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-08-02 06:24:52.000000 fake-bpy-module-latest-20230802/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 06:24:48.000000 fake-bpy-module-latest-20230802/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-08-02 06:24:52.000000 fake-bpy-module-latest-20230802/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-08-02 06:23:55.000000 fake-bpy-module-latest-20230802/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-08-02 06:24:55.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-08-02 06:23:55.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-08-02 06:24:08.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-08-02 06:24:09.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-08-02 06:24:28.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-02 06:24:28.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-08-02 06:24:06.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-08-02 06:24:55.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-02 06:24:45.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-08-02 06:26:04.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-08-02 06:24:10.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-08-02 06:24:49.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-02 06:23:56.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-02 06:24:10.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-08-02 06:24:44.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-02 06:26:01.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-08-02 06:24:28.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-08-02 06:26:01.000000 fake-bpy-module-latest-20230802/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-08-02 06:26:04.000000 fake-bpy-module-latest-20230802/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-08-02 06:24:31.000000 fake-bpy-module-latest-20230802/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-02 06:24:21.000000 fake-bpy-module-latest-20230802/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-08-02 06:24:42.000000 fake-bpy-module-latest-20230802/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-08-02 06:24:45.000000 fake-bpy-module-latest-20230802/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-08-02 06:24:50.000000 fake-bpy-module-latest-20230802/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-08-02 06:26:00.000000 fake-bpy-module-latest-20230802/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-02 06:24:31.000000 fake-bpy-module-latest-20230802/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-08-02 06:24:35.000000 fake-bpy-module-latest-20230802/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-08-02 06:24:10.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-02 06:24:52.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-08-02 06:24:07.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-08-02 06:24:44.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-08-02 06:26:03.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-02 06:24:31.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-02 06:24:08.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-08-02 06:24:21.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-08-02 06:24:46.000000 fake-bpy-module-latest-20230802/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    97011 2023-08-02 06:26:07.000000 fake-bpy-module-latest-20230802/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-08-02 06:24:31.000000 fake-bpy-module-latest-20230802/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-08-02 06:24:30.000000 fake-bpy-module-latest-20230802/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-08-02 06:24:29.000000 fake-bpy-module-latest-20230802/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-02 06:24:15.000000 fake-bpy-module-latest-20230802/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-02 06:24:27.000000 fake-bpy-module-latest-20230802/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-08-02 06:24:20.000000 fake-bpy-module-latest-20230802/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-08-02 06:26:01.000000 fake-bpy-module-latest-20230802/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-08-02 06:24:43.000000 fake-bpy-module-latest-20230802/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-08-02 06:24:48.000000 fake-bpy-module-latest-20230802/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-08-02 06:24:48.000000 fake-bpy-module-latest-20230802/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-08-02 06:24:15.000000 fake-bpy-module-latest-20230802/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-08-02 06:24:44.000000 fake-bpy-module-latest-20230802/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-08-02 06:24:45.000000 fake-bpy-module-latest-20230802/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    79895 2023-08-02 06:23:40.000000 fake-bpy-module-latest-20230802/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-08-02 06:24:54.000000 fake-bpy-module-latest-20230802/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-08-02 06:24:30.000000 fake-bpy-module-latest-20230802/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-08-02 06:24:27.000000 fake-bpy-module-latest-20230802/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-02 06:24:41.000000 fake-bpy-module-latest-20230802/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-02 06:24:50.000000 fake-bpy-module-latest-20230802/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-08-02 06:24:27.000000 fake-bpy-module-latest-20230802/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-08-02 06:24:16.000000 fake-bpy-module-latest-20230802/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-08-02 06:24:45.000000 fake-bpy-module-latest-20230802/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21729 2023-08-02 06:24:21.000000 fake-bpy-module-latest-20230802/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-08-02 06:24:53.000000 fake-bpy-module-latest-20230802/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   212630 2023-08-02 06:24:41.000000 fake-bpy-module-latest-20230802/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   629272 2023-08-02 06:25:59.000000 fake-bpy-module-latest-20230802/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-08-02 06:24:05.000000 fake-bpy-module-latest-20230802/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 06:24:08.000000 fake-bpy-module-latest-20230802/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-08-02 06:23:22.000000 fake-bpy-module-latest-20230802/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-02 06:23:27.000000 fake-bpy-module-latest-20230802/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 06:23:27.000000 fake-bpy-module-latest-20230802/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-08-02 06:23:27.000000 fake-bpy-module-latest-20230802/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-08-02 06:22:48.000000 fake-bpy-module-latest-20230802/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-08-02 06:22:59.000000 fake-bpy-module-latest-20230802/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-02 06:22:52.000000 fake-bpy-module-latest-20230802/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-02 06:23:00.000000 fake-bpy-module-latest-20230802/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-02 06:22:40.000000 fake-bpy-module-latest-20230802/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-08-02 06:23:18.000000 fake-bpy-module-latest-20230802/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-08-02 06:22:58.000000 fake-bpy-module-latest-20230802/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-02 06:22:43.000000 fake-bpy-module-latest-20230802/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70584 2023-08-02 06:23:18.000000 fake-bpy-module-latest-20230802/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 06:22:38.000000 fake-bpy-module-latest-20230802/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-02 06:23:00.000000 fake-bpy-module-latest-20230802/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-08-02 06:22:58.000000 fake-bpy-module-latest-20230802/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-08-02 06:22:57.000000 fake-bpy-module-latest-20230802/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-08-02 06:22:38.000000 fake-bpy-module-latest-20230802/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-08-02 06:22:52.000000 fake-bpy-module-latest-20230802/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-02 06:23:10.000000 fake-bpy-module-latest-20230802/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-08-02 06:22:45.000000 fake-bpy-module-latest-20230802/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-08-02 06:22:57.000000 fake-bpy-module-latest-20230802/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-08-02 06:22:43.000000 fake-bpy-module-latest-20230802/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-08-02 06:23:18.000000 fake-bpy-module-latest-20230802/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-08-02 06:22:43.000000 fake-bpy-module-latest-20230802/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-02 06:22:52.000000 fake-bpy-module-latest-20230802/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-02 06:22:55.000000 fake-bpy-module-latest-20230802/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132562 2023-08-02 06:22:51.000000 fake-bpy-module-latest-20230802/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-08-02 06:22:52.000000 fake-bpy-module-latest-20230802/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-02 06:22:45.000000 fake-bpy-module-latest-20230802/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-02 06:23:10.000000 fake-bpy-module-latest-20230802/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-08-02 06:22:58.000000 fake-bpy-module-latest-20230802/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-02 06:22:57.000000 fake-bpy-module-latest-20230802/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-02 06:22:40.000000 fake-bpy-module-latest-20230802/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-08-02 06:22:41.000000 fake-bpy-module-latest-20230802/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-02 06:23:00.000000 fake-bpy-module-latest-20230802/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   179167 2023-08-02 06:22:35.000000 fake-bpy-module-latest-20230802/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    75894 2023-08-02 06:22:43.000000 fake-bpy-module-latest-20230802/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-08-02 06:23:17.000000 fake-bpy-module-latest-20230802/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-08-02 06:23:10.000000 fake-bpy-module-latest-20230802/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43873 2023-08-02 06:22:45.000000 fake-bpy-module-latest-20230802/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-02 06:23:17.000000 fake-bpy-module-latest-20230802/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-02 06:23:09.000000 fake-bpy-module-latest-20230802/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-08-02 06:23:10.000000 fake-bpy-module-latest-20230802/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    37942 2023-08-02 06:22:48.000000 fake-bpy-module-latest-20230802/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-08-02 06:22:57.000000 fake-bpy-module-latest-20230802/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-08-02 06:23:02.000000 fake-bpy-module-latest-20230802/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-08-02 06:23:17.000000 fake-bpy-module-latest-20230802/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-08-02 06:22:57.000000 fake-bpy-module-latest-20230802/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-08-02 06:22:39.000000 fake-bpy-module-latest-20230802/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-02 06:23:00.000000 fake-bpy-module-latest-20230802/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-08-02 06:22:40.000000 fake-bpy-module-latest-20230802/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    94656 2023-08-02 06:22:54.000000 fake-bpy-module-latest-20230802/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-08-02 06:22:45.000000 fake-bpy-module-latest-20230802/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-02 06:22:52.000000 fake-bpy-module-latest-20230802/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-08-02 06:23:00.000000 fake-bpy-module-latest-20230802/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-02 06:22:46.000000 fake-bpy-module-latest-20230802/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    71993 2023-08-02 06:23:13.000000 fake-bpy-module-latest-20230802/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    57676 2023-08-02 06:22:36.000000 fake-bpy-module-latest-20230802/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-08-02 06:22:45.000000 fake-bpy-module-latest-20230802/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    55663 2023-08-02 06:22:38.000000 fake-bpy-module-latest-20230802/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246235 2023-08-02 06:23:09.000000 fake-bpy-module-latest-20230802/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 06:23:01.000000 fake-bpy-module-latest-20230802/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-08-02 06:23:20.000000 fake-bpy-module-latest-20230802/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3503219 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-08-02 06:22:30.000000 fake-bpy-module-latest-20230802/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-08-02 06:23:26.000000 fake-bpy-module-latest-20230802/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-02 06:23:25.000000 fake-bpy-module-latest-20230802/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-02 06:23:30.000000 fake-bpy-module-latest-20230802/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-08-02 06:26:08.000000 fake-bpy-module-latest-20230802/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86172 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-08-02 06:23:24.000000 fake-bpy-module-latest-20230802/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 06:13:43.000000 fake-bpy-module-latest-20230802/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-02 06:23:38.000000 fake-bpy-module-latest-20230802/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-02 06:26:08.000000 fake-bpy-module-latest-20230802/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 06:26:07.000000 fake-bpy-module-latest-20230802/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 06:26:09.000000 fake-bpy-module-latest-20230802/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-02 06:26:08.000000 fake-bpy-module-latest-20230802/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-02 06:23:31.000000 fake-bpy-module-latest-20230802/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 06:24:39.000000 fake-bpy-module-latest-20230803/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-08-03 06:24:24.000000 fake-bpy-module-latest-20230803/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-08-03 06:24:35.000000 fake-bpy-module-latest-20230803/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-08-03 06:24:39.000000 fake-bpy-module-latest-20230803/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-03 06:24:38.000000 fake-bpy-module-latest-20230803/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-08-03 06:24:36.000000 fake-bpy-module-latest-20230803/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21941 2023-08-03 06:24:35.000000 fake-bpy-module-latest-20230803/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-08-03 06:24:35.000000 fake-bpy-module-latest-20230803/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-03 06:24:35.000000 fake-bpy-module-latest-20230803/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-08-03 06:24:38.000000 fake-bpy-module-latest-20230803/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-08-03 06:24:36.000000 fake-bpy-module-latest-20230803/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-03 06:24:36.000000 fake-bpy-module-latest-20230803/bl_operators/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-08-03 06:24:39.000000 fake-bpy-module-latest-20230803/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-08-03 06:24:35.000000 fake-bpy-module-latest-20230803/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-08-03 06:24:38.000000 fake-bpy-module-latest-20230803/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-08-03 06:24:37.000000 fake-bpy-module-latest-20230803/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100551 2023-08-03 06:24:34.000000 fake-bpy-module-latest-20230803/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-08-03 06:24:57.000000 fake-bpy-module-latest-20230803/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-03 06:24:59.000000 fake-bpy-module-latest-20230803/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-08-03 06:27:17.000000 fake-bpy-module-latest-20230803/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 06:26:55.000000 fake-bpy-module-latest-20230803/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-08-03 06:27:11.000000 fake-bpy-module-latest-20230803/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-08-03 06:26:31.000000 fake-bpy-module-latest-20230803/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-08-03 06:26:53.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-08-03 06:26:51.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-08-03 06:24:57.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-08-03 06:24:53.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-08-03 06:27:11.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-03 06:24:53.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-08-03 06:24:46.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-08-03 06:26:54.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-03 06:26:54.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-08-03 06:25:08.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-08-03 06:24:57.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-08-03 06:25:00.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-03 06:26:52.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-03 06:26:43.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-08-03 06:26:52.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-03 06:24:59.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-08-03 06:25:06.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-08-03 06:24:46.000000 fake-bpy-module-latest-20230803/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-08-03 06:26:55.000000 fake-bpy-module-latest-20230803/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-08-03 06:25:00.000000 fake-bpy-module-latest-20230803/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-08-03 06:27:14.000000 fake-bpy-module-latest-20230803/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-08-03 06:26:50.000000 fake-bpy-module-latest-20230803/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-08-03 06:24:57.000000 fake-bpy-module-latest-20230803/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-08-03 06:26:31.000000 fake-bpy-module-latest-20230803/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-08-03 06:24:59.000000 fake-bpy-module-latest-20230803/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-03 06:27:11.000000 fake-bpy-module-latest-20230803/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-08-03 06:26:48.000000 fake-bpy-module-latest-20230803/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-08-03 06:26:52.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-03 06:27:10.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-08-03 06:27:09.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-08-03 06:24:56.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-03 06:24:57.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-08-03 06:27:14.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-08-03 06:26:33.000000 fake-bpy-module-latest-20230803/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97011 2023-08-03 06:25:08.000000 fake-bpy-module-latest-20230803/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-08-03 06:24:53.000000 fake-bpy-module-latest-20230803/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-08-03 06:26:50.000000 fake-bpy-module-latest-20230803/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-08-03 06:26:51.000000 fake-bpy-module-latest-20230803/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-03 06:25:09.000000 fake-bpy-module-latest-20230803/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-03 06:24:43.000000 fake-bpy-module-latest-20230803/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-08-03 06:26:43.000000 fake-bpy-module-latest-20230803/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-08-03 06:26:50.000000 fake-bpy-module-latest-20230803/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-08-03 06:27:14.000000 fake-bpy-module-latest-20230803/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-08-03 06:26:58.000000 fake-bpy-module-latest-20230803/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-08-03 06:24:43.000000 fake-bpy-module-latest-20230803/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-08-03 06:26:39.000000 fake-bpy-module-latest-20230803/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-08-03 06:26:39.000000 fake-bpy-module-latest-20230803/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-08-03 06:24:45.000000 fake-bpy-module-latest-20230803/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79895 2023-08-03 06:27:11.000000 fake-bpy-module-latest-20230803/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-08-03 06:26:53.000000 fake-bpy-module-latest-20230803/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-08-03 06:26:31.000000 fake-bpy-module-latest-20230803/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-08-03 06:25:06.000000 fake-bpy-module-latest-20230803/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-03 06:27:12.000000 fake-bpy-module-latest-20230803/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-03 06:24:56.000000 fake-bpy-module-latest-20230803/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-08-03 06:27:17.000000 fake-bpy-module-latest-20230803/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-08-03 06:24:46.000000 fake-bpy-module-latest-20230803/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-08-03 06:27:12.000000 fake-bpy-module-latest-20230803/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21729 2023-08-03 06:26:45.000000 fake-bpy-module-latest-20230803/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-08-03 06:26:56.000000 fake-bpy-module-latest-20230803/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212630 2023-08-03 06:24:52.000000 fake-bpy-module-latest-20230803/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   629272 2023-08-03 06:26:15.000000 fake-bpy-module-latest-20230803/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-08-03 06:27:08.000000 fake-bpy-module-latest-20230803/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 06:27:17.000000 fake-bpy-module-latest-20230803/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-08-03 06:24:24.000000 fake-bpy-module-latest-20230803/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-03 06:24:22.000000 fake-bpy-module-latest-20230803/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-03 06:23:29.000000 fake-bpy-module-latest-20230803/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-08-03 06:24:04.000000 fake-bpy-module-latest-20230803/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-08-03 06:23:43.000000 fake-bpy-module-latest-20230803/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25489 2023-08-03 06:23:32.000000 fake-bpy-module-latest-20230803/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-03 06:23:51.000000 fake-bpy-module-latest-20230803/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-03 06:24:00.000000 fake-bpy-module-latest-20230803/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-03 06:24:09.000000 fake-bpy-module-latest-20230803/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-08-03 06:23:30.000000 fake-bpy-module-latest-20230803/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-03 06:24:00.000000 fake-bpy-module-latest-20230803/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70584 2023-08-03 06:23:52.000000 fake-bpy-module-latest-20230803/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 06:23:52.000000 fake-bpy-module-latest-20230803/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-03 06:23:37.000000 fake-bpy-module-latest-20230803/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-08-03 06:23:32.000000 fake-bpy-module-latest-20230803/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-08-03 06:23:31.000000 fake-bpy-module-latest-20230803/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-03 06:23:30.000000 fake-bpy-module-latest-20230803/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-08-03 06:23:32.000000 fake-bpy-module-latest-20230803/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-08-03 06:23:43.000000 fake-bpy-module-latest-20230803/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-08-03 06:23:59.000000 fake-bpy-module-latest-20230803/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-08-03 06:24:00.000000 fake-bpy-module-latest-20230803/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-08-03 06:24:00.000000 fake-bpy-module-latest-20230803/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-08-03 06:24:08.000000 fake-bpy-module-latest-20230803/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-08-03 06:23:53.000000 fake-bpy-module-latest-20230803/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-03 06:23:33.000000 fake-bpy-module-latest-20230803/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132562 2023-08-03 06:24:17.000000 fake-bpy-module-latest-20230803/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-03 06:23:30.000000 fake-bpy-module-latest-20230803/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-08-03 06:24:18.000000 fake-bpy-module-latest-20230803/bpy/ops/grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-03 06:23:50.000000 fake-bpy-module-latest-20230803/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-03 06:23:33.000000 fake-bpy-module-latest-20230803/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-08-03 06:24:09.000000 fake-bpy-module-latest-20230803/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-03 06:23:53.000000 fake-bpy-module-latest-20230803/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-03 06:24:08.000000 fake-bpy-module-latest-20230803/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-03 06:23:52.000000 fake-bpy-module-latest-20230803/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-08-03 06:23:38.000000 fake-bpy-module-latest-20230803/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-03 06:23:38.000000 fake-bpy-module-latest-20230803/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-03 06:23:30.000000 fake-bpy-module-latest-20230803/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179167 2023-08-03 06:24:13.000000 fake-bpy-module-latest-20230803/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-08-03 06:23:37.000000 fake-bpy-module-latest-20230803/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75894 2023-08-03 06:24:03.000000 fake-bpy-module-latest-20230803/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-08-03 06:23:57.000000 fake-bpy-module-latest-20230803/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-08-03 06:24:08.000000 fake-bpy-module-latest-20230803/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43873 2023-08-03 06:23:37.000000 fake-bpy-module-latest-20230803/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-08-03 06:23:38.000000 fake-bpy-module-latest-20230803/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-03 06:24:07.000000 fake-bpy-module-latest-20230803/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-08-03 06:24:01.000000 fake-bpy-module-latest-20230803/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37942 2023-08-03 06:24:00.000000 fake-bpy-module-latest-20230803/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-08-03 06:23:53.000000 fake-bpy-module-latest-20230803/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-08-03 06:24:01.000000 fake-bpy-module-latest-20230803/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-03 06:24:05.000000 fake-bpy-module-latest-20230803/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-08-03 06:23:32.000000 fake-bpy-module-latest-20230803/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-03 06:24:05.000000 fake-bpy-module-latest-20230803/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-08-03 06:23:42.000000 fake-bpy-module-latest-20230803/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-08-03 06:23:33.000000 fake-bpy-module-latest-20230803/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-03 06:24:08.000000 fake-bpy-module-latest-20230803/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-08-03 06:24:05.000000 fake-bpy-module-latest-20230803/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-03 06:23:29.000000 fake-bpy-module-latest-20230803/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94656 2023-08-03 06:23:41.000000 fake-bpy-module-latest-20230803/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-08-03 06:23:38.000000 fake-bpy-module-latest-20230803/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-08-03 06:23:40.000000 fake-bpy-module-latest-20230803/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-03 06:23:32.000000 fake-bpy-module-latest-20230803/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-08-03 06:24:14.000000 fake-bpy-module-latest-20230803/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-03 06:24:18.000000 fake-bpy-module-latest-20230803/bpy/ops/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 06:23:42.000000 fake-bpy-module-latest-20230803/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71993 2023-08-03 06:24:20.000000 fake-bpy-module-latest-20230803/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-08-03 06:24:09.000000 fake-bpy-module-latest-20230803/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57676 2023-08-03 06:24:07.000000 fake-bpy-module-latest-20230803/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-08-03 06:23:42.000000 fake-bpy-module-latest-20230803/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55663 2023-08-03 06:24:15.000000 fake-bpy-module-latest-20230803/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246235 2023-08-03 06:23:50.000000 fake-bpy-module-latest-20230803/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-08-03 06:23:33.000000 fake-bpy-module-latest-20230803/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-03 06:23:39.000000 fake-bpy-module-latest-20230803/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-08-03 06:24:22.000000 fake-bpy-module-latest-20230803/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-08-03 06:24:22.000000 fake-bpy-module-latest-20230803/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3503219 2023-08-03 06:23:29.000000 fake-bpy-module-latest-20230803/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-08-03 06:24:21.000000 fake-bpy-module-latest-20230803/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-03 06:24:27.000000 fake-bpy-module-latest-20230803/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-08-03 06:24:28.000000 fake-bpy-module-latest-20230803/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-08-03 06:24:27.000000 fake-bpy-module-latest-20230803/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86172 2023-08-03 06:24:25.000000 fake-bpy-module-latest-20230803/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-08-03 06:24:25.000000 fake-bpy-module-latest-20230803/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-03 06:24:26.000000 fake-bpy-module-latest-20230803/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 06:24:25.000000 fake-bpy-module-latest-20230803/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-03 06:24:25.000000 fake-bpy-module-latest-20230803/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-08-03 06:24:25.000000 fake-bpy-module-latest-20230803/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:14:10.000000 fake-bpy-module-latest-20230803/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-03 06:24:42.000000 fake-bpy-module-latest-20230803/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-03 06:27:18.000000 fake-bpy-module-latest-20230803/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 06:24:39.000000 fake-bpy-module-latest-20230803/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-03 06:24:31.000000 fake-bpy-module-latest-20230803/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:27:20.000000 fake-bpy-module-latest-20230803/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-03 06:27:19.000000 fake-bpy-module-latest-20230803/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 06:24:41.000000 fake-bpy-module-latest-20230803/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230802/PKG-INFO` & `fake-bpy-module-latest-20230803/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230802
+Version: 20230803
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230802/README.rst` & `fake-bpy-module-latest-20230803/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/addon_utils.py` & `fake-bpy-module-latest-20230803/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/animsys_refactor.py` & `fake-bpy-module-latest-20230803/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/aud.py` & `fake-bpy-module-latest-20230803/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bgl.py` & `fake-bpy-module-latest-20230803/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230803/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230803/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230803/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230803/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230803/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_math.py` & `fake-bpy-module-latest-20230803/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/__init__.py` & `fake-bpy-module-latest-20230803/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
 import typing
+from . import vertexpaint_dirt
+from . import wm
+from . import screen_play_rendered_anim
+from . import anim
+from . import sequencer
+from . import mesh
+from . import constraint
+from . import uvcalc_lightmap
+from . import add_mesh_torus
+from . import object
+from . import uvcalc_follow_active
+from . import node
 from . import assets
-from . import freestyle
+from . import object_randomize_transform
+from . import geometry_nodes
+from . import rigidbody
 from . import text
-from . import file
+from . import clip
+from . import object_quick_effects
+from . import freestyle
 from . import object_align
-from . import rigidbody
 from . import bmesh
-from . import node
-from . import object_randomize_transform
-from . import uvcalc_follow_active
-from . import screen_play_rendered_anim
-from . import uvcalc_lightmap
-from . import wm
-from . import vertexpaint_dirt
+from . import image
 from . import spreadsheet
-from . import uvcalc_transform
+from . import view3d
 from . import presets
-from . import mesh
-from . import anim
-from . import clip
-from . import geometry_nodes
+from . import uvcalc_transform
+from . import file
 from . import userpref
-from . import object_quick_effects
-from . import image
-from . import sequencer
-from . import constraint
 from . import console
-from . import add_mesh_torus
-from . import view3d
-from . import object
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230802/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230803/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/anim.py` & `fake-bpy-module-latest-20230803/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/assets.py` & `fake-bpy-module-latest-20230803/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230803/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/clip.py` & `fake-bpy-module-latest-20230803/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/console.py` & `fake-bpy-module-latest-20230803/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/constraint.py` & `fake-bpy-module-latest-20230803/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/file.py` & `fake-bpy-module-latest-20230803/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230803/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230803/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/image.py` & `fake-bpy-module-latest-20230803/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/mesh.py` & `fake-bpy-module-latest-20230803/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/node.py` & `fake-bpy-module-latest-20230803/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/object.py` & `fake-bpy-module-latest-20230803/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/object_align.py` & `fake-bpy-module-latest-20230803/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230803/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230803/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/presets.py` & `fake-bpy-module-latest-20230803/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230803/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230803/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230803/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230803/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/text.py` & `fake-bpy-module-latest-20230803/bl_operators/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/userpref.py` & `fake-bpy-module-latest-20230803/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230803/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230803/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230803/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230803/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/view3d.py` & `fake-bpy-module-latest-20230803/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_operators/wm.py` & `fake-bpy-module-latest-20230803/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230803/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/__init__.py` & `fake-bpy-module-latest-20230803/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 import sys
 import typing
 import bpy_types
 
-from . import node_add_menu
-from . import space_node
-from . import properties_constraint
-from . import properties_data_bone
-from . import properties_data_metaball
-from . import space_view3d_toolbar
+from . import properties_physics_field
+from . import space_graph
+from . import properties_world
+from . import space_nla
 from . import properties_data_gpencil
-from . import properties_physics_dynamicpaint
-from . import properties_physics_rigidbody
-from . import properties_data_camera
-from . import utils
+from . import properties_data_volume
+from . import space_time
+from . import space_userpref
 from . import properties_data_curve
-from . import properties_physics_cloth
-from . import properties_data_modifier
+from . import properties_scene
+from . import properties_data_empty
+from . import properties_physics_fluid
+from . import space_statusbar
+from . import properties_data_camera
+from . import generic_ui_list
+from . import properties_physics_geometry_nodes
+from . import properties_material_gpencil
 from . import properties_data_lightprobe
-from . import space_image
-from . import properties_workspace
-from . import space_time
-from . import space_clip
-from . import properties_physics_rigidbody_constraint
-from . import properties_mask_common
-from . import space_toolsystem_toolbar
+from . import properties_output
+from . import node_add_menu
+from . import properties_data_shaderfx
+from . import properties_data_mesh
+from . import properties_grease_pencil_common
 from . import space_sequencer
-from . import space_text
-from . import properties_world
-from . import properties_data_curves
-from . import properties_data_empty
 from . import properties_data_speaker
-from . import properties_view_layer
-from . import properties_texture
+from . import properties_render
+from . import properties_data_light
+from . import properties_workspace
+from . import space_view3d
+from . import properties_constraint
 from . import space_properties
-from . import properties_scene
-from . import properties_physics_geometry_nodes
-from . import properties_grease_pencil_common
-from . import properties_paint_common
+from . import properties_object
+from . import properties_physics_softbody
+from . import space_image
+from . import space_info
+from . import space_clip
+from . import properties_data_modifier
+from . import space_toolsystem_toolbar
 from . import properties_particle
-from . import space_userpref
-from . import space_spreadsheet
+from . import properties_texture
 from . import properties_material
-from . import space_dopesheet
-from . import space_info
+from . import space_console
+from . import properties_data_bone
+from . import properties_view_layer
+from . import properties_physics_cloth
+from . import properties_data_metaball
 from . import properties_data_pointcloud
-from . import properties_physics_field
-from . import space_nla
-from . import properties_material_gpencil
-from . import space_toolsystem_common
-from . import properties_data_lattice
-from . import properties_physics_softbody
-from . import generic_ui_list
-from . import space_filebrowser
-from . import properties_animviz
-from . import space_graph
-from . import properties_data_mesh
-from . import properties_object
-from . import space_statusbar
-from . import node_add_menu_geometry
-from . import properties_collection
-from . import properties_physics_common
-from . import space_topbar
 from . import space_outliner
-from . import properties_data_grease_pencil
 from . import properties_data_armature
-from . import space_view3d
-from . import properties_output
-from . import properties_data_volume
-from . import space_console
-from . import properties_data_shaderfx
-from . import properties_physics_fluid
+from . import properties_data_lattice
+from . import properties_data_grease_pencil
 from . import properties_freestyle
-from . import properties_data_light
-from . import properties_render
+from . import properties_animviz
+from . import space_topbar
+from . import space_filebrowser
+from . import space_view3d_toolbar
+from . import properties_physics_dynamicpaint
+from . import properties_physics_common
+from . import space_node
+from . import properties_data_curves
+from . import properties_paint_common
+from . import properties_collection
+from . import space_toolsystem_common
+from . import space_spreadsheet
+from . import space_dopesheet
+from . import properties_physics_rigidbody
+from . import properties_mask_common
+from . import node_add_menu_geometry
+from . import space_text
+from . import utils
+from . import properties_physics_rigidbody_constraint
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230802/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230803/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230803/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_grease_pencil.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230803/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230803/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_console.py` & `fake-bpy-module-latest-20230803/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230803/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230803/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230803/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_image.py` & `fake-bpy-module-latest-20230803/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_info.py` & `fake-bpy-module-latest-20230803/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230803/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_node.py` & `fake-bpy-module-latest-20230803/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230803/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230803/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230803/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230803/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230803/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_text.py` & `fake-bpy-module-latest-20230803/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_time.py` & `fake-bpy-module-latest-20230803/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230803/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230803/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230803/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230803/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230803/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230803/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bl_ui/utils.py` & `fake-bpy-module-latest-20230803/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/blf.py` & `fake-bpy-module-latest-20230803/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bmesh/__init__.py` & `fake-bpy-module-latest-20230803/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bmesh/geometry.py` & `fake-bpy-module-latest-20230803/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bmesh/ops.py` & `fake-bpy-module-latest-20230803/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bmesh/types.py` & `fake-bpy-module-latest-20230803/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bmesh/utils.py` & `fake-bpy-module-latest-20230803/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/app/__init__.py` & `fake-bpy-module-latest-20230803/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import typing
-from . import translations
 from . import timers
+from . import translations
 from . import handlers
 from . import icons
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def help_text(all: typing.Optional[bool] = False):
```

### Comparing `fake-bpy-module-latest-20230802/bpy/app/handlers.py` & `fake-bpy-module-latest-20230803/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/app/icons.py` & `fake-bpy-module-latest-20230803/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/app/timers.py` & `fake-bpy-module-latest-20230803/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/app/translations.py` & `fake-bpy-module-latest-20230803/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/msgbus.py` & `fake-bpy-module-latest-20230803/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230803/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
-from . import import_curve
-from . import mesh
-from . import uv
-from . import view3d
+from . import sculpt_curves
+from . import graph
+from . import mball
+from . import curves
+from . import cachefile
 from . import curve
-from . import cloth
+from . import armature
+from . import surface
+from . import constraint
+from . import render
+from . import cycles
+from . import import_curve
 from . import screen
-from . import sculpt
-from . import lattice
-from . import brush
-from . import mask
-from . import node
-from . import font
-from . import camera
-from . import file
+from . import workspace
+from . import gizmogroup
 from . import paint
+from . import collection
+from . import nla
 from . import sound
-from . import view2d
-from . import ed
-from . import import_anim
+from . import mask
+from . import paintcurve
+from . import material
 from . import export_mesh
+from . import world
+from . import uilist
+from . import dpaint
+from . import export_anim
+from . import buttons
+from . import console
+from . import spreadsheet
+from . import sequencer
+from . import scene
+from . import view2d
 from . import texture
-from . import marker
-from . import rigidbody
-from . import text_editor
-from . import ptcache
-from . import nla
-from . import pose
 from . import anim
-from . import gpencil
-from . import image
-from . import cycles
+from . import ed
+from . import wm
+from . import import_anim
 from . import asset
+from . import clip
+from . import cloth
+from . import marker
+from . import info
+from . import poselib
 from . import geometry
-from . import surface
-from . import sequencer
-from . import gizmogroup
+from . import object
 from . import export_scene
-from . import constraint
-from . import poselib
-from . import scene
-from . import info
-from . import console
-from . import cachefile
-from . import import_scene
-from . import armature
-from . import collection
+from . import pose
+from . import fluid
 from . import boid
-from . import mball
-from . import script
-from . import text
-from . import ui
-from . import workspace
-from . import material
-from . import curves
-from . import spreadsheet
-from . import sculpt_curves
-from . import world
-from . import uilist
-from . import grease_pencil
+from . import file
+from . import camera
 from . import preferences
-from . import wm
-from . import palette
 from . import particle
+from . import node
+from . import action
+from . import sculpt
+from . import rigidbody
+from . import ptcache
+from . import uv
+from . import palette
 from . import outliner
-from . import import_mesh
-from . import dpaint
+from . import lattice
+from . import font
+from . import script
+from . import import_scene
+from . import brush
+from . import ui
+from . import mesh
+from . import text
+from . import view3d
+from . import gpencil
+from . import grease_pencil
+from . import text_editor
 from . import transform
-from . import object
-from . import render
-from . import paintcurve
-from . import clip
-from . import buttons
-from . import fluid
-from . import graph
-from . import export_anim
-from . import action
+from . import image
+from . import import_mesh
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/action.py` & `fake-bpy-module-latest-20230803/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/anim.py` & `fake-bpy-module-latest-20230803/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/armature.py` & `fake-bpy-module-latest-20230803/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/asset.py` & `fake-bpy-module-latest-20230803/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/boid.py` & `fake-bpy-module-latest-20230803/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/brush.py` & `fake-bpy-module-latest-20230803/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230803/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230803/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/camera.py` & `fake-bpy-module-latest-20230803/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/clip.py` & `fake-bpy-module-latest-20230803/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230803/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/collection.py` & `fake-bpy-module-latest-20230803/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/console.py` & `fake-bpy-module-latest-20230803/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230803/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/curve.py` & `fake-bpy-module-latest-20230803/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/curves.py` & `fake-bpy-module-latest-20230803/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230803/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230803/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/ed.py` & `fake-bpy-module-latest-20230803/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230803/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230803/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230803/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/file.py` & `fake-bpy-module-latest-20230803/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230803/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/font.py` & `fake-bpy-module-latest-20230803/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230803/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230803/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230803/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/graph.py` & `fake-bpy-module-latest-20230803/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/grease_pencil.py` & `fake-bpy-module-latest-20230803/bpy/ops/grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/image.py` & `fake-bpy-module-latest-20230803/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230803/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230803/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230803/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230803/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/info.py` & `fake-bpy-module-latest-20230803/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230803/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/marker.py` & `fake-bpy-module-latest-20230803/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/mask.py` & `fake-bpy-module-latest-20230803/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/material.py` & `fake-bpy-module-latest-20230803/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/mball.py` & `fake-bpy-module-latest-20230803/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230803/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/nla.py` & `fake-bpy-module-latest-20230803/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/node.py` & `fake-bpy-module-latest-20230803/bpy/ops/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1003,30 +1003,30 @@
 
 
 def new_geometry_node_group_assign(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:239 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L239>`__
+    ''' Create a new geometry node group and assign it to the active modifier :File: `startup/bl_operators/geometry_nodes.py\:245 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L245>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
 
 
 def new_geometry_nodes_modifier(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:216 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L216>`__
+    ''' Create a new modifier with a new geometry node group :File: `startup/bl_operators/geometry_nodes.py\:222 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L222>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1260,15 +1260,15 @@
     pass
 
 
 def repeat_zone_item_add(override_context: typing.
                          Union[typing.Dict, 'bpy.types.Context'] = None,
                          execution_context: typing.Union[str, int] = None,
                          undo: typing.Optional[bool] = None):
-    ''' Add a repeat item to the repeat zone :File: `startup/bl_operators/geometry_nodes.py\:388 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L388>`__
+    ''' Add a repeat item to the repeat zone :File: `startup/bl_operators/geometry_nodes.py\:394 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L394>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1276,15 +1276,15 @@
 
 def repeat_zone_item_move(override_context: typing.
                           Union[typing.Dict, 'bpy.types.Context'] = None,
                           execution_context: typing.Union[str, int] = None,
                           undo: typing.Optional[bool] = None,
                           *,
                           direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move a repeat item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:438 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L438>`__
+    ''' Move a repeat item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:444 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L444>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Direction
     :type direction: typing.Optional[typing.Any]
     '''
@@ -1292,15 +1292,15 @@
     pass
 
 
 def repeat_zone_item_remove(override_context: typing.
                             Union[typing.Dict, 'bpy.types.Context'] = None,
                             execution_context: typing.Union[str, int] = None,
                             undo: typing.Optional[bool] = None):
-    ''' Remove a repeat item from the repeat zone :File: `startup/bl_operators/geometry_nodes.py\:415 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L415>`__
+    ''' Remove a repeat item from the repeat zone :File: `startup/bl_operators/geometry_nodes.py\:421 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L421>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1571,15 +1571,15 @@
     pass
 
 
 def simulation_zone_item_add(override_context: typing.
                              Union[typing.Dict, 'bpy.types.Context'] = None,
                              execution_context: typing.Union[str, int] = None,
                              undo: typing.Optional[bool] = None):
-    ''' Add a state item to the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:289 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L289>`__
+    ''' Add a state item to the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:295 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L295>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
@@ -1587,15 +1587,15 @@
 
 def simulation_zone_item_move(override_context: typing.
                               Union[typing.Dict, 'bpy.types.Context'] = None,
                               execution_context: typing.Union[str, int] = None,
                               undo: typing.Optional[bool] = None,
                               *,
                               direction: typing.Optional[typing.Any] = 'UP'):
-    ''' Move a simulation state item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:339 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L339>`__
+    ''' Move a simulation state item up or down in the list :File: `startup/bl_operators/geometry_nodes.py\:345 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L345>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     :param direction: Direction
     :type direction: typing.Optional[typing.Any]
     '''
@@ -1604,15 +1604,15 @@
 
 
 def simulation_zone_item_remove(
         override_context: typing.Union[typing.
                                        Dict, 'bpy.types.Context'] = None,
         execution_context: typing.Union[str, int] = None,
         undo: typing.Optional[bool] = None):
-    ''' Remove a state item from the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:316 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L316>`__
+    ''' Remove a state item from the simulation zone :File: `startup/bl_operators/geometry_nodes.py\:322 <https://projects.blender.org/blender/blender/src/branch/main/scripts/startup/bl_operators/geometry_nodes.py#L322>`__
 
     :type override_context: typing.Union[typing.Dict, 'bpy.types.Context']
     :type execution_context: typing.Union[str, int]
     :type undo: typing.Optional[bool]
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/object.py` & `fake-bpy-module-latest-20230803/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230803/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/paint.py` & `fake-bpy-module-latest-20230803/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230803/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/palette.py` & `fake-bpy-module-latest-20230803/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/particle.py` & `fake-bpy-module-latest-20230803/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/pose.py` & `fake-bpy-module-latest-20230803/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230803/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230803/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230803/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/render.py` & `fake-bpy-module-latest-20230803/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230803/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/scene.py` & `fake-bpy-module-latest-20230803/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/screen.py` & `fake-bpy-module-latest-20230803/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/script.py` & `fake-bpy-module-latest-20230803/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230803/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230803/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230803/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/sound.py` & `fake-bpy-module-latest-20230803/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230803/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/surface.py` & `fake-bpy-module-latest-20230803/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/text.py` & `fake-bpy-module-latest-20230803/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/text_editor.py` & `fake-bpy-module-latest-20230803/bpy/ops/text_editor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/texture.py` & `fake-bpy-module-latest-20230803/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/transform.py` & `fake-bpy-module-latest-20230803/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/ui.py` & `fake-bpy-module-latest-20230803/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230803/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/uv.py` & `fake-bpy-module-latest-20230803/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230803/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230803/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/wm.py` & `fake-bpy-module-latest-20230803/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230803/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/ops/world.py` & `fake-bpy-module-latest-20230803/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/path.py` & `fake-bpy-module-latest-20230803/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/props.py` & `fake-bpy-module-latest-20230803/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/types.py` & `fake-bpy-module-latest-20230803/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1057 +1,1057 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
-00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f6f   bpy.import bl_o
-00000040: 7065 7261 746f 7273 2e61 7373 6574 730a  perators.assets.
-00000050: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-00000060: 6f72 732e 6672 6565 7374 796c 650a 696d  ors.freestyle.im
-00000070: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000080: 5f6e 6f64 650a 696d 706f 7274 2062 6c5f  _node.import bl_
-00000090: 7569 2e70 726f 7065 7274 6965 735f 636f  ui.properties_co
-000000a0: 6e73 7472 6169 6e74 0a69 6d70 6f72 7420  nstraint.import 
-000000b0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000000c0: 5f64 6174 615f 626f 6e65 0a69 6d70 6f72  _data_bone.impor
-000000d0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000000e0: 6573 5f64 6174 615f 6d65 7461 6261 6c6c  es_data_metaball
-000000f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000100: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00000110: 6172 0a69 6d70 6f72 7420 626c 5f6f 7065  ar.import bl_ope
-00000120: 7261 746f 7273 2e74 6578 740a 696d 706f  rators.text.impo
-00000130: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-00000140: 6669 6c65 0a69 6d70 6f72 7420 626c 5f75  file.import bl_u
-00000150: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000160: 615f 6770 656e 6369 6c0a 696d 706f 7274  a_gpencil.import
-00000170: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000180: 735f 7068 7973 6963 735f 6479 6e61 6d69  s_physics_dynami
-00000190: 6370 6169 6e74 0a69 6d70 6f72 7420 626c  cpaint.import bl
-000001a0: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
-000001b0: 6879 7369 6373 5f72 6967 6964 626f 6479  hysics_rigidbody
-000001c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000001d0: 6f70 6572 7469 6573 5f64 6174 615f 6361  operties_data_ca
-000001e0: 6d65 7261 0a69 6d70 6f72 7420 626c 5f75  mera.import bl_u
-000001f0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000200: 615f 6375 7276 650a 696d 706f 7274 2062  a_curve.import b
-00000210: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000220: 7068 7973 6963 735f 636c 6f74 680a 696d  physics_cloth.im
-00000230: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000240: 7274 6965 735f 6461 7461 5f6d 6f64 6966  rties_data_modif
-00000250: 6965 720a 696d 706f 7274 2062 6c5f 7569  ier.import bl_ui
-00000260: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
-00000270: 5f6c 6967 6874 7072 6f62 650a 696d 706f  _lightprobe.impo
-00000280: 7274 2062 6c5f 7569 2e73 7061 6365 5f69  rt bl_ui.space_i
-00000290: 6d61 6765 0a69 6d70 6f72 7420 626c 5f75  mage.import bl_u
-000002a0: 692e 7072 6f70 6572 7469 6573 5f77 6f72  i.properties_wor
-000002b0: 6b73 7061 6365 0a69 6d70 6f72 7420 626c  kspace.import bl
-000002c0: 5f75 692e 7370 6163 655f 7469 6d65 0a69  _ui.space_time.i
-000002d0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-000002e0: 7273 2e6e 6f64 650a 696d 706f 7274 2062  rs.node.import b
-000002f0: 6c5f 7569 2e73 7061 6365 5f63 6c69 700a  l_ui.space_clip.
-00000300: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000310: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
-00000320: 7269 6769 6462 6f64 795f 636f 6e73 7472  rigidbody_constr
-00000330: 6169 6e74 0a69 6d70 6f72 7420 626c 5f75  aint.import bl_u
-00000340: 692e 7072 6f70 6572 7469 6573 5f6d 6173  i.properties_mas
-00000350: 6b5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  k_common.import 
-00000360: 626c 5f6f 7065 7261 746f 7273 2e77 6d0a  bl_operators.wm.
-00000370: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000380: 6365 5f74 6f6f 6c73 7973 7465 6d5f 746f  ce_toolsystem_to
-00000390: 6f6c 6261 720a 696d 706f 7274 2062 6c5f  olbar.import bl_
-000003a0: 7569 2e73 7061 6365 5f73 6571 7565 6e63  ui.space_sequenc
-000003b0: 6572 0a69 6d70 6f72 7420 626c 5f6f 7065  er.import bl_ope
-000003c0: 7261 746f 7273 2e73 7072 6561 6473 6865  rators.spreadshe
-000003d0: 6574 0a69 6d70 6f72 7420 626c 5f75 692e  et.import bl_ui.
-000003e0: 7370 6163 655f 7465 7874 0a69 6d70 6f72  space_text.impor
-000003f0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000400: 6573 5f77 6f72 6c64 0a69 6d70 6f72 7420  es_world.import 
-00000410: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000420: 5f64 6174 615f 6375 7276 6573 0a69 6d70  _data_curves.imp
-00000430: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000440: 7469 6573 5f64 6174 615f 656d 7074 790a  ties_data_empty.
-00000450: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000460: 7065 7274 6965 735f 6461 7461 5f73 7065  perties_data_spe
-00000470: 616b 6572 0a69 6d70 6f72 7420 626c 5f75  aker.import bl_u
-00000480: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
-00000490: 775f 6c61 7965 720a 696d 706f 7274 2062  w_layer.import b
-000004a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000004b0: 7465 7874 7572 650a 696d 706f 7274 2062  texture.import b
-000004c0: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
-000004d0: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
-000004e0: 7569 2e70 726f 7065 7274 6965 735f 7363  ui.properties_sc
-000004f0: 656e 650a 696d 706f 7274 2062 6c5f 7569  ene.import bl_ui
-00000500: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
-00000510: 6963 735f 6765 6f6d 6574 7279 5f6e 6f64  ics_geometry_nod
-00000520: 6573 0a69 6d70 6f72 7420 626c 5f75 692e  es.import bl_ui.
-00000530: 7072 6f70 6572 7469 6573 5f67 7265 6173  properties_greas
-00000540: 655f 7065 6e63 696c 5f63 6f6d 6d6f 6e0a  e_pencil_common.
-00000550: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000560: 7065 7274 6965 735f 7061 696e 745f 636f  perties_paint_co
-00000570: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f75  mmon.import bl_u
-00000580: 692e 7072 6f70 6572 7469 6573 5f70 6172  i.properties_par
-00000590: 7469 636c 650a 696d 706f 7274 2062 6c5f  ticle.import bl_
-000005a0: 7569 2e73 7061 6365 5f75 7365 7270 7265  ui.space_userpre
-000005b0: 660a 696d 706f 7274 2062 6c5f 6f70 6572  f.import bl_oper
-000005c0: 6174 6f72 732e 7072 6573 6574 730a 696d  ators.presets.im
-000005d0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-000005e0: 5f73 7072 6561 6473 6865 6574 0a69 6d70  _spreadsheet.imp
-000005f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000600: 7469 6573 5f6d 6174 6572 6961 6c0a 696d  ties_material.im
-00000610: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000620: 5f64 6f70 6573 6865 6574 0a69 6d70 6f72  _dopesheet.impor
-00000630: 7420 626c 5f75 692e 7370 6163 655f 696e  t bl_ui.space_in
-00000640: 666f 0a69 6d70 6f72 7420 626c 5f75 692e  fo.import bl_ui.
-00000650: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-00000660: 706f 696e 7463 6c6f 7564 0a69 6d70 6f72  pointcloud.impor
-00000670: 7420 626c 5f6f 7065 7261 746f 7273 2e61  t bl_operators.a
-00000680: 6e69 6d0a 696d 706f 7274 2062 6c5f 7569  nim.import bl_ui
-00000690: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
-000006a0: 6963 735f 6669 656c 640a 696d 706f 7274  ics_field.import
-000006b0: 2062 6c5f 7569 2e73 7061 6365 5f6e 6c61   bl_ui.space_nla
-000006c0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000006d0: 746f 7273 2e63 6c69 700a 696d 706f 7274  tors.clip.import
-000006e0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000006f0: 735f 6d61 7465 7269 616c 5f67 7065 6e63  s_material_gpenc
-00000700: 696c 0a69 6d70 6f72 7420 626c 5f75 692e  il.import bl_ui.
-00000710: 7370 6163 655f 746f 6f6c 7379 7374 656d  space_toolsystem
-00000720: 5f63 6f6d 6d6f 6e0a 696d 706f 7274 2062  _common.import b
-00000730: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
-00000740: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
-00000750: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000760: 615f 6c61 7474 6963 650a 696d 706f 7274  a_lattice.import
-00000770: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000780: 735f 7068 7973 6963 735f 736f 6674 626f  s_physics_softbo
-00000790: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
-000007a0: 6765 6e65 7269 635f 7569 5f6c 6973 740a  generic_ui_list.
-000007b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000007c0: 6365 5f66 696c 6562 726f 7773 6572 0a69  ce_filebrowser.i
-000007d0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000007e0: 655f 6772 6170 680a 696d 706f 7274 2062  e_graph.import b
-000007f0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000800: 6461 7461 5f6d 6573 680a 696d 706f 7274  data_mesh.import
-00000810: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000820: 735f 6f62 6a65 6374 0a69 6d70 6f72 7420  s_object.import 
-00000830: 626c 5f75 692e 7370 6163 655f 7374 6174  bl_ui.space_stat
-00000840: 7573 6261 720a 696d 706f 7274 2062 6c5f  usbar.import bl_
-00000850: 7569 2e6e 6f64 655f 6164 645f 6d65 6e75  ui.node_add_menu
-00000860: 5f67 656f 6d65 7472 790a 696d 706f 7274  _geometry.import
-00000870: 2062 6c5f 6f70 6572 6174 6f72 732e 636f   bl_operators.co
-00000880: 6e73 7472 6169 6e74 0a69 6d70 6f72 7420  nstraint.import 
-00000890: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000008a0: 5f63 6f6c 6c65 6374 696f 6e0a 696d 706f  _collection.impo
-000008b0: 7274 2062 6c5f 7569 0a69 6d70 6f72 7420  rt bl_ui.import 
-000008c0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000008d0: 5f70 6879 7369 6373 5f63 6f6d 6d6f 6e0a  _physics_common.
-000008e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000008f0: 6365 5f74 6f70 6261 720a 696d 706f 7274  ce_topbar.import
-00000900: 2062 6c5f 7569 2e73 7061 6365 5f6f 7574   bl_ui.space_out
-00000910: 6c69 6e65 720a 696d 706f 7274 2062 6c5f  liner.import bl_
-00000920: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-00000930: 7461 5f67 7265 6173 655f 7065 6e63 696c  ta_grease_pencil
-00000940: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000950: 6f70 6572 7469 6573 5f64 6174 615f 6172  operties_data_ar
-00000960: 6d61 7475 7265 0a69 6d70 6f72 7420 626c  mature.import bl
-00000970: 5f6f 7065 7261 746f 7273 2e76 6965 7733  _operators.view3
-00000980: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
-00000990: 7061 6365 5f76 6965 7733 640a 696d 706f  pace_view3d.impo
-000009a0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000009b0: 6965 735f 6f75 7470 7574 0a69 6d70 6f72  ies_output.impor
-000009c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000009d0: 6573 5f64 6174 615f 766f 6c75 6d65 0a69  es_data_volume.i
-000009e0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-000009f0: 655f 636f 6e73 6f6c 650a 696d 706f 7274  e_console.import
-00000a00: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000a10: 735f 6461 7461 5f73 6861 6465 7266 780a  s_data_shaderfx.
-00000a20: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000a30: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
-00000a40: 666c 7569 640a 696d 706f 7274 2062 6c5f  fluid.import bl_
-00000a50: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-00000a60: 6565 7374 796c 650a 696d 706f 7274 2062  eestyle.import b
-00000a70: 6c5f 6f70 6572 6174 6f72 732e 6f62 6a65  l_operators.obje
-00000a80: 6374 0a69 6d70 6f72 7420 626c 5f75 692e  ct.import bl_ui.
-00000a90: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-00000aa0: 6c69 6768 740a 696d 706f 7274 2062 6c5f  light.import bl_
-00000ab0: 7569 2e70 726f 7065 7274 6965 735f 7265  ui.properties_re
-00000ac0: 6e64 6572 0a0a 4765 6e65 7269 6354 7970  nder..GenericTyp
+00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
+00000040: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000050: 7369 6373 5f66 6965 6c64 0a69 6d70 6f72  sics_field.impor
+00000060: 7420 626c 5f75 692e 7370 6163 655f 6772  t bl_ui.space_gr
+00000070: 6170 680a 696d 706f 7274 2062 6c5f 7569  aph.import bl_ui
+00000080: 2e70 726f 7065 7274 6965 735f 776f 726c  .properties_worl
+00000090: 640a 696d 706f 7274 2062 6c5f 7569 2e73  d.import bl_ui.s
+000000a0: 7061 6365 5f6e 6c61 0a69 6d70 6f72 7420  pace_nla.import 
+000000b0: 626c 5f6f 7065 7261 746f 7273 2e77 6d0a  bl_operators.wm.
+000000c0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000000d0: 7065 7274 6965 735f 6461 7461 5f67 7065  perties_data_gpe
+000000e0: 6e63 696c 0a69 6d70 6f72 7420 626c 5f75  ncil.import bl_u
+000000f0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000100: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
+00000110: 626c 5f6f 7065 7261 746f 7273 2e61 6e69  bl_operators.ani
+00000120: 6d0a 696d 706f 7274 2062 6c5f 7569 2e73  m.import bl_ui.s
+00000130: 7061 6365 5f74 696d 650a 696d 706f 7274  pace_time.import
+00000140: 2062 6c5f 7569 2e73 7061 6365 5f75 7365   bl_ui.space_use
+00000150: 7270 7265 660a 696d 706f 7274 2062 6c5f  rpref.import bl_
+00000160: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+00000170: 7461 5f63 7572 7665 0a69 6d70 6f72 7420  ta_curve.import 
+00000180: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000190: 5f73 6365 6e65 0a69 6d70 6f72 7420 626c  _scene.import bl
+000001a0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000001b0: 6174 615f 656d 7074 790a 696d 706f 7274  ata_empty.import
+000001c0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000001d0: 735f 7068 7973 6963 735f 666c 7569 640a  s_physics_fluid.
+000001e0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000001f0: 6f72 732e 636f 6e73 7472 6169 6e74 0a69  ors.constraint.i
+00000200: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000210: 655f 7374 6174 7573 6261 720a 696d 706f  e_statusbar.impo
+00000220: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000230: 6965 735f 6461 7461 5f63 616d 6572 610a  ies_data_camera.
+00000240: 696d 706f 7274 2062 6c5f 7569 2e67 656e  import bl_ui.gen
+00000250: 6572 6963 5f75 695f 6c69 7374 0a69 6d70  eric_ui_list.imp
+00000260: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000270: 7469 6573 5f70 6879 7369 6373 5f67 656f  ties_physics_geo
+00000280: 6d65 7472 795f 6e6f 6465 730a 696d 706f  metry_nodes.impo
+00000290: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000002a0: 6965 735f 6d61 7465 7269 616c 5f67 7065  ies_material_gpe
+000002b0: 6e63 696c 0a69 6d70 6f72 7420 626c 5f75  ncil.import bl_u
+000002c0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000002d0: 615f 6c69 6768 7470 726f 6265 0a69 6d70  a_lightprobe.imp
+000002e0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000002f0: 7469 6573 5f6f 7574 7075 740a 696d 706f  ties_output.impo
+00000300: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+00000310: 6f62 6a65 6374 0a69 6d70 6f72 7420 626c  object.import bl
+00000320: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000330: 6174 615f 7368 6164 6572 6678 0a69 6d70  ata_shaderfx.imp
+00000340: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000350: 7469 6573 5f64 6174 615f 6d65 7368 0a69  ties_data_mesh.i
+00000360: 6d70 6f72 7420 626c 5f75 690a 696d 706f  mport bl_ui.impo
+00000370: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000380: 6965 735f 6772 6561 7365 5f70 656e 6369  ies_grease_penci
+00000390: 6c5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  l_common.import 
+000003a0: 626c 5f75 692e 7370 6163 655f 7365 7175  bl_ui.space_sequ
+000003b0: 656e 6365 720a 696d 706f 7274 2062 6c5f  encer.import bl_
+000003c0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000003d0: 7461 5f73 7065 616b 6572 0a69 6d70 6f72  ta_speaker.impor
+000003e0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000003f0: 6573 5f72 656e 6465 720a 696d 706f 7274  es_render.import
+00000400: 2062 6c5f 6f70 6572 6174 6f72 732e 6e6f   bl_operators.no
+00000410: 6465 0a69 6d70 6f72 7420 626c 5f6f 7065  de.import bl_ope
+00000420: 7261 746f 7273 2e61 7373 6574 730a 696d  rators.assets.im
+00000430: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000440: 7274 6965 735f 6461 7461 5f6c 6967 6874  rties_data_light
+00000450: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000460: 6f70 6572 7469 6573 5f77 6f72 6b73 7061  operties_workspa
+00000470: 6365 0a69 6d70 6f72 7420 626c 5f75 692e  ce.import bl_ui.
+00000480: 7370 6163 655f 7669 6577 3364 0a69 6d70  space_view3d.imp
+00000490: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000004a0: 7469 6573 5f63 6f6e 7374 7261 696e 740a  ties_constraint.
+000004b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000004c0: 6365 5f70 726f 7065 7274 6965 730a 696d  ce_properties.im
+000004d0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000004e0: 7274 6965 735f 6f62 6a65 6374 0a69 6d70  rties_object.imp
+000004f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000500: 7469 6573 5f70 6879 7369 6373 5f73 6f66  ties_physics_sof
+00000510: 7462 6f64 790a 696d 706f 7274 2062 6c5f  tbody.import bl_
+00000520: 7569 2e73 7061 6365 5f69 6d61 6765 0a69  ui.space_image.i
+00000530: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000540: 655f 696e 666f 0a69 6d70 6f72 7420 626c  e_info.import bl
+00000550: 5f75 692e 7370 6163 655f 636c 6970 0a69  _ui.space_clip.i
+00000560: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000570: 6572 7469 6573 5f64 6174 615f 6d6f 6469  erties_data_modi
+00000580: 6669 6572 0a69 6d70 6f72 7420 626c 5f6f  fier.import bl_o
+00000590: 7065 7261 746f 7273 2e74 6578 740a 696d  perators.text.im
+000005a0: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
+000005b0: 732e 636c 6970 0a69 6d70 6f72 7420 626c  s.clip.import bl
+000005c0: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
+000005d0: 7374 656d 5f74 6f6f 6c62 6172 0a69 6d70  stem_toolbar.imp
+000005e0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000005f0: 7469 6573 5f70 6172 7469 636c 650a 696d  ties_particle.im
+00000600: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000610: 7274 6965 735f 7465 7874 7572 650a 696d  rties_texture.im
+00000620: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000630: 7274 6965 735f 6d61 7465 7269 616c 0a69  rties_material.i
+00000640: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000650: 7273 2e66 7265 6573 7479 6c65 0a69 6d70  rs.freestyle.imp
+00000660: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000670: 636f 6e73 6f6c 650a 696d 706f 7274 2062  console.import b
+00000680: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000690: 6461 7461 5f62 6f6e 650a 696d 706f 7274  data_bone.import
+000006a0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000006b0: 735f 7669 6577 5f6c 6179 6572 0a69 6d70  s_view_layer.imp
+000006c0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000006d0: 7469 6573 5f70 6879 7369 6373 5f63 6c6f  ties_physics_clo
+000006e0: 7468 0a69 6d70 6f72 7420 626c 5f75 692e  th.import bl_ui.
+000006f0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000700: 6d65 7461 6261 6c6c 0a69 6d70 6f72 7420  metaball.import 
+00000710: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000720: 5f64 6174 615f 706f 696e 7463 6c6f 7564  _data_pointcloud
+00000730: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000740: 6163 655f 6f75 746c 696e 6572 0a69 6d70  ace_outliner.imp
+00000750: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000760: 7469 6573 5f64 6174 615f 6172 6d61 7475  ties_data_armatu
+00000770: 7265 0a69 6d70 6f72 7420 626c 5f75 692e  re.import bl_ui.
+00000780: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000790: 6c61 7474 6963 650a 696d 706f 7274 2062  lattice.import b
+000007a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000007b0: 6461 7461 5f67 7265 6173 655f 7065 6e63  data_grease_penc
+000007c0: 696c 0a69 6d70 6f72 7420 626c 5f6f 7065  il.import bl_ope
+000007d0: 7261 746f 7273 2e73 7072 6561 6473 6865  rators.spreadshe
+000007e0: 6574 0a69 6d70 6f72 7420 626c 5f75 692e  et.import bl_ui.
+000007f0: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
+00000800: 7479 6c65 0a69 6d70 6f72 7420 626c 5f75  tyle.import bl_u
+00000810: 692e 7370 6163 655f 746f 7062 6172 0a69  i.space_topbar.i
+00000820: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000830: 655f 6669 6c65 6272 6f77 7365 720a 696d  e_filebrowser.im
+00000840: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000850: 5f76 6965 7733 645f 746f 6f6c 6261 720a  _view3d_toolbar.
+00000860: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000870: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
+00000880: 6479 6e61 6d69 6370 6169 6e74 0a69 6d70  dynamicpaint.imp
+00000890: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000008a0: 7469 6573 5f70 6879 7369 6373 5f63 6f6d  ties_physics_com
+000008b0: 6d6f 6e0a 696d 706f 7274 2062 6c5f 6f70  mon.import bl_op
+000008c0: 6572 6174 6f72 732e 7669 6577 3364 0a69  erators.view3d.i
+000008d0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+000008e0: 655f 6e6f 6465 0a69 6d70 6f72 7420 626c  e_node.import bl
+000008f0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000900: 6174 615f 6375 7276 6573 0a69 6d70 6f72  ata_curves.impor
+00000910: 7420 626c 5f6f 7065 7261 746f 7273 2e70  t bl_operators.p
+00000920: 7265 7365 7473 0a69 6d70 6f72 7420 626c  resets.import bl
+00000930: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
+00000940: 6169 6e74 5f63 6f6d 6d6f 6e0a 696d 706f  aint_common.impo
+00000950: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000960: 6965 735f 636f 6c6c 6563 7469 6f6e 0a69  ies_collection.i
+00000970: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000980: 655f 746f 6f6c 7379 7374 656d 5f63 6f6d  e_toolsystem_com
+00000990: 6d6f 6e0a 696d 706f 7274 2062 6c5f 7569  mon.import bl_ui
+000009a0: 2e73 7061 6365 5f73 7072 6561 6473 6865  .space_spreadshe
+000009b0: 6574 0a69 6d70 6f72 7420 626c 5f75 692e  et.import bl_ui.
+000009c0: 7370 6163 655f 646f 7065 7368 6565 740a  space_dopesheet.
+000009d0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000009e0: 6f72 732e 6669 6c65 0a69 6d70 6f72 7420  ors.file.import 
+000009f0: 626c 5f6f 7065 7261 746f 7273 2e75 7365  bl_operators.use
+00000a00: 7270 7265 660a 696d 706f 7274 2062 6c5f  rpref.import bl_
+00000a10: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000a20: 7973 6963 735f 7269 6769 6462 6f64 790a  ysics_rigidbody.
+00000a30: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000a40: 7065 7274 6965 735f 6d61 736b 5f63 6f6d  perties_mask_com
+00000a50: 6d6f 6e0a 696d 706f 7274 2062 6c5f 7569  mon.import bl_ui
+00000a60: 2e6e 6f64 655f 6164 645f 6d65 6e75 5f67  .node_add_menu_g
+00000a70: 656f 6d65 7472 790a 696d 706f 7274 2062  eometry.import b
+00000a80: 6c5f 7569 2e73 7061 6365 5f74 6578 740a  l_ui.space_text.
+00000a90: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000aa0: 7065 7274 6965 735f 7068 7973 6963 735f  perties_physics_
+00000ab0: 7269 6769 6462 6f64 795f 636f 6e73 7472  rigidbody_constr
+00000ac0: 6169 6e74 0a0a 4765 6e65 7269 6354 7970  aint..GenericTyp
 00000ad0: 6520 3d20 7479 7069 6e67 2e54 7970 6556  e = typing.TypeV
 00000ae0: 6172 2822 4765 6e65 7269 6354 7970 6522  ar("GenericType"
-00000af0: 290a 0a0a 636c 6173 7320 6270 795f 7072  )...class bpy_pr
-00000b00: 6f70 5f63 6f6c 6c65 6374 696f 6e28 7479  op_collection(ty
-00000b10: 7069 6e67 2e47 656e 6572 6963 5b47 656e  ping.Generic[Gen
-00000b20: 6572 6963 5479 7065 5d29 3a0a 2020 2020  ericType]):.    
-00000b30: 2727 2720 6275 696c 742d 696e 2063 6c61  ''' built-in cla
-00000b40: 7373 2075 7365 6420 666f 7220 616c 6c20  ss used for all 
-00000b50: 636f 6c6c 6563 7469 6f6e 732e 0a20 2020  collections..   
-00000b60: 2027 2727 0a0a 2020 2020 6465 6620 6669   '''..    def fi
-00000b70: 6e64 2873 656c 662c 206b 6579 3a20 7479  nd(self, key: ty
-00000b80: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00000b90: 725d 2920 2d3e 2069 6e74 3a0a 2020 2020  r]) -> int:.    
-00000ba0: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
-00000bb0: 7468 6520 696e 6465 7820 6f66 2061 206b  the index of a k
-00000bc0: 6579 2069 6e20 6120 636f 6c6c 6563 7469  ey in a collecti
-00000bd0: 6f6e 206f 7220 2d31 2077 6865 6e20 6e6f  on or -1 when no
-00000be0: 7420 666f 756e 6420 286d 6174 6368 6573  t found (matches
-00000bf0: 2050 7974 686f 6e27 7320 7374 7269 6e67   Python's string
-00000c00: 2066 696e 6420 6675 6e63 7469 6f6e 206f   find function o
-00000c10: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
-00000c20: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-00000c30: 6d20 6b65 793a 2054 6865 2069 6465 6e74  m key: The ident
-00000c40: 6966 6965 7220 666f 7220 7468 6520 636f  ifier for the co
-00000c50: 6c6c 6563 7469 6f6e 206d 656d 6265 722e  llection member.
-00000c60: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
-00000c70: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-00000c80: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
-00000c90: 203a 7274 7970 653a 2069 6e74 0a20 2020   :rtype: int.   
-00000ca0: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
-00000cb0: 6465 7820 6f66 2074 6865 206b 6579 2e0a  dex of the key..
-00000cc0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00000cd0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00000ce0: 6620 666f 7265 6163 685f 6765 7428 7365  f foreach_get(se
-00000cf0: 6c66 2c20 6174 7472 2c20 7365 7129 3a0a  lf, attr, seq):.
-00000d00: 2020 2020 2020 2020 2727 2720 5468 6973          ''' This
-00000d10: 2069 7320 6120 6675 6e63 7469 6f6e 2074   is a function t
-00000d20: 6f20 6769 7665 2066 6173 7420 6163 6365  o give fast acce
-00000d30: 7373 2074 6f20 6174 7472 6962 7574 6573  ss to attributes
-00000d40: 2077 6974 6869 6e20 6120 636f 6c6c 6563   within a collec
-00000d50: 7469 6f6e 2e20 4f6e 6c79 2077 6f72 6b73  tion. Only works
-00000d60: 2066 6f72 2027 6261 7369 6320 7479 7065   for 'basic type
-00000d70: 2720 7072 6f70 6572 7469 6573 2028 626f  ' properties (bo
-00000d80: 6f6c 2c20 696e 7420 616e 6420 666c 6f61  ol, int and floa
-00000d90: 7429 2120 4d75 6c74 692d 6469 6d65 6e73  t)! Multi-dimens
-00000da0: 696f 6e61 6c20 6172 7261 7973 2028 6c69  ional arrays (li
-00000db0: 6b65 2061 7272 6179 206f 6620 7665 6374  ke array of vect
-00000dc0: 6f72 7329 2077 696c 6c20 6265 2066 6c61  ors) will be fla
-00000dd0: 7474 656e 6564 2069 6e74 6f20 7365 712e  ttened into seq.
-00000de0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00000df0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00000e00: 6465 6620 666f 7265 6163 685f 7365 7428  def foreach_set(
-00000e10: 7365 6c66 2c20 6174 7472 2c20 7365 7129  self, attr, seq)
-00000e20: 3a0a 2020 2020 2020 2020 2727 2720 5468  :.        ''' Th
-00000e30: 6973 2069 7320 6120 6675 6e63 7469 6f6e  is is a function
-00000e40: 2074 6f20 6769 7665 2066 6173 7420 6163   to give fast ac
-00000e50: 6365 7373 2074 6f20 6174 7472 6962 7574  cess to attribut
-00000e60: 6573 2077 6974 6869 6e20 6120 636f 6c6c  es within a coll
-00000e70: 6563 7469 6f6e 2e20 4f6e 6c79 2077 6f72  ection. Only wor
-00000e80: 6b73 2066 6f72 2027 6261 7369 6320 7479  ks for 'basic ty
-00000e90: 7065 2720 7072 6f70 6572 7469 6573 2028  pe' properties (
-00000ea0: 626f 6f6c 2c20 696e 7420 616e 6420 666c  bool, int and fl
-00000eb0: 6f61 7429 2120 7365 7120 6d75 7374 2062  oat)! seq must b
-00000ec0: 6520 756e 692d 6469 6d65 6e73 696f 6e61  e uni-dimensiona
-00000ed0: 6c2c 206d 756c 7469 2d64 696d 656e 7369  l, multi-dimensi
-00000ee0: 6f6e 616c 2061 7272 6179 7320 286c 696b  onal arrays (lik
-00000ef0: 6520 6172 7261 7920 6f66 2076 6563 746f  e array of vecto
-00000f00: 7273 2920 7769 6c6c 2062 6520 7265 2d63  rs) will be re-c
-00000f10: 7265 6174 6564 2066 726f 6d20 6974 2e0a  reated from it..
-00000f20: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00000f30: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00000f40: 6566 2067 6574 2873 656c 662c 0a20 2020  ef get(self,.   
-00000f50: 2020 2020 2020 2020 206b 6579 3a20 7479           key: ty
-00000f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00000f70: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
-00000f80: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
-00000f90: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00000fa0: 416e 795d 203d 204e 6f6e 6529 3a0a 2020  Any] = None):.  
-00000fb0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00000fc0: 7320 7468 6520 7661 6c75 6520 6f66 2074  s the value of t
-00000fd0: 6865 2069 7465 6d20 6173 7369 676e 6564  he item assigned
-00000fe0: 2074 6f20 6b65 7920 6f72 2064 6566 6175   to key or defau
-00000ff0: 6c74 2077 6865 6e20 6e6f 7420 666f 756e  lt when not foun
-00001000: 6420 286d 6174 6368 6573 2050 7974 686f  d (matches Pytho
-00001010: 6e27 7320 6469 6374 696f 6e61 7279 2066  n's dictionary f
-00001020: 756e 6374 696f 6e20 6f66 2074 6865 2073  unction of the s
-00001030: 616d 6520 6e61 6d65 292e 0a0a 2020 2020  ame name)...    
-00001040: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00001050: 5468 6520 6964 656e 7469 6669 6572 2066  The identifier f
-00001060: 6f72 2074 6865 2063 6f6c 6c65 6374 696f  or the collectio
-00001070: 6e20 6d65 6d62 6572 2e0a 2020 2020 2020  n member..      
-00001080: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-00001090: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-000010a0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-000010b0: 2064 6566 6175 6c74 3a20 4f70 7469 6f6e   default: Option
-000010c0: 616c 2061 7267 756d 656e 7420 666f 7220  al argument for 
-000010d0: 7468 6520 7661 6c75 6520 746f 2072 6574  the value to ret
-000010e0: 7572 6e20 6966 202a 6b65 792a 2069 7320  urn if *key* is 
-000010f0: 6e6f 7420 666f 756e 642e 0a20 2020 2020  not found..     
-00001100: 2020 203a 7479 7065 2064 6566 6175 6c74     :type default
-00001110: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001120: 6c5b 7479 7069 6e67 2e41 6e79 5d0a 2020  l[typing.Any].  
-00001130: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00001140: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00001150: 6974 656d 7328 7365 6c66 2920 2d3e 2074  items(self) -> t
-00001160: 7970 696e 672e 4c69 7374 3a0a 2020 2020  yping.List:.    
-00001170: 2020 2020 2727 2720 5265 7475 726e 2074      ''' Return t
-00001180: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
-00001190: 6620 636f 6c6c 6563 7469 6f6e 206d 656d  f collection mem
-000011a0: 6265 7273 2028 6d61 7463 6869 6e67 2050  bers (matching P
-000011b0: 7974 686f 6e27 7320 6469 6374 2e69 7465  ython's dict.ite
-000011c0: 6d73 2829 2066 756e 6374 696f 6e61 6c69  ms() functionali
-000011d0: 7479 292e 0a0a 2020 2020 2020 2020 3a72  ty)...        :r
-000011e0: 7479 7065 3a20 7479 7069 6e67 2e4c 6973  type: typing.Lis
-000011f0: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
-00001200: 6e3a 2028 6b65 792c 2076 616c 7565 2920  n: (key, value) 
-00001210: 7061 6972 7320 666f 7220 6561 6368 206d  pairs for each m
-00001220: 656d 6265 7220 6f66 2074 6869 7320 636f  ember of this co
-00001230: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00001240: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00001250: 7373 0a0a 2020 2020 6465 6620 6b65 7973  ss..    def keys
-00001260: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-00001270: 2e4c 6973 745b 7374 725d 3a0a 2020 2020  .List[str]:.    
-00001280: 2020 2020 2727 2720 5265 7475 726e 2074      ''' Return t
-00001290: 6865 2069 6465 6e74 6966 6965 7273 206f  he identifiers o
-000012a0: 6620 636f 6c6c 6563 7469 6f6e 206d 656d  f collection mem
-000012b0: 6265 7273 2028 6d61 7463 6869 6e67 2050  bers (matching P
-000012c0: 7974 686f 6e27 7320 6469 6374 2e6b 6579  ython's dict.key
-000012d0: 7328 2920 6675 6e63 7469 6f6e 616c 6974  s() functionalit
-000012e0: 7929 2e0a 0a20 2020 2020 2020 203a 7274  y)...        :rt
-000012f0: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
-00001300: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
-00001310: 6574 7572 6e3a 2074 6865 2069 6465 6e74  eturn: the ident
-00001320: 6966 6965 7273 2066 6f72 2065 6163 6820  ifiers for each 
-00001330: 6d65 6d62 6572 206f 6620 7468 6973 2063  member of this c
-00001340: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00001350: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00001360: 6173 730a 0a20 2020 2064 6566 2076 616c  ass..    def val
-00001370: 7565 7328 7365 6c66 2920 2d3e 2074 7970  ues(self) -> typ
-00001380: 696e 672e 4c69 7374 3a0a 2020 2020 2020  ing.List:.      
-00001390: 2020 2727 2720 5265 7475 726e 2074 6865    ''' Return the
-000013a0: 2076 616c 7565 7320 6f66 2063 6f6c 6c65   values of colle
-000013b0: 6374 696f 6e20 286d 6174 6368 696e 6720  ction (matching 
-000013c0: 5079 7468 6f6e 2773 2064 6963 742e 7661  Python's dict.va
-000013d0: 6c75 6573 2829 2066 756e 6374 696f 6e61  lues() functiona
-000013e0: 6c69 7479 292e 0a0a 2020 2020 2020 2020  lity)...        
-000013f0: 3a72 7479 7065 3a20 7479 7069 6e67 2e4c  :rtype: typing.L
-00001400: 6973 740a 2020 2020 2020 2020 3a72 6574  ist.        :ret
-00001410: 7572 6e3a 2074 6865 206d 656d 6265 7273  urn: the members
-00001420: 206f 6620 7468 6973 2063 6f6c 6c65 6374   of this collect
-00001430: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
-00001440: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00001450: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
-00001460: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
-00001470: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00001480: 7374 725d 2920 2d3e 2027 4765 6e65 7269  str]) -> 'Generi
-00001490: 6354 7970 6527 3a0a 2020 2020 2020 2020  cType':.        
-000014a0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-000014b0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-000014c0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-000014d0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-000014e0: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-000014f0: 7970 653a 2027 4765 6e65 7269 6354 7970  ype: 'GenericTyp
-00001500: 6527 0a20 2020 2020 2020 2027 2727 0a20  e'.        '''. 
-00001510: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001520: 2064 6566 205f 5f73 6574 6974 656d 5f5f   def __setitem__
-00001530: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
-00001540: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00001550: 725d 2c20 7661 6c75 653a 2027 4765 6e65  r], value: 'Gene
-00001560: 7269 6354 7970 6527 293a 0a20 2020 2020  ricType'):.     
-00001570: 2020 2027 2727 200a 0a20 2020 2020 2020     ''' ..       
-00001580: 203a 7061 7261 6d20 6b65 793a 200a 2020   :param key: .  
-00001590: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-000015a0: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
-000015b0: 742c 2073 7472 5d0a 2020 2020 2020 2020  t, str].        
-000015c0: 3a70 6172 616d 2076 616c 7565 3a20 0a20  :param value: . 
-000015d0: 2020 2020 2020 203a 7479 7065 2076 616c         :type val
-000015e0: 7565 3a20 2747 656e 6572 6963 5479 7065  ue: 'GenericType
-000015f0: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
-00001600: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001610: 6465 6620 5f5f 6465 6c69 7465 6d5f 5f28  def __delitem__(
-00001620: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00001630: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00001640: 5d29 202d 3e20 2747 656e 6572 6963 5479  ]) -> 'GenericTy
-00001650: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
-00001660: 200a 0a20 2020 2020 2020 203a 7061 7261   ..        :para
-00001670: 6d20 6b65 793a 200a 2020 2020 2020 2020  m key: .        
-00001680: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
-00001690: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-000016a0: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-000016b0: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
-000016c0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000016d0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000016e0: 6620 5f5f 6974 6572 5f5f 2873 656c 6629  f __iter__(self)
-000016f0: 202d 3e20 7479 7069 6e67 2e49 7465 7261   -> typing.Itera
-00001700: 746f 725b 2747 656e 6572 6963 5479 7065  tor['GenericType
-00001710: 275d 3a0a 2020 2020 2020 2020 2727 2720  ']:.        ''' 
-00001720: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00001730: 3a20 7479 7069 6e67 2e49 7465 7261 746f  : typing.Iterato
-00001740: 725b 2747 656e 6572 6963 5479 7065 275d  r['GenericType']
-00001750: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00001760: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00001770: 6566 205f 5f6e 6578 745f 5f28 7365 6c66  ef __next__(self
-00001780: 2920 2d3e 2027 4765 6e65 7269 6354 7970  ) -> 'GenericTyp
-00001790: 6527 3a0a 2020 2020 2020 2020 2727 2720  e':.        ''' 
-000017a0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-000017b0: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
-000017c0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000017d0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000017e0: 6620 5f5f 6c65 6e5f 5f28 7365 6c66 2920  f __len__(self) 
-000017f0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00001800: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
-00001810: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-00001820: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00001830: 7373 0a0a 0a63 6c61 7373 2062 7079 5f73  ss...class bpy_s
-00001840: 7472 7563 743a 0a20 2020 2027 2727 2062  truct:.    ''' b
-00001850: 7569 6c74 2d69 6e20 6261 7365 2063 6c61  uilt-in base cla
-00001860: 7373 2066 6f72 2061 6c6c 2063 6c61 7373  ss for all class
-00001870: 6573 2069 6e20 6270 792e 7479 7065 732e  es in bpy.types.
-00001880: 0a20 2020 2027 2727 0a0a 2020 2020 6964  .    '''..    id
-00001890: 5f64 6174 6120 3d20 4e6f 6e65 0a20 2020  _data = None.   
-000018a0: 2027 2727 2054 6865 2060 6270 792e 7479   ''' The `bpy.ty
-000018b0: 7065 732e 4944 6020 6f62 6a65 6374 2074  pes.ID` object t
-000018c0: 6869 7320 6461 7461 626c 6f63 6b20 6973  his datablock is
-000018d0: 2066 726f 6d20 6f72 204e 6f6e 652c 2028   from or None, (
-000018e0: 6e6f 7420 6176 6169 6c61 626c 6520 666f  not available fo
-000018f0: 7220 616c 6c20 6461 7461 2074 7970 6573  r all data types
-00001900: 2927 2727 0a0a 2020 2020 6465 6620 6173  )'''..    def as
-00001910: 5f70 6f69 6e74 6572 2873 656c 6629 202d  _pointer(self) -
-00001920: 3e20 696e 743a 0a20 2020 2020 2020 2027  > int:.        '
-00001930: 2727 2052 6574 7572 6e73 2074 6865 206d  '' Returns the m
-00001940: 656d 6f72 7920 6164 6472 6573 7320 7768  emory address wh
-00001950: 6963 6820 686f 6c64 7320 6120 706f 696e  ich holds a poin
-00001960: 7465 7220 746f 2042 6c65 6e64 6572 2773  ter to Blender's
-00001970: 2069 6e74 6572 6e61 6c20 6461 7461 0a0a   internal data..
-00001980: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00001990: 696e 740a 2020 2020 2020 2020 3a72 6574  int.        :ret
-000019a0: 7572 6e3a 2069 6e74 2028 6d65 6d6f 7279  urn: int (memory
-000019b0: 2061 6464 7265 7373 292e 0a20 2020 2020   address)..     
-000019c0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-000019d0: 6173 730a 0a20 2020 2064 6566 2064 7269  ass..    def dri
-000019e0: 7665 725f 6164 6428 7365 6c66 2c0a 2020  ver_add(self,.  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2070 6174 683a 2074 7970 696e 672e 4f70   path: typing.Op
-00001a10: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
-00001a40: 7469 6f6e 616c 5b69 6e74 5d20 3d20 2d31  tional[int] = -1
-00001a50: 2920 2d3e 2027 4643 7572 7665 273a 0a20  ) -> 'FCurve':. 
-00001a60: 2020 2020 2020 2027 2727 2041 6464 7320         ''' Adds 
-00001a70: 6472 6976 6572 2873 2920 746f 2074 6865  driver(s) to the
-00001a80: 2067 6976 656e 2070 726f 7065 7274 790a   given property.
-00001a90: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001aa0: 7061 7468 3a20 7061 7468 2074 6f20 7468  path: path to th
-00001ab0: 6520 7072 6f70 6572 7479 2074 6f20 6472  e property to dr
-00001ac0: 6976 652c 2061 6e61 6c6f 676f 7573 2074  ive, analogous t
-00001ad0: 6f20 7468 6520 6663 7572 7665 2773 2064  o the fcurve's d
-00001ae0: 6174 6120 7061 7468 2e0a 2020 2020 2020  ata path..      
-00001af0: 2020 3a74 7970 6520 7061 7468 3a20 7479    :type path: ty
-00001b00: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00001b10: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
-00001b20: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
-00001b30: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
-00001b40: 6572 7479 2064 7269 7665 2e20 4465 6661  erty drive. Defa
-00001b50: 756c 7473 2074 6f20 2d31 2066 6f72 2061  ults to -1 for a
-00001b60: 6c6c 2069 6e64 6963 6573 206f 7220 6120  ll indices or a 
-00001b70: 7369 6e67 6c65 2063 6861 6e6e 656c 2069  single channel i
-00001b80: 6620 7468 6520 7072 6f70 6572 7479 2069  f the property i
-00001b90: 7320 6e6f 7420 616e 2061 7272 6179 2e0a  s not an array..
-00001ba0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
+00000af0: 290a 0a0a 636c 6173 7320 6270 795f 7374  )...class bpy_st
+00000b00: 7275 6374 3a0a 2020 2020 2727 2720 6275  ruct:.    ''' bu
+00000b10: 696c 742d 696e 2062 6173 6520 636c 6173  ilt-in base clas
+00000b20: 7320 666f 7220 616c 6c20 636c 6173 7365  s for all classe
+00000b30: 7320 696e 2062 7079 2e74 7970 6573 2e0a  s in bpy.types..
+00000b40: 2020 2020 2727 270a 0a20 2020 2069 645f      '''..    id_
+00000b50: 6461 7461 203d 204e 6f6e 650a 2020 2020  data = None.    
+00000b60: 2727 2720 5468 6520 6062 7079 2e74 7970  ''' The `bpy.typ
+00000b70: 6573 2e49 4460 206f 626a 6563 7420 7468  es.ID` object th
+00000b80: 6973 2064 6174 6162 6c6f 636b 2069 7320  is datablock is 
+00000b90: 6672 6f6d 206f 7220 4e6f 6e65 2c20 286e  from or None, (n
+00000ba0: 6f74 2061 7661 696c 6162 6c65 2066 6f72  ot available for
+00000bb0: 2061 6c6c 2064 6174 6120 7479 7065 7329   all data types)
+00000bc0: 2727 270a 0a20 2020 2064 6566 2061 735f  '''..    def as_
+00000bd0: 706f 696e 7465 7228 7365 6c66 2920 2d3e  pointer(self) ->
+00000be0: 2069 6e74 3a0a 2020 2020 2020 2020 2727   int:.        ''
+00000bf0: 2720 5265 7475 726e 7320 7468 6520 6d65  ' Returns the me
+00000c00: 6d6f 7279 2061 6464 7265 7373 2077 6869  mory address whi
+00000c10: 6368 2068 6f6c 6473 2061 2070 6f69 6e74  ch holds a point
+00000c20: 6572 2074 6f20 426c 656e 6465 7227 7320  er to Blender's 
+00000c30: 696e 7465 726e 616c 2064 6174 610a 0a20  internal data.. 
+00000c40: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
+00000c50: 6e74 0a20 2020 2020 2020 203a 7265 7475  nt.        :retu
+00000c60: 726e 3a20 696e 7420 286d 656d 6f72 7920  rn: int (memory 
+00000c70: 6164 6472 6573 7329 2e0a 2020 2020 2020  address)..      
+00000c80: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00000c90: 7373 0a0a 2020 2020 6465 6620 6472 6976  ss..    def driv
+00000ca0: 6572 5f61 6464 2873 656c 662c 0a20 2020  er_add(self,.   
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
+00000cd0: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000cf0: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
+00000d00: 696f 6e61 6c5b 696e 745d 203d 202d 3129  ional[int] = -1)
+00000d10: 202d 3e20 2746 4375 7276 6527 3a0a 2020   -> 'FCurve':.  
+00000d20: 2020 2020 2020 2727 2720 4164 6473 2064        ''' Adds d
+00000d30: 7269 7665 7228 7329 2074 6f20 7468 6520  river(s) to the 
+00000d40: 6769 7665 6e20 7072 6f70 6572 7479 0a0a  given property..
+00000d50: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00000d60: 6174 683a 2070 6174 6820 746f 2074 6865  ath: path to the
+00000d70: 2070 726f 7065 7274 7920 746f 2064 7269   property to dri
+00000d80: 7665 2c20 616e 616c 6f67 6f75 7320 746f  ve, analogous to
+00000d90: 2074 6865 2066 6375 7276 6527 7320 6461   the fcurve's da
+00000da0: 7461 2070 6174 682e 0a20 2020 2020 2020  ta path..       
+00000db0: 203a 7479 7065 2070 6174 683a 2074 7970   :type path: typ
+00000dc0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00000dd0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00000de0: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
+00000df0: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
+00000e00: 7274 7920 6472 6976 652e 2044 6566 6175  rty drive. Defau
+00000e10: 6c74 7320 746f 202d 3120 666f 7220 616c  lts to -1 for al
+00000e20: 6c20 696e 6469 6365 7320 6f72 2061 2073  l indices or a s
+00000e30: 696e 676c 6520 6368 616e 6e65 6c20 6966  ingle channel if
+00000e40: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+00000e50: 206e 6f74 2061 6e20 6172 7261 792e 0a20   not an array.. 
+00000e60: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
+00000e70: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+00000e80: 6e61 6c5b 696e 745d 0a20 2020 2020 2020  nal[int].       
+00000e90: 203a 7274 7970 653a 2027 4643 7572 7665   :rtype: 'FCurve
+00000ea0: 270a 2020 2020 2020 2020 3a72 6574 7572  '.        :retur
+00000eb0: 6e3a 2054 6865 2064 7269 7665 7228 7329  n: The driver(s)
+00000ec0: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
+00000ed0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00000ee0: 0a0a 2020 2020 6465 6620 6472 6976 6572  ..    def driver
+00000ef0: 5f72 656d 6f76 6528 7365 6c66 2c0a 2020  _remove(self,.  
+00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f10: 2020 2020 7061 7468 3a20 7479 7069 6e67      path: typing
+00000f20: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 696e 6465 783a 2074 7970        index: typ
+00000f50: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
+00000f60: 5d20 3d20 2d31 2920 2d3e 2062 6f6f 6c3a  ] = -1) -> bool:
+00000f70: 0a20 2020 2020 2020 2027 2727 2052 656d  .        ''' Rem
+00000f80: 6f76 6520 6472 6976 6572 2873 2920 6672  ove driver(s) fr
+00000f90: 6f6d 2074 6865 2067 6976 656e 2070 726f  om the given pro
+00000fa0: 7065 7274 790a 0a20 2020 2020 2020 203a  perty..        :
+00000fb0: 7061 7261 6d20 7061 7468 3a20 7061 7468  param path: path
+00000fc0: 2074 6f20 7468 6520 7072 6f70 6572 7479   to the property
+00000fd0: 2074 6f20 6472 6976 652c 2061 6e61 6c6f   to drive, analo
+00000fe0: 676f 7573 2074 6f20 7468 6520 6663 7572  gous to the fcur
+00000ff0: 7665 2773 2064 6174 6120 7061 7468 2e0a  ve's data path..
+00001000: 2020 2020 2020 2020 3a74 7970 6520 7061          :type pa
+00001010: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
+00001020: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
+00001030: 203a 7061 7261 6d20 696e 6465 783a 2061   :param index: a
+00001040: 7272 6179 2069 6e64 6578 206f 6620 7468  rray index of th
+00001050: 6520 7072 6f70 6572 7479 2064 7269 7665  e property drive
+00001060: 2e20 4465 6661 756c 7473 2074 6f20 2d31  . Defaults to -1
+00001070: 2066 6f72 2061 6c6c 2069 6e64 6963 6573   for all indices
+00001080: 206f 7220 6120 7369 6e67 6c65 2063 6861   or a single cha
+00001090: 6e6e 656c 2069 6620 7468 6520 7072 6f70  nnel if the prop
+000010a0: 6572 7479 2069 7320 6e6f 7420 616e 2061  erty is not an a
+000010b0: 7272 6179 2e0a 2020 2020 2020 2020 3a74  rray..        :t
+000010c0: 7970 6520 696e 6465 783a 2074 7970 696e  ype index: typin
+000010d0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d0a  g.Optional[int].
+000010e0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000010f0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+00001100: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
+00001110: 2064 7269 7665 7220 7265 6d6f 7661 6c2e   driver removal.
+00001120: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00001130: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00001140: 6566 2067 6574 2873 656c 662c 0a20 2020  ef get(self,.   
+00001150: 2020 2020 2020 2020 206b 6579 3a20 7479           key: ty
+00001160: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00001170: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
+00001180: 6465 6661 756c 743a 2074 7970 696e 672e  default: typing.
+00001190: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+000011a0: 416e 795d 203d 204e 6f6e 6529 3a0a 2020  Any] = None):.  
+000011b0: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+000011c0: 7320 7468 6520 7661 6c75 6520 6f66 2074  s the value of t
+000011d0: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
+000011e0: 7479 2061 7373 6967 6e65 6420 746f 206b  ty assigned to k
+000011f0: 6579 206f 7220 6465 6661 756c 7420 7768  ey or default wh
+00001200: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
+00001210: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
+00001220: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
+00001230: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
+00001240: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
+00001250: 7061 7261 6d20 6b65 793a 2054 6865 206b  param key: The k
+00001260: 6579 2061 7373 6f63 6961 7465 6420 7769  ey associated wi
+00001270: 7468 2074 6865 2063 7573 746f 6d20 7072  th the custom pr
+00001280: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
+00001290: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+000012a0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+000012b0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+000012c0: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
+000012d0: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
+000012e0: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
+000012f0: 6e20 6966 202a 6b65 792a 2069 7320 6e6f  n if *key* is no
+00001300: 7420 666f 756e 642e 0a20 2020 2020 2020  t found..       
+00001310: 203a 7479 7065 2064 6566 6175 6c74 3a20   :type default: 
+00001320: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001330: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
+00001340: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001350: 7061 7373 0a0a 2020 2020 6465 6620 6964  pass..    def id
+00001360: 5f70 726f 7065 7274 6965 735f 636c 6561  _properties_clea
+00001370: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00001380: 2027 2727 200a 0a20 2020 2020 2020 2027   ''' ..        '
+00001390: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000013a0: 0a20 2020 2064 6566 2069 645f 7072 6f70  .    def id_prop
+000013b0: 6572 7469 6573 5f65 6e73 7572 6528 7365  erties_ensure(se
+000013c0: 6c66 2920 2d3e 2074 7970 696e 672e 416e  lf) -> typing.An
+000013d0: 793a 0a20 2020 2020 2020 2027 2727 200a  y:.        ''' .
+000013e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000013f0: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
+00001400: 2020 2020 3a72 6574 7572 6e3a 2074 6865      :return: the
+00001410: 2070 6172 656e 7420 6772 6f75 7020 666f   parent group fo
+00001420: 7220 616e 2052 4e41 2073 7472 7563 7427  r an RNA struct'
+00001430: 7320 6375 7374 6f6d 2049 4450 726f 7065  s custom IDPrope
+00001440: 7274 6965 732e 0a20 2020 2020 2020 2027  rties..        '
+00001450: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001460: 0a20 2020 2064 6566 2069 645f 7072 6f70  .    def id_prop
+00001470: 6572 7469 6573 5f75 6928 7365 6c66 2c20  erties_ui(self, 
+00001480: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
+00001490: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
+000014a0: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
+000014b0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000014c0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+000014d0: 793a 2020 5374 7269 6e67 206e 616d 6520  y:  String name 
+000014e0: 6f66 2074 6865 2070 726f 7065 7274 792e  of the property.
+000014f0: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
+00001500: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
+00001510: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
+00001520: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00001530: 7479 7069 6e67 2e41 6e79 0a20 2020 2020  typing.Any.     
+00001540: 2020 203a 7265 7475 726e 3a20 5265 7475     :return: Retu
+00001550: 726e 2061 6e20 6f62 6a65 6374 2075 7365  rn an object use
+00001560: 6420 746f 206d 616e 6167 6520 616e 2049  d to manage an I
+00001570: 4450 726f 7065 7274 7927 7320 5549 2064  DProperty's UI d
+00001580: 6174 612e 0a20 2020 2020 2020 2027 2727  ata..        '''
+00001590: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000015a0: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+000015b0: 7479 5f68 6964 6465 6e28 7365 6c66 2c20  ty_hidden(self, 
+000015c0: 7072 6f70 6572 7479 2920 2d3e 2062 6f6f  property) -> boo
+000015d0: 6c3a 0a20 2020 2020 2020 2027 2727 2043  l:.        ''' C
+000015e0: 6865 636b 2069 6620 6120 7072 6f70 6572  heck if a proper
+000015f0: 7479 2069 7320 6869 6464 656e 2e0a 0a20  ty is hidden... 
+00001600: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00001610: 6f6f 6c0a 2020 2020 2020 2020 3a72 6574  ool.        :ret
+00001620: 7572 6e3a 2054 7275 6520 7768 656e 2074  urn: True when t
+00001630: 6865 2070 726f 7065 7274 7920 6973 2068  he property is h
+00001640: 6964 6465 6e2e 0a20 2020 2020 2020 2027  idden..        '
+00001650: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001660: 0a20 2020 2064 6566 2069 735f 7072 6f70  .    def is_prop
+00001670: 6572 7479 5f6f 7665 7272 6964 6162 6c65  erty_overridable
+00001680: 5f6c 6962 7261 7279 2873 656c 662c 2070  _library(self, p
+00001690: 726f 7065 7274 7929 202d 3e20 626f 6f6c  roperty) -> bool
+000016a0: 3a0a 2020 2020 2020 2020 2727 2720 4368  :.        ''' Ch
+000016b0: 6563 6b20 6966 2061 2070 726f 7065 7274  eck if a propert
+000016c0: 7920 6973 206f 7665 7272 6964 6162 6c65  y is overridable
+000016d0: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+000016e0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+000016f0: 3a72 6574 7572 6e3a 2054 7275 6520 7768  :return: True wh
+00001700: 656e 2074 6865 2070 726f 7065 7274 7920  en the property 
+00001710: 6973 206f 7665 7272 6964 6162 6c65 2e0a  is overridable..
+00001720: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001730: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00001740: 6620 6973 5f70 726f 7065 7274 795f 7265  f is_property_re
+00001750: 6164 6f6e 6c79 2873 656c 662c 2070 726f  adonly(self, pro
+00001760: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
+00001770: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
+00001780: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
+00001790: 6973 2072 6561 646f 6e6c 792e 0a0a 2020  is readonly...  
+000017a0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+000017b0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+000017c0: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
+000017d0: 6520 7072 6f70 6572 7479 2069 7320 7265  e property is re
+000017e0: 6164 6f6e 6c79 2028 6e6f 7420 7772 6974  adonly (not writ
+000017f0: 6162 6c65 292e 0a20 2020 2020 2020 2027  able)..        '
+00001800: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00001810: 0a20 2020 2064 6566 2069 735f 7072 6f70  .    def is_prop
+00001820: 6572 7479 5f73 6574 2873 656c 662c 2070  erty_set(self, p
+00001830: 726f 7065 7274 792c 0a20 2020 2020 2020  roperty,.       
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2067 686f 7374 3a20 7479 7069 6e67 2e4f   ghost: typing.O
+00001860: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00001870: 5472 7565 2920 2d3e 2062 6f6f 6c3a 0a20  True) -> bool:. 
+00001880: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
+00001890: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
+000018a0: 7320 7365 742c 2075 7365 2066 6f72 2074  s set, use for t
+000018b0: 6573 7469 6e67 206f 7065 7261 746f 7220  esting operator 
+000018c0: 7072 6f70 6572 7469 6573 2e0a 0a20 2020  properties...   
+000018d0: 2020 2020 203a 7061 7261 6d20 6768 6f73       :param ghos
+000018e0: 743a 2055 7365 6420 666f 7220 6f70 6572  t: Used for oper
+000018f0: 6174 6f72 7320 7468 6174 2072 652d 7275  ators that re-ru
+00001900: 6e20 7769 7468 2070 7265 7669 6f75 7320  n with previous 
+00001910: 7365 7474 696e 6773 2e20 496e 2074 6869  settings. In thi
+00001920: 7320 6361 7365 2074 6865 2070 726f 7065  s case the prope
+00001930: 7274 7920 6973 206e 6f74 206d 6172 6b65  rty is not marke
+00001940: 6420 6173 2073 6574 2c20 7965 7420 7468  d as set, yet th
+00001950: 6520 7661 6c75 6520 6672 6f6d 2074 6865  e value from the
+00001960: 2070 7265 7669 6f75 7320 6578 6563 7574   previous execut
+00001970: 696f 6e20 6973 2075 7365 642e 2049 6e20  ion is used. In 
+00001980: 7261 7265 2063 6173 6573 2079 6f75 206d  rare cases you m
+00001990: 6179 2077 616e 7420 746f 2073 6574 2074  ay want to set t
+000019a0: 6869 7320 6f70 7469 6f6e 2074 6f20 6661  his option to fa
+000019b0: 6c73 652e 0a20 2020 2020 2020 203a 7479  lse..        :ty
+000019c0: 7065 2067 686f 7374 3a20 7479 7069 6e67  pe ghost: typing
+000019d0: 2e4f 7074 696f 6e61 6c5b 626f 6f6c 5d0a  .Optional[bool].
+000019e0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000019f0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+00001a00: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
+00001a10: 7468 6520 7072 6f70 6572 7479 2068 6173  the property has
+00001a20: 2062 6565 6e20 7365 742e 0a20 2020 2020   been set..     
+00001a30: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+00001a40: 6173 730a 0a20 2020 2064 6566 2069 7465  ass..    def ite
+00001a50: 6d73 2873 656c 6629 202d 3e20 7479 7069  ms(self) -> typi
+00001a60: 6e67 2e41 6e79 3a0a 2020 2020 2020 2020  ng.Any:.        
+00001a70: 2727 2720 5265 7475 726e 7320 7468 6520  ''' Returns the 
+00001a80: 6974 656d 7320 6f66 2074 6869 7320 6f62  items of this ob
+00001a90: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
+00001aa0: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
+00001ab0: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
+00001ac0: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
+00001ad0: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+00001ae0: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00001af0: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
+00001b00: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
+00001b10: 7374 6f6d 2070 726f 7065 7274 7920 6b65  stom property ke
+00001b20: 792c 2076 616c 7565 2070 6169 7273 2e0a  y, value pairs..
+00001b30: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00001b40: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00001b50: 6620 6b65 7966 7261 6d65 5f64 656c 6574  f keyframe_delet
+00001b60: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
+00001b70: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00001b80: 2064 6174 615f 7061 7468 3a20 7479 7069   data_path: typi
+00001b90: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00001ba0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
 00001bb0: 6465 783a 2074 7970 696e 672e 4f70 7469  dex: typing.Opti
-00001bc0: 6f6e 616c 5b69 6e74 5d0a 2020 2020 2020  onal[int].      
-00001bd0: 2020 3a72 7479 7065 3a20 2746 4375 7276    :rtype: 'FCurv
-00001be0: 6527 0a20 2020 2020 2020 203a 7265 7475  e'.        :retu
-00001bf0: 726e 3a20 5468 6520 6472 6976 6572 2873  rn: The driver(s
-00001c00: 2920 6164 6465 642e 0a20 2020 2020 2020  ) added..       
-00001c10: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00001c20: 730a 0a20 2020 2064 6566 2064 7269 7665  s..    def drive
-00001c30: 725f 7265 6d6f 7665 2873 656c 662c 0a20  r_remove(self,. 
-00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c50: 2020 2020 2070 6174 683a 2074 7970 696e       path: typin
-00001c60: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
-00001c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001c80: 2020 2020 2020 2069 6e64 6578 3a20 7479         index: ty
-00001c90: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00001ca0: 745d 203d 202d 3129 202d 3e20 626f 6f6c  t] = -1) -> bool
-00001cb0: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00001cc0: 6d6f 7665 2064 7269 7665 7228 7329 2066  move driver(s) f
-00001cd0: 726f 6d20 7468 6520 6769 7665 6e20 7072  rom the given pr
-00001ce0: 6f70 6572 7479 0a0a 2020 2020 2020 2020  operty..        
-00001cf0: 3a70 6172 616d 2070 6174 683a 2070 6174  :param path: pat
-00001d00: 6820 746f 2074 6865 2070 726f 7065 7274  h to the propert
-00001d10: 7920 746f 2064 7269 7665 2c20 616e 616c  y to drive, anal
-00001d20: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
-00001d30: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
-00001d40: 0a20 2020 2020 2020 203a 7479 7065 2070  .        :type p
-00001d50: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
-00001d60: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
-00001d70: 2020 3a70 6172 616d 2069 6e64 6578 3a20    :param index: 
-00001d80: 6172 7261 7920 696e 6465 7820 6f66 2074  array index of t
-00001d90: 6865 2070 726f 7065 7274 7920 6472 6976  he property driv
-00001da0: 652e 2044 6566 6175 6c74 7320 746f 202d  e. Defaults to -
-00001db0: 3120 666f 7220 616c 6c20 696e 6469 6365  1 for all indice
-00001dc0: 7320 6f72 2061 2073 696e 676c 6520 6368  s or a single ch
-00001dd0: 616e 6e65 6c20 6966 2074 6865 2070 726f  annel if the pro
-00001de0: 7065 7274 7920 6973 206e 6f74 2061 6e20  perty is not an 
-00001df0: 6172 7261 792e 0a20 2020 2020 2020 203a  array..        :
-00001e00: 7479 7065 2069 6e64 6578 3a20 7479 7069  type index: typi
-00001e10: 6e67 2e4f 7074 696f 6e61 6c5b 696e 745d  ng.Optional[int]
-00001e20: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00001e30: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
-00001e40: 6574 7572 6e3a 2053 7563 6365 7373 206f  eturn: Success o
-00001e50: 6620 6472 6976 6572 2072 656d 6f76 616c  f driver removal
-00001e60: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00001e70: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001e80: 6465 6620 6765 7428 7365 6c66 2c0a 2020  def get(self,.  
-00001e90: 2020 2020 2020 2020 2020 6b65 793a 2074            key: t
-00001ea0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00001eb0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00001ec0: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
-00001ed0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00001ee0: 2e41 6e79 5d20 3d20 4e6f 6e65 293a 0a20  .Any] = None):. 
-00001ef0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-00001f00: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
-00001f10: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
-00001f20: 7274 7920 6173 7369 676e 6564 2074 6f20  rty assigned to 
-00001f30: 6b65 7920 6f72 2064 6566 6175 6c74 2077  key or default w
-00001f40: 6865 6e20 6e6f 7420 666f 756e 6420 286d  hen not found (m
-00001f50: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
-00001f60: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
-00001f70: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
-00001f80: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
-00001f90: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
-00001fa0: 6b65 7920 6173 736f 6369 6174 6564 2077  key associated w
-00001fb0: 6974 6820 7468 6520 6375 7374 6f6d 2070  ith the custom p
-00001fc0: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
-00001fd0: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
-00001fe0: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00001ff0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002000: 6465 6661 756c 743a 204f 7074 696f 6e61  default: Optiona
-00002010: 6c20 6172 6775 6d65 6e74 2066 6f72 2074  l argument for t
-00002020: 6865 2076 616c 7565 2074 6f20 7265 7475  he value to retu
-00002030: 726e 2069 6620 2a6b 6579 2a20 6973 206e  rn if *key* is n
-00002040: 6f74 2066 6f75 6e64 2e0a 2020 2020 2020  ot found..      
-00002050: 2020 3a74 7970 6520 6465 6661 756c 743a    :type default:
-00002060: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002070: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
-00002080: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002090: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-000020a0: 645f 7072 6f70 6572 7469 6573 5f63 6c65  d_properties_cle
-000020b0: 6172 2873 656c 6629 3a0a 2020 2020 2020  ar(self):.      
-000020c0: 2020 2727 2720 0a0a 2020 2020 2020 2020    ''' ..        
-000020d0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000020e0: 0a0a 2020 2020 6465 6620 6964 5f70 726f  ..    def id_pro
-000020f0: 7065 7274 6965 735f 656e 7375 7265 2873  perties_ensure(s
-00002100: 656c 6629 202d 3e20 7479 7069 6e67 2e41  elf) -> typing.A
-00002110: 6e79 3a0a 2020 2020 2020 2020 2727 2720  ny:.        ''' 
-00002120: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00002130: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
-00002140: 2020 2020 203a 7265 7475 726e 3a20 7468       :return: th
-00002150: 6520 7061 7265 6e74 2067 726f 7570 2066  e parent group f
-00002160: 6f72 2061 6e20 524e 4120 7374 7275 6374  or an RNA struct
-00002170: 2773 2063 7573 746f 6d20 4944 5072 6f70  's custom IDProp
-00002180: 6572 7469 6573 2e0a 2020 2020 2020 2020  erties..        
-00002190: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000021a0: 0a0a 2020 2020 6465 6620 6964 5f70 726f  ..    def id_pro
-000021b0: 7065 7274 6965 735f 7569 2873 656c 662c  perties_ui(self,
-000021c0: 206b 6579 3a20 7479 7069 6e67 2e4f 7074   key: typing.Opt
-000021d0: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
-000021e0: 5d29 202d 3e20 7479 7069 6e67 2e41 6e79  ]) -> typing.Any
-000021f0: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
-00002200: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00002210: 6579 3a20 2053 7472 696e 6720 6e61 6d65  ey:  String name
-00002220: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00002230: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00002240: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
-00002250: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
-00002260: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002270: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
-00002280: 2020 2020 3a72 6574 7572 6e3a 2052 6574      :return: Ret
-00002290: 7572 6e20 616e 206f 626a 6563 7420 7573  urn an object us
-000022a0: 6564 2074 6f20 6d61 6e61 6765 2061 6e20  ed to manage an 
-000022b0: 4944 5072 6f70 6572 7479 2773 2055 4920  IDProperty's UI 
-000022c0: 6461 7461 2e0a 2020 2020 2020 2020 2727  data..        ''
-000022d0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-000022e0: 2020 2020 6465 6620 6973 5f70 726f 7065      def is_prope
-000022f0: 7274 795f 6869 6464 656e 2873 656c 662c  rty_hidden(self,
-00002300: 2070 726f 7065 7274 7929 202d 3e20 626f   property) -> bo
-00002310: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
-00002320: 4368 6563 6b20 6966 2061 2070 726f 7065  Check if a prope
-00002330: 7274 7920 6973 2068 6964 6465 6e2e 0a0a  rty is hidden...
-00002340: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00002350: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
-00002360: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
-00002370: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
-00002380: 6869 6464 656e 2e0a 2020 2020 2020 2020  hidden..        
-00002390: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000023a0: 0a0a 2020 2020 6465 6620 6973 5f70 726f  ..    def is_pro
-000023b0: 7065 7274 795f 6f76 6572 7269 6461 626c  perty_overridabl
-000023c0: 655f 6c69 6272 6172 7928 7365 6c66 2c20  e_library(self, 
-000023d0: 7072 6f70 6572 7479 2920 2d3e 2062 6f6f  property) -> boo
-000023e0: 6c3a 0a20 2020 2020 2020 2027 2727 2043  l:.        ''' C
-000023f0: 6865 636b 2069 6620 6120 7072 6f70 6572  heck if a proper
-00002400: 7479 2069 7320 6f76 6572 7269 6461 626c  ty is overridabl
-00002410: 652e 0a0a 2020 2020 2020 2020 3a72 7479  e...        :rty
-00002420: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-00002430: 203a 7265 7475 726e 3a20 5472 7565 2077   :return: True w
-00002440: 6865 6e20 7468 6520 7072 6f70 6572 7479  hen the property
-00002450: 2069 7320 6f76 6572 7269 6461 626c 652e   is overridable.
-00002460: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00002470: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00002480: 6566 2069 735f 7072 6f70 6572 7479 5f72  ef is_property_r
-00002490: 6561 646f 6e6c 7928 7365 6c66 2c20 7072  eadonly(self, pr
-000024a0: 6f70 6572 7479 2920 2d3e 2062 6f6f 6c3a  operty) -> bool:
-000024b0: 0a20 2020 2020 2020 2027 2727 2043 6865  .        ''' Che
-000024c0: 636b 2069 6620 6120 7072 6f70 6572 7479  ck if a property
-000024d0: 2069 7320 7265 6164 6f6e 6c79 2e0a 0a20   is readonly... 
-000024e0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-000024f0: 6f6f 6c0a 2020 2020 2020 2020 3a72 6574  ool.        :ret
-00002500: 7572 6e3a 2054 7275 6520 7768 656e 2074  urn: True when t
-00002510: 6865 2070 726f 7065 7274 7920 6973 2072  he property is r
-00002520: 6561 646f 6e6c 7920 286e 6f74 2077 7269  eadonly (not wri
-00002530: 7461 626c 6529 2e0a 2020 2020 2020 2020  table)..        
-00002540: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00002550: 0a0a 2020 2020 6465 6620 6973 5f70 726f  ..    def is_pro
-00002560: 7065 7274 795f 7365 7428 7365 6c66 2c20  perty_set(self, 
-00002570: 7072 6f70 6572 7479 2c0a 2020 2020 2020  property,.      
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 6768 6f73 743a 2074 7970 696e 672e    ghost: typing.
-000025a0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-000025b0: 2054 7275 6529 202d 3e20 626f 6f6c 3a0a   True) -> bool:.
-000025c0: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
-000025d0: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
-000025e0: 6973 2073 6574 2c20 7573 6520 666f 7220  is set, use for 
-000025f0: 7465 7374 696e 6720 6f70 6572 6174 6f72  testing operator
-00002600: 2070 726f 7065 7274 6965 732e 0a0a 2020   properties...  
-00002610: 2020 2020 2020 3a70 6172 616d 2067 686f        :param gho
-00002620: 7374 3a20 5573 6564 2066 6f72 206f 7065  st: Used for ope
-00002630: 7261 746f 7273 2074 6861 7420 7265 2d72  rators that re-r
-00002640: 756e 2077 6974 6820 7072 6576 696f 7573  un with previous
-00002650: 2073 6574 7469 6e67 732e 2049 6e20 7468   settings. In th
-00002660: 6973 2063 6173 6520 7468 6520 7072 6f70  is case the prop
-00002670: 6572 7479 2069 7320 6e6f 7420 6d61 726b  erty is not mark
-00002680: 6564 2061 7320 7365 742c 2079 6574 2074  ed as set, yet t
-00002690: 6865 2076 616c 7565 2066 726f 6d20 7468  he value from th
-000026a0: 6520 7072 6576 696f 7573 2065 7865 6375  e previous execu
-000026b0: 7469 6f6e 2069 7320 7573 6564 2e20 496e  tion is used. In
-000026c0: 2072 6172 6520 6361 7365 7320 796f 7520   rare cases you 
-000026d0: 6d61 7920 7761 6e74 2074 6f20 7365 7420  may want to set 
-000026e0: 7468 6973 206f 7074 696f 6e20 746f 2066  this option to f
-000026f0: 616c 7365 2e0a 2020 2020 2020 2020 3a74  alse..        :t
-00002700: 7970 6520 6768 6f73 743a 2074 7970 696e  ype ghost: typin
-00002710: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
-00002720: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002730: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
-00002740: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
-00002750: 2074 6865 2070 726f 7065 7274 7920 6861   the property ha
-00002760: 7320 6265 656e 2073 6574 2e0a 2020 2020  s been set..    
-00002770: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00002780: 7061 7373 0a0a 2020 2020 6465 6620 6974  pass..    def it
-00002790: 656d 7328 7365 6c66 2920 2d3e 2074 7970  ems(self) -> typ
-000027a0: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
-000027b0: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
-000027c0: 2069 7465 6d73 206f 6620 7468 6973 206f   items of this o
-000027d0: 626a 6563 7473 2063 7573 746f 6d20 7072  bjects custom pr
-000027e0: 6f70 6572 7469 6573 2028 6d61 7463 6865  operties (matche
-000027f0: 7320 5079 7468 6f6e 2773 2064 6963 7469  s Python's dicti
-00002800: 6f6e 6172 7920 6675 6e63 7469 6f6e 206f  onary function o
-00002810: 6620 7468 6520 7361 6d65 206e 616d 6529  f the same name)
-00002820: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
-00002830: 653a 2074 7970 696e 672e 416e 790a 2020  e: typing.Any.  
-00002840: 2020 2020 2020 3a72 6574 7572 6e3a 2063        :return: c
-00002850: 7573 746f 6d20 7072 6f70 6572 7479 206b  ustom property k
-00002860: 6579 2c20 7661 6c75 6520 7061 6972 732e  ey, value pairs.
-00002870: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00002880: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00002890: 6566 206b 6579 6672 616d 655f 6465 6c65  ef keyframe_dele
-000028a0: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-000028b0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-000028c0: 2020 6461 7461 5f70 6174 683a 2074 7970    data_path: typ
-000028d0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-000028e0: 5d2c 0a20 2020 2020 2020 2020 2020 2069  ],.            i
-000028f0: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
-00002900: 696f 6e61 6c5b 696e 745d 203d 202d 312c  ional[int] = -1,
-00002910: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
-00002920: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
-00002930: 6e61 6c5b 666c 6f61 745d 203d 2027 6270  nal[float] = 'bp
-00002940: 792e 636f 6e74 6578 742e 7363 656e 652e  y.context.scene.
-00002950: 6672 616d 655f 6375 7272 656e 7427 2c0a  frame_current',.
-00002960: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-00002970: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
-00002980: 616c 5b73 7472 5d20 3d20 2222 2920 2d3e  al[str] = "") ->
-00002990: 2062 6f6f 6c3a 0a20 2020 2020 2020 2027   bool:.        '
-000029a0: 2727 2052 656d 6f76 6520 6120 6b65 7966  '' Remove a keyf
-000029b0: 7261 6d65 2066 726f 6d20 7468 6973 2070  rame from this p
-000029c0: 726f 7065 7274 6965 7320 6663 7572 7665  roperties fcurve
-000029d0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000029e0: 6d20 6461 7461 5f70 6174 683a 2070 6174  m data_path: pat
-000029f0: 6820 746f 2074 6865 2070 726f 7065 7274  h to the propert
-00002a00: 7920 746f 2072 656d 6f76 6520 6120 6b65  y to remove a ke
-00002a10: 792c 2061 6e61 6c6f 676f 7573 2074 6f20  y, analogous to 
-00002a20: 7468 6520 6663 7572 7665 2773 2064 6174  the fcurve's dat
-00002a30: 6120 7061 7468 2e0a 2020 2020 2020 2020  a path..        
-00002a40: 3a74 7970 6520 6461 7461 5f70 6174 683a  :type data_path:
-00002a50: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002a60: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
-00002a70: 6172 616d 2069 6e64 6578 3a20 6172 7261  aram index: arra
-00002a80: 7920 696e 6465 7820 6f66 2074 6865 2070  y index of the p
-00002a90: 726f 7065 7274 7920 746f 2072 656d 6f76  roperty to remov
-00002aa0: 6520 6120 6b65 792e 2044 6566 6175 6c74  e a key. Default
-00002ab0: 7320 746f 202d 3120 7265 6d6f 7669 6e67  s to -1 removing
-00002ac0: 2061 6c6c 2069 6e64 6963 6573 206f 7220   all indices or 
-00002ad0: 6120 7369 6e67 6c65 2063 6861 6e6e 656c  a single channel
-00002ae0: 2069 6620 7468 6520 7072 6f70 6572 7479   if the property
-00002af0: 2069 7320 6e6f 7420 616e 2061 7272 6179   is not an array
-00002b00: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00002b10: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
-00002b20: 7469 6f6e 616c 5b69 6e74 5d0a 2020 2020  tional[int].    
-00002b30: 2020 2020 3a70 6172 616d 2066 7261 6d65      :param frame
-00002b40: 3a20 5468 6520 6672 616d 6520 6f6e 2077  : The frame on w
-00002b50: 6869 6368 2074 6865 206b 6579 6672 616d  hich the keyfram
-00002b60: 6520 6973 2064 656c 6574 6564 2c20 6465  e is deleted, de
-00002b70: 6661 756c 7469 6e67 2074 6f20 7468 6520  faulting to the 
-00002b80: 6375 7272 656e 7420 6672 616d 652e 0a20  current frame.. 
-00002b90: 2020 2020 2020 203a 7479 7065 2066 7261         :type fra
-00002ba0: 6d65 3a20 7479 7069 6e67 2e4f 7074 696f  me: typing.Optio
-00002bb0: 6e61 6c5b 666c 6f61 745d 0a20 2020 2020  nal[float].     
-00002bc0: 2020 203a 7061 7261 6d20 6772 6f75 703a     :param group:
-00002bd0: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00002be0: 2067 726f 7570 2074 6865 2046 2d43 7572   group the F-Cur
-00002bf0: 7665 2073 686f 756c 6420 6265 2061 6464  ve should be add
-00002c00: 6564 2074 6f20 6966 2069 7420 646f 6573  ed to if it does
-00002c10: 6e27 7420 6578 6973 7420 7965 742e 0a20  n't exist yet.. 
-00002c20: 2020 2020 2020 203a 7479 7065 2067 726f         :type gro
-00002c30: 7570 3a20 7479 7069 6e67 2e4f 7074 696f  up: typing.Optio
-00002c40: 6e61 6c5b 7374 725d 0a20 2020 2020 2020  nal[str].       
-00002c50: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00002c60: 2020 2020 2020 3a72 6574 7572 6e3a 2053        :return: S
-00002c70: 7563 6365 7373 206f 6620 6b65 7966 7261  uccess of keyfra
-00002c80: 6d65 2064 656c 6574 696f 6e2e 0a20 2020  me deletion..   
-00002c90: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00002ca0: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
-00002cb0: 6579 6672 616d 655f 696e 7365 7274 280a  eyframe_insert(.
-00002cc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002cd0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00002ce0: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
-00002cf0: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
-00002d00: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00002d10: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002d20: 6c5b 696e 745d 203d 202d 312c 0a20 2020  l[int] = -1,.   
-00002d30: 2020 2020 2020 2020 2066 7261 6d65 3a20           frame: 
-00002d40: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002d50: 666c 6f61 745d 203d 2027 6270 792e 636f  float] = 'bpy.co
-00002d60: 6e74 6578 742e 7363 656e 652e 6672 616d  ntext.scene.fram
-00002d70: 655f 6375 7272 656e 7427 2c0a 2020 2020  e_current',.    
-00002d80: 2020 2020 2020 2020 6772 6f75 703a 2074          group: t
-00002d90: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00002da0: 7472 5d20 3d20 2222 2c0a 2020 2020 2020  tr] = "",.      
-00002db0: 2020 2020 2020 6f70 7469 6f6e 733a 2074        options: t
-00002dc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00002dd0: 7970 696e 672e 416e 795d 203d 2027 7365  yping.Any] = 'se
-00002de0: 7428 2927 2920 2d3e 2062 6f6f 6c3a 0a20  t()') -> bool:. 
-00002df0: 2020 2020 2020 2027 2727 2049 6e73 6572         ''' Inser
-00002e00: 7420 6120 6b65 7966 7261 6d65 206f 6e20  t a keyframe on 
-00002e10: 7468 6520 7072 6f70 6572 7479 2067 6976  the property giv
-00002e20: 656e 2c20 6164 6469 6e67 2066 6375 7276  en, adding fcurv
-00002e30: 6573 2061 6e64 2061 6e69 6d61 7469 6f6e  es and animation
-00002e40: 2064 6174 6120 7768 656e 206e 6563 6573   data when neces
-00002e50: 7361 7279 2e20 5468 6973 2069 7320 7468  sary. This is th
-00002e60: 6520 6d6f 7374 2073 696d 706c 6520 6578  e most simple ex
-00002e70: 616d 706c 6520 6f66 2069 6e73 6572 7469  ample of inserti
-00002e80: 6e67 2061 206b 6579 6672 616d 6520 6672  ng a keyframe fr
-00002e90: 6f6d 2070 7974 686f 6e2e 204e 6f74 6520  om python. Note 
-00002ea0: 7468 6174 2077 6865 6e20 6b65 7969 6e67  that when keying
-00002eb0: 2064 6174 6120 7061 7468 7320 7768 6963   data paths whic
-00002ec0: 6820 636f 6e74 6169 6e20 6e65 7374 6564  h contain nested
-00002ed0: 2070 726f 7065 7274 6965 7320 7468 6973   properties this
-00002ee0: 206d 7573 7420 6265 2064 6f6e 6520 6672   must be done fr
-00002ef0: 6f6d 2074 6865 2060 4944 6020 7375 6263  om the `ID` subc
-00002f00: 6c61 7373 2c20 696e 2074 6869 7320 6361  lass, in this ca
-00002f10: 7365 2074 6865 2060 4172 6d61 7475 7265  se the `Armature
-00002f20: 6020 7261 7468 6572 2074 6861 6e20 7468  ` rather than th
-00002f30: 6520 626f 6e65 2e0a 0a20 2020 2020 2020  e bone...       
-00002f40: 203a 7061 7261 6d20 6461 7461 5f70 6174   :param data_pat
-00002f50: 683a 2070 6174 6820 746f 2074 6865 2070  h: path to the p
-00002f60: 726f 7065 7274 7920 746f 206b 6579 2c20  roperty to key, 
-00002f70: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
-00002f80: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
-00002f90: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
-00002fa0: 7065 2064 6174 615f 7061 7468 3a20 7479  pe data_path: ty
-00002fb0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00002fc0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
-00002fd0: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
-00002fe0: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
-00002ff0: 6572 7479 2074 6f20 6b65 792e 2044 6566  erty to key. Def
-00003000: 6175 6c74 7320 746f 202d 3120 7768 6963  aults to -1 whic
-00003010: 6820 7769 6c6c 206b 6579 2061 6c6c 2069  h will key all i
-00003020: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
-00003030: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
-00003040: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
-00003050: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
-00003060: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
-00003070: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00003080: 5b69 6e74 5d0a 2020 2020 2020 2020 3a70  [int].        :p
-00003090: 6172 616d 2066 7261 6d65 3a20 5468 6520  aram frame: The 
-000030a0: 6672 616d 6520 6f6e 2077 6869 6368 2074  frame on which t
-000030b0: 6865 206b 6579 6672 616d 6520 6973 2069  he keyframe is i
-000030c0: 6e73 6572 7465 642c 2064 6566 6175 6c74  nserted, default
-000030d0: 696e 6720 746f 2074 6865 2063 7572 7265  ing to the curre
-000030e0: 6e74 2066 7261 6d65 2e0a 2020 2020 2020  nt frame..      
-000030f0: 2020 3a74 7970 6520 6672 616d 653a 2074    :type frame: t
-00003100: 7970 696e 672e 4f70 7469 6f6e 616c 5b66  yping.Optional[f
-00003110: 6c6f 6174 5d0a 2020 2020 2020 2020 3a70  loat].        :p
-00003120: 6172 616d 2067 726f 7570 3a20 5468 6520  aram group: The 
-00003130: 6e61 6d65 206f 6620 7468 6520 6772 6f75  name of the grou
-00003140: 7020 7468 6520 462d 4375 7276 6520 7368  p the F-Curve sh
-00003150: 6f75 6c64 2062 6520 6164 6465 6420 746f  ould be added to
-00003160: 2069 6620 6974 2064 6f65 736e 2774 2065   if it doesn't e
-00003170: 7869 7374 2079 6574 2e0a 2020 2020 2020  xist yet..      
-00003180: 2020 3a74 7970 6520 6772 6f75 703a 2074    :type group: t
-00003190: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-000031a0: 7472 5d0a 2020 2020 2020 2020 3a70 6172  tr].        :par
-000031b0: 616d 2066 6c61 673a 200a 2020 2020 2020  am flag: .      
-000031c0: 2020 3a74 7970 6520 666c 6167 3a20 7479    :type flag: ty
-000031d0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-000031e0: 7069 6e67 2e53 6574 5d0a 2020 2020 2020  ping.Set].      
-000031f0: 2020 3a70 6172 616d 206f 7074 696f 6e73    :param options
-00003200: 3a20 202d 2060 6049 4e53 4552 544b 4559  :  - ``INSERTKEY
-00003210: 5f4e 4545 4445 4460 6020 4f6e 6c79 2069  _NEEDED`` Only i
-00003220: 6e73 6572 7420 6b65 7966 7261 6d65 7320  nsert keyframes 
-00003230: 7768 6572 6520 7468 6579 2772 6520 6e65  where they're ne
-00003240: 6564 6564 2069 6e20 7468 6520 7265 6c65  eded in the rele
-00003250: 7661 6e74 2046 2d43 7572 7665 732e 202d  vant F-Curves. -
-00003260: 2060 6049 4e53 4552 544b 4559 5f56 4953   ``INSERTKEY_VIS
-00003270: 5541 4c60 6020 496e 7365 7274 206b 6579  UAL`` Insert key
-00003280: 6672 616d 6573 2062 6173 6564 206f 6e20  frames based on 
-00003290: 2776 6973 7561 6c20 7472 616e 7366 6f72  'visual transfor
-000032a0: 6d73 272e 202d 2060 6049 4e53 4552 544b  ms'. - ``INSERTK
-000032b0: 4559 5f58 595a 5f54 4f5f 5247 4260 6020  EY_XYZ_TO_RGB`` 
-000032c0: 436f 6c6f 7220 666f 7220 6e65 776c 7920  Color for newly 
-000032d0: 6164 6465 6420 7472 616e 7366 6f72 6d61  added transforma
-000032e0: 7469 6f6e 2046 2d43 7572 7665 7320 284c  tion F-Curves (L
-000032f0: 6f63 6174 696f 6e2c 2052 6f74 6174 696f  ocation, Rotatio
-00003300: 6e2c 2053 6361 6c65 2920 6973 2062 6173  n, Scale) is bas
-00003310: 6564 206f 6e20 7468 6520 7472 616e 7366  ed on the transf
-00003320: 6f72 6d20 6178 6973 2e20 2d20 6060 494e  orm axis. - ``IN
-00003330: 5345 5254 4b45 595f 5245 504c 4143 4560  SERTKEY_REPLACE`
-00003340: 6020 4f6e 6c79 2072 6570 6c61 6365 2061  ` Only replace a
-00003350: 6c72 6561 6479 2065 7869 7374 696e 6720  lready existing 
-00003360: 6b65 7966 7261 6d65 732e 202d 2060 6049  keyframes. - ``I
-00003370: 4e53 4552 544b 4559 5f41 5641 494c 4142  NSERTKEY_AVAILAB
-00003380: 4c45 6060 204f 6e6c 7920 696e 7365 7274  LE`` Only insert
-00003390: 2069 6e74 6f20 616c 7265 6164 7920 6578   into already ex
-000033a0: 6973 7469 6e67 2046 2d43 7572 7665 732e  isting F-Curves.
-000033b0: 202d 2060 6049 4e53 4552 544b 4559 5f43   - ``INSERTKEY_C
-000033c0: 5943 4c45 5f41 5741 5245 6060 2054 616b  YCLE_AWARE`` Tak
-000033d0: 6520 6379 636c 6963 2065 7874 7261 706f  e cyclic extrapo
-000033e0: 6c61 7469 6f6e 2069 6e74 6f20 6163 636f  lation into acco
-000033f0: 756e 7420 2843 7963 6c65 2d41 7761 7265  unt (Cycle-Aware
-00003400: 204b 6579 696e 6720 6f70 7469 6f6e 292e   Keying option).
-00003410: 0a20 2020 2020 2020 203a 7479 7065 206f  .        :type o
-00003420: 7074 696f 6e73 3a20 7479 7069 6e67 2e4f  ptions: typing.O
-00003430: 7074 696f 6e61 6c5b 7479 7069 6e67 2e41  ptional[typing.A
-00003440: 6e79 5d0a 2020 2020 2020 2020 3a72 7479  ny].        :rty
-00003450: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-00003460: 203a 7265 7475 726e 3a20 5375 6363 6573   :return: Succes
-00003470: 7320 6f66 206b 6579 6672 616d 6520 696e  s of keyframe in
-00003480: 7365 7274 696f 6e2e 0a20 2020 2020 2020  sertion..       
-00003490: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-000034a0: 730a 0a20 2020 2064 6566 206b 6579 7328  s..    def keys(
-000034b0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
-000034c0: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
-000034d0: 2052 6574 7572 6e73 2074 6865 206b 6579   Returns the key
-000034e0: 7320 6f66 2074 6869 7320 6f62 6a65 6374  s of this object
-000034f0: 7320 6375 7374 6f6d 2070 726f 7065 7274  s custom propert
-00003500: 6965 7320 286d 6174 6368 6573 2050 7974  ies (matches Pyt
-00003510: 686f 6e27 7320 6469 6374 696f 6e61 7279  hon's dictionary
-00003520: 2066 756e 6374 696f 6e20 6f66 2074 6865   function of the
-00003530: 2073 616d 6520 6e61 6d65 292e 0a0a 2020   same name)...  
-00003540: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00003550: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
-00003560: 203a 7265 7475 726e 3a20 6375 7374 6f6d   :return: custom
-00003570: 2070 726f 7065 7274 7920 6b65 7973 2e0a   property keys..
-00003580: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003590: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000035a0: 6620 7061 7468 5f66 726f 6d5f 6964 2873  f path_from_id(s
-000035b0: 656c 662c 2070 726f 7065 7274 793a 2074  elf, property: t
-000035c0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-000035d0: 7472 5d20 3d20 2222 2920 2d3e 2073 7472  tr] = "") -> str
-000035e0: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-000035f0: 7475 726e 7320 7468 6520 6461 7461 2070  turns the data p
-00003600: 6174 6820 6672 6f6d 2074 6865 2049 4420  ath from the ID 
-00003610: 746f 2074 6869 7320 6f62 6a65 6374 2028  to this object (
-00003620: 7374 7269 6e67 292e 0a0a 2020 2020 2020  string)...      
-00003630: 2020 3a70 6172 616d 2070 726f 7065 7274    :param propert
-00003640: 793a 204f 7074 696f 6e61 6c20 7072 6f70  y: Optional prop
-00003650: 6572 7479 206e 616d 6520 7768 6963 6820  erty name which 
-00003660: 6361 6e20 6265 2075 7365 6420 6966 2074  can be used if t
-00003670: 6865 2070 6174 6820 6973 2074 6f20 6120  he path is to a 
-00003680: 7072 6f70 6572 7479 206f 6620 7468 6973  property of this
-00003690: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-000036a0: 203a 7479 7065 2070 726f 7065 7274 793a   :type property:
-000036b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000036c0: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
-000036d0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-000036e0: 2020 3a72 6574 7572 6e3a 2060 6270 792e    :return: `bpy.
-000036f0: 7479 7065 732e 6270 795f 7374 7275 6374  types.bpy_struct
-00003700: 2e69 645f 6461 7461 6020 746f 2074 6869  .id_data` to thi
-00003710: 7320 7374 7275 6374 2061 6e64 2070 726f  s struct and pro
-00003720: 7065 7274 7920 2877 6865 6e20 6769 7665  perty (when give
-00003730: 6e29 2e0a 2020 2020 2020 2020 2727 270a  n)..        '''.
-00003740: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00003750: 2020 6465 6620 7061 7468 5f72 6573 6f6c    def path_resol
-00003760: 7665 2873 656c 662c 0a20 2020 2020 2020  ve(self,.       
-00003770: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00003780: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
-00003790: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000037b0: 6f65 7263 653a 2074 7970 696e 672e 4f70  oerce: typing.Op
-000037c0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
-000037d0: 7275 6529 3a0a 2020 2020 2020 2020 2727  rue):.        ''
-000037e0: 2720 5265 7475 726e 7320 7468 6520 7072  ' Returns the pr
-000037f0: 6f70 6572 7479 2066 726f 6d20 7468 6520  operty from the 
-00003800: 7061 7468 2c20 7261 6973 6520 616e 2065  path, raise an e
-00003810: 7863 6570 7469 6f6e 2077 6865 6e20 6e6f  xception when no
-00003820: 7420 666f 756e 642e 0a0a 2020 2020 2020  t found...      
-00003830: 2020 3a70 6172 616d 2070 6174 683a 2070    :param path: p
-00003840: 6174 6820 7768 6963 6820 7468 6973 2070  ath which this p
-00003850: 726f 7065 7274 7920 7265 736f 6c76 6573  roperty resolves
-00003860: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003870: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
-00003880: 696f 6e61 6c5b 7374 725d 0a20 2020 2020  ional[str].     
-00003890: 2020 203a 7061 7261 6d20 636f 6572 6365     :param coerce
-000038a0: 3a20 6f70 7469 6f6e 616c 2061 7267 756d  : optional argum
-000038b0: 656e 742c 2077 6865 6e20 5472 7565 2c20  ent, when True, 
-000038c0: 7468 6520 7072 6f70 6572 7479 2077 696c  the property wil
-000038d0: 6c20 6265 2063 6f6e 7665 7274 6564 2069  l be converted i
-000038e0: 6e74 6f20 6974 7320 5079 7468 6f6e 2072  nto its Python r
-000038f0: 6570 7265 7365 6e74 6174 696f 6e2e 0a20  epresentation.. 
-00003900: 2020 2020 2020 203a 7479 7065 2063 6f65         :type coe
-00003910: 7263 653a 2074 7970 696e 672e 4f70 7469  rce: typing.Opti
-00003920: 6f6e 616c 5b62 6f6f 6c5d 0a20 2020 2020  onal[bool].     
-00003930: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003940: 6173 730a 0a20 2020 2064 6566 2070 6f70  ass..    def pop
-00003950: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00003960: 2020 206b 6579 3a20 7479 7069 6e67 2e4f     key: typing.O
-00003970: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
-00003980: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-00003990: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-000039a0: 616c 5b74 7970 696e 672e 416e 795d 203d  al[typing.Any] =
-000039b0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000039c0: 2727 2720 5265 6d6f 7665 2061 6e64 2072  ''' Remove and r
-000039d0: 6574 7572 6e20 7468 6520 7661 6c75 6520  eturn the value 
-000039e0: 6f66 2074 6865 2063 7573 746f 6d20 7072  of the custom pr
-000039f0: 6f70 6572 7479 2061 7373 6967 6e65 6420  operty assigned 
-00003a00: 746f 206b 6579 206f 7220 6465 6661 756c  to key or defaul
-00003a10: 7420 7768 656e 206e 6f74 2066 6f75 6e64  t when not found
-00003a20: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
-00003a30: 2773 2064 6963 7469 6f6e 6172 7920 6675  's dictionary fu
-00003a40: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
-00003a50: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
-00003a60: 2020 203a 7061 7261 6d20 6b65 793a 2054     :param key: T
-00003a70: 6865 206b 6579 2061 7373 6f63 6961 7465  he key associate
-00003a80: 6420 7769 7468 2074 6865 2063 7573 746f  d with the custo
-00003a90: 6d20 7072 6f70 6572 7479 2e0a 2020 2020  m property..    
-00003aa0: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
-00003ab0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00003ac0: 7472 5d0a 2020 2020 2020 2020 3a70 6172  tr].        :par
-00003ad0: 616d 2064 6566 6175 6c74 3a20 4f70 7469  am default: Opti
-00003ae0: 6f6e 616c 2061 7267 756d 656e 7420 666f  onal argument fo
-00003af0: 7220 7468 6520 7661 6c75 6520 746f 2072  r the value to r
-00003b00: 6574 7572 6e20 6966 202a 6b65 792a 2069  eturn if *key* i
-00003b10: 7320 6e6f 7420 666f 756e 642e 0a20 2020  s not found..   
-00003b20: 2020 2020 203a 7479 7065 2064 6566 6175       :type defau
-00003b30: 6c74 3a20 7479 7069 6e67 2e4f 7074 696f  lt: typing.Optio
-00003b40: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
-00003b50: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00003b60: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00003b70: 6620 7072 6f70 6572 7479 5f6f 7665 7272  f property_overr
-00003b80: 6964 6162 6c65 5f6c 6962 7261 7279 5f73  idable_library_s
-00003b90: 6574 2873 656c 662c 2070 726f 7065 7274  et(self, propert
-00003ba0: 792c 206f 7665 7272 6964 6162 6c65 2920  y, overridable) 
-00003bb0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00003bc0: 2027 2727 2044 6566 696e 6520 6120 7072   ''' Define a pr
-00003bd0: 6f70 6572 7479 2061 7320 6f76 6572 7269  operty as overri
-00003be0: 6461 626c 6520 6f72 206e 6f74 2028 6f6e  dable or not (on
-00003bf0: 6c79 2066 6f72 2063 7573 746f 6d20 7072  ly for custom pr
-00003c00: 6f70 6572 7469 6573 2129 2e0a 0a20 2020  operties!)...   
-00003c10: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00003c20: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00003c30: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
-00003c40: 206f 7665 7272 6964 6162 6c65 2073 7461   overridable sta
-00003c50: 7475 7320 6f66 2074 6865 2070 726f 7065  tus of the prope
-00003c60: 7274 7920 7761 7320 7375 6363 6573 7366  rty was successf
-00003c70: 756c 6c79 2073 6574 2e0a 2020 2020 2020  ully set..      
-00003c80: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003c90: 7373 0a0a 2020 2020 6465 6620 7072 6f70  ss..    def prop
-00003ca0: 6572 7479 5f75 6e73 6574 2873 656c 662c  erty_unset(self,
-00003cb0: 2070 726f 7065 7274 7929 3a0a 2020 2020   property):.    
-00003cc0: 2020 2020 2727 2720 556e 7365 7420 6120      ''' Unset a 
-00003cd0: 7072 6f70 6572 7479 2c20 7769 6c6c 2075  property, will u
-00003ce0: 7365 2064 6566 6175 6c74 2076 616c 7565  se default value
-00003cf0: 2061 6674 6572 7761 7264 2e0a 0a20 2020   afterward...   
-00003d00: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00003d10: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00003d20: 7970 655f 7265 6361 7374 2873 656c 6629  ype_recast(self)
-00003d30: 202d 3e20 2762 7079 5f73 7472 7563 7427   -> 'bpy_struct'
-00003d40: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00003d50: 7475 726e 2061 206e 6577 2069 6e73 7461  turn a new insta
-00003d60: 6e63 652c 2074 6869 7320 6973 206e 6565  nce, this is nee
-00003d70: 6465 6420 6265 6361 7573 6520 7479 7065  ded because type
-00003d80: 7320 7375 6368 2061 7320 7465 7874 7572  s such as textur
-00003d90: 6573 2063 616e 2062 6520 6368 616e 6765  es can be change
-00003da0: 6420 6174 2072 756e 7469 6d65 2e0a 0a20  d at runtime... 
-00003db0: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
-00003dc0: 6270 795f 7374 7275 6374 270a 2020 2020  bpy_struct'.    
-00003dd0: 2020 2020 3a72 6574 7572 6e3a 2061 206e      :return: a n
-00003de0: 6577 2069 6e73 7461 6e63 6520 6f66 2074  ew instance of t
-00003df0: 6869 7320 6f62 6a65 6374 2077 6974 6820  his object with 
-00003e00: 7468 6520 7479 7065 2069 6e69 7469 616c  the type initial
-00003e10: 697a 6564 2061 6761 696e 2e0a 2020 2020  ized again..    
-00003e20: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00003e30: 7061 7373 0a0a 2020 2020 6465 6620 7661  pass..    def va
-00003e40: 6c75 6573 2873 656c 6629 202d 3e20 7479  lues(self) -> ty
-00003e50: 7069 6e67 2e41 6e79 3a0a 2020 2020 2020  ping.Any:.      
-00003e60: 2020 2727 2720 5265 7475 726e 7320 7468    ''' Returns th
-00003e70: 6520 7661 6c75 6573 206f 6620 7468 6973  e values of this
-00003e80: 206f 626a 6563 7473 2063 7573 746f 6d20   objects custom 
-00003e90: 7072 6f70 6572 7469 6573 2028 6d61 7463  properties (matc
-00003ea0: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
-00003eb0: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
-00003ec0: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
-00003ed0: 6529 2e0a 0a20 2020 2020 2020 203a 7274  e)...        :rt
-00003ee0: 7970 653a 2074 7970 696e 672e 416e 790a  ype: typing.Any.
-00003ef0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00003f00: 2063 7573 746f 6d20 7072 6f70 6572 7479   custom property
-00003f10: 2076 616c 7565 732e 0a20 2020 2020 2020   values..       
-00003f20: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003f30: 730a 0a20 2020 2064 6566 205f 5f67 6574  s..    def __get
-00003f40: 6974 656d 5f5f 2873 656c 662c 206b 6579  item__(self, key
-00003f50: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
-00003f60: 6e74 2c20 7374 725d 2920 2d3e 2027 7479  nt, str]) -> 'ty
-00003f70: 7069 6e67 2e41 6e79 273a 0a20 2020 2020  ping.Any':.     
-00003f80: 2020 2027 2727 200a 0a20 2020 2020 2020     ''' ..       
-00003f90: 203a 7061 7261 6d20 6b65 793a 200a 2020   :param key: .  
-00003fa0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00003fb0: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
-00003fc0: 742c 2073 7472 5d0a 2020 2020 2020 2020  t, str].        
-00003fd0: 3a72 7479 7065 3a20 2774 7970 696e 672e  :rtype: 'typing.
-00003fe0: 416e 7927 0a20 2020 2020 2020 2027 2727  Any'.        '''
-00003ff0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00004000: 2020 2064 6566 205f 5f73 6574 6974 656d     def __setitem
-00004010: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
-00004020: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00004030: 7374 725d 2c20 7661 6c75 653a 2027 7479  str], value: 'ty
-00004040: 7069 6e67 2e41 6e79 2729 3a0a 2020 2020  ping.Any'):.    
-00004050: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
-00004060: 2020 3a70 6172 616d 206b 6579 3a20 0a20    :param key: . 
-00004070: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-00004080: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
-00004090: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
-000040a0: 203a 7061 7261 6d20 7661 6c75 653a 200a   :param value: .
-000040b0: 2020 2020 2020 2020 3a74 7970 6520 7661          :type va
-000040c0: 6c75 653a 2027 7479 7069 6e67 2e41 6e79  lue: 'typing.Any
-000040d0: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
-000040e0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000040f0: 6465 6620 5f5f 6465 6c69 7465 6d5f 5f28  def __delitem__(
-00004100: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00004110: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00004120: 5d29 202d 3e20 2774 7970 696e 672e 416e  ]) -> 'typing.An
-00004130: 7927 3a0a 2020 2020 2020 2020 2727 2720  y':.        ''' 
-00004140: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00004150: 206b 6579 3a20 0a20 2020 2020 2020 203a   key: .        :
-00004160: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00004170: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
-00004180: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00004190: 2027 7479 7069 6e67 2e41 6e79 270a 2020   'typing.Any'.  
+00001bc0: 6f6e 616c 5b69 6e74 5d20 3d20 2d31 2c0a  onal[int] = -1,.
+00001bd0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+00001be0: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+00001bf0: 616c 5b66 6c6f 6174 5d20 3d20 2762 7079  al[float] = 'bpy
+00001c00: 2e63 6f6e 7465 7874 2e73 6365 6e65 2e66  .context.scene.f
+00001c10: 7261 6d65 5f63 7572 7265 6e74 272c 0a20  rame_current',. 
+00001c20: 2020 2020 2020 2020 2020 2067 726f 7570             group
+00001c30: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00001c40: 6c5b 7374 725d 203d 2022 2229 202d 3e20  l[str] = "") -> 
+00001c50: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00001c60: 2720 5265 6d6f 7665 2061 206b 6579 6672  ' Remove a keyfr
+00001c70: 616d 6520 6672 6f6d 2074 6869 7320 7072  ame from this pr
+00001c80: 6f70 6572 7469 6573 2066 6375 7276 652e  operties fcurve.
+00001c90: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001ca0: 2064 6174 615f 7061 7468 3a20 7061 7468   data_path: path
+00001cb0: 2074 6f20 7468 6520 7072 6f70 6572 7479   to the property
+00001cc0: 2074 6f20 7265 6d6f 7665 2061 206b 6579   to remove a key
+00001cd0: 2c20 616e 616c 6f67 6f75 7320 746f 2074  , analogous to t
+00001ce0: 6865 2066 6375 7276 6527 7320 6461 7461  he fcurve's data
+00001cf0: 2070 6174 682e 0a20 2020 2020 2020 203a   path..        :
+00001d00: 7479 7065 2064 6174 615f 7061 7468 3a20  type data_path: 
+00001d10: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001d20: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+00001d30: 7261 6d20 696e 6465 783a 2061 7272 6179  ram index: array
+00001d40: 2069 6e64 6578 206f 6620 7468 6520 7072   index of the pr
+00001d50: 6f70 6572 7479 2074 6f20 7265 6d6f 7665  operty to remove
+00001d60: 2061 206b 6579 2e20 4465 6661 756c 7473   a key. Defaults
+00001d70: 2074 6f20 2d31 2072 656d 6f76 696e 6720   to -1 removing 
+00001d80: 616c 6c20 696e 6469 6365 7320 6f72 2061  all indices or a
+00001d90: 2073 696e 676c 6520 6368 616e 6e65 6c20   single channel 
+00001da0: 6966 2074 6865 2070 726f 7065 7274 7920  if the property 
+00001db0: 6973 206e 6f74 2061 6e20 6172 7261 792e  is not an array.
+00001dc0: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
+00001dd0: 6e64 6578 3a20 7479 7069 6e67 2e4f 7074  ndex: typing.Opt
+00001de0: 696f 6e61 6c5b 696e 745d 0a20 2020 2020  ional[int].     
+00001df0: 2020 203a 7061 7261 6d20 6672 616d 653a     :param frame:
+00001e00: 2054 6865 2066 7261 6d65 206f 6e20 7768   The frame on wh
+00001e10: 6963 6820 7468 6520 6b65 7966 7261 6d65  ich the keyframe
+00001e20: 2069 7320 6465 6c65 7465 642c 2064 6566   is deleted, def
+00001e30: 6175 6c74 696e 6720 746f 2074 6865 2063  aulting to the c
+00001e40: 7572 7265 6e74 2066 7261 6d65 2e0a 2020  urrent frame..  
+00001e50: 2020 2020 2020 3a74 7970 6520 6672 616d        :type fram
+00001e60: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+00001e70: 616c 5b66 6c6f 6174 5d0a 2020 2020 2020  al[float].      
+00001e80: 2020 3a70 6172 616d 2067 726f 7570 3a20    :param group: 
+00001e90: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+00001ea0: 6772 6f75 7020 7468 6520 462d 4375 7276  group the F-Curv
+00001eb0: 6520 7368 6f75 6c64 2062 6520 6164 6465  e should be adde
+00001ec0: 6420 746f 2069 6620 6974 2064 6f65 736e  d to if it doesn
+00001ed0: 2774 2065 7869 7374 2079 6574 2e0a 2020  't exist yet..  
+00001ee0: 2020 2020 2020 3a74 7970 6520 6772 6f75        :type grou
+00001ef0: 703a 2074 7970 696e 672e 4f70 7469 6f6e  p: typing.Option
+00001f00: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00001f10: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+00001f20: 2020 2020 203a 7265 7475 726e 3a20 5375       :return: Su
+00001f30: 6363 6573 7320 6f66 206b 6579 6672 616d  ccess of keyfram
+00001f40: 6520 6465 6c65 7469 6f6e 2e0a 2020 2020  e deletion..    
+00001f50: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001f60: 7061 7373 0a0a 2020 2020 6465 6620 6b65  pass..    def ke
+00001f70: 7966 7261 6d65 5f69 6e73 6572 7428 0a20  yframe_insert(. 
+00001f80: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00001f90: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00001fa0: 615f 7061 7468 3a20 7479 7069 6e67 2e4f  a_path: typing.O
+00001fb0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+00001fc0: 2020 2020 2020 2020 2020 696e 6465 783a            index:
+00001fd0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00001fe0: 5b69 6e74 5d20 3d20 2d31 2c0a 2020 2020  [int] = -1,.    
+00001ff0: 2020 2020 2020 2020 6672 616d 653a 2074          frame: t
+00002000: 7970 696e 672e 4f70 7469 6f6e 616c 5b66  yping.Optional[f
+00002010: 6c6f 6174 5d20 3d20 2762 7079 2e63 6f6e  loat] = 'bpy.con
+00002020: 7465 7874 2e73 6365 6e65 2e66 7261 6d65  text.scene.frame
+00002030: 5f63 7572 7265 6e74 272c 0a20 2020 2020  _current',.     
+00002040: 2020 2020 2020 2067 726f 7570 3a20 7479         group: ty
+00002050: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00002060: 725d 203d 2022 222c 0a20 2020 2020 2020  r] = "",.       
+00002070: 2020 2020 206f 7074 696f 6e73 3a20 7479       options: ty
+00002080: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00002090: 7069 6e67 2e41 6e79 5d20 3d20 2773 6574  ping.Any] = 'set
+000020a0: 2829 2729 202d 3e20 626f 6f6c 3a0a 2020  ()') -> bool:.  
+000020b0: 2020 2020 2020 2727 2720 496e 7365 7274        ''' Insert
+000020c0: 2061 206b 6579 6672 616d 6520 6f6e 2074   a keyframe on t
+000020d0: 6865 2070 726f 7065 7274 7920 6769 7665  he property give
+000020e0: 6e2c 2061 6464 696e 6720 6663 7572 7665  n, adding fcurve
+000020f0: 7320 616e 6420 616e 696d 6174 696f 6e20  s and animation 
+00002100: 6461 7461 2077 6865 6e20 6e65 6365 7373  data when necess
+00002110: 6172 792e 2054 6869 7320 6973 2074 6865  ary. This is the
+00002120: 206d 6f73 7420 7369 6d70 6c65 2065 7861   most simple exa
+00002130: 6d70 6c65 206f 6620 696e 7365 7274 696e  mple of insertin
+00002140: 6720 6120 6b65 7966 7261 6d65 2066 726f  g a keyframe fro
+00002150: 6d20 7079 7468 6f6e 2e20 4e6f 7465 2074  m python. Note t
+00002160: 6861 7420 7768 656e 206b 6579 696e 6720  hat when keying 
+00002170: 6461 7461 2070 6174 6873 2077 6869 6368  data paths which
+00002180: 2063 6f6e 7461 696e 206e 6573 7465 6420   contain nested 
+00002190: 7072 6f70 6572 7469 6573 2074 6869 7320  properties this 
+000021a0: 6d75 7374 2062 6520 646f 6e65 2066 726f  must be done fro
+000021b0: 6d20 7468 6520 6049 4460 2073 7562 636c  m the `ID` subcl
+000021c0: 6173 732c 2069 6e20 7468 6973 2063 6173  ass, in this cas
+000021d0: 6520 7468 6520 6041 726d 6174 7572 6560  e the `Armature`
+000021e0: 2072 6174 6865 7220 7468 616e 2074 6865   rather than the
+000021f0: 2062 6f6e 652e 0a0a 2020 2020 2020 2020   bone...        
+00002200: 3a70 6172 616d 2064 6174 615f 7061 7468  :param data_path
+00002210: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
+00002220: 6f70 6572 7479 2074 6f20 6b65 792c 2061  operty to key, a
+00002230: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
+00002240: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
+00002250: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
+00002260: 6520 6461 7461 5f70 6174 683a 2074 7970  e data_path: typ
+00002270: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00002280: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00002290: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
+000022a0: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
+000022b0: 7274 7920 746f 206b 6579 2e20 4465 6661  rty to key. Defa
+000022c0: 756c 7473 2074 6f20 2d31 2077 6869 6368  ults to -1 which
+000022d0: 2077 696c 6c20 6b65 7920 616c 6c20 696e   will key all in
+000022e0: 6469 6365 7320 6f72 2061 2073 696e 676c  dices or a singl
+000022f0: 6520 6368 616e 6e65 6c20 6966 2074 6865  e channel if the
+00002300: 2070 726f 7065 7274 7920 6973 206e 6f74   property is not
+00002310: 2061 6e20 6172 7261 792e 0a20 2020 2020   an array..     
+00002320: 2020 203a 7479 7065 2069 6e64 6578 3a20     :type index: 
+00002330: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002340: 696e 745d 0a20 2020 2020 2020 203a 7061  int].        :pa
+00002350: 7261 6d20 6672 616d 653a 2054 6865 2066  ram frame: The f
+00002360: 7261 6d65 206f 6e20 7768 6963 6820 7468  rame on which th
+00002370: 6520 6b65 7966 7261 6d65 2069 7320 696e  e keyframe is in
+00002380: 7365 7274 6564 2c20 6465 6661 756c 7469  serted, defaulti
+00002390: 6e67 2074 6f20 7468 6520 6375 7272 656e  ng to the curren
+000023a0: 7420 6672 616d 652e 0a20 2020 2020 2020  t frame..       
+000023b0: 203a 7479 7065 2066 7261 6d65 3a20 7479   :type frame: ty
+000023c0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 666c  ping.Optional[fl
+000023d0: 6f61 745d 0a20 2020 2020 2020 203a 7061  oat].        :pa
+000023e0: 7261 6d20 6772 6f75 703a 2054 6865 206e  ram group: The n
+000023f0: 616d 6520 6f66 2074 6865 2067 726f 7570  ame of the group
+00002400: 2074 6865 2046 2d43 7572 7665 2073 686f   the F-Curve sho
+00002410: 756c 6420 6265 2061 6464 6564 2074 6f20  uld be added to 
+00002420: 6966 2069 7420 646f 6573 6e27 7420 6578  if it doesn't ex
+00002430: 6973 7420 7965 742e 0a20 2020 2020 2020  ist yet..       
+00002440: 203a 7479 7065 2067 726f 7570 3a20 7479   :type group: ty
+00002450: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00002460: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
+00002470: 6d20 666c 6167 3a20 0a20 2020 2020 2020  m flag: .       
+00002480: 203a 7479 7065 2066 6c61 673a 2074 7970   :type flag: typ
+00002490: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+000024a0: 696e 672e 5365 745d 0a20 2020 2020 2020  ing.Set].       
+000024b0: 203a 7061 7261 6d20 6f70 7469 6f6e 733a   :param options:
+000024c0: 2020 2d20 6060 494e 5345 5254 4b45 595f    - ``INSERTKEY_
+000024d0: 4e45 4544 4544 6060 204f 6e6c 7920 696e  NEEDED`` Only in
+000024e0: 7365 7274 206b 6579 6672 616d 6573 2077  sert keyframes w
+000024f0: 6865 7265 2074 6865 7927 7265 206e 6565  here they're nee
+00002500: 6465 6420 696e 2074 6865 2072 656c 6576  ded in the relev
+00002510: 616e 7420 462d 4375 7276 6573 2e20 2d20  ant F-Curves. - 
+00002520: 6060 494e 5345 5254 4b45 595f 5649 5355  ``INSERTKEY_VISU
+00002530: 414c 6060 2049 6e73 6572 7420 6b65 7966  AL`` Insert keyf
+00002540: 7261 6d65 7320 6261 7365 6420 6f6e 2027  rames based on '
+00002550: 7669 7375 616c 2074 7261 6e73 666f 726d  visual transform
+00002560: 7327 2e20 2d20 6060 494e 5345 5254 4b45  s'. - ``INSERTKE
+00002570: 595f 5859 5a5f 544f 5f52 4742 6060 2043  Y_XYZ_TO_RGB`` C
+00002580: 6f6c 6f72 2066 6f72 206e 6577 6c79 2061  olor for newly a
+00002590: 6464 6564 2074 7261 6e73 666f 726d 6174  dded transformat
+000025a0: 696f 6e20 462d 4375 7276 6573 2028 4c6f  ion F-Curves (Lo
+000025b0: 6361 7469 6f6e 2c20 526f 7461 7469 6f6e  cation, Rotation
+000025c0: 2c20 5363 616c 6529 2069 7320 6261 7365  , Scale) is base
+000025d0: 6420 6f6e 2074 6865 2074 7261 6e73 666f  d on the transfo
+000025e0: 726d 2061 7869 732e 202d 2060 6049 4e53  rm axis. - ``INS
+000025f0: 4552 544b 4559 5f52 4550 4c41 4345 6060  ERTKEY_REPLACE``
+00002600: 204f 6e6c 7920 7265 706c 6163 6520 616c   Only replace al
+00002610: 7265 6164 7920 6578 6973 7469 6e67 206b  ready existing k
+00002620: 6579 6672 616d 6573 2e20 2d20 6060 494e  eyframes. - ``IN
+00002630: 5345 5254 4b45 595f 4156 4149 4c41 424c  SERTKEY_AVAILABL
+00002640: 4560 6020 4f6e 6c79 2069 6e73 6572 7420  E`` Only insert 
+00002650: 696e 746f 2061 6c72 6561 6479 2065 7869  into already exi
+00002660: 7374 696e 6720 462d 4375 7276 6573 2e20  sting F-Curves. 
+00002670: 2d20 6060 494e 5345 5254 4b45 595f 4359  - ``INSERTKEY_CY
+00002680: 434c 455f 4157 4152 4560 6020 5461 6b65  CLE_AWARE`` Take
+00002690: 2063 7963 6c69 6320 6578 7472 6170 6f6c   cyclic extrapol
+000026a0: 6174 696f 6e20 696e 746f 2061 6363 6f75  ation into accou
+000026b0: 6e74 2028 4379 636c 652d 4177 6172 6520  nt (Cycle-Aware 
+000026c0: 4b65 7969 6e67 206f 7074 696f 6e29 2e0a  Keying option)..
+000026d0: 2020 2020 2020 2020 3a74 7970 6520 6f70          :type op
+000026e0: 7469 6f6e 733a 2074 7970 696e 672e 4f70  tions: typing.Op
+000026f0: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
+00002700: 795d 0a20 2020 2020 2020 203a 7274 7970  y].        :rtyp
+00002710: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00002720: 3a72 6574 7572 6e3a 2053 7563 6365 7373  :return: Success
+00002730: 206f 6620 6b65 7966 7261 6d65 2069 6e73   of keyframe ins
+00002740: 6572 7469 6f6e 2e0a 2020 2020 2020 2020  ertion..        
+00002750: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00002760: 0a0a 2020 2020 6465 6620 6b65 7973 2873  ..    def keys(s
+00002770: 656c 6629 202d 3e20 7479 7069 6e67 2e41  elf) -> typing.A
+00002780: 6e79 3a0a 2020 2020 2020 2020 2727 2720  ny:.        ''' 
+00002790: 5265 7475 726e 7320 7468 6520 6b65 7973  Returns the keys
+000027a0: 206f 6620 7468 6973 206f 626a 6563 7473   of this objects
+000027b0: 2063 7573 746f 6d20 7072 6f70 6572 7469   custom properti
+000027c0: 6573 2028 6d61 7463 6865 7320 5079 7468  es (matches Pyth
+000027d0: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
+000027e0: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
+000027f0: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
+00002800: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
+00002810: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
+00002820: 3a72 6574 7572 6e3a 2063 7573 746f 6d20  :return: custom 
+00002830: 7072 6f70 6572 7479 206b 6579 732e 0a20  property keys.. 
+00002840: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00002850: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00002860: 2070 6174 685f 6672 6f6d 5f69 6428 7365   path_from_id(se
+00002870: 6c66 2c20 7072 6f70 6572 7479 3a20 7479  lf, property: ty
+00002880: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00002890: 725d 203d 2022 2229 202d 3e20 7374 723a  r] = "") -> str:
+000028a0: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+000028b0: 7572 6e73 2074 6865 2064 6174 6120 7061  urns the data pa
+000028c0: 7468 2066 726f 6d20 7468 6520 4944 2074  th from the ID t
+000028d0: 6f20 7468 6973 206f 626a 6563 7420 2873  o this object (s
+000028e0: 7472 696e 6729 2e0a 0a20 2020 2020 2020  tring)...       
+000028f0: 203a 7061 7261 6d20 7072 6f70 6572 7479   :param property
+00002900: 3a20 4f70 7469 6f6e 616c 2070 726f 7065  : Optional prope
+00002910: 7274 7920 6e61 6d65 2077 6869 6368 2063  rty name which c
+00002920: 616e 2062 6520 7573 6564 2069 6620 7468  an be used if th
+00002930: 6520 7061 7468 2069 7320 746f 2061 2070  e path is to a p
+00002940: 726f 7065 7274 7920 6f66 2074 6869 7320  roperty of this 
+00002950: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00002960: 3a74 7970 6520 7072 6f70 6572 7479 3a20  :type property: 
+00002970: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002980: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00002990: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+000029a0: 203a 7265 7475 726e 3a20 6062 7079 2e74   :return: `bpy.t
+000029b0: 7970 6573 2e62 7079 5f73 7472 7563 742e  ypes.bpy_struct.
+000029c0: 6964 5f64 6174 6160 2074 6f20 7468 6973  id_data` to this
+000029d0: 2073 7472 7563 7420 616e 6420 7072 6f70   struct and prop
+000029e0: 6572 7479 2028 7768 656e 2067 6976 656e  erty (when given
+000029f0: 292e 0a20 2020 2020 2020 2027 2727 0a20  )..        '''. 
+00002a00: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00002a10: 2064 6566 2070 6174 685f 7265 736f 6c76   def path_resolv
+00002a20: 6528 7365 6c66 2c0a 2020 2020 2020 2020  e(self,.        
+00002a30: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+00002a40: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00002a50: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
+00002a60: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002a70: 6572 6365 3a20 7479 7069 6e67 2e4f 7074  erce: typing.Opt
+00002a80: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
+00002a90: 7565 293a 0a20 2020 2020 2020 2027 2727  ue):.        '''
+00002aa0: 2052 6574 7572 6e73 2074 6865 2070 726f   Returns the pro
+00002ab0: 7065 7274 7920 6672 6f6d 2074 6865 2070  perty from the p
+00002ac0: 6174 682c 2072 6169 7365 2061 6e20 6578  ath, raise an ex
+00002ad0: 6365 7074 696f 6e20 7768 656e 206e 6f74  ception when not
+00002ae0: 2066 6f75 6e64 2e0a 0a20 2020 2020 2020   found...       
+00002af0: 203a 7061 7261 6d20 7061 7468 3a20 7061   :param path: pa
+00002b00: 7468 2077 6869 6368 2074 6869 7320 7072  th which this pr
+00002b10: 6f70 6572 7479 2072 6573 6f6c 7665 732e  operty resolves.
+00002b20: 0a20 2020 2020 2020 203a 7479 7065 2070  .        :type p
+00002b30: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
+00002b40: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
+00002b50: 2020 3a70 6172 616d 2063 6f65 7263 653a    :param coerce:
+00002b60: 206f 7074 696f 6e61 6c20 6172 6775 6d65   optional argume
+00002b70: 6e74 2c20 7768 656e 2054 7275 652c 2074  nt, when True, t
+00002b80: 6865 2070 726f 7065 7274 7920 7769 6c6c  he property will
+00002b90: 2062 6520 636f 6e76 6572 7465 6420 696e   be converted in
+00002ba0: 746f 2069 7473 2050 7974 686f 6e20 7265  to its Python re
+00002bb0: 7072 6573 656e 7461 7469 6f6e 2e0a 2020  presentation..  
+00002bc0: 2020 2020 2020 3a74 7970 6520 636f 6572        :type coer
+00002bd0: 6365 3a20 7479 7069 6e67 2e4f 7074 696f  ce: typing.Optio
+00002be0: 6e61 6c5b 626f 6f6c 5d0a 2020 2020 2020  nal[bool].      
+00002bf0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00002c00: 7373 0a0a 2020 2020 6465 6620 706f 7028  ss..    def pop(
+00002c10: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00002c20: 2020 6b65 793a 2074 7970 696e 672e 4f70    key: typing.Op
+00002c30: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+00002c40: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00002c50: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002c60: 6c5b 7479 7069 6e67 2e41 6e79 5d20 3d20  l[typing.Any] = 
+00002c70: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
+00002c80: 2727 2052 656d 6f76 6520 616e 6420 7265  '' Remove and re
+00002c90: 7475 726e 2074 6865 2076 616c 7565 206f  turn the value o
+00002ca0: 6620 7468 6520 6375 7374 6f6d 2070 726f  f the custom pro
+00002cb0: 7065 7274 7920 6173 7369 676e 6564 2074  perty assigned t
+00002cc0: 6f20 6b65 7920 6f72 2064 6566 6175 6c74  o key or default
+00002cd0: 2077 6865 6e20 6e6f 7420 666f 756e 6420   when not found 
+00002ce0: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
+00002cf0: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
+00002d00: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
+00002d10: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
+00002d20: 2020 3a70 6172 616d 206b 6579 3a20 5468    :param key: Th
+00002d30: 6520 6b65 7920 6173 736f 6369 6174 6564  e key associated
+00002d40: 2077 6974 6820 7468 6520 6375 7374 6f6d   with the custom
+00002d50: 2070 726f 7065 7274 792e 0a20 2020 2020   property..     
+00002d60: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00002d70: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00002d80: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
+00002d90: 6d20 6465 6661 756c 743a 204f 7074 696f  m default: Optio
+00002da0: 6e61 6c20 6172 6775 6d65 6e74 2066 6f72  nal argument for
+00002db0: 2074 6865 2076 616c 7565 2074 6f20 7265   the value to re
+00002dc0: 7475 726e 2069 6620 2a6b 6579 2a20 6973  turn if *key* is
+00002dd0: 206e 6f74 2066 6f75 6e64 2e0a 2020 2020   not found..    
+00002de0: 2020 2020 3a74 7970 6520 6465 6661 756c      :type defaul
+00002df0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
+00002e00: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
+00002e10: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00002e20: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00002e30: 2070 726f 7065 7274 795f 6f76 6572 7269   property_overri
+00002e40: 6461 626c 655f 6c69 6272 6172 795f 7365  dable_library_se
+00002e50: 7428 7365 6c66 2c20 7072 6f70 6572 7479  t(self, property
+00002e60: 2c20 6f76 6572 7269 6461 626c 6529 202d  , overridable) -
+00002e70: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00002e80: 2727 2720 4465 6669 6e65 2061 2070 726f  ''' Define a pro
+00002e90: 7065 7274 7920 6173 206f 7665 7272 6964  perty as overrid
+00002ea0: 6162 6c65 206f 7220 6e6f 7420 286f 6e6c  able or not (onl
+00002eb0: 7920 666f 7220 6375 7374 6f6d 2070 726f  y for custom pro
+00002ec0: 7065 7274 6965 7321 292e 0a0a 2020 2020  perties!)...    
+00002ed0: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00002ee0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002ef0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+00002f00: 6f76 6572 7269 6461 626c 6520 7374 6174  overridable stat
+00002f10: 7573 206f 6620 7468 6520 7072 6f70 6572  us of the proper
+00002f20: 7479 2077 6173 2073 7563 6365 7373 6675  ty was successfu
+00002f30: 6c6c 7920 7365 742e 0a20 2020 2020 2020  lly set..       
+00002f40: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002f50: 730a 0a20 2020 2064 6566 2070 726f 7065  s..    def prope
+00002f60: 7274 795f 756e 7365 7428 7365 6c66 2c20  rty_unset(self, 
+00002f70: 7072 6f70 6572 7479 293a 0a20 2020 2020  property):.     
+00002f80: 2020 2027 2727 2055 6e73 6574 2061 2070     ''' Unset a p
+00002f90: 726f 7065 7274 792c 2077 696c 6c20 7573  roperty, will us
+00002fa0: 6520 6465 6661 756c 7420 7661 6c75 6520  e default value 
+00002fb0: 6166 7465 7277 6172 642e 0a0a 2020 2020  afterward...    
+00002fc0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00002fd0: 7061 7373 0a0a 2020 2020 6465 6620 7479  pass..    def ty
+00002fe0: 7065 5f72 6563 6173 7428 7365 6c66 2920  pe_recast(self) 
+00002ff0: 2d3e 2027 6270 795f 7374 7275 6374 273a  -> 'bpy_struct':
+00003000: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00003010: 7572 6e20 6120 6e65 7720 696e 7374 616e  urn a new instan
+00003020: 6365 2c20 7468 6973 2069 7320 6e65 6564  ce, this is need
+00003030: 6564 2062 6563 6175 7365 2074 7970 6573  ed because types
+00003040: 2073 7563 6820 6173 2074 6578 7475 7265   such as texture
+00003050: 7320 6361 6e20 6265 2063 6861 6e67 6564  s can be changed
+00003060: 2061 7420 7275 6e74 696d 652e 0a0a 2020   at runtime...  
+00003070: 2020 2020 2020 3a72 7479 7065 3a20 2762        :rtype: 'b
+00003080: 7079 5f73 7472 7563 7427 0a20 2020 2020  py_struct'.     
+00003090: 2020 203a 7265 7475 726e 3a20 6120 6e65     :return: a ne
+000030a0: 7720 696e 7374 616e 6365 206f 6620 7468  w instance of th
+000030b0: 6973 206f 626a 6563 7420 7769 7468 2074  is object with t
+000030c0: 6865 2074 7970 6520 696e 6974 6961 6c69  he type initiali
+000030d0: 7a65 6420 6167 6169 6e2e 0a20 2020 2020  zed again..     
+000030e0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+000030f0: 6173 730a 0a20 2020 2064 6566 2076 616c  ass..    def val
+00003100: 7565 7328 7365 6c66 2920 2d3e 2074 7970  ues(self) -> typ
+00003110: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
+00003120: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
+00003130: 2076 616c 7565 7320 6f66 2074 6869 7320   values of this 
+00003140: 6f62 6a65 6374 7320 6375 7374 6f6d 2070  objects custom p
+00003150: 726f 7065 7274 6965 7320 286d 6174 6368  roperties (match
+00003160: 6573 2050 7974 686f 6e27 7320 6469 6374  es Python's dict
+00003170: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
+00003180: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
+00003190: 292e 0a0a 2020 2020 2020 2020 3a72 7479  )...        :rty
+000031a0: 7065 3a20 7479 7069 6e67 2e41 6e79 0a20  pe: typing.Any. 
+000031b0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000031c0: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
+000031d0: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
+000031e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000031f0: 0a0a 2020 2020 6465 6620 5f5f 6765 7469  ..    def __geti
+00003200: 7465 6d5f 5f28 7365 6c66 2c20 6b65 793a  tem__(self, key:
+00003210: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
+00003220: 742c 2073 7472 5d29 202d 3e20 2774 7970  t, str]) -> 'typ
+00003230: 696e 672e 416e 7927 3a0a 2020 2020 2020  ing.Any':.      
+00003240: 2020 2727 2720 0a0a 2020 2020 2020 2020    ''' ..        
+00003250: 3a70 6172 616d 206b 6579 3a20 0a20 2020  :param key: .   
+00003260: 2020 2020 203a 7479 7065 206b 6579 3a20       :type key: 
+00003270: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+00003280: 2c20 7374 725d 0a20 2020 2020 2020 203a  , str].        :
+00003290: 7274 7970 653a 2027 7479 7069 6e67 2e41  rtype: 'typing.A
+000032a0: 6e79 270a 2020 2020 2020 2020 2727 270a  ny'.        '''.
+000032b0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000032c0: 2020 6465 6620 5f5f 7365 7469 7465 6d5f    def __setitem_
+000032d0: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
+000032e0: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+000032f0: 7472 5d2c 2076 616c 7565 3a20 2774 7970  tr], value: 'typ
+00003300: 696e 672e 416e 7927 293a 0a20 2020 2020  ing.Any'):.     
+00003310: 2020 2027 2727 200a 0a20 2020 2020 2020     ''' ..       
+00003320: 203a 7061 7261 6d20 6b65 793a 200a 2020   :param key: .  
+00003330: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00003340: 2074 7970 696e 672e 556e 696f 6e5b 696e   typing.Union[in
+00003350: 742c 2073 7472 5d0a 2020 2020 2020 2020  t, str].        
+00003360: 3a70 6172 616d 2076 616c 7565 3a20 0a20  :param value: . 
+00003370: 2020 2020 2020 203a 7479 7065 2076 616c         :type val
+00003380: 7565 3a20 2774 7970 696e 672e 416e 7927  ue: 'typing.Any'
+00003390: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000033a0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000033b0: 6566 205f 5f64 656c 6974 656d 5f5f 2873  ef __delitem__(s
+000033c0: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+000033d0: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+000033e0: 2920 2d3e 2027 7479 7069 6e67 2e41 6e79  ) -> 'typing.Any
+000033f0: 273a 0a20 2020 2020 2020 2027 2727 200a  ':.        ''' .
+00003400: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003410: 6b65 793a 200a 2020 2020 2020 2020 3a74  key: .        :t
+00003420: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+00003430: 556e 696f 6e5b 696e 742c 2073 7472 5d0a  Union[int, str].
+00003440: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00003450: 2774 7970 696e 672e 416e 7927 0a20 2020  'typing.Any'.   
+00003460: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003470: 2070 6173 730a 0a0a 636c 6173 7320 6270   pass...class bp
+00003480: 795f 7072 6f70 5f63 6f6c 6c65 6374 696f  y_prop_collectio
+00003490: 6e28 7479 7069 6e67 2e47 656e 6572 6963  n(typing.Generic
+000034a0: 5b47 656e 6572 6963 5479 7065 5d29 3a0a  [GenericType]):.
+000034b0: 2020 2020 2727 2720 6275 696c 742d 696e      ''' built-in
+000034c0: 2063 6c61 7373 2075 7365 6420 666f 7220   class used for 
+000034d0: 616c 6c20 636f 6c6c 6563 7469 6f6e 732e  all collections.
+000034e0: 0a20 2020 2027 2727 0a0a 2020 2020 6465  .    '''..    de
+000034f0: 6620 6669 6e64 2873 656c 662c 206b 6579  f find(self, key
+00003500: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00003510: 6c5b 7374 725d 2920 2d3e 2069 6e74 3a0a  l[str]) -> int:.
+00003520: 2020 2020 2020 2020 2727 2720 5265 7475          ''' Retu
+00003530: 726e 7320 7468 6520 696e 6465 7820 6f66  rns the index of
+00003540: 2061 206b 6579 2069 6e20 6120 636f 6c6c   a key in a coll
+00003550: 6563 7469 6f6e 206f 7220 2d31 2077 6865  ection or -1 whe
+00003560: 6e20 6e6f 7420 666f 756e 6420 286d 6174  n not found (mat
+00003570: 6368 6573 2050 7974 686f 6e27 7320 7374  ches Python's st
+00003580: 7269 6e67 2066 696e 6420 6675 6e63 7469  ring find functi
+00003590: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
+000035a0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
+000035b0: 7061 7261 6d20 6b65 793a 2054 6865 2069  param key: The i
+000035c0: 6465 6e74 6966 6965 7220 666f 7220 7468  dentifier for th
+000035d0: 6520 636f 6c6c 6563 7469 6f6e 206d 656d  e collection mem
+000035e0: 6265 722e 0a20 2020 2020 2020 203a 7479  ber..        :ty
+000035f0: 7065 206b 6579 3a20 7479 7069 6e67 2e4f  pe key: typing.O
+00003600: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
+00003610: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+00003620: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00003630: 3a20 696e 6465 7820 6f66 2074 6865 206b  : index of the k
+00003640: 6579 2e0a 2020 2020 2020 2020 2727 270a  ey..        '''.
+00003650: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00003660: 2020 6465 6620 666f 7265 6163 685f 6765    def foreach_ge
+00003670: 7428 7365 6c66 2c20 6174 7472 2c20 7365  t(self, attr, se
+00003680: 7129 3a0a 2020 2020 2020 2020 2727 2720  q):.        ''' 
+00003690: 5468 6973 2069 7320 6120 6675 6e63 7469  This is a functi
+000036a0: 6f6e 2074 6f20 6769 7665 2066 6173 7420  on to give fast 
+000036b0: 6163 6365 7373 2074 6f20 6174 7472 6962  access to attrib
+000036c0: 7574 6573 2077 6974 6869 6e20 6120 636f  utes within a co
+000036d0: 6c6c 6563 7469 6f6e 2e20 4f6e 6c79 2077  llection. Only w
+000036e0: 6f72 6b73 2066 6f72 2027 6261 7369 6320  orks for 'basic 
+000036f0: 7479 7065 2720 7072 6f70 6572 7469 6573  type' properties
+00003700: 2028 626f 6f6c 2c20 696e 7420 616e 6420   (bool, int and 
+00003710: 666c 6f61 7429 2120 4d75 6c74 692d 6469  float)! Multi-di
+00003720: 6d65 6e73 696f 6e61 6c20 6172 7261 7973  mensional arrays
+00003730: 2028 6c69 6b65 2061 7272 6179 206f 6620   (like array of 
+00003740: 7665 6374 6f72 7329 2077 696c 6c20 6265  vectors) will be
+00003750: 2066 6c61 7474 656e 6564 2069 6e74 6f20   flattened into 
+00003760: 7365 712e 0a0a 2020 2020 2020 2020 2727  seq...        ''
+00003770: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003780: 2020 2020 6465 6620 666f 7265 6163 685f      def foreach_
+00003790: 7365 7428 7365 6c66 2c20 6174 7472 2c20  set(self, attr, 
+000037a0: 7365 7129 3a0a 2020 2020 2020 2020 2727  seq):.        ''
+000037b0: 2720 5468 6973 2069 7320 6120 6675 6e63  ' This is a func
+000037c0: 7469 6f6e 2074 6f20 6769 7665 2066 6173  tion to give fas
+000037d0: 7420 6163 6365 7373 2074 6f20 6174 7472  t access to attr
+000037e0: 6962 7574 6573 2077 6974 6869 6e20 6120  ibutes within a 
+000037f0: 636f 6c6c 6563 7469 6f6e 2e20 4f6e 6c79  collection. Only
+00003800: 2077 6f72 6b73 2066 6f72 2027 6261 7369   works for 'basi
+00003810: 6320 7479 7065 2720 7072 6f70 6572 7469  c type' properti
+00003820: 6573 2028 626f 6f6c 2c20 696e 7420 616e  es (bool, int an
+00003830: 6420 666c 6f61 7429 2120 7365 7120 6d75  d float)! seq mu
+00003840: 7374 2062 6520 756e 692d 6469 6d65 6e73  st be uni-dimens
+00003850: 696f 6e61 6c2c 206d 756c 7469 2d64 696d  ional, multi-dim
+00003860: 656e 7369 6f6e 616c 2061 7272 6179 7320  ensional arrays 
+00003870: 286c 696b 6520 6172 7261 7920 6f66 2076  (like array of v
+00003880: 6563 746f 7273 2920 7769 6c6c 2062 6520  ectors) will be 
+00003890: 7265 2d63 7265 6174 6564 2066 726f 6d20  re-created from 
+000038a0: 6974 2e0a 0a20 2020 2020 2020 2027 2727  it...        '''
+000038b0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000038c0: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
+000038d0: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
+000038e0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000038f0: 6c5b 7374 725d 2c0a 2020 2020 2020 2020  l[str],.        
+00003900: 2020 2020 6465 6661 756c 743a 2074 7970      default: typ
+00003910: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00003920: 696e 672e 416e 795d 203d 204e 6f6e 6529  ing.Any] = None)
+00003930: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
+00003940: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
+00003950: 6f66 2074 6865 2069 7465 6d20 6173 7369  of the item assi
+00003960: 676e 6564 2074 6f20 6b65 7920 6f72 2064  gned to key or d
+00003970: 6566 6175 6c74 2077 6865 6e20 6e6f 7420  efault when not 
+00003980: 666f 756e 6420 286d 6174 6368 6573 2050  found (matches P
+00003990: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
+000039a0: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
+000039b0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+000039c0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+000039d0: 6579 3a20 5468 6520 6964 656e 7469 6669  ey: The identifi
+000039e0: 6572 2066 6f72 2074 6865 2063 6f6c 6c65  er for the colle
+000039f0: 6374 696f 6e20 6d65 6d62 6572 2e0a 2020  ction member..  
+00003a00: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00003a10: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003a20: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
+00003a30: 6172 616d 2064 6566 6175 6c74 3a20 4f70  aram default: Op
+00003a40: 7469 6f6e 616c 2061 7267 756d 656e 7420  tional argument 
+00003a50: 666f 7220 7468 6520 7661 6c75 6520 746f  for the value to
+00003a60: 2072 6574 7572 6e20 6966 202a 6b65 792a   return if *key*
+00003a70: 2069 7320 6e6f 7420 666f 756e 642e 0a20   is not found.. 
+00003a80: 2020 2020 2020 203a 7479 7065 2064 6566         :type def
+00003a90: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00003aa0: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00003ab0: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
+00003ac0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00003ad0: 6465 6620 6974 656d 7328 7365 6c66 2920  def items(self) 
+00003ae0: 2d3e 2074 7970 696e 672e 4c69 7374 3a0a  -> typing.List:.
+00003af0: 2020 2020 2020 2020 2727 2720 5265 7475          ''' Retu
+00003b00: 726e 2074 6865 2069 6465 6e74 6966 6965  rn the identifie
+00003b10: 7273 206f 6620 636f 6c6c 6563 7469 6f6e  rs of collection
+00003b20: 206d 656d 6265 7273 2028 6d61 7463 6869   members (matchi
+00003b30: 6e67 2050 7974 686f 6e27 7320 6469 6374  ng Python's dict
+00003b40: 2e69 7465 6d73 2829 2066 756e 6374 696f  .items() functio
+00003b50: 6e61 6c69 7479 292e 0a0a 2020 2020 2020  nality)...      
+00003b60: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+00003b70: 2e4c 6973 740a 2020 2020 2020 2020 3a72  .List.        :r
+00003b80: 6574 7572 6e3a 2028 6b65 792c 2076 616c  eturn: (key, val
+00003b90: 7565 2920 7061 6972 7320 666f 7220 6561  ue) pairs for ea
+00003ba0: 6368 206d 656d 6265 7220 6f66 2074 6869  ch member of thi
+00003bb0: 7320 636f 6c6c 6563 7469 6f6e 2e0a 2020  s collection..  
+00003bc0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00003bd0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00003be0: 6b65 7973 2873 656c 6629 202d 3e20 7479  keys(self) -> ty
+00003bf0: 7069 6e67 2e4c 6973 745b 7374 725d 3a0a  ping.List[str]:.
+00003c00: 2020 2020 2020 2020 2727 2720 5265 7475          ''' Retu
+00003c10: 726e 2074 6865 2069 6465 6e74 6966 6965  rn the identifie
+00003c20: 7273 206f 6620 636f 6c6c 6563 7469 6f6e  rs of collection
+00003c30: 206d 656d 6265 7273 2028 6d61 7463 6869   members (matchi
+00003c40: 6e67 2050 7974 686f 6e27 7320 6469 6374  ng Python's dict
+00003c50: 2e6b 6579 7328 2920 6675 6e63 7469 6f6e  .keys() function
+00003c60: 616c 6974 7929 2e0a 0a20 2020 2020 2020  ality)...       
+00003c70: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
+00003c80: 4c69 7374 5b73 7472 5d0a 2020 2020 2020  List[str].      
+00003c90: 2020 3a72 6574 7572 6e3a 2074 6865 2069    :return: the i
+00003ca0: 6465 6e74 6966 6965 7273 2066 6f72 2065  dentifiers for e
+00003cb0: 6163 6820 6d65 6d62 6572 206f 6620 7468  ach member of th
+00003cc0: 6973 2063 6f6c 6c65 6374 696f 6e2e 0a20  is collection.. 
+00003cd0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00003ce0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00003cf0: 2076 616c 7565 7328 7365 6c66 2920 2d3e   values(self) ->
+00003d00: 2074 7970 696e 672e 4c69 7374 3a0a 2020   typing.List:.  
+00003d10: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00003d20: 2074 6865 2076 616c 7565 7320 6f66 2063   the values of c
+00003d30: 6f6c 6c65 6374 696f 6e20 286d 6174 6368  ollection (match
+00003d40: 696e 6720 5079 7468 6f6e 2773 2064 6963  ing Python's dic
+00003d50: 742e 7661 6c75 6573 2829 2066 756e 6374  t.values() funct
+00003d60: 696f 6e61 6c69 7479 292e 0a0a 2020 2020  ionality)...    
+00003d70: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
+00003d80: 6e67 2e4c 6973 740a 2020 2020 2020 2020  ng.List.        
+00003d90: 3a72 6574 7572 6e3a 2074 6865 206d 656d  :return: the mem
+00003da0: 6265 7273 206f 6620 7468 6973 2063 6f6c  bers of this col
+00003db0: 6c65 6374 696f 6e2e 0a20 2020 2020 2020  lection..       
+00003dc0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003dd0: 730a 0a20 2020 2064 6566 205f 5f67 6574  s..    def __get
+00003de0: 6974 656d 5f5f 2873 656c 662c 206b 6579  item__(self, key
+00003df0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
+00003e00: 6e74 2c20 7374 725d 2920 2d3e 2027 4765  nt, str]) -> 'Ge
+00003e10: 6e65 7269 6354 7970 6527 3a0a 2020 2020  nericType':.    
+00003e20: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
+00003e30: 2020 3a70 6172 616d 206b 6579 3a20 0a20    :param key: . 
+00003e40: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+00003e50: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
+00003e60: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
+00003e70: 203a 7274 7970 653a 2027 4765 6e65 7269   :rtype: 'Generi
+00003e80: 6354 7970 6527 0a20 2020 2020 2020 2027  cType'.        '
+00003e90: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00003ea0: 0a20 2020 2064 6566 205f 5f73 6574 6974  .    def __setit
+00003eb0: 656d 5f5f 2873 656c 662c 206b 6579 3a20  em__(self, key: 
+00003ec0: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+00003ed0: 2c20 7374 725d 2c20 7661 6c75 653a 2027  , str], value: '
+00003ee0: 4765 6e65 7269 6354 7970 6527 293a 0a20  GenericType'):. 
+00003ef0: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
+00003f00: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+00003f10: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
+00003f20: 6b65 793a 2074 7970 696e 672e 556e 696f  key: typing.Unio
+00003f30: 6e5b 696e 742c 2073 7472 5d0a 2020 2020  n[int, str].    
+00003f40: 2020 2020 3a70 6172 616d 2076 616c 7565      :param value
+00003f50: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+00003f60: 2076 616c 7565 3a20 2747 656e 6572 6963   value: 'Generic
+00003f70: 5479 7065 270a 2020 2020 2020 2020 2727  Type'.        ''
+00003f80: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003f90: 2020 2020 6465 6620 5f5f 6465 6c69 7465      def __delite
+00003fa0: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+00003fb0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00003fc0: 2073 7472 5d29 202d 3e20 2747 656e 6572   str]) -> 'Gener
+00003fd0: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
+00003fe0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00003ff0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
+00004000: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
+00004010: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00004020: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
+00004030: 7479 7065 3a20 2747 656e 6572 6963 5479  type: 'GenericTy
+00004040: 7065 270a 2020 2020 2020 2020 2727 270a  pe'.        '''.
+00004050: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00004060: 2020 6465 6620 5f5f 6974 6572 5f5f 2873    def __iter__(s
+00004070: 656c 6629 202d 3e20 7479 7069 6e67 2e49  elf) -> typing.I
+00004080: 7465 7261 746f 725b 2747 656e 6572 6963  terator['Generic
+00004090: 5479 7065 275d 3a0a 2020 2020 2020 2020  Type']:.        
+000040a0: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
+000040b0: 7479 7065 3a20 7479 7069 6e67 2e49 7465  type: typing.Ite
+000040c0: 7261 746f 725b 2747 656e 6572 6963 5479  rator['GenericTy
+000040d0: 7065 275d 0a20 2020 2020 2020 2027 2727  pe'].        '''
+000040e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000040f0: 2020 2064 6566 205f 5f6e 6578 745f 5f28     def __next__(
+00004100: 7365 6c66 2920 2d3e 2027 4765 6e65 7269  self) -> 'Generi
+00004110: 6354 7970 6527 3a0a 2020 2020 2020 2020  cType':.        
+00004120: 2727 2720 0a0a 2020 2020 2020 2020 3a72  ''' ..        :r
+00004130: 7479 7065 3a20 2747 656e 6572 6963 5479  type: 'GenericTy
+00004140: 7065 270a 2020 2020 2020 2020 2727 270a  pe'.        '''.
+00004150: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00004160: 2020 6465 6620 5f5f 6c65 6e5f 5f28 7365    def __len__(se
+00004170: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00004180: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
+00004190: 2020 3a72 7479 7065 3a20 696e 740a 2020    :rtype: int.  
 000041a0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
 000041b0: 2020 7061 7373 0a0a 0a63 6c61 7373 2062    pass...class b
 000041c0: 7079 5f70 726f 705f 6172 7261 7928 7479  py_prop_array(ty
 000041d0: 7069 6e67 2e47 656e 6572 6963 5b47 656e  ping.Generic[Gen
 000041e0: 6572 6963 5479 7065 5d29 3a0a 2020 2020  ericType]):.    
 000041f0: 6465 6620 666f 7265 6163 685f 6765 7428  def foreach_get(
 00004200: 7365 6c66 2c20 6174 7472 2c20 7365 7129  self, attr, seq)
@@ -10305,27 +10305,27 @@
 00028400: 4b65 7966 7261 6d65 275d 0a20 2020 2027  Keyframe'].    '
 00028410: 2727 0a0a 2020 2020 7569 5f6c 6973 743a  ''..    ui_list:
 00028420: 2027 5549 4c69 7374 2720 3d20 4e6f 6e65   'UIList' = None
 00028430: 0a20 2020 2027 2727 200a 0a20 2020 203a  .    ''' ..    :
 00028440: 7479 7065 3a20 2755 494c 6973 7427 0a20  type: 'UIList'. 
 00028450: 2020 2027 2727 0a0a 2020 2020 7072 6f70     '''..    prop
 00028460: 6572 7479 3a20 7479 7069 6e67 2e55 6e69  erty: typing.Uni
-00028470: 6f6e 5b73 7472 2c20 696e 742c 2027 4944  on[str, int, 'ID
+00028470: 6f6e 5b69 6e74 2c20 7374 722c 2027 4944  on[int, str, 'ID
 00028480: 275d 203d 204e 6f6e 650a 2020 2020 2727  '] = None.    ''
 00028490: 2720 4765 7420 7468 6520 7072 6f70 6572  ' Get the proper
 000284a0: 7479 2061 7373 6f63 6961 7465 6420 7769  ty associated wi
 000284b0: 7468 2061 2068 6f76 6572 6564 2062 7574  th a hovered but
 000284c0: 746f 6e2e 2052 6574 7572 6e73 2061 2074  ton. Returns a t
 000284d0: 7570 6c65 206f 6620 7468 6520 6461 7461  uple of the data
 000284e0: 626c 6f63 6b2c 2064 6174 6120 7061 7468  block, data path
 000284f0: 2074 6f20 7468 6520 7072 6f70 6572 7479   to the property
 00028500: 2c20 616e 6420 6172 7261 7920 696e 6465  , and array inde
 00028510: 782e 0a0a 2020 2020 3a74 7970 653a 2074  x...    :type: t
-00028520: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
-00028530: 2069 6e74 2c20 2749 4427 5d0a 2020 2020   int, 'ID'].    
+00028520: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00028530: 2073 7472 2c20 2749 4427 5d0a 2020 2020   str, 'ID'].    
 00028540: 2727 270a 0a20 2020 2065 6469 745f 7465  '''..    edit_te
 00028550: 7874 3a20 2754 6578 7427 203d 204e 6f6e  xt: 'Text' = Non
 00028560: 650a 2020 2020 2727 2720 0a0a 2020 2020  e.    ''' ..    
 00028570: 3a74 7970 653a 2027 5465 7874 270a 2020  :type: 'Text'.  
 00028580: 2020 2727 270a 0a20 2020 2064 6566 2065    '''..    def e
 00028590: 7661 6c75 6174 6564 5f64 6570 7367 7261  valuated_depsgra
 000285a0: 7068 5f67 6574 2873 656c 6629 202d 3e20  ph_get(self) ->
```

### Comparing `fake-bpy-module-latest-20230802/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230803/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import previews
 from . import units
+from . import previews
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230802/bpy/utils/previews.py` & `fake-bpy-module-latest-20230803/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy/utils/units.py` & `fake-bpy-module-latest-20230803/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object'],
+        Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230803/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230803/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/bpy_types.py` & `fake-bpy-module-latest-20230803/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230802
+Version: 20230803
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230802/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230803/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230803/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/functions.py` & `fake-bpy-module-latest-20230803/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/predicates.py` & `fake-bpy-module-latest-20230803/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/shaders.py` & `fake-bpy-module-latest-20230803/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/types.py` & `fake-bpy-module-latest-20230803/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230803/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230803/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/capabilities.py` & `fake-bpy-module-latest-20230803/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/matrix.py` & `fake-bpy-module-latest-20230803/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/platform.py` & `fake-bpy-module-latest-20230803/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/shader.py` & `fake-bpy-module-latest-20230803/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/state.py` & `fake-bpy-module-latest-20230803/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/texture.py` & `fake-bpy-module-latest-20230803/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu/types.py` & `fake-bpy-module-latest-20230803/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu_extras/batch.py` & `fake-bpy-module-latest-20230803/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/gpu_extras/presets.py` & `fake-bpy-module-latest-20230803/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/idprop/types.py` & `fake-bpy-module-latest-20230803/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/imbuf/__init__.py` & `fake-bpy-module-latest-20230803/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/imbuf/types.py` & `fake-bpy-module-latest-20230803/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/keyingsets_builtins.py` & `fake-bpy-module-latest-20230803/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/keyingsets_utils.py` & `fake-bpy-module-latest-20230803/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/mathutils/__init__.py` & `fake-bpy-module-latest-20230803/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230803/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/mathutils/geometry.py` & `fake-bpy-module-latest-20230803/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/mathutils/kdtree.py` & `fake-bpy-module-latest-20230803/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/mathutils/noise.py` & `fake-bpy-module-latest-20230803/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/nodeitems_builtins.py` & `fake-bpy-module-latest-20230803/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/nodeitems_utils.py` & `fake-bpy-module-latest-20230803/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/rna_info.py` & `fake-bpy-module-latest-20230803/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/rna_keymap_ui.py` & `fake-bpy-module-latest-20230803/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/rna_prop_ui.py` & `fake-bpy-module-latest-20230803/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/rna_xml.py` & `fake-bpy-module-latest-20230803/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230802/setup.py` & `fake-bpy-module-latest-20230803/setup.py`

 * *Files identical despite different names*

