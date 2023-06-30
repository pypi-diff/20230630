# Comparing `tmp/fake-bpy-module-latest-20230628.tar.gz` & `tmp/fake-bpy-module-latest-20230629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230628.tar", last modified: Wed Jun 28 06:27:06 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230629.tar", last modified: Thu Jun 29 06:28:59 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230628.tar` & `fake-bpy-module-latest-20230629.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-28 06:24:32.000000 fake-bpy-module-latest-20230628/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-28 06:26:58.000000 fake-bpy-module-latest-20230628/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-28 06:26:58.000000 fake-bpy-module-latest-20230628/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-28 06:26:59.000000 fake-bpy-module-latest-20230628/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-28 06:26:58.000000 fake-bpy-module-latest-20230628/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-28 06:26:59.000000 fake-bpy-module-latest-20230628/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-28 06:27:01.000000 fake-bpy-module-latest-20230628/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-28 06:27:01.000000 fake-bpy-module-latest-20230628/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-28 06:27:01.000000 fake-bpy-module-latest-20230628/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-28 06:27:01.000000 fake-bpy-module-latest-20230628/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-28 06:27:01.000000 fake-bpy-module-latest-20230628/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-28 06:26:58.000000 fake-bpy-module-latest-20230628/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-28 06:27:00.000000 fake-bpy-module-latest-20230628/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-28 06:26:59.000000 fake-bpy-module-latest-20230628/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-28 06:26:57.000000 fake-bpy-module-latest-20230628/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-28 06:24:40.000000 fake-bpy-module-latest-20230628/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-28 06:26:48.000000 fake-bpy-module-latest-20230628/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-28 06:25:17.000000 fake-bpy-module-latest-20230628/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-28 06:25:23.000000 fake-bpy-module-latest-20230628/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-28 06:24:40.000000 fake-bpy-module-latest-20230628/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-28 06:26:51.000000 fake-bpy-module-latest-20230628/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-28 06:25:39.000000 fake-bpy-module-latest-20230628/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-28 06:26:48.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-28 06:25:17.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-28 06:25:11.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-28 06:24:41.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-28 06:24:43.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-28 06:24:59.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-28 06:24:44.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-28 06:26:50.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-28 06:24:45.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-28 06:25:00.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-28 06:24:54.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-28 06:24:44.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-28 06:24:45.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-28 06:24:48.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-28 06:24:48.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-28 06:26:49.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-28 06:25:18.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-28 06:24:45.000000 fake-bpy-module-latest-20230628/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-28 06:24:53.000000 fake-bpy-module-latest-20230628/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-28 06:25:40.000000 fake-bpy-module-latest-20230628/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-28 06:25:00.000000 fake-bpy-module-latest-20230628/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-28 06:24:51.000000 fake-bpy-module-latest-20230628/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-28 06:24:40.000000 fake-bpy-module-latest-20230628/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-28 06:24:45.000000 fake-bpy-module-latest-20230628/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-28 06:24:43.000000 fake-bpy-module-latest-20230628/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-28 06:24:55.000000 fake-bpy-module-latest-20230628/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-28 06:25:26.000000 fake-bpy-module-latest-20230628/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-28 06:26:47.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-28 06:25:17.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-28 06:26:45.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-28 06:24:52.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-28 06:24:51.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-28 06:26:48.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-28 06:24:52.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-28 06:25:39.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-28 06:25:17.000000 fake-bpy-module-latest-20230628/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    94500 2023-06-28 06:25:20.000000 fake-bpy-module-latest-20230628/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-28 06:24:49.000000 fake-bpy-module-latest-20230628/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-28 06:25:02.000000 fake-bpy-module-latest-20230628/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-28 06:26:46.000000 fake-bpy-module-latest-20230628/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-28 06:24:46.000000 fake-bpy-module-latest-20230628/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-28 06:24:59.000000 fake-bpy-module-latest-20230628/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-28 06:24:59.000000 fake-bpy-module-latest-20230628/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-28 06:24:55.000000 fake-bpy-module-latest-20230628/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-28 06:26:50.000000 fake-bpy-module-latest-20230628/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-28 06:24:48.000000 fake-bpy-module-latest-20230628/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-28 06:24:46.000000 fake-bpy-module-latest-20230628/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-28 06:26:48.000000 fake-bpy-module-latest-20230628/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-28 06:26:51.000000 fake-bpy-module-latest-20230628/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-28 06:24:47.000000 fake-bpy-module-latest-20230628/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-28 06:24:46.000000 fake-bpy-module-latest-20230628/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-28 06:26:44.000000 fake-bpy-module-latest-20230628/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-28 06:25:39.000000 fake-bpy-module-latest-20230628/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-28 06:24:47.000000 fake-bpy-module-latest-20230628/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-28 06:24:43.000000 fake-bpy-module-latest-20230628/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-28 06:24:51.000000 fake-bpy-module-latest-20230628/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-28 06:25:20.000000 fake-bpy-module-latest-20230628/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-28 06:24:41.000000 fake-bpy-module-latest-20230628/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-28 06:25:17.000000 fake-bpy-module-latest-20230628/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   618961 2023-06-28 06:26:40.000000 fake-bpy-module-latest-20230628/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-28 06:25:10.000000 fake-bpy-module-latest-20230628/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-28 06:25:11.000000 fake-bpy-module-latest-20230628/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-28 06:24:32.000000 fake-bpy-module-latest-20230628/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-28 06:23:42.000000 fake-bpy-module-latest-20230628/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-28 06:24:03.000000 fake-bpy-module-latest-20230628/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-28 06:24:02.000000 fake-bpy-module-latest-20230628/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-28 06:23:45.000000 fake-bpy-module-latest-20230628/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-28 06:24:27.000000 fake-bpy-module-latest-20230628/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-28 06:23:50.000000 fake-bpy-module-latest-20230628/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-28 06:24:21.000000 fake-bpy-module-latest-20230628/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-28 06:23:44.000000 fake-bpy-module-latest-20230628/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-28 06:23:51.000000 fake-bpy-module-latest-20230628/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-28 06:24:06.000000 fake-bpy-module-latest-20230628/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-28 06:24:22.000000 fake-bpy-module-latest-20230628/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-28 06:24:00.000000 fake-bpy-module-latest-20230628/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-28 06:23:56.000000 fake-bpy-module-latest-20230628/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-28 06:23:46.000000 fake-bpy-module-latest-20230628/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-28 06:24:01.000000 fake-bpy-module-latest-20230628/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-28 06:23:58.000000 fake-bpy-module-latest-20230628/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-28 06:23:51.000000 fake-bpy-module-latest-20230628/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-28 06:23:50.000000 fake-bpy-module-latest-20230628/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-28 06:24:28.000000 fake-bpy-module-latest-20230628/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-28 06:24:09.000000 fake-bpy-module-latest-20230628/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-28 06:23:55.000000 fake-bpy-module-latest-20230628/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-28 06:24:00.000000 fake-bpy-module-latest-20230628/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-28 06:24:27.000000 fake-bpy-module-latest-20230628/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-28 06:23:55.000000 fake-bpy-module-latest-20230628/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-28 06:24:21.000000 fake-bpy-module-latest-20230628/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-28 06:24:27.000000 fake-bpy-module-latest-20230628/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-28 06:24:03.000000 fake-bpy-module-latest-20230628/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-28 06:24:20.000000 fake-bpy-module-latest-20230628/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-28 06:24:00.000000 fake-bpy-module-latest-20230628/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-28 06:24:20.000000 fake-bpy-module-latest-20230628/bpy/ops/grease_pencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-28 06:23:56.000000 fake-bpy-module-latest-20230628/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-28 06:24:10.000000 fake-bpy-module-latest-20230628/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-28 06:24:10.000000 fake-bpy-module-latest-20230628/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-28 06:24:05.000000 fake-bpy-module-latest-20230628/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-28 06:24:22.000000 fake-bpy-module-latest-20230628/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-28 06:24:00.000000 fake-bpy-module-latest-20230628/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-28 06:23:56.000000 fake-bpy-module-latest-20230628/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-28 06:24:05.000000 fake-bpy-module-latest-20230628/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-28 06:24:18.000000 fake-bpy-module-latest-20230628/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-28 06:24:09.000000 fake-bpy-module-latest-20230628/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-28 06:24:09.000000 fake-bpy-module-latest-20230628/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-28 06:23:52.000000 fake-bpy-module-latest-20230628/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-06-28 06:24:26.000000 fake-bpy-module-latest-20230628/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-28 06:24:17.000000 fake-bpy-module-latest-20230628/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-28 06:23:46.000000 fake-bpy-module-latest-20230628/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-28 06:23:55.000000 fake-bpy-module-latest-20230628/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-28 06:24:23.000000 fake-bpy-module-latest-20230628/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-28 06:23:51.000000 fake-bpy-module-latest-20230628/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-28 06:23:50.000000 fake-bpy-module-latest-20230628/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-28 06:23:45.000000 fake-bpy-module-latest-20230628/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-28 06:24:22.000000 fake-bpy-module-latest-20230628/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-28 06:23:50.000000 fake-bpy-module-latest-20230628/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-28 06:23:51.000000 fake-bpy-module-latest-20230628/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-28 06:23:48.000000 fake-bpy-module-latest-20230628/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-28 06:23:42.000000 fake-bpy-module-latest-20230628/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-28 06:23:53.000000 fake-bpy-module-latest-20230628/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-28 06:24:00.000000 fake-bpy-module-latest-20230628/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-28 06:23:49.000000 fake-bpy-module-latest-20230628/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-28 06:24:03.000000 fake-bpy-module-latest-20230628/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-28 06:24:01.000000 fake-bpy-module-latest-20230628/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-28 06:23:44.000000 fake-bpy-module-latest-20230628/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-28 06:24:21.000000 fake-bpy-module-latest-20230628/bpy/ops/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70745 2023-06-28 06:24:05.000000 fake-bpy-module-latest-20230628/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-28 06:23:45.000000 fake-bpy-module-latest-20230628/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-28 06:23:50.000000 fake-bpy-module-latest-20230628/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    57277 2023-06-28 06:23:57.000000 fake-bpy-module-latest-20230628/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-28 06:24:06.000000 fake-bpy-module-latest-20230628/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-06-28 06:23:48.000000 fake-bpy-module-latest-20230628/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-28 06:24:17.000000 fake-bpy-module-latest-20230628/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-28 06:23:54.000000 fake-bpy-module-latest-20230628/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-28 06:24:30.000000 fake-bpy-module-latest-20230628/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-28 06:24:30.000000 fake-bpy-module-latest-20230628/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3496876 2023-06-28 06:23:42.000000 fake-bpy-module-latest-20230628/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-28 06:24:29.000000 fake-bpy-module-latest-20230628/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-28 06:24:36.000000 fake-bpy-module-latest-20230628/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-28 06:27:04.000000 fake-bpy-module-latest-20230628/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-28 06:24:35.000000 fake-bpy-module-latest-20230628/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-28 06:27:05.000000 fake-bpy-module-latest-20230628/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-28 06:24:33.000000 fake-bpy-module-latest-20230628/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-28 06:24:33.000000 fake-bpy-module-latest-20230628/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-28 06:24:33.000000 fake-bpy-module-latest-20230628/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-28 06:24:33.000000 fake-bpy-module-latest-20230628/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-28 06:24:34.000000 fake-bpy-module-latest-20230628/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 06:15:11.000000 fake-bpy-module-latest-20230628/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-28 06:24:39.000000 fake-bpy-module-latest-20230628/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-28 06:27:03.000000 fake-bpy-module-latest-20230628/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-28 06:27:06.000000 fake-bpy-module-latest-20230628/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-28 06:26:56.000000 fake-bpy-module-latest-20230628/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-29 06:28:58.000000 fake-bpy-module-latest-20230629/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30417 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-06-29 06:26:20.000000 fake-bpy-module-latest-20230629/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-06-29 06:28:50.000000 fake-bpy-module-latest-20230629/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-29 06:28:54.000000 fake-bpy-module-latest-20230629/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-29 06:28:50.000000 fake-bpy-module-latest-20230629/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-06-29 06:28:54.000000 fake-bpy-module-latest-20230629/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18689 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38122 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-29 06:28:54.000000 fake-bpy-module-latest-20230629/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 06:28:51.000000 fake-bpy-module-latest-20230629/bl_operators/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-29 06:28:55.000000 fake-bpy-module-latest-20230629/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-06-29 06:28:53.000000 fake-bpy-module-latest-20230629/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 06:28:58.000000 fake-bpy-module-latest-20230629/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-29 06:28:58.000000 fake-bpy-module-latest-20230629/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-29 06:28:08.000000 fake-bpy-module-latest-20230629/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110864 2023-06-29 06:28:10.000000 fake-bpy-module-latest-20230629/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-29 06:26:31.000000 fake-bpy-module-latest-20230629/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-06-29 06:28:25.000000 fake-bpy-module-latest-20230629/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-06-29 06:28:11.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-06-29 06:27:45.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-06-29 06:27:34.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-29 06:28:34.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-29 06:28:48.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-29 06:28:36.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-06-29 06:28:05.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-29 06:28:08.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-29 06:28:33.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-06-29 06:27:47.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-06-29 06:28:11.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52746 2023-06-29 06:27:57.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-29 06:27:46.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-29 06:28:33.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-29 06:28:48.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-06-29 06:28:33.000000 fake-bpy-module-latest-20230629/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-06-29 06:27:44.000000 fake-bpy-module-latest-20230629/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-06-29 06:27:50.000000 fake-bpy-module-latest-20230629/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-06-29 06:28:48.000000 fake-bpy-module-latest-20230629/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-06-29 06:27:40.000000 fake-bpy-module-latest-20230629/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-06-29 06:26:31.000000 fake-bpy-module-latest-20230629/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-06-29 06:27:42.000000 fake-bpy-module-latest-20230629/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-29 06:27:46.000000 fake-bpy-module-latest-20230629/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-06-29 06:28:28.000000 fake-bpy-module-latest-20230629/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-29 06:28:04.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-29 06:28:35.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-06-29 06:28:07.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-06-29 06:27:45.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-06-29 06:28:38.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-29 06:28:02.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-06-29 06:28:05.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-06-29 06:27:46.000000 fake-bpy-module-latest-20230629/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94500 2023-06-29 06:27:49.000000 fake-bpy-module-latest-20230629/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-06-29 06:28:04.000000 fake-bpy-module-latest-20230629/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-06-29 06:27:43.000000 fake-bpy-module-latest-20230629/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-29 06:27:46.000000 fake-bpy-module-latest-20230629/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-06-29 06:28:02.000000 fake-bpy-module-latest-20230629/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   176850 2023-06-29 06:28:01.000000 fake-bpy-module-latest-20230629/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64929 2023-06-29 06:28:35.000000 fake-bpy-module-latest-20230629/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-06-29 06:27:51.000000 fake-bpy-module-latest-20230629/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50899 2023-06-29 06:27:50.000000 fake-bpy-module-latest-20230629/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-06-29 06:28:33.000000 fake-bpy-module-latest-20230629/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-06-29 06:28:01.000000 fake-bpy-module-latest-20230629/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-06-29 06:28:03.000000 fake-bpy-module-latest-20230629/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75065 2023-06-29 06:28:08.000000 fake-bpy-module-latest-20230629/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-06-29 06:27:41.000000 fake-bpy-module-latest-20230629/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-29 06:27:40.000000 fake-bpy-module-latest-20230629/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-06-29 06:27:56.000000 fake-bpy-module-latest-20230629/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-29 06:28:35.000000 fake-bpy-module-latest-20230629/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-29 06:27:34.000000 fake-bpy-module-latest-20230629/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-06-29 06:28:39.000000 fake-bpy-module-latest-20230629/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-29 06:28:11.000000 fake-bpy-module-latest-20230629/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-06-29 06:28:03.000000 fake-bpy-module-latest-20230629/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-06-29 06:28:36.000000 fake-bpy-module-latest-20230629/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   215185 2023-06-29 06:27:40.000000 fake-bpy-module-latest-20230629/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   624121 2023-06-29 06:27:33.000000 fake-bpy-module-latest-20230629/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239548 2023-06-29 06:28:48.000000 fake-bpy-module-latest-20230629/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-29 06:27:34.000000 fake-bpy-module-latest-20230629/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-29 06:26:20.000000 fake-bpy-module-latest-20230629/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-29 06:26:28.000000 fake-bpy-module-latest-20230629/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77492 2023-06-29 06:26:28.000000 fake-bpy-module-latest-20230629/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-29 06:26:28.000000 fake-bpy-module-latest-20230629/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-29 06:26:28.000000 fake-bpy-module-latest-20230629/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-29 06:26:18.000000 fake-bpy-module-latest-20230629/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-06-29 06:16:43.000000 fake-bpy-module-latest-20230629/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-06-29 06:17:04.000000 fake-bpy-module-latest-20230629/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25486 2023-06-29 06:17:28.000000 fake-bpy-module-latest-20230629/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-29 06:17:08.000000 fake-bpy-module-latest-20230629/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-29 06:16:47.000000 fake-bpy-module-latest-20230629/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-29 06:16:58.000000 fake-bpy-module-latest-20230629/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-29 06:17:07.000000 fake-bpy-module-latest-20230629/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70588 2023-06-29 06:16:46.000000 fake-bpy-module-latest-20230629/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-29 06:17:29.000000 fake-bpy-module-latest-20230629/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-29 06:17:29.000000 fake-bpy-module-latest-20230629/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-29 06:17:13.000000 fake-bpy-module-latest-20230629/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-29 06:17:06.000000 fake-bpy-module-latest-20230629/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40670 2023-06-29 06:17:08.000000 fake-bpy-module-latest-20230629/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-29 06:16:58.000000 fake-bpy-module-latest-20230629/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-29 06:16:47.000000 fake-bpy-module-latest-20230629/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-29 06:16:43.000000 fake-bpy-module-latest-20230629/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-29 06:17:12.000000 fake-bpy-module-latest-20230629/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-29 06:16:52.000000 fake-bpy-module-latest-20230629/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-29 06:17:06.000000 fake-bpy-module-latest-20230629/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35992 2023-06-29 06:17:00.000000 fake-bpy-module-latest-20230629/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-06-29 06:16:49.000000 fake-bpy-module-latest-20230629/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-06-29 06:17:15.000000 fake-bpy-module-latest-20230629/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-29 06:17:07.000000 fake-bpy-module-latest-20230629/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-29 06:16:48.000000 fake-bpy-module-latest-20230629/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-06-29 06:17:27.000000 fake-bpy-module-latest-20230629/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50489 2023-06-29 06:16:47.000000 fake-bpy-module-latest-20230629/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-29 06:17:09.000000 fake-bpy-module-latest-20230629/bpy/ops/grease_pencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-06-29 06:16:52.000000 fake-bpy-module-latest-20230629/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-29 06:16:44.000000 fake-bpy-module-latest-20230629/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-29 06:17:23.000000 fake-bpy-module-latest-20230629/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-29 06:16:43.000000 fake-bpy-module-latest-20230629/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-29 06:17:24.000000 fake-bpy-module-latest-20230629/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-29 06:16:58.000000 fake-bpy-module-latest-20230629/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-29 06:17:07.000000 fake-bpy-module-latest-20230629/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-29 06:17:23.000000 fake-bpy-module-latest-20230629/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-29 06:16:47.000000 fake-bpy-module-latest-20230629/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179170 2023-06-29 06:16:56.000000 fake-bpy-module-latest-20230629/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-06-29 06:17:15.000000 fake-bpy-module-latest-20230629/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72286 2023-06-29 06:16:50.000000 fake-bpy-module-latest-20230629/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226228 2023-06-29 06:17:04.000000 fake-bpy-module-latest-20230629/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-06-29 06:17:24.000000 fake-bpy-module-latest-20230629/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44093 2023-06-29 06:17:09.000000 fake-bpy-module-latest-20230629/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-29 06:17:29.000000 fake-bpy-module-latest-20230629/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-29 06:17:04.000000 fake-bpy-module-latest-20230629/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-06-29 06:17:25.000000 fake-bpy-module-latest-20230629/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39854 2023-06-29 06:17:05.000000 fake-bpy-module-latest-20230629/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-29 06:17:11.000000 fake-bpy-module-latest-20230629/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32889 2023-06-29 06:16:48.000000 fake-bpy-module-latest-20230629/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-29 06:17:07.000000 fake-bpy-module-latest-20230629/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-06-29 06:17:08.000000 fake-bpy-module-latest-20230629/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-29 06:17:16.000000 fake-bpy-module-latest-20230629/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-06-29 06:16:45.000000 fake-bpy-module-latest-20230629/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-29 06:16:44.000000 fake-bpy-module-latest-20230629/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-29 06:17:04.000000 fake-bpy-module-latest-20230629/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-06-29 06:17:11.000000 fake-bpy-module-latest-20230629/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-29 06:17:12.000000 fake-bpy-module-latest-20230629/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94657 2023-06-29 06:17:15.000000 fake-bpy-module-latest-20230629/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-29 06:17:11.000000 fake-bpy-module-latest-20230629/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-29 06:17:07.000000 fake-bpy-module-latest-20230629/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-29 06:17:24.000000 fake-bpy-module-latest-20230629/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-06-29 06:16:52.000000 fake-bpy-module-latest-20230629/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-29 06:17:24.000000 fake-bpy-module-latest-20230629/bpy/ops/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-29 06:17:15.000000 fake-bpy-module-latest-20230629/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70745 2023-06-29 06:16:58.000000 fake-bpy-module-latest-20230629/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-06-29 06:17:23.000000 fake-bpy-module-latest-20230629/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-29 06:16:58.000000 fake-bpy-module-latest-20230629/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57277 2023-06-29 06:17:06.000000 fake-bpy-module-latest-20230629/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-29 06:17:25.000000 fake-bpy-module-latest-20230629/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54854 2023-06-29 06:17:12.000000 fake-bpy-module-latest-20230629/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246250 2023-06-29 06:17:23.000000 fake-bpy-module-latest-20230629/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-29 06:17:23.000000 fake-bpy-module-latest-20230629/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-29 06:16:44.000000 fake-bpy-module-latest-20230629/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-06-29 06:26:18.000000 fake-bpy-module-latest-20230629/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3497056 2023-06-29 06:26:17.000000 fake-bpy-module-latest-20230629/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-29 06:26:18.000000 fake-bpy-module-latest-20230629/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-29 06:26:18.000000 fake-bpy-module-latest-20230629/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-29 06:26:18.000000 fake-bpy-module-latest-20230629/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-06-29 06:26:25.000000 fake-bpy-module-latest-20230629/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-29 06:26:24.000000 fake-bpy-module-latest-20230629/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 06:26:28.000000 fake-bpy-module-latest-20230629/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-06-29 06:28:58.000000 fake-bpy-module-latest-20230629/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-29 06:26:30.000000 fake-bpy-module-latest-20230629/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-06-29 06:26:23.000000 fake-bpy-module-latest-20230629/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:16:42.000000 fake-bpy-module-latest-20230629/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-29 06:26:29.000000 fake-bpy-module-latest-20230629/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-29 06:28:56.000000 fake-bpy-module-latest-20230629/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 06:28:59.000000 fake-bpy-module-latest-20230629/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-29 06:28:58.000000 fake-bpy-module-latest-20230629/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 06:28:49.000000 fake-bpy-module-latest-20230629/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230628/PKG-INFO` & `fake-bpy-module-latest-20230629/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230628
+Version: 20230629
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230628/README.rst` & `fake-bpy-module-latest-20230629/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/addon_utils.py` & `fake-bpy-module-latest-20230629/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/animsys_refactor.py` & `fake-bpy-module-latest-20230629/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/aud.py` & `fake-bpy-module-latest-20230629/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bgl.py` & `fake-bpy-module-latest-20230629/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230629/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230629/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230629/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230629/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230629/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_math.py` & `fake-bpy-module-latest-20230629/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/__init__.py` & `fake-bpy-module-latest-20230629/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import sys
 import typing
-from . import constraint
-from . import screen_play_rendered_anim
-from . import image
-from . import file
-from . import vertexpaint_dirt
-from . import sequencer
-from . import object
-from . import add_mesh_torus
-from . import userpref
-from . import freestyle
-from . import anim
-from . import geometry_nodes
-from . import uvcalc_transform
-from . import assets
-from . import object_quick_effects
-from . import uvcalc_follow_active
 from . import uvcalc_lightmap
 from . import clip
+from . import file
+from . import object_quick_effects
 from . import text
-from . import mesh
-from . import presets
-from . import object_randomize_transform
+from . import anim
+from . import add_mesh_torus
 from . import node
-from . import object_align
-from . import rigidbody
+from . import constraint
 from . import wm
-from . import view3d
+from . import sequencer
+from . import freestyle
+from . import assets
 from . import spreadsheet
+from . import rigidbody
+from . import presets
 from . import console
+from . import image
+from . import geometry_nodes
+from . import uvcalc_transform
+from . import object
+from . import view3d
 from . import bmesh
+from . import mesh
+from . import object_randomize_transform
+from . import screen_play_rendered_anim
+from . import object_align
+from . import userpref
+from . import vertexpaint_dirt
+from . import uvcalc_follow_active
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230628/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230629/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/anim.py` & `fake-bpy-module-latest-20230629/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/assets.py` & `fake-bpy-module-latest-20230629/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230629/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/clip.py` & `fake-bpy-module-latest-20230629/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/console.py` & `fake-bpy-module-latest-20230629/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/constraint.py` & `fake-bpy-module-latest-20230629/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/file.py` & `fake-bpy-module-latest-20230629/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230629/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230629/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/image.py` & `fake-bpy-module-latest-20230629/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/mesh.py` & `fake-bpy-module-latest-20230629/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/node.py` & `fake-bpy-module-latest-20230629/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/object.py` & `fake-bpy-module-latest-20230629/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/object_align.py` & `fake-bpy-module-latest-20230629/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230629/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230629/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/presets.py` & `fake-bpy-module-latest-20230629/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230629/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230629/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230629/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230629/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/text.py` & `fake-bpy-module-latest-20230629/bl_operators/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/userpref.py` & `fake-bpy-module-latest-20230629/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230629/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230629/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230629/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230629/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/view3d.py` & `fake-bpy-module-latest-20230629/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_operators/wm.py` & `fake-bpy-module-latest-20230629/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230629/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/__init__.py` & `fake-bpy-module-latest-20230629/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_material_gpencil
-from . import properties_animviz
-from . import space_topbar
-from . import properties_data_curve
-from . import properties_output
-from . import space_time
-from . import properties_data_curves
-from . import properties_data_mesh
-from . import properties_data_gpencil
-from . import properties_data_volume
-from . import properties_data_metaball
-from . import properties_data_lattice
-from . import properties_object
-from . import properties_workspace
-from . import space_info
-from . import space_properties
-from . import space_outliner
-from . import space_text
-from . import space_graph
 from . import properties_data_modifier
-from . import properties_data_pointcloud
-from . import properties_scene
-from . import properties_physics_fluid
-from . import properties_material
-from . import space_toolsystem_common
-from . import properties_physics_rigidbody
-from . import properties_physics_field
-from . import properties_freestyle
-from . import properties_data_lightprobe
-from . import space_dopesheet
-from . import properties_paint_common
-from . import space_clip
-from . import properties_data_empty
 from . import space_console
-from . import properties_data_light
-from . import properties_mask_common
-from . import properties_texture
-from . import space_view3d_toolbar
+from . import properties_object
+from . import properties_physics_geometry_nodes
+from . import properties_collection
+from . import properties_material_gpencil
+from . import space_view3d
 from . import properties_data_camera
 from . import utils
+from . import space_statusbar
 from . import space_userpref
-from . import properties_physics_common
-from . import properties_physics_softbody
-from . import node_add_menu
+from . import space_properties
+from . import properties_material
+from . import space_outliner
+from . import properties_output
+from . import properties_texture
+from . import properties_freestyle
 from . import properties_data_bone
-from . import properties_data_speaker
+from . import properties_physics_field
+from . import properties_paint_common
+from . import properties_data_metaball
+from . import properties_workspace
+from . import properties_physics_softbody
+from . import properties_data_light
 from . import properties_render
-from . import space_toolsystem_toolbar
-from . import node_add_menu_geometry
-from . import properties_particle
-from . import properties_constraint
-from . import space_spreadsheet
-from . import properties_physics_rigidbody_constraint
 from . import properties_grease_pencil_common
-from . import space_view3d
+from . import space_graph
+from . import space_filebrowser
 from . import space_sequencer
-from . import properties_physics_dynamicpaint
-from . import properties_view_layer
-from . import properties_physics_cloth
-from . import properties_physics_geometry_nodes
+from . import properties_data_mesh
+from . import space_clip
+from . import space_info
+from . import properties_world
+from . import properties_physics_rigidbody
+from . import space_toolsystem_toolbar
 from . import space_nla
-from . import properties_data_armature
-from . import generic_ui_list
-from . import properties_data_shaderfx
-from . import space_filebrowser
-from . import properties_data_grease_pencil
+from . import properties_scene
+from . import properties_physics_cloth
+from . import properties_physics_rigidbody_constraint
+from . import properties_data_gpencil
+from . import properties_physics_dynamicpaint
 from . import space_node
-from . import properties_collection
+from . import properties_data_grease_pencil
+from . import generic_ui_list
+from . import node_add_menu_geometry
+from . import properties_data_armature
+from . import properties_data_lightprobe
+from . import space_time
+from . import properties_constraint
+from . import properties_particle
 from . import space_image
-from . import properties_world
-from . import space_statusbar
+from . import properties_data_lattice
+from . import properties_data_shaderfx
+from . import properties_data_volume
+from . import properties_data_curve
+from . import space_dopesheet
+from . import properties_physics_common
+from . import space_spreadsheet
+from . import space_topbar
+from . import properties_data_empty
+from . import properties_physics_fluid
+from . import space_text
+from . import space_view3d_toolbar
+from . import properties_mask_common
+from . import properties_data_curves
+from . import properties_data_speaker
+from . import properties_animviz
+from . import node_add_menu
+from . import properties_view_layer
+from . import properties_data_pointcloud
+from . import space_toolsystem_common
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230628/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230629/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230629/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_grease_pencil.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_geometry_nodes.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230629/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230629/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_console.py` & `fake-bpy-module-latest-20230629/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230629/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230629/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230629/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_image.py` & `fake-bpy-module-latest-20230629/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_info.py` & `fake-bpy-module-latest-20230629/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230629/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_node.py` & `fake-bpy-module-latest-20230629/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230629/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230629/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230629/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230629/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230629/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_text.py` & `fake-bpy-module-latest-20230629/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_time.py` & `fake-bpy-module-latest-20230629/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230629/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230629/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230629/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230629/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230629/bl_ui/space_view3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -13912,14 +13912,218 @@
     def values(self):
         ''' 
 
         '''
         pass
 
 
+class VIEW3D_MT_edit_pointcloud(bpy_types.Menu, bpy_types._GenericUI):
+    bl_label = None
+    ''' '''
+
+    bl_rna = None
+    ''' '''
+
+    id_data = None
+    ''' '''
+
+    def append(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def as_pointer(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass_py(self):
+        ''' 
+
+        '''
+        pass
+
+    def draw(self, _self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def draw_collapsible(self, context, layout):
+        ''' 
+
+        '''
+        pass
+
+    def draw_preset(self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def driver_add(self):
+        ''' 
+
+        '''
+        pass
+
+    def driver_remove(self):
+        ''' 
+
+        '''
+        pass
+
+    def get(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_clear(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ensure(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ui(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_extended(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_hidden(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_overridable_library(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_readonly(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def items(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_delete(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_insert(self):
+        ''' 
+
+        '''
+        pass
+
+    def keys(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_from_id(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_menu(self, searchpaths, operator, props_default, prop_filepath,
+                  filter_ext, filter_path, display_name, add_operator):
+        ''' 
+
+        '''
+        pass
+
+    def path_resolve(self):
+        ''' 
+
+        '''
+        pass
+
+    def pop(self):
+        ''' 
+
+        '''
+        pass
+
+    def prepend(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def property_overridable_library_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def property_unset(self):
+        ''' 
+
+        '''
+        pass
+
+    def remove(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def type_recast(self):
+        ''' 
+
+        '''
+        pass
+
+    def values(self):
+        ''' 
+
+        '''
+        pass
+
+
 class VIEW3D_MT_edit_surface(bpy_types.Menu, bpy_types._GenericUI):
     bl_label = None
     ''' '''
 
     bl_rna = None
     ''' '''
 
@@ -29088,14 +29292,218 @@
         ''' 
 
         '''
         pass
 
     def draw_collapsible(self, context, layout):
         ''' 
+
+        '''
+        pass
+
+    def draw_preset(self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def driver_add(self):
+        ''' 
+
+        '''
+        pass
+
+    def driver_remove(self):
+        ''' 
+
+        '''
+        pass
+
+    def get(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_clear(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ensure(self):
+        ''' 
+
+        '''
+        pass
+
+    def id_properties_ui(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_extended(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_hidden(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_overridable_library(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_readonly(self):
+        ''' 
+
+        '''
+        pass
+
+    def is_property_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def items(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_delete(self):
+        ''' 
+
+        '''
+        pass
+
+    def keyframe_insert(self):
+        ''' 
+
+        '''
+        pass
+
+    def keys(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_from_id(self):
+        ''' 
+
+        '''
+        pass
+
+    def path_menu(self, searchpaths, operator, props_default, prop_filepath,
+                  filter_ext, filter_path, display_name, add_operator):
+        ''' 
+
+        '''
+        pass
+
+    def path_resolve(self):
+        ''' 
+
+        '''
+        pass
+
+    def pop(self):
+        ''' 
+
+        '''
+        pass
+
+    def prepend(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def property_overridable_library_set(self):
+        ''' 
+
+        '''
+        pass
+
+    def property_unset(self):
+        ''' 
+
+        '''
+        pass
+
+    def remove(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def type_recast(self):
+        ''' 
+
+        '''
+        pass
+
+    def values(self):
+        ''' 
+
+        '''
+        pass
+
+
+class VIEW3D_MT_select_edit_point_cloud(bpy_types.Menu, bpy_types._GenericUI):
+    bl_label = None
+    ''' '''
+
+    bl_rna = None
+    ''' '''
+
+    id_data = None
+    ''' '''
+
+    def append(self, draw_func):
+        ''' 
+
+        '''
+        pass
+
+    def as_pointer(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass(self):
+        ''' 
+
+        '''
+        pass
+
+    def bl_rna_get_subclass_py(self):
+        ''' 
+
+        '''
+        pass
+
+    def draw(self, _self, _context):
+        ''' 
+
+        '''
+        pass
+
+    def draw_collapsible(self, context, layout):
+        ''' 
 
         '''
         pass
 
     def draw_preset(self, _context):
         '''
```

### Comparing `fake-bpy-module-latest-20230628/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230629/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bl_ui/utils.py` & `fake-bpy-module-latest-20230629/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/blf.py` & `fake-bpy-module-latest-20230629/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bmesh/__init__.py` & `fake-bpy-module-latest-20230629/bmesh/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import typing
 import bpy.types
 import bmesh.types
 
+from . import ops
 from . import types
 from . import utils
-from . import ops
 from . import geometry
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def from_edit_mesh(mesh: 'bpy.types.Mesh') -> 'bmesh.types.BMesh':
     ''' Return a BMesh from this mesh, currently the mesh must already be in editmode.
```

### Comparing `fake-bpy-module-latest-20230628/bmesh/geometry.py` & `fake-bpy-module-latest-20230629/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bmesh/ops.py` & `fake-bpy-module-latest-20230629/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bmesh/types.py` & `fake-bpy-module-latest-20230629/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bmesh/utils.py` & `fake-bpy-module-latest-20230629/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/app/__init__.py` & `fake-bpy-module-latest-20230629/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import typing
+from . import icons
 from . import timers
 from . import handlers
-from . import icons
 from . import translations
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def help_text(all: typing.Optional[bool] = False):
     ''' Return the help text as a string.
```

### Comparing `fake-bpy-module-latest-20230628/bpy/app/handlers.py` & `fake-bpy-module-latest-20230629/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/app/icons.py` & `fake-bpy-module-latest-20230629/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/app/timers.py` & `fake-bpy-module-latest-20230629/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/app/translations.py` & `fake-bpy-module-latest-20230629/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/msgbus.py` & `fake-bpy-module-latest-20230629/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230629/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 import sys
 import typing
-from . import scene
-from . import surface
-from . import buttons
-from . import ui
-from . import armature
-from . import poselib
-from . import paint
-from . import constraint
-from . import view3d
-from . import rigidbody
-from . import sculpt
-from . import pose
-from . import uilist
+from . import import_scene
 from . import dpaint
-from . import boid
-from . import ptcache
-from . import particle
-from . import render
-from . import cycles
-from . import cachefile
-from . import node
+from . import action
 from . import screen
-from . import mask
-from . import import_curve
-from . import text
-from . import sculpt_curves
+from . import import_anim
 from . import world
-from . import cloth
-from . import workspace
-from . import export_mesh
-from . import paintcurve
+from . import mask
 from . import fluid
-from . import image
-from . import console
-from . import marker
-from . import uv
-from . import curves
-from . import export_scene
-from . import script
-from . import collection
+from . import buttons
+from . import scene
+from . import import_curve
+from . import camera
+from . import clip
 from . import graph
-from . import lattice
-from . import curve
-from . import spreadsheet
-from . import anim
-from . import sound
-from . import action
+from . import mball
+from . import boid
+from . import cycles
+from . import preferences
 from . import gizmogroup
-from . import transform
-from . import material
-from . import import_scene
-from . import view2d
-from . import camera
-from . import mesh
-from . import nla
+from . import file
+from . import node
+from . import image
 from . import export_anim
-from . import import_anim
-from . import import_mesh
-from . import wm
-from . import outliner
-from . import mball
-from . import gpencil
-from . import grease_pencil
-from . import font
-from . import text_editor
+from . import text
+from . import mesh
+from . import transform
 from . import brush
-from . import clip
-from . import info
-from . import preferences
-from . import palette
+from . import curves
+from . import lattice
+from . import uilist
+from . import export_scene
 from . import object
-from . import file
+from . import script
+from . import palette
+from . import anim
+from . import pose
+from . import uv
+from . import constraint
+from . import export_mesh
+from . import cachefile
+from . import marker
+from . import ptcache
 from . import geometry
+from . import spreadsheet
+from . import render
+from . import curve
 from . import asset
+from . import grease_pencil
+from . import paint
+from . import sculpt
+from . import sound
+from . import poselib
+from . import view3d
+from . import sculpt_curves
 from . import ed
+from . import console
 from . import sequencer
+from . import nla
 from . import texture
+from . import font
+from . import rigidbody
+from . import wm
+from . import material
+from . import import_mesh
+from . import ui
+from . import workspace
+from . import outliner
+from . import info
+from . import surface
+from . import text_editor
+from . import particle
+from . import view2d
+from . import gpencil
+from . import armature
+from . import collection
+from . import paintcurve
+from . import cloth
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/action.py` & `fake-bpy-module-latest-20230629/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/anim.py` & `fake-bpy-module-latest-20230629/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/armature.py` & `fake-bpy-module-latest-20230629/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/asset.py` & `fake-bpy-module-latest-20230629/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/boid.py` & `fake-bpy-module-latest-20230629/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/brush.py` & `fake-bpy-module-latest-20230629/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230629/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230629/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/camera.py` & `fake-bpy-module-latest-20230629/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/clip.py` & `fake-bpy-module-latest-20230629/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230629/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/collection.py` & `fake-bpy-module-latest-20230629/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/console.py` & `fake-bpy-module-latest-20230629/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230629/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/curve.py` & `fake-bpy-module-latest-20230629/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/curves.py` & `fake-bpy-module-latest-20230629/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230629/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230629/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/ed.py` & `fake-bpy-module-latest-20230629/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230629/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230629/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230629/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/file.py` & `fake-bpy-module-latest-20230629/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230629/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/font.py` & `fake-bpy-module-latest-20230629/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230629/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230629/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230629/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/graph.py` & `fake-bpy-module-latest-20230629/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/grease_pencil.py` & `fake-bpy-module-latest-20230629/bpy/ops/grease_pencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/image.py` & `fake-bpy-module-latest-20230629/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230629/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230629/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230629/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230629/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/info.py` & `fake-bpy-module-latest-20230629/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230629/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/marker.py` & `fake-bpy-module-latest-20230629/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/mask.py` & `fake-bpy-module-latest-20230629/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/material.py` & `fake-bpy-module-latest-20230629/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/mball.py` & `fake-bpy-module-latest-20230629/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230629/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/nla.py` & `fake-bpy-module-latest-20230629/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/node.py` & `fake-bpy-module-latest-20230629/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/object.py` & `fake-bpy-module-latest-20230629/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230629/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/paint.py` & `fake-bpy-module-latest-20230629/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230629/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/palette.py` & `fake-bpy-module-latest-20230629/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/particle.py` & `fake-bpy-module-latest-20230629/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/pose.py` & `fake-bpy-module-latest-20230629/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230629/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230629/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230629/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/render.py` & `fake-bpy-module-latest-20230629/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230629/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/scene.py` & `fake-bpy-module-latest-20230629/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/screen.py` & `fake-bpy-module-latest-20230629/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/script.py` & `fake-bpy-module-latest-20230629/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230629/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230629/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230629/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/sound.py` & `fake-bpy-module-latest-20230629/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230629/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/surface.py` & `fake-bpy-module-latest-20230629/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/text.py` & `fake-bpy-module-latest-20230629/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/text_editor.py` & `fake-bpy-module-latest-20230629/bpy/ops/text_editor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/texture.py` & `fake-bpy-module-latest-20230629/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/transform.py` & `fake-bpy-module-latest-20230629/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/ui.py` & `fake-bpy-module-latest-20230629/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230629/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/uv.py` & `fake-bpy-module-latest-20230629/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230629/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230629/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/wm.py` & `fake-bpy-module-latest-20230629/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230629/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/ops/world.py` & `fake-bpy-module-latest-20230629/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/path.py` & `fake-bpy-module-latest-20230629/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/props.py` & `fake-bpy-module-latest-20230629/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/types.py` & `fake-bpy-module-latest-20230629/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,180 +1,180 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7072 6f70 6572 7469 6573 5f6d 6174  i.properties_mat
-00000050: 6572 6961 6c5f 6770 656e 6369 6c0a 696d  erial_gpencil.im
-00000060: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000070: 5f74 6f70 6261 720a 696d 706f 7274 2062  _topbar.import b
-00000080: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000090: 6461 7461 5f63 7572 7665 0a69 6d70 6f72  data_curve.impor
-000000a0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000000b0: 6573 5f6f 7574 7075 740a 696d 706f 7274  es_output.import
-000000c0: 2062 6c5f 7569 2e73 7061 6365 5f74 696d   bl_ui.space_tim
-000000d0: 650a 696d 706f 7274 2062 6c5f 6f70 6572  e.import bl_oper
-000000e0: 6174 6f72 732e 636f 6e73 7472 6169 6e74  ators.constraint
-000000f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000100: 6f70 6572 7469 6573 5f64 6174 615f 6375  operties_data_cu
-00000110: 7276 6573 0a69 6d70 6f72 7420 626c 5f75  rves.import bl_u
-00000120: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000130: 615f 6d65 7368 0a69 6d70 6f72 7420 626c  a_mesh.import bl
-00000140: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
-00000150: 6174 615f 6770 656e 6369 6c0a 696d 706f  ata_gpencil.impo
+00000040: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000050: 615f 6d6f 6469 6669 6572 0a69 6d70 6f72  a_modifier.impor
+00000060: 7420 626c 5f75 692e 7370 6163 655f 636f  t bl_ui.space_co
+00000070: 6e73 6f6c 650a 696d 706f 7274 2062 6c5f  nsole.import bl_
+00000080: 7569 2e70 726f 7065 7274 6965 735f 6f62  ui.properties_ob
+00000090: 6a65 6374 0a69 6d70 6f72 7420 626c 5f6f  ject.import bl_o
+000000a0: 7065 7261 746f 7273 2e63 6c69 700a 696d  perators.clip.im
+000000b0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000000c0: 7274 6965 735f 7068 7973 6963 735f 6765  rties_physics_ge
+000000d0: 6f6d 6574 7279 5f6e 6f64 6573 0a69 6d70  ometry_nodes.imp
+000000e0: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+000000f0: 2e66 696c 650a 696d 706f 7274 2062 6c5f  .file.import bl_
+00000100: 7569 2e70 726f 7065 7274 6965 735f 636f  ui.properties_co
+00000110: 6c6c 6563 7469 6f6e 0a69 6d70 6f72 7420  llection.import 
+00000120: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000130: 5f6d 6174 6572 6961 6c5f 6770 656e 6369  _material_gpenci
+00000140: 6c0a 696d 706f 7274 2062 6c5f 7569 2e73  l.import bl_ui.s
+00000150: 7061 6365 5f76 6965 7733 640a 696d 706f  pace_view3d.impo
 00000160: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000170: 6965 735f 6461 7461 5f76 6f6c 756d 650a  ies_data_volume.
-00000180: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-00000190: 6f72 732e 6669 6c65 0a69 6d70 6f72 7420  ors.file.import 
-000001a0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000001b0: 5f64 6174 615f 6d65 7461 6261 6c6c 0a69  _data_metaball.i
-000001c0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000001d0: 6572 7469 6573 5f64 6174 615f 6c61 7474  erties_data_latt
-000001e0: 6963 650a 696d 706f 7274 2062 6c5f 6f70  ice.import bl_op
-000001f0: 6572 6174 6f72 732e 6f62 6a65 6374 0a69  erators.object.i
-00000200: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000210: 6572 7469 6573 5f6f 626a 6563 740a 696d  erties_object.im
-00000220: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000230: 7274 6965 735f 776f 726b 7370 6163 650a  rties_workspace.
-00000240: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000250: 6365 5f69 6e66 6f0a 696d 706f 7274 2062  ce_info.import b
-00000260: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
-00000270: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
-00000280: 7569 2e73 7061 6365 5f6f 7574 6c69 6e65  ui.space_outline
-00000290: 720a 696d 706f 7274 2062 6c5f 7569 2e73  r.import bl_ui.s
-000002a0: 7061 6365 5f74 6578 740a 696d 706f 7274  pace_text.import
-000002b0: 2062 6c5f 7569 2e73 7061 6365 5f67 7261   bl_ui.space_gra
-000002c0: 7068 0a69 6d70 6f72 7420 626c 5f75 692e  ph.import bl_ui.
-000002d0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000002e0: 6d6f 6469 6669 6572 0a69 6d70 6f72 7420  modifier.import 
-000002f0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000300: 5f64 6174 615f 706f 696e 7463 6c6f 7564  _data_pointcloud
-00000310: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000320: 6f70 6572 7469 6573 5f73 6365 6e65 0a69  operties_scene.i
-00000330: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000340: 7273 2e75 7365 7270 7265 660a 696d 706f  rs.userpref.impo
-00000350: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000360: 6965 735f 7068 7973 6963 735f 666c 7569  ies_physics_flui
-00000370: 640a 696d 706f 7274 2062 6c5f 7569 2e70  d.import bl_ui.p
-00000380: 726f 7065 7274 6965 735f 6d61 7465 7269  roperties_materi
-00000390: 616c 0a69 6d70 6f72 7420 626c 5f6f 7065  al.import bl_ope
-000003a0: 7261 746f 7273 2e66 7265 6573 7479 6c65  rators.freestyle
-000003b0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000003c0: 746f 7273 2e61 6e69 6d0a 696d 706f 7274  tors.anim.import
-000003d0: 2062 6c5f 7569 2e73 7061 6365 5f74 6f6f   bl_ui.space_too
-000003e0: 6c73 7973 7465 6d5f 636f 6d6d 6f6e 0a69  lsystem_common.i
-000003f0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000400: 6572 7469 6573 5f70 6879 7369 6373 5f72  erties_physics_r
-00000410: 6967 6964 626f 6479 0a69 6d70 6f72 7420  igidbody.import 
-00000420: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000430: 5f70 6879 7369 6373 5f66 6965 6c64 0a69  _physics_field.i
-00000440: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000450: 7273 2e61 7373 6574 730a 696d 706f 7274  rs.assets.import
-00000460: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000470: 735f 6672 6565 7374 796c 650a 696d 706f  s_freestyle.impo
-00000480: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000490: 6965 735f 6461 7461 5f6c 6967 6874 7072  ies_data_lightpr
-000004a0: 6f62 650a 696d 706f 7274 2062 6c5f 7569  obe.import bl_ui
-000004b0: 2e73 7061 6365 5f64 6f70 6573 6865 6574  .space_dopesheet
-000004c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000004d0: 6f70 6572 7469 6573 5f70 6169 6e74 5f63  operties_paint_c
-000004e0: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
-000004f0: 7569 2e73 7061 6365 5f63 6c69 700a 696d  ui.space_clip.im
-00000500: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000510: 7274 6965 735f 6461 7461 5f65 6d70 7479  rties_data_empty
-00000520: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000530: 6163 655f 636f 6e73 6f6c 650a 696d 706f  ace_console.impo
-00000540: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000550: 6965 735f 6461 7461 5f6c 6967 6874 0a69  ies_data_light.i
+00000170: 6965 735f 6461 7461 5f63 616d 6572 610a  ies_data_camera.
+00000180: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000190: 6365 5f73 7461 7475 7362 6172 0a69 6d70  ce_statusbar.imp
+000001a0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000001b0: 7573 6572 7072 6566 0a69 6d70 6f72 7420  userpref.import 
+000001c0: 626c 5f75 692e 7370 6163 655f 7072 6f70  bl_ui.space_prop
+000001d0: 6572 7469 6573 0a69 6d70 6f72 7420 626c  erties.import bl
+000001e0: 5f6f 7065 7261 746f 7273 2e74 6578 740a  _operators.text.
+000001f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000200: 7065 7274 6965 735f 6d61 7465 7269 616c  perties_material
+00000210: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000220: 6163 655f 6f75 746c 696e 6572 0a69 6d70  ace_outliner.imp
+00000230: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000240: 7469 6573 5f6f 7574 7075 740a 696d 706f  ties_output.impo
+00000250: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000260: 6965 735f 7465 7874 7572 650a 696d 706f  ies_texture.impo
+00000270: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000280: 6965 735f 6672 6565 7374 796c 650a 696d  ies_freestyle.im
+00000290: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000002a0: 7274 6965 735f 6461 7461 5f62 6f6e 650a  rties_data_bone.
+000002b0: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000002c0: 6f72 732e 616e 696d 0a69 6d70 6f72 7420  ors.anim.import 
+000002d0: 626c 5f6f 7065 7261 746f 7273 2e6e 6f64  bl_operators.nod
+000002e0: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
+000002f0: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+00000300: 735f 6669 656c 640a 696d 706f 7274 2062  s_field.import b
+00000310: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000320: 7061 696e 745f 636f 6d6d 6f6e 0a69 6d70  paint_common.imp
+00000330: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000340: 7469 6573 5f64 6174 615f 6d65 7461 6261  ties_data_metaba
+00000350: 6c6c 0a69 6d70 6f72 7420 626c 5f75 692e  ll.import bl_ui.
+00000360: 7072 6f70 6572 7469 6573 5f77 6f72 6b73  properties_works
+00000370: 7061 6365 0a69 6d70 6f72 7420 626c 5f6f  pace.import bl_o
+00000380: 7065 7261 746f 7273 2e63 6f6e 7374 7261  perators.constra
+00000390: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
+000003a0: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
+000003b0: 6963 735f 736f 6674 626f 6479 0a69 6d70  ics_softbody.imp
+000003c0: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+000003d0: 2e77 6d0a 696d 706f 7274 2062 6c5f 7569  .wm.import bl_ui
+000003e0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+000003f0: 5f6c 6967 6874 0a69 6d70 6f72 7420 626c  _light.import bl
+00000400: 5f75 692e 7072 6f70 6572 7469 6573 5f72  _ui.properties_r
+00000410: 656e 6465 720a 696d 706f 7274 2062 6c5f  ender.import bl_
+00000420: 7569 2e70 726f 7065 7274 6965 735f 6772  ui.properties_gr
+00000430: 6561 7365 5f70 656e 6369 6c5f 636f 6d6d  ease_pencil_comm
+00000440: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
+00000450: 7370 6163 655f 6772 6170 680a 696d 706f  space_graph.impo
+00000460: 7274 2062 6c5f 7569 2e73 7061 6365 5f66  rt bl_ui.space_f
+00000470: 696c 6562 726f 7773 6572 0a69 6d70 6f72  ilebrowser.impor
+00000480: 7420 626c 5f75 692e 7370 6163 655f 7365  t bl_ui.space_se
+00000490: 7175 656e 6365 720a 696d 706f 7274 2062  quencer.import b
+000004a0: 6c5f 6f70 6572 6174 6f72 732e 6672 6565  l_operators.free
+000004b0: 7374 796c 650a 696d 706f 7274 2062 6c5f  style.import bl_
+000004c0: 6f70 6572 6174 6f72 732e 6173 7365 7473  operators.assets
+000004d0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000004e0: 6f70 6572 7469 6573 5f64 6174 615f 6d65  operties_data_me
+000004f0: 7368 0a69 6d70 6f72 7420 626c 5f6f 7065  sh.import bl_ope
+00000500: 7261 746f 7273 2e73 7072 6561 6473 6865  rators.spreadshe
+00000510: 6574 0a69 6d70 6f72 7420 626c 5f75 692e  et.import bl_ui.
+00000520: 7370 6163 655f 636c 6970 0a69 6d70 6f72  space_clip.impor
+00000530: 7420 626c 5f75 692e 7370 6163 655f 696e  t bl_ui.space_in
+00000540: 666f 0a69 6d70 6f72 7420 626c 5f6f 7065  fo.import bl_ope
+00000550: 7261 746f 7273 2e70 7265 7365 7473 0a69  rators.presets.i
 00000560: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000570: 6572 7469 6573 5f6d 6173 6b5f 636f 6d6d  erties_mask_comm
-00000580: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-00000590: 7072 6f70 6572 7469 6573 5f74 6578 7475  properties_textu
-000005a0: 7265 0a69 6d70 6f72 7420 626c 5f75 692e  re.import bl_ui.
-000005b0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-000005c0: 6c62 6172 0a69 6d70 6f72 7420 626c 5f6f  lbar.import bl_o
-000005d0: 7065 7261 746f 7273 2e63 6c69 700a 696d  perators.clip.im
-000005e0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-000005f0: 7274 6965 735f 6461 7461 5f63 616d 6572  rties_data_camer
-00000600: 610a 696d 706f 7274 2062 6c5f 6f70 6572  a.import bl_oper
-00000610: 6174 6f72 732e 7465 7874 0a69 6d70 6f72  ators.text.impor
-00000620: 7420 626c 5f6f 7065 7261 746f 7273 2e70  t bl_operators.p
-00000630: 7265 7365 7473 0a69 6d70 6f72 7420 626c  resets.import bl
-00000640: 5f75 692e 7370 6163 655f 7573 6572 7072  _ui.space_userpr
-00000650: 6566 0a69 6d70 6f72 7420 626c 5f75 692e  ef.import bl_ui.
-00000660: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-00000670: 6373 5f63 6f6d 6d6f 6e0a 696d 706f 7274  cs_common.import
-00000680: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000690: 735f 7068 7973 6963 735f 736f 6674 626f  s_physics_softbo
-000006a0: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
-000006b0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000006c0: 626f 6e65 0a69 6d70 6f72 7420 626c 5f75  bone.import bl_u
-000006d0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-000006e0: 615f 7370 6561 6b65 720a 696d 706f 7274  a_speaker.import
-000006f0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000700: 735f 7265 6e64 6572 0a69 6d70 6f72 7420  s_render.import 
-00000710: 626c 5f75 692e 7370 6163 655f 746f 6f6c  bl_ui.space_tool
-00000720: 7379 7374 656d 5f74 6f6f 6c62 6172 0a69  system_toolbar.i
-00000730: 6d70 6f72 7420 626c 5f75 692e 6e6f 6465  mport bl_ui.node
-00000740: 5f61 6464 5f6d 656e 755f 6765 6f6d 6574  _add_menu_geomet
-00000750: 7279 0a69 6d70 6f72 7420 626c 5f75 692e  ry.import bl_ui.
-00000760: 7072 6f70 6572 7469 6573 5f70 6172 7469  properties_parti
-00000770: 636c 650a 696d 706f 7274 2062 6c5f 6f70  cle.import bl_op
-00000780: 6572 6174 6f72 732e 6e6f 6465 0a69 6d70  erators.node.imp
-00000790: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000007a0: 7469 6573 5f63 6f6e 7374 7261 696e 740a  ties_constraint.
-000007b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000007c0: 6365 5f73 7072 6561 6473 6865 6574 0a69  ce_spreadsheet.i
-000007d0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000007e0: 6572 7469 6573 5f70 6879 7369 6373 5f72  erties_physics_r
-000007f0: 6967 6964 626f 6479 5f63 6f6e 7374 7261  igidbody_constra
-00000800: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
-00000810: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000820: 6f70 6572 7469 6573 5f67 7265 6173 655f  operties_grease_
-00000830: 7065 6e63 696c 5f63 6f6d 6d6f 6e0a 696d  pencil_common.im
-00000840: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000850: 5f76 6965 7733 640a 696d 706f 7274 2062  _view3d.import b
-00000860: 6c5f 7569 2e73 7061 6365 5f73 6571 7565  l_ui.space_seque
-00000870: 6e63 6572 0a69 6d70 6f72 7420 626c 5f75  ncer.import bl_u
-00000880: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-00000890: 7369 6373 5f64 796e 616d 6963 7061 696e  sics_dynamicpain
-000008a0: 740a 696d 706f 7274 2062 6c5f 7569 2e70  t.import bl_ui.p
-000008b0: 726f 7065 7274 6965 735f 7669 6577 5f6c  roperties_view_l
-000008c0: 6179 6572 0a69 6d70 6f72 7420 626c 5f75  ayer.import bl_u
-000008d0: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-000008e0: 7369 6373 5f63 6c6f 7468 0a69 6d70 6f72  sics_cloth.impor
-000008f0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000900: 6573 5f70 6879 7369 6373 5f67 656f 6d65  es_physics_geome
-00000910: 7472 795f 6e6f 6465 730a 696d 706f 7274  try_nodes.import
-00000920: 2062 6c5f 6f70 6572 6174 6f72 732e 776d   bl_operators.wm
-00000930: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000940: 6163 655f 6e6c 610a 696d 706f 7274 2062  ace_nla.import b
-00000950: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000960: 6461 7461 5f61 726d 6174 7572 650a 696d  data_armature.im
-00000970: 706f 7274 2062 6c5f 7569 2e67 656e 6572  port bl_ui.gener
-00000980: 6963 5f75 695f 6c69 7374 0a69 6d70 6f72  ic_ui_list.impor
-00000990: 7420 626c 5f6f 7065 7261 746f 7273 2e76  t bl_operators.v
-000009a0: 6965 7733 640a 696d 706f 7274 2062 6c5f  iew3d.import bl_
-000009b0: 6f70 6572 6174 6f72 732e 7370 7265 6164  operators.spread
-000009c0: 7368 6565 740a 696d 706f 7274 2062 6c5f  sheet.import bl_
-000009d0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-000009e0: 7461 5f73 6861 6465 7266 780a 696d 706f  ta_shaderfx.impo
-000009f0: 7274 2062 6c5f 7569 2e73 7061 6365 5f66  rt bl_ui.space_f
-00000a00: 696c 6562 726f 7773 6572 0a69 6d70 6f72  ilebrowser.impor
-00000a10: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000a20: 6573 5f64 6174 615f 6772 6561 7365 5f70  es_data_grease_p
-00000a30: 656e 6369 6c0a 696d 706f 7274 2062 6c5f  encil.import bl_
-00000a40: 7569 2e73 7061 6365 5f6e 6f64 650a 696d  ui.space_node.im
-00000a50: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000a60: 7274 6965 735f 636f 6c6c 6563 7469 6f6e  rties_collection
-00000a70: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000a80: 6163 655f 696d 6167 650a 696d 706f 7274  ace_image.import
-00000a90: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000aa0: 735f 776f 726c 640a 696d 706f 7274 2062  s_world.import b
-00000ab0: 6c5f 7569 2e73 7061 6365 5f73 7461 7475  l_ui.space_statu
-00000ac0: 7362 6172 0a0a 4765 6e65 7269 6354 7970  sbar..GenericTyp
+00000570: 6572 7469 6573 5f77 6f72 6c64 0a69 6d70  erties_world.imp
+00000580: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000590: 7469 6573 5f70 6879 7369 6373 5f72 6967  ties_physics_rig
+000005a0: 6964 626f 6479 0a69 6d70 6f72 7420 626c  idbody.import bl
+000005b0: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
+000005c0: 7374 656d 5f74 6f6f 6c62 6172 0a69 6d70  stem_toolbar.imp
+000005d0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000005e0: 6e6c 610a 696d 706f 7274 2062 6c5f 7569  nla.import bl_ui
+000005f0: 2e70 726f 7065 7274 6965 735f 7363 656e  .properties_scen
+00000600: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
+00000610: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+00000620: 735f 636c 6f74 680a 696d 706f 7274 2062  s_cloth.import b
+00000630: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000640: 7068 7973 6963 735f 7269 6769 6462 6f64  physics_rigidbod
+00000650: 795f 636f 6e73 7472 6169 6e74 0a69 6d70  y_constraint.imp
+00000660: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000670: 7469 6573 5f64 6174 615f 6770 656e 6369  ties_data_gpenci
+00000680: 6c0a 696d 706f 7274 2062 6c5f 7569 2e70  l.import bl_ui.p
+00000690: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+000006a0: 735f 6479 6e61 6d69 6370 6169 6e74 0a69  s_dynamicpaint.i
+000006b0: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+000006c0: 655f 6e6f 6465 0a69 6d70 6f72 7420 626c  e_node.import bl
+000006d0: 5f6f 7065 7261 746f 7273 2e6f 626a 6563  _operators.objec
+000006e0: 740a 696d 706f 7274 2062 6c5f 7569 2e70  t.import bl_ui.p
+000006f0: 726f 7065 7274 6965 735f 6461 7461 5f67  roperties_data_g
+00000700: 7265 6173 655f 7065 6e63 696c 0a69 6d70  rease_pencil.imp
+00000710: 6f72 7420 626c 5f75 692e 6765 6e65 7269  ort bl_ui.generi
+00000720: 635f 7569 5f6c 6973 740a 696d 706f 7274  c_ui_list.import
+00000730: 2062 6c5f 7569 2e6e 6f64 655f 6164 645f   bl_ui.node_add_
+00000740: 6d65 6e75 5f67 656f 6d65 7472 790a 696d  menu_geometry.im
+00000750: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000760: 7274 6965 735f 6461 7461 5f61 726d 6174  rties_data_armat
+00000770: 7572 650a 696d 706f 7274 2062 6c5f 6f70  ure.import bl_op
+00000780: 6572 6174 6f72 732e 7669 6577 3364 0a69  erators.view3d.i
+00000790: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000007a0: 6572 7469 6573 5f64 6174 615f 6c69 6768  erties_data_ligh
+000007b0: 7470 726f 6265 0a69 6d70 6f72 7420 626c  tprobe.import bl
+000007c0: 5f75 692e 7370 6163 655f 7469 6d65 0a69  _ui.space_time.i
+000007d0: 6d70 6f72 7420 626c 5f75 690a 696d 706f  mport bl_ui.impo
+000007e0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000007f0: 6965 735f 636f 6e73 7472 6169 6e74 0a69  ies_constraint.i
+00000800: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000810: 6572 7469 6573 5f70 6172 7469 636c 650a  erties_particle.
+00000820: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000830: 6365 5f69 6d61 6765 0a69 6d70 6f72 7420  ce_image.import 
+00000840: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000850: 5f64 6174 615f 6c61 7474 6963 650a 696d  _data_lattice.im
+00000860: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000870: 7274 6965 735f 6461 7461 5f73 6861 6465  rties_data_shade
+00000880: 7266 780a 696d 706f 7274 2062 6c5f 7569  rfx.import bl_ui
+00000890: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+000008a0: 5f76 6f6c 756d 650a 696d 706f 7274 2062  _volume.import b
+000008b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000008c0: 6461 7461 5f63 7572 7665 0a69 6d70 6f72  data_curve.impor
+000008d0: 7420 626c 5f75 692e 7370 6163 655f 646f  t bl_ui.space_do
+000008e0: 7065 7368 6565 740a 696d 706f 7274 2062  pesheet.import b
+000008f0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000900: 7068 7973 6963 735f 636f 6d6d 6f6e 0a69  physics_common.i
+00000910: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000920: 655f 7370 7265 6164 7368 6565 740a 696d  e_spreadsheet.im
+00000930: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000940: 5f74 6f70 6261 720a 696d 706f 7274 2062  _topbar.import b
+00000950: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
+00000960: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+00000970: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000980: 615f 656d 7074 790a 696d 706f 7274 2062  a_empty.import b
+00000990: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000009a0: 7068 7973 6963 735f 666c 7569 640a 696d  physics_fluid.im
+000009b0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+000009c0: 5f74 6578 740a 696d 706f 7274 2062 6c5f  _text.import bl_
+000009d0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+000009e0: 746f 6f6c 6261 720a 696d 706f 7274 2062  toolbar.import b
+000009f0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000a00: 6d61 736b 5f63 6f6d 6d6f 6e0a 696d 706f  mask_common.impo
+00000a10: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000a20: 6965 735f 6461 7461 5f63 7572 7665 730a  ies_data_curves.
+00000a30: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000a40: 7065 7274 6965 735f 6461 7461 5f73 7065  perties_data_spe
+00000a50: 616b 6572 0a69 6d70 6f72 7420 626c 5f75  aker.import bl_u
+00000a60: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+00000a70: 775f 6c61 7965 720a 696d 706f 7274 2062  w_layer.import b
+00000a80: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00000a90: 6461 7461 5f70 6f69 6e74 636c 6f75 640a  data_pointcloud.
+00000aa0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000ab0: 6365 5f74 6f6f 6c73 7973 7465 6d5f 636f  ce_toolsystem_co
+00000ac0: 6d6d 6f6e 0a0a 4765 6e65 7269 6354 7970  mmon..GenericTyp
 00000ad0: 6520 3d20 7479 7069 6e67 2e54 7970 6556  e = typing.TypeV
 00000ae0: 6172 2822 4765 6e65 7269 6354 7970 6522  ar("GenericType"
 00000af0: 290a 0a0a 636c 6173 7320 6270 795f 7072  )...class bpy_pr
 00000b00: 6f70 5f63 6f6c 6c65 6374 696f 6e28 7479  op_collection(ty
 00000b10: 7069 6e67 2e47 656e 6572 6963 5b47 656e  ping.Generic[Gen
 00000b20: 6572 6963 5479 7065 5d29 3a0a 2020 2020  ericType]):.    
 00000b30: 2727 2720 6275 696c 742d 696e 2063 6c61  ''' built-in cla
@@ -23296,16 +23296,16 @@
 0005aff0: 2027 4576 656e 7427 2c0a 2020 2020 2020   'Event',.      
 0005b000: 2020 2020 2020 2020 7477 6561 6b3a 2074          tweak: t
 0005b010: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
 0005b020: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
 0005b030: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0005b040: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
 0005b050: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0005b060: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-0005b070: 7970 696e 672e 5365 745b 696e 745d 5d3a  yping.Set[int]]:
+0005b060: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+0005b070: 7970 696e 672e 5365 745b 7374 725d 5d3a  yping.Set[str]]:
 0005b080: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
 0005b090: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
 0005b0a0: 6e74 6578 743a 200a 2020 2020 2020 2020  ntext: .        
 0005b0b0: 3a74 7970 6520 636f 6e74 6578 743a 2027  :type context: '
 0005b0c0: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
 0005b0d0: 203a 7061 7261 6d20 6576 656e 743a 200a   :param event: .
 0005b0e0: 2020 2020 2020 2020 3a74 7970 6520 6576          :type ev
@@ -23314,42 +23314,42 @@
 0005b110: 6b3a 2054 7765 616b 0a20 2020 2020 2020  k: Tweak.       
 0005b120: 203a 7479 7065 2074 7765 616b 3a20 7479   :type tweak: ty
 0005b130: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
 0005b140: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
 0005b150: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
 0005b160: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 0005b170: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0005b180: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-0005b190: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
+0005b180: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+0005b190: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
 0005b1a0: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 0005b1b0: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 0005b1c0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 0005b1d0: 2020 6465 6620 7365 7475 7028 7365 6c66    def setup(self
 0005b1e0: 293a 0a20 2020 2020 2020 2027 2727 200a  ):.        ''' .
 0005b1f0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 0005b200: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
 0005b210: 6566 2069 6e76 6f6b 6528 7365 6c66 2c20  ef invoke(self, 
 0005b220: 636f 6e74 6578 743a 2027 436f 6e74 6578  context: 'Contex
 0005b230: 7427 2c20 6576 656e 743a 2027 4576 656e  t', event: 'Even
 0005b240: 7427 0a20 2020 2020 2020 2020 2020 2020  t'.             
 0005b250: 2020 2920 2d3e 2074 7970 696e 672e 556e    ) -> typing.Un
-0005b260: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-0005b270: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-0005b280: 696e 745d 5d3a 0a20 2020 2020 2020 2027  int]]:.        '
+0005b260: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+0005b270: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+0005b280: 7374 725d 5d3a 0a20 2020 2020 2020 2027  str]]:.        '
 0005b290: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
 0005b2a0: 7261 6d20 636f 6e74 6578 743a 200a 2020  ram context: .  
 0005b2b0: 2020 2020 2020 3a74 7970 6520 636f 6e74        :type cont
 0005b2c0: 6578 743a 2027 436f 6e74 6578 7427 0a20  ext: 'Context'. 
 0005b2d0: 2020 2020 2020 203a 7061 7261 6d20 6576         :param ev
 0005b2e0: 656e 743a 200a 2020 2020 2020 2020 3a74  ent: .        :t
 0005b2f0: 7970 6520 6576 656e 743a 2027 4576 656e  ype event: 'Even
 0005b300: 7427 0a20 2020 2020 2020 203a 7274 7970  t'.        :rtyp
 0005b310: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0005b320: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-0005b330: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+0005b320: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+0005b330: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 0005b340: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
 0005b350: 6e3a 2072 6573 756c 740a 2020 2020 2020  n: result.      
 0005b360: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 0005b370: 7373 0a0a 2020 2020 6465 6620 6578 6974  ss..    def exit
 0005b380: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
 0005b390: 2743 6f6e 7465 7874 272c 2063 616e 6365  'Context', cance
 0005b3a0: 6c3a 2074 7970 696e 672e 4f70 7469 6f6e  l: typing.Option
@@ -27567,24 +27567,24 @@
 0006bae0: 696e 672e 416e 795d 203d 204e 6f6e 650a  ing.Any] = None.
 0006baf0: 2020 2020 2727 2720 0a0a 2020 2020 3a74      ''' ..    :t
 0006bb00: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
 0006bb10: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0006bb20: 795d 0a20 2020 2027 2727 0a0a 2020 2020  y].    '''..    
 0006bb30: 626c 5f6f 7074 696f 6e73 3a20 7479 7069  bl_options: typi
 0006bb40: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-0006bb50: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
-0006bb60: 2e53 6574 5b69 6e74 5d5d 203d 204e 6f6e  .Set[int]] = Non
+0006bb50: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
+0006bb60: 2e53 6574 5b73 7472 5d5d 203d 204e 6f6e  .Set[str]] = Non
 0006bb70: 650a 2020 2020 2727 2720 4b65 7969 6e67  e.    ''' Keying
 0006bb80: 2053 6574 206f 7074 696f 6e73 2074 6f20   Set options to 
 0006bb90: 7573 6520 7768 656e 2069 6e73 6572 7469  use when inserti
 0006bba0: 6e67 206b 6579 6672 616d 6573 0a0a 2020  ng keyframes..  
 0006bbb0: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 0006bbc0: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-0006bbd0: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
-0006bbe0: 745b 696e 745d 5d0a 2020 2020 2727 270a  t[int]].    '''.
+0006bbd0: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
+0006bbe0: 745b 7374 725d 5d0a 2020 2020 2727 270a  t[str]].    '''.
 0006bbf0: 0a20 2020 2064 6566 2070 6f6c 6c28 7365  .    def poll(se
 0006bc00: 6c66 2c20 636f 6e74 6578 743a 2074 7970  lf, context: typ
 0006bc10: 696e 672e 4f70 7469 6f6e 616c 5b27 436f  ing.Optional['Co
 0006bc20: 6e74 6578 7427 5d29 3a0a 2020 2020 2020  ntext']):.      
 0006bc30: 2020 2727 2720 5465 7374 2069 6620 4b65    ''' Test if Ke
 0006bc40: 7969 6e67 2053 6574 2063 616e 2062 6520  ying Set can be 
 0006bc50: 7573 6564 206f 7220 6e6f 740a 0a20 2020  used or not..   
@@ -28327,23 +28327,23 @@
 0006ea60: 5b73 7472 2c20 7479 7069 6e67 2e41 6e79  [str, typing.Any
 0006ea70: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 0006ea80: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 0006ea90: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 0006eaa0: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 0006eab0: 2727 270a 0a20 2020 2062 6c5f 6f70 7469  '''..    bl_opti
 0006eac0: 6f6e 733a 2074 7970 696e 672e 556e 696f  ons: typing.Unio
-0006ead0: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
-0006eae0: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
-0006eaf0: 745d 5d20 3d20 4e6f 6e65 0a20 2020 2027  t]] = None.    '
+0006ead0: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
+0006eae0: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
+0006eaf0: 725d 5d20 3d20 4e6f 6e65 0a20 2020 2027  r]] = None.    '
 0006eb00: 2727 204f 7074 696f 6e73 2066 6f72 2074  '' Options for t
 0006eb10: 6869 7320 6f70 6572 6174 6f72 2074 7970  his operator typ
 0006eb20: 650a 0a20 2020 203a 7479 7065 3a20 7479  e..    :type: ty
 0006eb30: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0006eb40: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-0006eb50: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+0006eb40: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+0006eb50: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 0006eb60: 2027 2727 0a0a 2020 2020 626c 5f74 7261   '''..    bl_tra
 0006eb70: 6e73 6c61 7469 6f6e 5f63 6f6e 7465 7874  nslation_context
 0006eb80: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b73  : typing.Union[s
 0006eb90: 7472 2c20 7479 7069 6e67 2e41 6e79 5d20  tr, typing.Any] 
 0006eba0: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 0006ebb0: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 0006ebc0: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
@@ -28378,27 +28378,27 @@
 0006ed90: 6572 6174 6f72 5072 6f70 6572 7469 6573  eratorProperties
 0006eda0: 2720 3d20 4e6f 6e65 0a20 2020 2027 2727  ' = None.    '''
 0006edb0: 200a 0a20 2020 203a 7479 7065 3a20 274f   ..    :type: 'O
 0006edc0: 7065 7261 746f 7250 726f 7065 7274 6965  peratorPropertie
 0006edd0: 7327 0a20 2020 2027 2727 0a0a 2020 2020  s'.    '''..    
 0006ede0: 6465 6620 7265 706f 7274 2873 656c 662c  def report(self,
 0006edf0: 2074 7970 653a 2074 7970 696e 672e 556e   type: typing.Un
-0006ee00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-0006ee10: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-0006ee20: 696e 745d 5d2c 0a20 2020 2020 2020 2020  int]],.         
+0006ee00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+0006ee10: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+0006ee20: 7374 725d 5d2c 0a20 2020 2020 2020 2020  str]],.         
 0006ee30: 2020 2020 2020 6d65 7373 6167 653a 2074        message: t
 0006ee40: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 0006ee50: 2074 7970 696e 672e 416e 795d 293a 0a20   typing.Any]):. 
 0006ee60: 2020 2020 2020 2027 2727 2072 6570 6f72         ''' repor
 0006ee70: 740a 0a20 2020 2020 2020 203a 7061 7261  t..        :para
 0006ee80: 6d20 7479 7065 3a20 5479 7065 0a20 2020  m type: Type.   
 0006ee90: 2020 2020 203a 7479 7065 2074 7970 653a       :type type:
 0006eea0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0006eeb0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-0006eec0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
+0006eeb0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+0006eec0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
 0006eed0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
 0006eee0: 6573 7361 6765 3a20 5265 706f 7274 204d  essage: Report M
 0006eef0: 6573 7361 6765 0a20 2020 2020 2020 203a  essage.        :
 0006ef00: 7479 7065 206d 6573 7361 6765 3a20 7479  type message: ty
 0006ef10: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 0006ef20: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 0006ef30: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
@@ -36383,22 +36383,22 @@
 0008e1e0: 416e 795d 203d 204e 6f6e 650a 2020 2020  Any] = None.    
 0008e1f0: 2727 2720 0a0a 2020 2020 3a74 7970 653a  ''' ..    :type:
 0008e200: 2074 7970 696e 672e 556e 696f 6e5b 7374   typing.Union[st
 0008e210: 722c 2074 7970 696e 672e 416e 795d 0a20  r, typing.Any]. 
 0008e220: 2020 2027 2727 0a0a 2020 2020 626c 5f6f     '''..    bl_o
 0008e230: 7074 696f 6e73 3a20 7479 7069 6e67 2e55  ptions: typing.U
 0008e240: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0008e250: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-0008e260: 5b69 6e74 5d5d 203d 204e 6f6e 650a 2020  [int]] = None.  
+0008e250: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+0008e260: 5b73 7472 5d5d 203d 204e 6f6e 650a 2020  [str]] = None.  
 0008e270: 2020 2727 2720 4f70 7469 6f6e 7320 666f    ''' Options fo
 0008e280: 7220 7468 6973 206f 7065 7261 746f 7220  r this operator 
 0008e290: 7479 7065 0a0a 2020 2020 3a74 7970 653a  type..    :type:
 0008e2a0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0008e2b0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
-0008e2c0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
+0008e2b0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
+0008e2c0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
 0008e2d0: 2020 2020 2727 270a 0a20 2020 2062 6c5f      '''..    bl_
 0008e2e0: 7472 616e 736c 6174 696f 6e5f 636f 6e74  translation_cont
 0008e2f0: 6578 743a 2074 7970 696e 672e 556e 696f  ext: typing.Unio
 0008e300: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0008e310: 795d 203d 204e 6f6e 650a 2020 2020 2727  y] = None.    ''
 0008e320: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 0008e330: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
@@ -36465,27 +36465,27 @@
 0008e700: 6f70 6572 7479 2077 6865 6e20 6578 7061  operty when expa
 0008e710: 6e64 696e 6720 616e 206f 7065 7261 746f  nding an operato
 0008e720: 7220 696e 746f 2061 206d 656e 752e 0a0a  r into a menu...
 0008e730: 2020 2020 3a74 7970 653a 2073 7472 0a20      :type: str. 
 0008e740: 2020 2027 2727 0a0a 2020 2020 6465 6620     '''..    def 
 0008e750: 7265 706f 7274 2873 656c 662c 2074 7970  report(self, typ
 0008e760: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0008e770: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
-0008e780: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
+0008e770: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
+0008e780: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
 0008e790: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 0008e7a0: 2020 6d65 7373 6167 653a 2074 7970 696e    message: typin
 0008e7b0: 672e 556e 696f 6e5b 7374 722c 2074 7970  g.Union[str, typ
 0008e7c0: 696e 672e 416e 795d 293a 0a20 2020 2020  ing.Any]):.     
 0008e7d0: 2020 2027 2727 2072 6570 6f72 740a 0a20     ''' report.. 
 0008e7e0: 2020 2020 2020 203a 7061 7261 6d20 7479         :param ty
 0008e7f0: 7065 3a20 5479 7065 0a20 2020 2020 2020  pe: Type.       
 0008e800: 203a 7479 7065 2074 7970 653a 2074 7970   :type type: typ
 0008e810: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0008e820: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-0008e830: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
+0008e820: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+0008e830: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
 0008e840: 2020 2020 3a70 6172 616d 206d 6573 7361      :param messa
 0008e850: 6765 3a20 5265 706f 7274 204d 6573 7361  ge: Report Messa
 0008e860: 6765 0a20 2020 2020 2020 203a 7479 7065  ge.        :type
 0008e870: 206d 6573 7361 6765 3a20 7479 7069 6e67   message: typing
 0008e880: 2e55 6e69 6f6e 5b73 7472 2c20 7479 7069  .Union[str, typi
 0008e890: 6e67 2e41 6e79 5d0a 2020 2020 2020 2020  ng.Any].        
 0008e8a0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
@@ -36510,26 +36510,26 @@
 0008e9d0: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0008e9e0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 0008e9f0: 7373 0a0a 2020 2020 6465 6620 6578 6563  ss..    def exec
 0008ea00: 7574 6528 7365 6c66 2c20 636f 6e74 6578  ute(self, contex
 0008ea10: 743a 2027 436f 6e74 6578 7427 0a20 2020  t: 'Context'.   
 0008ea20: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 0008ea30: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-0008ea40: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-0008ea50: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+0008ea40: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+0008ea50: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 0008ea60: 3a0a 2020 2020 2020 2020 2727 2720 4578  :.        ''' Ex
 0008ea70: 6563 7574 6520 7468 6520 6f70 6572 6174  ecute the operat
 0008ea80: 6f72 0a0a 2020 2020 2020 2020 3a70 6172  or..        :par
 0008ea90: 616d 2063 6f6e 7465 7874 3a20 0a20 2020  am context: .   
 0008eaa0: 2020 2020 203a 7479 7065 2063 6f6e 7465       :type conte
 0008eab0: 7874 3a20 2743 6f6e 7465 7874 270a 2020  xt: 'Context'.  
 0008eac0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 0008ead0: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0008eae0: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-0008eaf0: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
+0008eae0: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+0008eaf0: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
 0008eb00: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 0008eb10: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 0008eb20: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 0008eb30: 2020 2064 6566 2063 6865 636b 2873 656c     def check(sel
 0008eb40: 662c 2063 6f6e 7465 7874 3a20 2743 6f6e  f, context: 'Con
 0008eb50: 7465 7874 2729 202d 3e20 626f 6f6c 3a0a  text') -> bool:.
 0008eb60: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
@@ -36547,53 +36547,53 @@
 0008ec20: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 0008ec30: 7373 0a0a 2020 2020 6465 6620 696e 766f  ss..    def invo
 0008ec40: 6b65 2873 656c 662c 2063 6f6e 7465 7874  ke(self, context
 0008ec50: 3a20 2743 6f6e 7465 7874 272c 2065 7665  : 'Context', eve
 0008ec60: 6e74 3a20 2745 7665 6e74 270a 2020 2020  nt: 'Event'.    
 0008ec70: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
 0008ec80: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-0008ec90: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
-0008eca0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 3a0a  ping.Set[int]]:.
+0008ec90: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
+0008eca0: 7069 6e67 2e53 6574 5b73 7472 5d5d 3a0a  ping.Set[str]]:.
 0008ecb0: 2020 2020 2020 2020 2727 2720 496e 766f          ''' Invo
 0008ecc0: 6b65 2074 6865 206f 7065 7261 746f 720a  ke the operator.
 0008ecd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
 0008ece0: 636f 6e74 6578 743a 200a 2020 2020 2020  context: .      
 0008ecf0: 2020 3a74 7970 6520 636f 6e74 6578 743a    :type context:
 0008ed00: 2027 436f 6e74 6578 7427 0a20 2020 2020   'Context'.     
 0008ed10: 2020 203a 7061 7261 6d20 6576 656e 743a     :param event:
 0008ed20: 200a 2020 2020 2020 2020 3a74 7970 6520   .        :type 
 0008ed30: 6576 656e 743a 2027 4576 656e 7427 0a20  event: 'Event'. 
 0008ed40: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
 0008ed50: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0008ed60: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-0008ed70: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
+0008ed60: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+0008ed70: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
 0008ed80: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
 0008ed90: 6573 756c 740a 2020 2020 2020 2020 2727  esult.        ''
 0008eda0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
 0008edb0: 2020 2020 6465 6620 6d6f 6461 6c28 7365      def modal(se
 0008edc0: 6c66 2c20 636f 6e74 6578 743a 2027 436f  lf, context: 'Co
 0008edd0: 6e74 6578 7427 2c20 6576 656e 743a 2027  ntext', event: '
 0008ede0: 4576 656e 7427 0a20 2020 2020 2020 2020  Event'.         
 0008edf0: 2020 2020 2029 202d 3e20 7479 7069 6e67       ) -> typing
 0008ee00: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-0008ee10: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-0008ee20: 6574 5b69 6e74 5d5d 3a0a 2020 2020 2020  et[int]]:.      
+0008ee10: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+0008ee20: 6574 5b73 7472 5d5d 3a0a 2020 2020 2020  et[str]]:.      
 0008ee30: 2020 2727 2720 4d6f 6461 6c20 6f70 6572    ''' Modal oper
 0008ee40: 6174 6f72 2066 756e 6374 696f 6e0a 0a20  ator function.. 
 0008ee50: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
 0008ee60: 6e74 6578 743a 200a 2020 2020 2020 2020  ntext: .        
 0008ee70: 3a74 7970 6520 636f 6e74 6578 743a 2027  :type context: '
 0008ee80: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
 0008ee90: 203a 7061 7261 6d20 6576 656e 743a 200a   :param event: .
 0008eea0: 2020 2020 2020 2020 3a74 7970 6520 6576          :type ev
 0008eeb0: 656e 743a 2027 4576 656e 7427 0a20 2020  ent: 'Event'.   
 0008eec0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 0008eed0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-0008eee0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
-0008eef0: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
+0008eee0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
+0008eef0: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
 0008ef00: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 0008ef10: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 0008ef20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 0008ef30: 2020 6465 6620 6472 6177 2873 656c 662c    def draw(self,
 0008ef40: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0008ef50: 7874 2729 3a0a 2020 2020 2020 2020 2727  xt'):.        ''
 0008ef60: 2720 4472 6177 2066 756e 6374 696f 6e20  ' Draw function 
@@ -46460,28 +46460,28 @@
 000b57b0: 7279 5f70 6561 6b3a 2074 7970 696e 672e  ry_peak: typing.
 000b57c0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
 000b57d0: 416e 795d 0a20 2020 2020 2020 2027 2727  Any].        '''
 000b57e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 000b57f0: 2020 2064 6566 2072 6570 6f72 7428 7365     def report(se
 000b5800: 6c66 2c20 7479 7065 3a20 7479 7069 6e67  lf, type: typing
 000b5810: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-000b5820: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-000b5830: 6574 5b69 6e74 5d5d 2c0a 2020 2020 2020  et[int]],.      
+000b5820: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+000b5830: 6574 5b73 7472 5d5d 2c0a 2020 2020 2020  et[str]],.      
 000b5840: 2020 2020 2020 2020 206d 6573 7361 6765           message
 000b5850: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b73  : typing.Union[s
 000b5860: 7472 2c20 7479 7069 6e67 2e41 6e79 5d29  tr, typing.Any])
 000b5870: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
 000b5880: 706f 7274 2069 6e66 6f2c 2077 6172 6e69  port info, warni
 000b5890: 6e67 206f 7220 6572 726f 7220 6d65 7373  ng or error mess
 000b58a0: 6167 6573 0a0a 2020 2020 2020 2020 3a70  ages..        :p
 000b58b0: 6172 616d 2074 7970 653a 2054 7970 650a  aram type: Type.
 000b58c0: 2020 2020 2020 2020 3a74 7970 6520 7479          :type ty
 000b58d0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-000b58e0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-000b58f0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+000b58e0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+000b58f0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 000b5900: 5d5d 0a20 2020 2020 2020 203a 7061 7261  ]].        :para
 000b5910: 6d20 6d65 7373 6167 653a 2052 6570 6f72  m message: Repor
 000b5920: 7420 4d65 7373 6167 650a 2020 2020 2020  t Message.      
 000b5930: 2020 3a74 7970 6520 6d65 7373 6167 653a    :type message:
 000b5940: 2074 7970 696e 672e 556e 696f 6e5b 7374   typing.Union[st
 000b5950: 722c 2074 7970 696e 672e 416e 795d 0a20  r, typing.Any]. 
 000b5960: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
@@ -66193,23 +66193,23 @@
 00102900: 7920 6f6e 6c79 2066 6163 6573 2077 6974  y only faces wit
 00102910: 6820 7468 6520 6375 7272 656e 746c 7920  h the currently 
 00102920: 6469 7370 6c61 7965 6420 696d 6167 6520  displayed image 
 00102930: 6173 7369 676e 6564 0a0a 2020 2020 3a74  assigned..    :t
 00102940: 7970 653a 2062 6f6f 6c0a 2020 2020 2727  ype: bool.    ''
 00102950: 270a 0a20 2020 2073 6e61 705f 656c 656d  '..    snap_elem
 00102960: 656e 7473 3a20 7479 7069 6e67 2e55 6e69  ents: typing.Uni
-00102970: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-00102980: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-00102990: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
+00102970: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+00102980: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+00102990: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
 001029a0: 2727 2720 5479 7065 206f 6620 656c 656d  ''' Type of elem
 001029b0: 656e 7420 746f 2073 6e61 7020 746f 0a0a  ent to snap to..
 001029c0: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001029d0: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-001029e0: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
-001029f0: 5365 745b 696e 745d 5d0a 2020 2020 2727  Set[int]].    ''
+001029e0: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
+001029f0: 5365 745b 7374 725d 5d0a 2020 2020 2727  Set[str]].    ''
 00102a00: 270a 0a20 2020 2073 6e61 705f 656c 656d  '..    snap_elem
 00102a10: 656e 7473 5f62 6173 653a 2074 7970 696e  ents_base: typin
 00102a20: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
 00102a30: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
 00102a40: 5365 745b 696e 745d 5d20 3d20 4e6f 6e65  Set[int]] = None
 00102a50: 0a20 2020 2027 2727 2054 7970 6520 6f66  .    ''' Type of
 00102a60: 2065 6c65 6d65 6e74 2066 6f72 2074 6865   element for the
@@ -108059,16 +108059,16 @@
 001a61a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a61b0: 2020 2020 2020 2020 2020 6576 656e 743a            event:
 001a61c0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a61d0: 5b27 4576 656e 7427 5d0a 2020 2020 2020  ['Event'].      
 001a61e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a61f0: 2020 2020 2029 202d 3e20 7479 7069 6e67       ) -> typing
 001a6200: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a6210: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
-001a6220: 6574 5b69 6e74 5d5d 3a0a 2020 2020 2020  et[int]]:.      
+001a6210: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
+001a6220: 6574 5b73 7472 5d5d 3a0a 2020 2020 2020  et[str]]:.      
 001a6230: 2020 2727 2720 4f70 6572 6174 6f72 2070    ''' Operator p
 001a6240: 6f70 7570 2069 6e76 6f6b 6520 2873 686f  opup invoke (sho
 001a6250: 7720 6f70 6572 6174 6f72 2070 726f 7065  w operator prope
 001a6260: 7274 6965 7320 616e 6420 6578 6563 7574  rties and execut
 001a6270: 6520 6974 2061 7574 6f6d 6174 6963 616c  e it automatical
 001a6280: 6c79 206f 6e20 6368 616e 6765 7329 0a0a  ly on changes)..
 001a6290: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
@@ -108080,16 +108080,16 @@
 001a62f0: 2020 2020 2020 3a70 6172 616d 2065 7665        :param eve
 001a6300: 6e74 3a20 4576 656e 740a 2020 2020 2020  nt: Event.      
 001a6310: 2020 3a74 7970 6520 6576 656e 743a 2074    :type event: t
 001a6320: 7970 696e 672e 4f70 7469 6f6e 616c 5b27  yping.Optional['
 001a6330: 4576 656e 7427 5d0a 2020 2020 2020 2020  Event'].        
 001a6340: 3a72 7479 7065 3a20 7479 7069 6e67 2e55  :rtype: typing.U
 001a6350: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001a6360: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
-001a6370: 5b69 6e74 5d5d 0a20 2020 2020 2020 203a  [int]].        :
+001a6360: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
+001a6370: 5b73 7472 5d5d 0a20 2020 2020 2020 203a  [str]].        :
 001a6380: 7265 7475 726e 3a20 7265 7375 6c74 0a20  return: result. 
 001a6390: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
 001a63a0: 2020 2070 6173 730a 0a20 2020 2040 636c     pass..    @cl
 001a63b0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
 001a63c0: 6620 696e 766f 6b65 5f70 726f 7073 5f64  f invoke_props_d
 001a63d0: 6961 6c6f 6728 0a20 2020 2020 2020 2020  ialog(.         
 001a63e0: 2020 2063 6c73 2c0a 2020 2020 2020 2020     cls,.        
@@ -108097,16 +108097,16 @@
 001a6400: 7069 6e67 2e4f 7074 696f 6e61 6c5b 274f  ping.Optional['O
 001a6410: 7065 7261 746f 7227 5d2c 0a20 2020 2020  perator'],.     
 001a6420: 2020 2020 2020 2077 6964 7468 3a20 7479         width: ty
 001a6430: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
 001a6440: 7069 6e67 2e41 6e79 5d20 3d20 3330 300a  ping.Any] = 300.
 001a6450: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
 001a6460: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-001a6470: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
-001a6480: 745b 696e 745d 5d3a 0a20 2020 2020 2020  t[int]]:.       
+001a6470: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
+001a6480: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
 001a6490: 2027 2727 204f 7065 7261 746f 7220 6469   ''' Operator di
 001a64a0: 616c 6f67 2028 6e6f 6e2d 6175 746f 6578  alog (non-autoex
 001a64b0: 6563 2070 6f70 7570 2920 696e 766f 6b65  ec popup) invoke
 001a64c0: 2028 7368 6f77 206f 7065 7261 746f 7220   (show operator 
 001a64d0: 7072 6f70 6572 7469 6573 2061 6e64 206f  properties and o
 001a64e0: 6e6c 7920 6578 6563 7574 6520 6974 206f  nly execute it o
 001a64f0: 6e20 636c 6963 6b20 6f6e 204f 4b20 6275  n click on OK bu
@@ -108120,16 +108120,16 @@
 001a6570: 7261 6d20 7769 6474 683a 2057 6964 7468  ram width: Width
 001a6580: 206f 6620 7468 6520 706f 7075 700a 2020   of the popup.  
 001a6590: 2020 2020 2020 3a74 7970 6520 7769 6474        :type widt
 001a65a0: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
 001a65b0: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
 001a65c0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
 001a65d0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-001a65e0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-001a65f0: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
+001a65e0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+001a65f0: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
 001a6600: 2020 2020 2020 3a72 6574 7572 6e3a 2072        :return: r
 001a6610: 6573 756c 740a 2020 2020 2020 2020 2727  esult.        ''
 001a6620: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
 001a6630: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
 001a6640: 0a20 2020 2064 6566 2069 6e76 6f6b 655f  .    def invoke_
 001a6650: 7365 6172 6368 5f70 6f70 7570 2863 6c73  search_popup(cls
 001a6660: 2c20 6f70 6572 6174 6f72 3a20 7479 7069  , operator: typi
@@ -108162,16 +108162,16 @@
 001a6810: 6572 6174 6f72 275d 2c0a 2020 2020 2020  erator'],.      
 001a6820: 2020 2020 2020 2020 2020 2020 2020 2077                 w
 001a6830: 6964 7468 3a20 7479 7069 6e67 2e4f 7074  idth: typing.Opt
 001a6840: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
 001a6850: 5d20 3d20 3330 300a 2020 2020 2020 2020  ] = 300.        
 001a6860: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 001a6870: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-001a6880: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
-001a6890: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
+001a6880: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
+001a6890: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
 001a68a0: 3a0a 2020 2020 2020 2020 2727 2720 4f70  :.        ''' Op
 001a68b0: 6572 6174 6f72 2070 6f70 7570 2069 6e76  erator popup inv
 001a68c0: 6f6b 6520 286f 6e6c 7920 7368 6f77 7320  oke (only shows 
 001a68d0: 6f70 6572 6174 6f72 2773 2070 726f 7065  operator's prope
 001a68e0: 7274 6965 732c 2077 6974 686f 7574 2065  rties, without e
 001a68f0: 7865 6375 7469 6e67 2069 7429 0a0a 2020  xecuting it)..  
 001a6900: 2020 2020 2020 3a70 6172 616d 206f 7065        :param ope
@@ -108183,33 +108183,33 @@
 001a6960: 2020 2020 3a70 6172 616d 2077 6964 7468      :param width
 001a6970: 3a20 5769 6474 6820 6f66 2074 6865 2070  : Width of the p
 001a6980: 6f70 7570 0a20 2020 2020 2020 203a 7479  opup.        :ty
 001a6990: 7065 2077 6964 7468 3a20 7479 7069 6e67  pe width: typing
 001a69a0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
 001a69b0: 2e41 6e79 5d0a 2020 2020 2020 2020 3a72  .Any].        :r
 001a69c0: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
-001a69d0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001a69e0: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001a69f0: 6e74 5d5d 0a20 2020 2020 2020 203a 7265  nt]].        :re
+001a69d0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001a69e0: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001a69f0: 7472 5d5d 0a20 2020 2020 2020 203a 7265  tr]].        :re
 001a6a00: 7475 726e 3a20 7265 7375 6c74 0a20 2020  turn: result.   
 001a6a10: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
 001a6a20: 2070 6173 730a 0a20 2020 2040 636c 6173   pass..    @clas
 001a6a30: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
 001a6a40: 696e 766f 6b65 5f63 6f6e 6669 726d 2863  invoke_confirm(c
 001a6a50: 6c73 2c20 6f70 6572 6174 6f72 3a20 7479  ls, operator: ty
 001a6a60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 274f  ping.Optional['O
 001a6a70: 7065 7261 746f 7227 5d2c 0a20 2020 2020  perator'],.     
 001a6a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a6a90: 2020 6576 656e 743a 2074 7970 696e 672e    event: typing.
 001a6aa0: 4f70 7469 6f6e 616c 5b27 4576 656e 7427  Optional['Event'
 001a6ab0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
 001a6ac0: 2020 2020 2020 2020 2029 202d 3e20 7479           ) -> ty
 001a6ad0: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-001a6ae0: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
-001a6af0: 6e67 2e53 6574 5b69 6e74 5d5d 3a0a 2020  ng.Set[int]]:.  
+001a6ae0: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
+001a6af0: 6e67 2e53 6574 5b73 7472 5d5d 3a0a 2020  ng.Set[str]]:.  
 001a6b00: 2020 2020 2020 2727 2720 4f70 6572 6174        ''' Operat
 001a6b10: 6f72 2063 6f6e 6669 726d 6174 696f 6e20  or confirmation 
 001a6b20: 706f 7075 7020 286f 6e6c 7920 746f 206c  popup (only to l
 001a6b30: 6574 2075 7365 7220 636f 6e66 6972 6d20  et user confirm 
 001a6b40: 7468 6520 6578 6563 7574 696f 6e2c 206e  the execution, n
 001a6b50: 6f20 6f70 6572 6174 6f72 2070 726f 7065  o operator prope
 001a6b60: 7274 6965 7320 7368 6f77 6e29 0a0a 2020  rties shown)..  
@@ -108221,17 +108221,17 @@
 001a6bc0: 274f 7065 7261 746f 7227 5d0a 2020 2020  'Operator'].    
 001a6bd0: 2020 2020 3a70 6172 616d 2065 7665 6e74      :param event
 001a6be0: 3a20 4576 656e 740a 2020 2020 2020 2020  : Event.        
 001a6bf0: 3a74 7970 6520 6576 656e 743a 2074 7970  :type event: typ
 001a6c00: 696e 672e 4f70 7469 6f6e 616c 5b27 4576  ing.Optional['Ev
 001a6c10: 656e 7427 5d0a 2020 2020 2020 2020 3a72  ent'].        :r
 001a6c20: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
-001a6c30: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001a6c40: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001a6c50: 6e74 5d5d 0a20 2020 2020 2020 203a 7265  nt]].        :re
+001a6c30: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001a6c40: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001a6c50: 7472 5d5d 0a20 2020 2020 2020 203a 7265  tr]].        :re
 001a6c60: 7475 726e 3a20 7265 7375 6c74 0a20 2020  turn: result.   
 001a6c70: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
 001a6c80: 2070 6173 730a 0a20 2020 2040 636c 6173   pass..    @clas
 001a6c90: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
 001a6ca0: 706f 706d 656e 755f 6265 6769 6e5f 5f69  popmenu_begin__i
 001a6cb0: 6e74 6572 6e61 6c28 636c 732c 0a20 2020  nternal(cls,.   
 001a6cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
@@ -113566,23 +113566,23 @@
 001bb9d0: 2d20 4469 7373 6f6c 7665 2067 656f 6d65  - Dissolve geome
 001bb9e0: 7472 7920 746f 2066 6f72 6d20 706c 616e  try to form plan
 001bb9f0: 6172 2070 6f6c 7967 6f6e 732e 0a0a 2020  ar polygons...  
 001bba00: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 001bba10: 556e 696f 6e5b 7374 722c 2069 6e74 5d0a  Union[str, int].
 001bba20: 2020 2020 2727 270a 0a20 2020 2064 656c      '''..    del
 001bba30: 696d 6974 3a20 7479 7069 6e67 2e55 6e69  imit: typing.Uni
-001bba40: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
-001bba50: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
-001bba60: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
+001bba40: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
+001bba50: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
+001bba60: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
 001bba70: 2727 2720 4c69 6d69 7420 6d65 7267 696e  ''' Limit mergin
 001bba80: 6720 6765 6f6d 6574 7279 0a0a 2020 2020  g geometry..    
 001bba90: 3a74 7970 653a 2074 7970 696e 672e 556e  :type: typing.Un
-001bbaa0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
-001bbab0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
-001bbac0: 696e 745d 5d0a 2020 2020 2727 270a 0a20  int]].    '''.. 
+001bbaa0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
+001bbab0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
+001bbac0: 7374 725d 5d0a 2020 2020 2727 270a 0a20  str]].    '''.. 
 001bbad0: 2020 2066 6163 655f 636f 756e 743a 2069     face_count: i
 001bbae0: 6e74 203d 204e 6f6e 650a 2020 2020 2727  nt = None.    ''
 001bbaf0: 2720 5468 6520 6375 7272 656e 7420 6e75  ' The current nu
 001bbb00: 6d62 6572 206f 6620 6661 6365 7320 696e  mber of faces in
 001bbb10: 2074 6865 2064 6563 696d 6174 6564 206d   the decimated m
 001bbb20: 6573 680a 0a20 2020 203a 7479 7065 3a20  esh..    :type: 
 001bbb30: 696e 740a 2020 2020 2727 270a 0a20 2020  int.    '''..   
@@ -114850,21 +114850,21 @@
 001c0a10: 7468 2074 6f20 6578 7465 726e 616c 2064  th to external d
 001c0a20: 6973 706c 6163 656d 656e 7473 2066 696c  isplacements fil
 001c0a30: 650a 0a20 2020 203a 7479 7065 3a20 7479  e..    :type: ty
 001c0a40: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 001c0a50: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 001c0a60: 2727 270a 0a20 2020 2066 6c69 705f 6178  '''..    flip_ax
 001c0a70: 6973 3a20 7479 7069 6e67 2e55 6e69 6f6e  is: typing.Union
-001c0a80: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
-001c0a90: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
+001c0a80: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
+001c0a90: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
 001c0aa0: 5d5d 203d 204e 6f6e 650a 2020 2020 2727  ]] = None.    ''
 001c0ab0: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 001c0ac0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-001c0ad0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
-001c0ae0: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
+001c0ad0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
+001c0ae0: 696e 672e 5365 745b 7374 725d 5d0a 2020  ing.Set[str]].  
 001c0af0: 2020 2727 270a 0a20 2020 2066 6f72 7761    '''..    forwa
 001c0b00: 7264 5f61 7869 733a 2074 7970 696e 672e  rd_axis: typing.
 001c0b10: 556e 696f 6e5b 7374 722c 2069 6e74 5d20  Union[str, int] 
 001c0b20: 3d20 4e6f 6e65 0a20 2020 2027 2727 200a  = None.    ''' .
 001c0b30: 0a20 2020 203a 7479 7065 3a20 7479 7069  .    :type: typi
 001c0b40: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 696e  ng.Union[str, in
 001c0b50: 745d 0a20 2020 2027 2727 0a0a 2020 2020  t].    '''..    
@@ -216544,2012 +216544,2023 @@
 0034ddf0: 5649 4557 3344 5f4d 545f 6564 6974 5f6d  VIEW3D_MT_edit_m
 0034de00: 6574 6162 616c 6c5f 636f 6e74 6578 745f  etaball_context_
 0034de10: 6d65 6e75 3a20 2762 6c5f 7569 2e73 7061  menu: 'bl_ui.spa
 0034de20: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
 0034de30: 5f4d 545f 6564 6974 5f6d 6574 6162 616c  _MT_edit_metabal
 0034de40: 6c5f 636f 6e74 6578 745f 6d65 6e75 2720  l_context_menu' 
 0034de50: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034de60: 545f 6564 6974 5f73 7572 6661 6365 3a20  T_edit_surface: 
-0034de70: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034de80: 7733 642e 5649 4557 3344 5f4d 545f 6564  w3d.VIEW3D_MT_ed
-0034de90: 6974 5f73 7572 6661 6365 2720 3d20 4e6f  it_surface' = No
-0034dea0: 6e65 0a0a 5649 4557 3344 5f4d 545f 6564  ne..VIEW3D_MT_ed
-0034deb0: 6974 6f72 5f6d 656e 7573 3a20 2762 6c5f  itor_menus: 'bl_
-0034dec0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034ded0: 5649 4557 3344 5f4d 545f 6564 6974 6f72  VIEW3D_MT_editor
-0034dee0: 5f6d 656e 7573 2720 3d20 4e6f 6e65 0a0a  _menus' = None..
-0034def0: 5649 4557 3344 5f4d 545f 6661 6365 5f73  VIEW3D_MT_face_s
-0034df00: 6574 733a 2027 626c 5f75 692e 7370 6163  ets: 'bl_ui.spac
-0034df10: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034df20: 4d54 5f66 6163 655f 7365 7473 2720 3d20  MT_face_sets' = 
-0034df30: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034df40: 6661 6365 5f73 6574 735f 696e 6974 3a20  face_sets_init: 
-0034df50: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034df60: 7733 642e 5649 4557 3344 5f4d 545f 6661  w3d.VIEW3D_MT_fa
-0034df70: 6365 5f73 6574 735f 696e 6974 2720 3d20  ce_sets_init' = 
-0034df80: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034df90: 6770 656e 6369 6c5f 616e 696d 6174 696f  gpencil_animatio
-0034dfa0: 6e3a 2027 626c 5f75 692e 7370 6163 655f  n: 'bl_ui.space_
-0034dfb0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034dfc0: 5f67 7065 6e63 696c 5f61 6e69 6d61 7469  _gpencil_animati
-0034dfd0: 6f6e 2720 3d20 4e6f 6e65 0a0a 5649 4557  on' = None..VIEW
-0034dfe0: 3344 5f4d 545f 6770 656e 6369 6c5f 6175  3D_MT_gpencil_au
-0034dff0: 746f 7765 6967 6874 733a 2027 626c 5f75  toweights: 'bl_u
-0034e000: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034e010: 4945 5733 445f 4d54 5f67 7065 6e63 696c  IEW3D_MT_gpencil
-0034e020: 5f61 7574 6f77 6569 6768 7473 2720 3d20  _autoweights' = 
-0034e030: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e040: 6770 656e 6369 6c5f 6564 6974 5f63 6f6e  gpencil_edit_con
-0034e050: 7465 7874 5f6d 656e 753a 2027 626c 5f75  text_menu: 'bl_u
-0034e060: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034e070: 4945 5733 445f 4d54 5f67 7065 6e63 696c  IEW3D_MT_gpencil
-0034e080: 5f65 6469 745f 636f 6e74 6578 745f 6d65  _edit_context_me
-0034e090: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
-0034e0a0: 3344 5f4d 545f 6770 656e 6369 6c5f 7369  3D_MT_gpencil_si
-0034e0b0: 6d70 6c69 6679 3a20 2762 6c5f 7569 2e73  mplify: 'bl_ui.s
-0034e0c0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034e0d0: 3344 5f4d 545f 6770 656e 6369 6c5f 7369  3D_MT_gpencil_si
-0034e0e0: 6d70 6c69 6679 2720 3d20 4e6f 6e65 0a0a  mplify' = None..
-0034e0f0: 5649 4557 3344 5f4d 545f 6770 656e 6369  VIEW3D_MT_gpenci
-0034e100: 6c5f 7665 7274 6578 5f67 726f 7570 3a20  l_vertex_group: 
-0034e110: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034e120: 7733 642e 5649 4557 3344 5f4d 545f 6770  w3d.VIEW3D_MT_gp
-0034e130: 656e 6369 6c5f 7665 7274 6578 5f67 726f  encil_vertex_gro
-0034e140: 7570 2720 3d20 4e6f 6e65 0a0a 5649 4557  up' = None..VIEW
-0034e150: 3344 5f4d 545f 6772 6561 7365 5f70 656e  3D_MT_grease_pen
-0034e160: 6369 6c5f 6164 643a 2027 626c 5f75 692e  cil_add: 'bl_ui.
-0034e170: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034e180: 5733 445f 4d54 5f67 7265 6173 655f 7065  W3D_MT_grease_pe
-0034e190: 6e63 696c 5f61 6464 2720 3d20 4e6f 6e65  ncil_add' = None
-0034e1a0: 0a0a 5649 4557 3344 5f4d 545f 686f 6f6b  ..VIEW3D_MT_hook
-0034e1b0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034e1c0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034e1d0: 686f 6f6b 2720 3d20 4e6f 6e65 0a0a 5649  hook' = None..VI
-0034e1e0: 4557 3344 5f4d 545f 696d 6167 655f 6164  EW3D_MT_image_ad
-0034e1f0: 643a 2027 626c 5f75 692e 7370 6163 655f  d: 'bl_ui.space_
-0034e200: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034e210: 5f69 6d61 6765 5f61 6464 2720 3d20 4e6f  _image_add' = No
-0034e220: 6e65 0a0a 5649 4557 3344 5f4d 545f 6c69  ne..VIEW3D_MT_li
-0034e230: 6768 745f 6164 643a 2027 626c 5f75 692e  ght_add: 'bl_ui.
-0034e240: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034e250: 5733 445f 4d54 5f6c 6967 6874 5f61 6464  W3D_MT_light_add
-0034e260: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e270: 5f4d 545f 6c69 6768 7470 726f 6265 5f61  _MT_lightprobe_a
-0034e280: 6464 3a20 2762 6c5f 7569 2e73 7061 6365  dd: 'bl_ui.space
-0034e290: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e2a0: 545f 6c69 6768 7470 726f 6265 5f61 6464  T_lightprobe_add
-0034e2b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e2c0: 5f4d 545f 6d61 6b65 5f6c 696e 6b73 3a20  _MT_make_links: 
-0034e2d0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034e2e0: 7733 642e 5649 4557 3344 5f4d 545f 6d61  w3d.VIEW3D_MT_ma
-0034e2f0: 6b65 5f6c 696e 6b73 2720 3d20 4e6f 6e65  ke_links' = None
-0034e300: 0a0a 5649 4557 3344 5f4d 545f 6d61 6b65  ..VIEW3D_MT_make
-0034e310: 5f73 696e 676c 655f 7573 6572 3a20 2762  _single_user: 'b
-0034e320: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e330: 642e 5649 4557 3344 5f4d 545f 6d61 6b65  d.VIEW3D_MT_make
-0034e340: 5f73 696e 676c 655f 7573 6572 2720 3d20  _single_user' = 
-0034e350: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e360: 6d61 736b 3a20 2762 6c5f 7569 2e73 7061  mask: 'bl_ui.spa
-0034e370: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034e380: 5f4d 545f 6d61 736b 2720 3d20 4e6f 6e65  _MT_mask' = None
-0034e390: 0a0a 5649 4557 3344 5f4d 545f 6d65 7368  ..VIEW3D_MT_mesh
-0034e3a0: 5f61 6464 3a20 2762 6c5f 7569 2e73 7061  _add: 'bl_ui.spa
-0034e3b0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034e3c0: 5f4d 545f 6d65 7368 5f61 6464 2720 3d20  _MT_mesh_add' = 
-0034e3d0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e3e0: 6d65 7461 6261 6c6c 5f61 6464 3a20 2762  metaball_add: 'b
-0034e3f0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e400: 642e 5649 4557 3344 5f4d 545f 6d65 7461  d.VIEW3D_MT_meta
-0034e410: 6261 6c6c 5f61 6464 2720 3d20 4e6f 6e65  ball_add' = None
-0034e420: 0a0a 5649 4557 3344 5f4d 545f 6d69 7272  ..VIEW3D_MT_mirr
-0034e430: 6f72 3a20 2762 6c5f 7569 2e73 7061 6365  or: 'bl_ui.space
-0034e440: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e450: 545f 6d69 7272 6f72 2720 3d20 4e6f 6e65  T_mirror' = None
-0034e460: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034e470: 6374 3a20 2762 6c5f 7569 2e73 7061 6365  ct: 'bl_ui.space
-0034e480: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034e490: 545f 6f62 6a65 6374 2720 3d20 4e6f 6e65  T_object' = None
-0034e4a0: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034e4b0: 6374 5f61 6e69 6d61 7469 6f6e 3a20 2762  ct_animation: 'b
-0034e4c0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e4d0: 642e 5649 4557 3344 5f4d 545f 6f62 6a65  d.VIEW3D_MT_obje
-0034e4e0: 6374 5f61 6e69 6d61 7469 6f6e 2720 3d20  ct_animation' = 
-0034e4f0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e500: 6f62 6a65 6374 5f61 7070 6c79 3a20 2762  object_apply: 'b
-0034e510: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e520: 642e 5649 4557 3344 5f4d 545f 6f62 6a65  d.VIEW3D_MT_obje
-0034e530: 6374 5f61 7070 6c79 2720 3d20 4e6f 6e65  ct_apply' = None
-0034e540: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034e550: 6374 5f61 7373 6574 3a20 2762 6c5f 7569  ct_asset: 'bl_ui
-0034e560: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034e570: 4557 3344 5f4d 545f 6f62 6a65 6374 5f61  EW3D_MT_object_a
-0034e580: 7373 6574 2720 3d20 4e6f 6e65 0a0a 5649  sset' = None..VI
-0034e590: 4557 3344 5f4d 545f 6f62 6a65 6374 5f63  EW3D_MT_object_c
-0034e5a0: 6c65 616e 7570 3a20 2762 6c5f 7569 2e73  leanup: 'bl_ui.s
-0034e5b0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034e5c0: 3344 5f4d 545f 6f62 6a65 6374 5f63 6c65  3D_MT_object_cle
-0034e5d0: 616e 7570 2720 3d20 4e6f 6e65 0a0a 5649  anup' = None..VI
-0034e5e0: 4557 3344 5f4d 545f 6f62 6a65 6374 5f63  EW3D_MT_object_c
-0034e5f0: 6c65 6172 3a20 2762 6c5f 7569 2e73 7061  lear: 'bl_ui.spa
-0034e600: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034e610: 5f4d 545f 6f62 6a65 6374 5f63 6c65 6172  _MT_object_clear
-0034e620: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e630: 5f4d 545f 6f62 6a65 6374 5f63 6f6c 6c65  _MT_object_colle
-0034e640: 6374 696f 6e3a 2027 626c 5f75 692e 7370  ction: 'bl_ui.sp
-0034e650: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034e660: 445f 4d54 5f6f 626a 6563 745f 636f 6c6c  D_MT_object_coll
-0034e670: 6563 7469 6f6e 2720 3d20 4e6f 6e65 0a0a  ection' = None..
-0034e680: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
-0034e690: 5f63 6f6e 7374 7261 696e 7473 3a20 2762  _constraints: 'b
-0034e6a0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034e6b0: 642e 5649 4557 3344 5f4d 545f 6f62 6a65  d.VIEW3D_MT_obje
-0034e6c0: 6374 5f63 6f6e 7374 7261 696e 7473 2720  ct_constraints' 
-0034e6d0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034e6e0: 545f 6f62 6a65 6374 5f63 6f6e 7465 7874  T_object_context
-0034e6f0: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
-0034e700: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034e710: 445f 4d54 5f6f 626a 6563 745f 636f 6e74  D_MT_object_cont
-0034e720: 6578 745f 6d65 6e75 2720 3d20 4e6f 6e65  ext_menu' = None
-0034e730: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034e740: 6374 5f63 6f6e 7665 7274 3a20 2762 6c5f  ct_convert: 'bl_
-0034e750: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034e760: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
-0034e770: 5f63 6f6e 7665 7274 2720 3d20 4e6f 6e65  _convert' = None
-0034e780: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034e790: 6374 5f6c 6962 6f76 6572 7269 6465 3a20  ct_liboverride: 
-0034e7a0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034e7b0: 7733 642e 5649 4557 3344 5f4d 545f 6f62  w3d.VIEW3D_MT_ob
-0034e7c0: 6a65 6374 5f6c 6962 6f76 6572 7269 6465  ject_liboverride
-0034e7d0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e7e0: 5f4d 545f 6f62 6a65 6374 5f6d 6f64 655f  _MT_object_mode_
-0034e7f0: 7069 653a 2027 626c 5f75 692e 7370 6163  pie: 'bl_ui.spac
-0034e800: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034e810: 4d54 5f6f 626a 6563 745f 6d6f 6465 5f70  MT_object_mode_p
-0034e820: 6965 2720 3d20 4e6f 6e65 0a0a 5649 4557  ie' = None..VIEW
-0034e830: 3344 5f4d 545f 6f62 6a65 6374 5f70 6172  3D_MT_object_par
-0034e840: 656e 743a 2027 626c 5f75 692e 7370 6163  ent: 'bl_ui.spac
-0034e850: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034e860: 4d54 5f6f 626a 6563 745f 7061 7265 6e74  MT_object_parent
-0034e870: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e880: 5f4d 545f 6f62 6a65 6374 5f71 7569 636b  _MT_object_quick
-0034e890: 5f65 6666 6563 7473 3a20 2762 6c5f 7569  _effects: 'bl_ui
-0034e8a0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034e8b0: 4557 3344 5f4d 545f 6f62 6a65 6374 5f71  EW3D_MT_object_q
-0034e8c0: 7569 636b 5f65 6666 6563 7473 2720 3d20  uick_effects' = 
-0034e8d0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034e8e0: 6f62 6a65 6374 5f72 656c 6174 696f 6e73  object_relations
-0034e8f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034e900: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034e910: 6f62 6a65 6374 5f72 656c 6174 696f 6e73  object_relations
-0034e920: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034e930: 5f4d 545f 6f62 6a65 6374 5f72 6967 6964  _MT_object_rigid
-0034e940: 5f62 6f64 793a 2027 626c 5f75 692e 7370  _body: 'bl_ui.sp
-0034e950: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034e960: 445f 4d54 5f6f 626a 6563 745f 7269 6769  D_MT_object_rigi
-0034e970: 645f 626f 6479 2720 3d20 4e6f 6e65 0a0a  d_body' = None..
-0034e980: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
-0034e990: 5f73 6861 6469 6e67 3a20 2762 6c5f 7569  _shading: 'bl_ui
-0034e9a0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034e9b0: 4557 3344 5f4d 545f 6f62 6a65 6374 5f73  EW3D_MT_object_s
-0034e9c0: 6861 6469 6e67 2720 3d20 4e6f 6e65 0a0a  hading' = None..
-0034e9d0: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
-0034e9e0: 5f73 686f 7768 6964 653a 2027 626c 5f75  _showhide: 'bl_u
-0034e9f0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ea00: 4945 5733 445f 4d54 5f6f 626a 6563 745f  IEW3D_MT_object_
-0034ea10: 7368 6f77 6869 6465 2720 3d20 4e6f 6e65  showhide' = None
+0034de60: 545f 6564 6974 5f70 6f69 6e74 636c 6f75  T_edit_pointclou
+0034de70: 643a 2027 626c 5f75 692e 7370 6163 655f  d: 'bl_ui.space_
+0034de80: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034de90: 5f65 6469 745f 706f 696e 7463 6c6f 7564  _edit_pointcloud
+0034dea0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034deb0: 5f4d 545f 6564 6974 5f73 7572 6661 6365  _MT_edit_surface
+0034dec0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034ded0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034dee0: 6564 6974 5f73 7572 6661 6365 2720 3d20  edit_surface' = 
+0034def0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034df00: 6564 6974 6f72 5f6d 656e 7573 3a20 2762  editor_menus: 'b
+0034df10: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034df20: 642e 5649 4557 3344 5f4d 545f 6564 6974  d.VIEW3D_MT_edit
+0034df30: 6f72 5f6d 656e 7573 2720 3d20 4e6f 6e65  or_menus' = None
+0034df40: 0a0a 5649 4557 3344 5f4d 545f 6661 6365  ..VIEW3D_MT_face
+0034df50: 5f73 6574 733a 2027 626c 5f75 692e 7370  _sets: 'bl_ui.sp
+0034df60: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034df70: 445f 4d54 5f66 6163 655f 7365 7473 2720  D_MT_face_sets' 
+0034df80: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034df90: 545f 6661 6365 5f73 6574 735f 696e 6974  T_face_sets_init
+0034dfa0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034dfb0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034dfc0: 6661 6365 5f73 6574 735f 696e 6974 2720  face_sets_init' 
+0034dfd0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034dfe0: 545f 6770 656e 6369 6c5f 616e 696d 6174  T_gpencil_animat
+0034dff0: 696f 6e3a 2027 626c 5f75 692e 7370 6163  ion: 'bl_ui.spac
+0034e000: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034e010: 4d54 5f67 7065 6e63 696c 5f61 6e69 6d61  MT_gpencil_anima
+0034e020: 7469 6f6e 2720 3d20 4e6f 6e65 0a0a 5649  tion' = None..VI
+0034e030: 4557 3344 5f4d 545f 6770 656e 6369 6c5f  EW3D_MT_gpencil_
+0034e040: 6175 746f 7765 6967 6874 733a 2027 626c  autoweights: 'bl
+0034e050: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034e060: 2e56 4945 5733 445f 4d54 5f67 7065 6e63  .VIEW3D_MT_gpenc
+0034e070: 696c 5f61 7574 6f77 6569 6768 7473 2720  il_autoweights' 
+0034e080: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e090: 545f 6770 656e 6369 6c5f 6564 6974 5f63  T_gpencil_edit_c
+0034e0a0: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
+0034e0b0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034e0c0: 2e56 4945 5733 445f 4d54 5f67 7065 6e63  .VIEW3D_MT_gpenc
+0034e0d0: 696c 5f65 6469 745f 636f 6e74 6578 745f  il_edit_context_
+0034e0e0: 6d65 6e75 2720 3d20 4e6f 6e65 0a0a 5649  menu' = None..VI
+0034e0f0: 4557 3344 5f4d 545f 6770 656e 6369 6c5f  EW3D_MT_gpencil_
+0034e100: 7369 6d70 6c69 6679 3a20 2762 6c5f 7569  simplify: 'bl_ui
+0034e110: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e120: 4557 3344 5f4d 545f 6770 656e 6369 6c5f  EW3D_MT_gpencil_
+0034e130: 7369 6d70 6c69 6679 2720 3d20 4e6f 6e65  simplify' = None
+0034e140: 0a0a 5649 4557 3344 5f4d 545f 6770 656e  ..VIEW3D_MT_gpen
+0034e150: 6369 6c5f 7665 7274 6578 5f67 726f 7570  cil_vertex_group
+0034e160: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034e170: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034e180: 6770 656e 6369 6c5f 7665 7274 6578 5f67  gpencil_vertex_g
+0034e190: 726f 7570 2720 3d20 4e6f 6e65 0a0a 5649  roup' = None..VI
+0034e1a0: 4557 3344 5f4d 545f 6772 6561 7365 5f70  EW3D_MT_grease_p
+0034e1b0: 656e 6369 6c5f 6164 643a 2027 626c 5f75  encil_add: 'bl_u
+0034e1c0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034e1d0: 4945 5733 445f 4d54 5f67 7265 6173 655f  IEW3D_MT_grease_
+0034e1e0: 7065 6e63 696c 5f61 6464 2720 3d20 4e6f  pencil_add' = No
+0034e1f0: 6e65 0a0a 5649 4557 3344 5f4d 545f 686f  ne..VIEW3D_MT_ho
+0034e200: 6f6b 3a20 2762 6c5f 7569 2e73 7061 6365  ok: 'bl_ui.space
+0034e210: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034e220: 545f 686f 6f6b 2720 3d20 4e6f 6e65 0a0a  T_hook' = None..
+0034e230: 5649 4557 3344 5f4d 545f 696d 6167 655f  VIEW3D_MT_image_
+0034e240: 6164 643a 2027 626c 5f75 692e 7370 6163  add: 'bl_ui.spac
+0034e250: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034e260: 4d54 5f69 6d61 6765 5f61 6464 2720 3d20  MT_image_add' = 
+0034e270: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034e280: 6c69 6768 745f 6164 643a 2027 626c 5f75  light_add: 'bl_u
+0034e290: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034e2a0: 4945 5733 445f 4d54 5f6c 6967 6874 5f61  IEW3D_MT_light_a
+0034e2b0: 6464 2720 3d20 4e6f 6e65 0a0a 5649 4557  dd' = None..VIEW
+0034e2c0: 3344 5f4d 545f 6c69 6768 7470 726f 6265  3D_MT_lightprobe
+0034e2d0: 5f61 6464 3a20 2762 6c5f 7569 2e73 7061  _add: 'bl_ui.spa
+0034e2e0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034e2f0: 5f4d 545f 6c69 6768 7470 726f 6265 5f61  _MT_lightprobe_a
+0034e300: 6464 2720 3d20 4e6f 6e65 0a0a 5649 4557  dd' = None..VIEW
+0034e310: 3344 5f4d 545f 6d61 6b65 5f6c 696e 6b73  3D_MT_make_links
+0034e320: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034e330: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034e340: 6d61 6b65 5f6c 696e 6b73 2720 3d20 4e6f  make_links' = No
+0034e350: 6e65 0a0a 5649 4557 3344 5f4d 545f 6d61  ne..VIEW3D_MT_ma
+0034e360: 6b65 5f73 696e 676c 655f 7573 6572 3a20  ke_single_user: 
+0034e370: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034e380: 7733 642e 5649 4557 3344 5f4d 545f 6d61  w3d.VIEW3D_MT_ma
+0034e390: 6b65 5f73 696e 676c 655f 7573 6572 2720  ke_single_user' 
+0034e3a0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e3b0: 545f 6d61 736b 3a20 2762 6c5f 7569 2e73  T_mask: 'bl_ui.s
+0034e3c0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034e3d0: 3344 5f4d 545f 6d61 736b 2720 3d20 4e6f  3D_MT_mask' = No
+0034e3e0: 6e65 0a0a 5649 4557 3344 5f4d 545f 6d65  ne..VIEW3D_MT_me
+0034e3f0: 7368 5f61 6464 3a20 2762 6c5f 7569 2e73  sh_add: 'bl_ui.s
+0034e400: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034e410: 3344 5f4d 545f 6d65 7368 5f61 6464 2720  3D_MT_mesh_add' 
+0034e420: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e430: 545f 6d65 7461 6261 6c6c 5f61 6464 3a20  T_metaball_add: 
+0034e440: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034e450: 7733 642e 5649 4557 3344 5f4d 545f 6d65  w3d.VIEW3D_MT_me
+0034e460: 7461 6261 6c6c 5f61 6464 2720 3d20 4e6f  taball_add' = No
+0034e470: 6e65 0a0a 5649 4557 3344 5f4d 545f 6d69  ne..VIEW3D_MT_mi
+0034e480: 7272 6f72 3a20 2762 6c5f 7569 2e73 7061  rror: 'bl_ui.spa
+0034e490: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034e4a0: 5f4d 545f 6d69 7272 6f72 2720 3d20 4e6f  _MT_mirror' = No
+0034e4b0: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034e4c0: 6a65 6374 3a20 2762 6c5f 7569 2e73 7061  ject: 'bl_ui.spa
+0034e4d0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034e4e0: 5f4d 545f 6f62 6a65 6374 2720 3d20 4e6f  _MT_object' = No
+0034e4f0: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034e500: 6a65 6374 5f61 6e69 6d61 7469 6f6e 3a20  ject_animation: 
+0034e510: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034e520: 7733 642e 5649 4557 3344 5f4d 545f 6f62  w3d.VIEW3D_MT_ob
+0034e530: 6a65 6374 5f61 6e69 6d61 7469 6f6e 2720  ject_animation' 
+0034e540: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e550: 545f 6f62 6a65 6374 5f61 7070 6c79 3a20  T_object_apply: 
+0034e560: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034e570: 7733 642e 5649 4557 3344 5f4d 545f 6f62  w3d.VIEW3D_MT_ob
+0034e580: 6a65 6374 5f61 7070 6c79 2720 3d20 4e6f  ject_apply' = No
+0034e590: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034e5a0: 6a65 6374 5f61 7373 6574 3a20 2762 6c5f  ject_asset: 'bl_
+0034e5b0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034e5c0: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034e5d0: 5f61 7373 6574 2720 3d20 4e6f 6e65 0a0a  _asset' = None..
+0034e5e0: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034e5f0: 5f63 6c65 616e 7570 3a20 2762 6c5f 7569  _cleanup: 'bl_ui
+0034e600: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034e610: 4557 3344 5f4d 545f 6f62 6a65 6374 5f63  EW3D_MT_object_c
+0034e620: 6c65 616e 7570 2720 3d20 4e6f 6e65 0a0a  leanup' = None..
+0034e630: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034e640: 5f63 6c65 6172 3a20 2762 6c5f 7569 2e73  _clear: 'bl_ui.s
+0034e650: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034e660: 3344 5f4d 545f 6f62 6a65 6374 5f63 6c65  3D_MT_object_cle
+0034e670: 6172 2720 3d20 4e6f 6e65 0a0a 5649 4557  ar' = None..VIEW
+0034e680: 3344 5f4d 545f 6f62 6a65 6374 5f63 6f6c  3D_MT_object_col
+0034e690: 6c65 6374 696f 6e3a 2027 626c 5f75 692e  lection: 'bl_ui.
+0034e6a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034e6b0: 5733 445f 4d54 5f6f 626a 6563 745f 636f  W3D_MT_object_co
+0034e6c0: 6c6c 6563 7469 6f6e 2720 3d20 4e6f 6e65  llection' = None
+0034e6d0: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
+0034e6e0: 6374 5f63 6f6e 7374 7261 696e 7473 3a20  ct_constraints: 
+0034e6f0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034e700: 7733 642e 5649 4557 3344 5f4d 545f 6f62  w3d.VIEW3D_MT_ob
+0034e710: 6a65 6374 5f63 6f6e 7374 7261 696e 7473  ject_constraints
+0034e720: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034e730: 5f4d 545f 6f62 6a65 6374 5f63 6f6e 7465  _MT_object_conte
+0034e740: 7874 5f6d 656e 753a 2027 626c 5f75 692e  xt_menu: 'bl_ui.
+0034e750: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034e760: 5733 445f 4d54 5f6f 626a 6563 745f 636f  W3D_MT_object_co
+0034e770: 6e74 6578 745f 6d65 6e75 2720 3d20 4e6f  ntext_menu' = No
+0034e780: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034e790: 6a65 6374 5f63 6f6e 7665 7274 3a20 2762  ject_convert: 'b
+0034e7a0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034e7b0: 642e 5649 4557 3344 5f4d 545f 6f62 6a65  d.VIEW3D_MT_obje
+0034e7c0: 6374 5f63 6f6e 7665 7274 2720 3d20 4e6f  ct_convert' = No
+0034e7d0: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034e7e0: 6a65 6374 5f6c 6962 6f76 6572 7269 6465  ject_liboverride
+0034e7f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034e800: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034e810: 6f62 6a65 6374 5f6c 6962 6f76 6572 7269  object_liboverri
+0034e820: 6465 2720 3d20 4e6f 6e65 0a0a 5649 4557  de' = None..VIEW
+0034e830: 3344 5f4d 545f 6f62 6a65 6374 5f6d 6f64  3D_MT_object_mod
+0034e840: 655f 7069 653a 2027 626c 5f75 692e 7370  e_pie: 'bl_ui.sp
+0034e850: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e860: 445f 4d54 5f6f 626a 6563 745f 6d6f 6465  D_MT_object_mode
+0034e870: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
+0034e880: 4557 3344 5f4d 545f 6f62 6a65 6374 5f70  EW3D_MT_object_p
+0034e890: 6172 656e 743a 2027 626c 5f75 692e 7370  arent: 'bl_ui.sp
+0034e8a0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034e8b0: 445f 4d54 5f6f 626a 6563 745f 7061 7265  D_MT_object_pare
+0034e8c0: 6e74 2720 3d20 4e6f 6e65 0a0a 5649 4557  nt' = None..VIEW
+0034e8d0: 3344 5f4d 545f 6f62 6a65 6374 5f71 7569  3D_MT_object_qui
+0034e8e0: 636b 5f65 6666 6563 7473 3a20 2762 6c5f  ck_effects: 'bl_
+0034e8f0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034e900: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034e910: 5f71 7569 636b 5f65 6666 6563 7473 2720  _quick_effects' 
+0034e920: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034e930: 545f 6f62 6a65 6374 5f72 656c 6174 696f  T_object_relatio
+0034e940: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
+0034e950: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034e960: 545f 6f62 6a65 6374 5f72 656c 6174 696f  T_object_relatio
+0034e970: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
+0034e980: 3344 5f4d 545f 6f62 6a65 6374 5f72 6967  3D_MT_object_rig
+0034e990: 6964 5f62 6f64 793a 2027 626c 5f75 692e  id_body: 'bl_ui.
+0034e9a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034e9b0: 5733 445f 4d54 5f6f 626a 6563 745f 7269  W3D_MT_object_ri
+0034e9c0: 6769 645f 626f 6479 2720 3d20 4e6f 6e65  gid_body' = None
+0034e9d0: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
+0034e9e0: 6374 5f73 6861 6469 6e67 3a20 2762 6c5f  ct_shading: 'bl_
+0034e9f0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034ea00: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034ea10: 5f73 6861 6469 6e67 2720 3d20 4e6f 6e65  _shading' = None
 0034ea20: 0a0a 5649 4557 3344 5f4d 545f 6f62 6a65  ..VIEW3D_MT_obje
-0034ea30: 6374 5f74 7261 636b 3a20 2762 6c5f 7569  ct_track: 'bl_ui
-0034ea40: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034ea50: 4557 3344 5f4d 545f 6f62 6a65 6374 5f74  EW3D_MT_object_t
-0034ea60: 7261 636b 2720 3d20 4e6f 6e65 0a0a 5649  rack' = None..VI
-0034ea70: 4557 3344 5f4d 545f 6f72 6965 6e74 6174  EW3D_MT_orientat
-0034ea80: 696f 6e73 5f70 6965 3a20 2762 6c5f 7569  ions_pie: 'bl_ui
-0034ea90: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034eaa0: 4557 3344 5f4d 545f 6f72 6965 6e74 6174  EW3D_MT_orientat
-0034eab0: 696f 6e73 5f70 6965 2720 3d20 4e6f 6e65  ions_pie' = None
-0034eac0: 0a0a 5649 4557 3344 5f4d 545f 7061 696e  ..VIEW3D_MT_pain
-0034ead0: 745f 6770 656e 6369 6c3a 2027 626c 5f75  t_gpencil: 'bl_u
-0034eae0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034eaf0: 4945 5733 445f 4d54 5f70 6169 6e74 5f67  IEW3D_MT_paint_g
-0034eb00: 7065 6e63 696c 2720 3d20 4e6f 6e65 0a0a  pencil' = None..
-0034eb10: 5649 4557 3344 5f4d 545f 7061 696e 745f  VIEW3D_MT_paint_
-0034eb20: 7665 7274 6578 3a20 2762 6c5f 7569 2e73  vertex: 'bl_ui.s
-0034eb30: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034eb40: 3344 5f4d 545f 7061 696e 745f 7665 7274  3D_MT_paint_vert
-0034eb50: 6578 2720 3d20 4e6f 6e65 0a0a 5649 4557  ex' = None..VIEW
-0034eb60: 3344 5f4d 545f 7061 696e 745f 7765 6967  3D_MT_paint_weig
-0034eb70: 6874 3a20 2762 6c5f 7569 2e73 7061 6365  ht: 'bl_ui.space
-0034eb80: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034eb90: 545f 7061 696e 745f 7765 6967 6874 2720  T_paint_weight' 
-0034eba0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034ebb0: 545f 7061 696e 745f 7765 6967 6874 5f6c  T_paint_weight_l
-0034ebc0: 6f63 6b3a 2027 626c 5f75 692e 7370 6163  ock: 'bl_ui.spac
-0034ebd0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034ebe0: 4d54 5f70 6169 6e74 5f77 6569 6768 745f  MT_paint_weight_
-0034ebf0: 6c6f 636b 2720 3d20 4e6f 6e65 0a0a 5649  lock' = None..VI
-0034ec00: 4557 3344 5f4d 545f 7061 7274 6963 6c65  EW3D_MT_particle
-0034ec10: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-0034ec20: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
-0034ec30: 7061 7274 6963 6c65 2720 3d20 4e6f 6e65  particle' = None
-0034ec40: 0a0a 5649 4557 3344 5f4d 545f 7061 7274  ..VIEW3D_MT_part
-0034ec50: 6963 6c65 5f63 6f6e 7465 7874 5f6d 656e  icle_context_men
-0034ec60: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
-0034ec70: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034ec80: 5f70 6172 7469 636c 655f 636f 6e74 6578  _particle_contex
-0034ec90: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
-0034eca0: 5649 4557 3344 5f4d 545f 7061 7274 6963  VIEW3D_MT_partic
-0034ecb0: 6c65 5f73 686f 7768 6964 653a 2027 626c  le_showhide: 'bl
-0034ecc0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034ecd0: 2e56 4945 5733 445f 4d54 5f70 6172 7469  .VIEW3D_MT_parti
-0034ece0: 636c 655f 7368 6f77 6869 6465 2720 3d20  cle_showhide' = 
-0034ecf0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034ed00: 7069 766f 745f 7069 653a 2027 626c 5f75  pivot_pie: 'bl_u
-0034ed10: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ed20: 4945 5733 445f 4d54 5f70 6976 6f74 5f70  IEW3D_MT_pivot_p
-0034ed30: 6965 2720 3d20 4e6f 6e65 0a0a 5649 4557  ie' = None..VIEW
-0034ed40: 3344 5f4d 545f 706f 7365 3a20 2762 6c5f  3D_MT_pose: 'bl_
-0034ed50: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034ed60: 5649 4557 3344 5f4d 545f 706f 7365 2720  VIEW3D_MT_pose' 
-0034ed70: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034ed80: 545f 706f 7365 5f61 7070 6c79 3a20 2762  T_pose_apply: 'b
-0034ed90: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034eda0: 642e 5649 4557 3344 5f4d 545f 706f 7365  d.VIEW3D_MT_pose
-0034edb0: 5f61 7070 6c79 2720 3d20 4e6f 6e65 0a0a  _apply' = None..
-0034edc0: 5649 4557 3344 5f4d 545f 706f 7365 5f63  VIEW3D_MT_pose_c
-0034edd0: 6f6e 7374 7261 696e 7473 3a20 2762 6c5f  onstraints: 'bl_
-0034ede0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034edf0: 5649 4557 3344 5f4d 545f 706f 7365 5f63  VIEW3D_MT_pose_c
-0034ee00: 6f6e 7374 7261 696e 7473 2720 3d20 4e6f  onstraints' = No
-0034ee10: 6e65 0a0a 5649 4557 3344 5f4d 545f 706f  ne..VIEW3D_MT_po
-0034ee20: 7365 5f63 6f6e 7465 7874 5f6d 656e 753a  se_context_menu:
-0034ee30: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ee40: 6577 3364 2e56 4945 5733 445f 4d54 5f70  ew3d.VIEW3D_MT_p
-0034ee50: 6f73 655f 636f 6e74 6578 745f 6d65 6e75  ose_context_menu
-0034ee60: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034ee70: 5f4d 545f 706f 7365 5f67 726f 7570 3a20  _MT_pose_group: 
-0034ee80: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034ee90: 7733 642e 5649 4557 3344 5f4d 545f 706f  w3d.VIEW3D_MT_po
-0034eea0: 7365 5f67 726f 7570 2720 3d20 4e6f 6e65  se_group' = None
-0034eeb0: 0a0a 5649 4557 3344 5f4d 545f 706f 7365  ..VIEW3D_MT_pose
-0034eec0: 5f69 6b3a 2027 626c 5f75 692e 7370 6163  _ik: 'bl_ui.spac
-0034eed0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034eee0: 4d54 5f70 6f73 655f 696b 2720 3d20 4e6f  MT_pose_ik' = No
-0034eef0: 6e65 0a0a 5649 4557 3344 5f4d 545f 706f  ne..VIEW3D_MT_po
-0034ef00: 7365 5f6d 6f74 696f 6e3a 2027 626c 5f75  se_motion: 'bl_u
-0034ef10: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034ef20: 4945 5733 445f 4d54 5f70 6f73 655f 6d6f  IEW3D_MT_pose_mo
-0034ef30: 7469 6f6e 2720 3d20 4e6f 6e65 0a0a 5649  tion' = None..VI
-0034ef40: 4557 3344 5f4d 545f 706f 7365 5f6e 616d  EW3D_MT_pose_nam
-0034ef50: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
-0034ef60: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034ef70: 545f 706f 7365 5f6e 616d 6573 2720 3d20  T_pose_names' = 
-0034ef80: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034ef90: 706f 7365 5f70 726f 7061 6761 7465 3a20  pose_propagate: 
-0034efa0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034efb0: 7733 642e 5649 4557 3344 5f4d 545f 706f  w3d.VIEW3D_MT_po
-0034efc0: 7365 5f70 726f 7061 6761 7465 2720 3d20  se_propagate' = 
-0034efd0: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034efe0: 706f 7365 5f73 686f 7768 6964 653a 2027  pose_showhide: '
-0034eff0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-0034f000: 3364 2e56 4945 5733 445f 4d54 5f70 6f73  3d.VIEW3D_MT_pos
-0034f010: 655f 7368 6f77 6869 6465 2720 3d20 4e6f  e_showhide' = No
-0034f020: 6e65 0a0a 5649 4557 3344 5f4d 545f 706f  ne..VIEW3D_MT_po
-0034f030: 7365 5f73 6c69 6465 3a20 2762 6c5f 7569  se_slide: 'bl_ui
-0034f040: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034f050: 4557 3344 5f4d 545f 706f 7365 5f73 6c69  EW3D_MT_pose_sli
-0034f060: 6465 2720 3d20 4e6f 6e65 0a0a 5649 4557  de' = None..VIEW
-0034f070: 3344 5f4d 545f 706f 7365 5f74 7261 6e73  3D_MT_pose_trans
-0034f080: 666f 726d 3a20 2762 6c5f 7569 2e73 7061  form: 'bl_ui.spa
-0034f090: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034f0a0: 5f4d 545f 706f 7365 5f74 7261 6e73 666f  _MT_pose_transfo
-0034f0b0: 726d 2720 3d20 4e6f 6e65 0a0a 5649 4557  rm' = None..VIEW
-0034f0c0: 3344 5f4d 545f 7072 6f70 6f72 7469 6f6e  3D_MT_proportion
-0034f0d0: 616c 5f65 6469 7469 6e67 5f66 616c 6c6f  al_editing_fallo
-0034f0e0: 6666 5f70 6965 3a20 2762 6c5f 7569 2e73  ff_pie: 'bl_ui.s
-0034f0f0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034f100: 3344 5f4d 545f 7072 6f70 6f72 7469 6f6e  3D_MT_proportion
-0034f110: 616c 5f65 6469 7469 6e67 5f66 616c 6c6f  al_editing_fallo
-0034f120: 6666 5f70 6965 2720 3d20 4e6f 6e65 0a0a  ff_pie' = None..
-0034f130: 5649 4557 3344 5f4d 545f 7261 6e64 6f6d  VIEW3D_MT_random
-0034f140: 5f6d 6173 6b3a 2027 626c 5f75 692e 7370  _mask: 'bl_ui.sp
-0034f150: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f160: 445f 4d54 5f72 616e 646f 6d5f 6d61 736b  D_MT_random_mask
-0034f170: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f180: 5f4d 545f 7363 756c 7074 3a20 2762 6c5f  _MT_sculpt: 'bl_
-0034f190: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f1a0: 5649 4557 3344 5f4d 545f 7363 756c 7074  VIEW3D_MT_sculpt
-0034f1b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f1c0: 5f4d 545f 7363 756c 7074 5f61 7574 6f6d  _MT_sculpt_autom
-0034f1d0: 6173 6b69 6e67 5f70 6965 3a20 2762 6c5f  asking_pie: 'bl_
-0034f1e0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
-0034f1f0: 5649 4557 3344 5f4d 545f 7363 756c 7074  VIEW3D_MT_sculpt
-0034f200: 5f61 7574 6f6d 6173 6b69 6e67 5f70 6965  _automasking_pie
-0034f210: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f220: 5f4d 545f 7363 756c 7074 5f63 7572 7665  _MT_sculpt_curve
-0034f230: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-0034f240: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f250: 5f73 6375 6c70 745f 6375 7276 6573 2720  _sculpt_curves' 
-0034f260: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034f270: 545f 7363 756c 7074 5f66 6163 655f 7365  T_sculpt_face_se
-0034f280: 7473 5f65 6469 745f 7069 653a 2027 626c  ts_edit_pie: 'bl
-0034f290: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034f2a0: 2e56 4945 5733 445f 4d54 5f73 6375 6c70  .VIEW3D_MT_sculp
-0034f2b0: 745f 6661 6365 5f73 6574 735f 6564 6974  t_face_sets_edit
-0034f2c0: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
-0034f2d0: 4557 3344 5f4d 545f 7363 756c 7074 5f67  EW3D_MT_sculpt_g
-0034f2e0: 7065 6e63 696c 5f61 7574 6f6d 6173 6b69  pencil_automaski
-0034f2f0: 6e67 5f70 6965 3a20 2762 6c5f 7569 2e73  ng_pie: 'bl_ui.s
-0034f300: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034f310: 3344 5f4d 545f 7363 756c 7074 5f67 7065  3D_MT_sculpt_gpe
-0034f320: 6e63 696c 5f61 7574 6f6d 6173 6b69 6e67  ncil_automasking
-0034f330: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
-0034f340: 4557 3344 5f4d 545f 7363 756c 7074 5f6d  EW3D_MT_sculpt_m
-0034f350: 6173 6b5f 6564 6974 5f70 6965 3a20 2762  ask_edit_pie: 'b
-0034f360: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f370: 642e 5649 4557 3344 5f4d 545f 7363 756c  d.VIEW3D_MT_scul
-0034f380: 7074 5f6d 6173 6b5f 6564 6974 5f70 6965  pt_mask_edit_pie
-0034f390: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f3a0: 5f4d 545f 7363 756c 7074 5f73 6574 5f70  _MT_sculpt_set_p
-0034f3b0: 6976 6f74 3a20 2762 6c5f 7569 2e73 7061  ivot: 'bl_ui.spa
-0034f3c0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034f3d0: 5f4d 545f 7363 756c 7074 5f73 6574 5f70  _MT_sculpt_set_p
-0034f3e0: 6976 6f74 2720 3d20 4e6f 6e65 0a0a 5649  ivot' = None..VI
-0034f3f0: 4557 3344 5f4d 545f 7365 6c65 6374 5f65  EW3D_MT_select_e
-0034f400: 6469 745f 6172 6d61 7475 7265 3a20 2762  dit_armature: 'b
-0034f410: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f420: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
-0034f430: 6374 5f65 6469 745f 6172 6d61 7475 7265  ct_edit_armature
-0034f440: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f450: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
-0034f460: 6375 7276 653a 2027 626c 5f75 692e 7370  curve: 'bl_ui.sp
-0034f470: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f480: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
-0034f490: 5f63 7572 7665 2720 3d20 4e6f 6e65 0a0a  _curve' = None..
-0034f4a0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f4b0: 5f65 6469 745f 6375 7276 6573 3a20 2762  _edit_curves: 'b
-0034f4c0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f4d0: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
-0034f4e0: 6374 5f65 6469 745f 6375 7276 6573 2720  ct_edit_curves' 
-0034f4f0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034f500: 545f 7365 6c65 6374 5f65 6469 745f 6770  T_select_edit_gp
-0034f510: 656e 6369 6c3a 2027 626c 5f75 692e 7370  encil: 'bl_ui.sp
-0034f520: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f530: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
-0034f540: 5f67 7065 6e63 696c 2720 3d20 4e6f 6e65  _gpencil' = None
-0034f550: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
-0034f560: 6374 5f65 6469 745f 6772 6561 7365 5f70  ct_edit_grease_p
-0034f570: 656e 6369 6c3a 2027 626c 5f75 692e 7370  encil: 'bl_ui.sp
-0034f580: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f590: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
-0034f5a0: 5f67 7265 6173 655f 7065 6e63 696c 2720  _grease_pencil' 
-0034f5b0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
-0034f5c0: 545f 7365 6c65 6374 5f65 6469 745f 6c61  T_select_edit_la
-0034f5d0: 7474 6963 653a 2027 626c 5f75 692e 7370  ttice: 'bl_ui.sp
-0034f5e0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f5f0: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
-0034f600: 5f6c 6174 7469 6365 2720 3d20 4e6f 6e65  _lattice' = None
-0034f610: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
-0034f620: 6374 5f65 6469 745f 6d65 7368 3a20 2762  ct_edit_mesh: 'b
-0034f630: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034f640: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
-0034f650: 6374 5f65 6469 745f 6d65 7368 2720 3d20  ct_edit_mesh' = 
-0034f660: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034f670: 7365 6c65 6374 5f65 6469 745f 6d65 7461  select_edit_meta
-0034f680: 6261 6c6c 3a20 2762 6c5f 7569 2e73 7061  ball: 'bl_ui.spa
-0034f690: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-0034f6a0: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
-0034f6b0: 6d65 7461 6261 6c6c 2720 3d20 4e6f 6e65  metaball' = None
-0034f6c0: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
-0034f6d0: 6374 5f65 6469 745f 7375 7266 6163 653a  ct_edit_surface:
-0034f6e0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f6f0: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034f700: 656c 6563 745f 6564 6974 5f73 7572 6661  elect_edit_surfa
-0034f710: 6365 2720 3d20 4e6f 6e65 0a0a 5649 4557  ce' = None..VIEW
-0034f720: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034f730: 745f 7465 7874 3a20 2762 6c5f 7569 2e73  t_text: 'bl_ui.s
-0034f740: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034f750: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
-0034f760: 745f 7465 7874 2720 3d20 4e6f 6e65 0a0a  t_text' = None..
-0034f770: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f780: 5f6f 626a 6563 743a 2027 626c 5f75 692e  _object: 'bl_ui.
-0034f790: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-0034f7a0: 5733 445f 4d54 5f73 656c 6563 745f 6f62  W3D_MT_select_ob
-0034f7b0: 6a65 6374 2720 3d20 4e6f 6e65 0a0a 5649  ject' = None..VI
-0034f7c0: 4557 3344 5f4d 545f 7365 6c65 6374 5f6f  EW3D_MT_select_o
-0034f7d0: 626a 6563 745f 6d6f 7265 5f6c 6573 733a  bject_more_less:
-0034f7e0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034f7f0: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034f800: 656c 6563 745f 6f62 6a65 6374 5f6d 6f72  elect_object_mor
-0034f810: 655f 6c65 7373 2720 3d20 4e6f 6e65 0a0a  e_less' = None..
-0034f820: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
-0034f830: 5f70 6169 6e74 5f6d 6173 6b3a 2027 626c  _paint_mask: 'bl
+0034ea30: 6374 5f73 686f 7768 6964 653a 2027 626c  ct_showhide: 'bl
+0034ea40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034ea50: 2e56 4945 5733 445f 4d54 5f6f 626a 6563  .VIEW3D_MT_objec
+0034ea60: 745f 7368 6f77 6869 6465 2720 3d20 4e6f  t_showhide' = No
+0034ea70: 6e65 0a0a 5649 4557 3344 5f4d 545f 6f62  ne..VIEW3D_MT_ob
+0034ea80: 6a65 6374 5f74 7261 636b 3a20 2762 6c5f  ject_track: 'bl_
+0034ea90: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034eaa0: 5649 4557 3344 5f4d 545f 6f62 6a65 6374  VIEW3D_MT_object
+0034eab0: 5f74 7261 636b 2720 3d20 4e6f 6e65 0a0a  _track' = None..
+0034eac0: 5649 4557 3344 5f4d 545f 6f72 6965 6e74  VIEW3D_MT_orient
+0034ead0: 6174 696f 6e73 5f70 6965 3a20 2762 6c5f  ations_pie: 'bl_
+0034eae0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034eaf0: 5649 4557 3344 5f4d 545f 6f72 6965 6e74  VIEW3D_MT_orient
+0034eb00: 6174 696f 6e73 5f70 6965 2720 3d20 4e6f  ations_pie' = No
+0034eb10: 6e65 0a0a 5649 4557 3344 5f4d 545f 7061  ne..VIEW3D_MT_pa
+0034eb20: 696e 745f 6770 656e 6369 6c3a 2027 626c  int_gpencil: 'bl
+0034eb30: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034eb40: 2e56 4945 5733 445f 4d54 5f70 6169 6e74  .VIEW3D_MT_paint
+0034eb50: 5f67 7065 6e63 696c 2720 3d20 4e6f 6e65  _gpencil' = None
+0034eb60: 0a0a 5649 4557 3344 5f4d 545f 7061 696e  ..VIEW3D_MT_pain
+0034eb70: 745f 7665 7274 6578 3a20 2762 6c5f 7569  t_vertex: 'bl_ui
+0034eb80: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034eb90: 4557 3344 5f4d 545f 7061 696e 745f 7665  EW3D_MT_paint_ve
+0034eba0: 7274 6578 2720 3d20 4e6f 6e65 0a0a 5649  rtex' = None..VI
+0034ebb0: 4557 3344 5f4d 545f 7061 696e 745f 7765  EW3D_MT_paint_we
+0034ebc0: 6967 6874 3a20 2762 6c5f 7569 2e73 7061  ight: 'bl_ui.spa
+0034ebd0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034ebe0: 5f4d 545f 7061 696e 745f 7765 6967 6874  _MT_paint_weight
+0034ebf0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034ec00: 5f4d 545f 7061 696e 745f 7765 6967 6874  _MT_paint_weight
+0034ec10: 5f6c 6f63 6b3a 2027 626c 5f75 692e 7370  _lock: 'bl_ui.sp
+0034ec20: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ec30: 445f 4d54 5f70 6169 6e74 5f77 6569 6768  D_MT_paint_weigh
+0034ec40: 745f 6c6f 636b 2720 3d20 4e6f 6e65 0a0a  t_lock' = None..
+0034ec50: 5649 4557 3344 5f4d 545f 7061 7274 6963  VIEW3D_MT_partic
+0034ec60: 6c65 3a20 2762 6c5f 7569 2e73 7061 6365  le: 'bl_ui.space
+0034ec70: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034ec80: 545f 7061 7274 6963 6c65 2720 3d20 4e6f  T_particle' = No
+0034ec90: 6e65 0a0a 5649 4557 3344 5f4d 545f 7061  ne..VIEW3D_MT_pa
+0034eca0: 7274 6963 6c65 5f63 6f6e 7465 7874 5f6d  rticle_context_m
+0034ecb0: 656e 753a 2027 626c 5f75 692e 7370 6163  enu: 'bl_ui.spac
+0034ecc0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034ecd0: 4d54 5f70 6172 7469 636c 655f 636f 6e74  MT_particle_cont
+0034ece0: 6578 745f 6d65 6e75 2720 3d20 4e6f 6e65  ext_menu' = None
+0034ecf0: 0a0a 5649 4557 3344 5f4d 545f 7061 7274  ..VIEW3D_MT_part
+0034ed00: 6963 6c65 5f73 686f 7768 6964 653a 2027  icle_showhide: '
+0034ed10: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034ed20: 3364 2e56 4945 5733 445f 4d54 5f70 6172  3d.VIEW3D_MT_par
+0034ed30: 7469 636c 655f 7368 6f77 6869 6465 2720  ticle_showhide' 
+0034ed40: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034ed50: 545f 7069 766f 745f 7069 653a 2027 626c  T_pivot_pie: 'bl
+0034ed60: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034ed70: 2e56 4945 5733 445f 4d54 5f70 6976 6f74  .VIEW3D_MT_pivot
+0034ed80: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
+0034ed90: 4557 3344 5f4d 545f 706f 7365 3a20 2762  EW3D_MT_pose: 'b
+0034eda0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034edb0: 642e 5649 4557 3344 5f4d 545f 706f 7365  d.VIEW3D_MT_pose
+0034edc0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034edd0: 5f4d 545f 706f 7365 5f61 7070 6c79 3a20  _MT_pose_apply: 
+0034ede0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034edf0: 7733 642e 5649 4557 3344 5f4d 545f 706f  w3d.VIEW3D_MT_po
+0034ee00: 7365 5f61 7070 6c79 2720 3d20 4e6f 6e65  se_apply' = None
+0034ee10: 0a0a 5649 4557 3344 5f4d 545f 706f 7365  ..VIEW3D_MT_pose
+0034ee20: 5f63 6f6e 7374 7261 696e 7473 3a20 2762  _constraints: 'b
+0034ee30: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034ee40: 642e 5649 4557 3344 5f4d 545f 706f 7365  d.VIEW3D_MT_pose
+0034ee50: 5f63 6f6e 7374 7261 696e 7473 2720 3d20  _constraints' = 
+0034ee60: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034ee70: 706f 7365 5f63 6f6e 7465 7874 5f6d 656e  pose_context_men
+0034ee80: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
+0034ee90: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
+0034eea0: 5f70 6f73 655f 636f 6e74 6578 745f 6d65  _pose_context_me
+0034eeb0: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
+0034eec0: 3344 5f4d 545f 706f 7365 5f67 726f 7570  3D_MT_pose_group
+0034eed0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034eee0: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034eef0: 706f 7365 5f67 726f 7570 2720 3d20 4e6f  pose_group' = No
+0034ef00: 6e65 0a0a 5649 4557 3344 5f4d 545f 706f  ne..VIEW3D_MT_po
+0034ef10: 7365 5f69 6b3a 2027 626c 5f75 692e 7370  se_ik: 'bl_ui.sp
+0034ef20: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034ef30: 445f 4d54 5f70 6f73 655f 696b 2720 3d20  D_MT_pose_ik' = 
+0034ef40: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034ef50: 706f 7365 5f6d 6f74 696f 6e3a 2027 626c  pose_motion: 'bl
+0034ef60: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034ef70: 2e56 4945 5733 445f 4d54 5f70 6f73 655f  .VIEW3D_MT_pose_
+0034ef80: 6d6f 7469 6f6e 2720 3d20 4e6f 6e65 0a0a  motion' = None..
+0034ef90: 5649 4557 3344 5f4d 545f 706f 7365 5f6e  VIEW3D_MT_pose_n
+0034efa0: 616d 6573 3a20 2762 6c5f 7569 2e73 7061  ames: 'bl_ui.spa
+0034efb0: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+0034efc0: 5f4d 545f 706f 7365 5f6e 616d 6573 2720  _MT_pose_names' 
+0034efd0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034efe0: 545f 706f 7365 5f70 726f 7061 6761 7465  T_pose_propagate
+0034eff0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+0034f000: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+0034f010: 706f 7365 5f70 726f 7061 6761 7465 2720  pose_propagate' 
+0034f020: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034f030: 545f 706f 7365 5f73 686f 7768 6964 653a  T_pose_showhide:
+0034f040: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034f050: 6577 3364 2e56 4945 5733 445f 4d54 5f70  ew3d.VIEW3D_MT_p
+0034f060: 6f73 655f 7368 6f77 6869 6465 2720 3d20  ose_showhide' = 
+0034f070: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034f080: 706f 7365 5f73 6c69 6465 3a20 2762 6c5f  pose_slide: 'bl_
+0034f090: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034f0a0: 5649 4557 3344 5f4d 545f 706f 7365 5f73  VIEW3D_MT_pose_s
+0034f0b0: 6c69 6465 2720 3d20 4e6f 6e65 0a0a 5649  lide' = None..VI
+0034f0c0: 4557 3344 5f4d 545f 706f 7365 5f74 7261  EW3D_MT_pose_tra
+0034f0d0: 6e73 666f 726d 3a20 2762 6c5f 7569 2e73  nsform: 'bl_ui.s
+0034f0e0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034f0f0: 3344 5f4d 545f 706f 7365 5f74 7261 6e73  3D_MT_pose_trans
+0034f100: 666f 726d 2720 3d20 4e6f 6e65 0a0a 5649  form' = None..VI
+0034f110: 4557 3344 5f4d 545f 7072 6f70 6f72 7469  EW3D_MT_proporti
+0034f120: 6f6e 616c 5f65 6469 7469 6e67 5f66 616c  onal_editing_fal
+0034f130: 6c6f 6666 5f70 6965 3a20 2762 6c5f 7569  loff_pie: 'bl_ui
+0034f140: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034f150: 4557 3344 5f4d 545f 7072 6f70 6f72 7469  EW3D_MT_proporti
+0034f160: 6f6e 616c 5f65 6469 7469 6e67 5f66 616c  onal_editing_fal
+0034f170: 6c6f 6666 5f70 6965 2720 3d20 4e6f 6e65  loff_pie' = None
+0034f180: 0a0a 5649 4557 3344 5f4d 545f 7261 6e64  ..VIEW3D_MT_rand
+0034f190: 6f6d 5f6d 6173 6b3a 2027 626c 5f75 692e  om_mask: 'bl_ui.
+0034f1a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f1b0: 5733 445f 4d54 5f72 616e 646f 6d5f 6d61  W3D_MT_random_ma
+0034f1c0: 736b 2720 3d20 4e6f 6e65 0a0a 5649 4557  sk' = None..VIEW
+0034f1d0: 3344 5f4d 545f 7363 756c 7074 3a20 2762  3D_MT_sculpt: 'b
+0034f1e0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034f1f0: 642e 5649 4557 3344 5f4d 545f 7363 756c  d.VIEW3D_MT_scul
+0034f200: 7074 2720 3d20 4e6f 6e65 0a0a 5649 4557  pt' = None..VIEW
+0034f210: 3344 5f4d 545f 7363 756c 7074 5f61 7574  3D_MT_sculpt_aut
+0034f220: 6f6d 6173 6b69 6e67 5f70 6965 3a20 2762  omasking_pie: 'b
+0034f230: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034f240: 642e 5649 4557 3344 5f4d 545f 7363 756c  d.VIEW3D_MT_scul
+0034f250: 7074 5f61 7574 6f6d 6173 6b69 6e67 5f70  pt_automasking_p
+0034f260: 6965 2720 3d20 4e6f 6e65 0a0a 5649 4557  ie' = None..VIEW
+0034f270: 3344 5f4d 545f 7363 756c 7074 5f63 7572  3D_MT_sculpt_cur
+0034f280: 7665 733a 2027 626c 5f75 692e 7370 6163  ves: 'bl_ui.spac
+0034f290: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034f2a0: 4d54 5f73 6375 6c70 745f 6375 7276 6573  MT_sculpt_curves
+0034f2b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f2c0: 5f4d 545f 7363 756c 7074 5f66 6163 655f  _MT_sculpt_face_
+0034f2d0: 7365 7473 5f65 6469 745f 7069 653a 2027  sets_edit_pie: '
+0034f2e0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034f2f0: 3364 2e56 4945 5733 445f 4d54 5f73 6375  3d.VIEW3D_MT_scu
+0034f300: 6c70 745f 6661 6365 5f73 6574 735f 6564  lpt_face_sets_ed
+0034f310: 6974 5f70 6965 2720 3d20 4e6f 6e65 0a0a  it_pie' = None..
+0034f320: 5649 4557 3344 5f4d 545f 7363 756c 7074  VIEW3D_MT_sculpt
+0034f330: 5f67 7065 6e63 696c 5f61 7574 6f6d 6173  _gpencil_automas
+0034f340: 6b69 6e67 5f70 6965 3a20 2762 6c5f 7569  king_pie: 'bl_ui
+0034f350: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+0034f360: 4557 3344 5f4d 545f 7363 756c 7074 5f67  EW3D_MT_sculpt_g
+0034f370: 7065 6e63 696c 5f61 7574 6f6d 6173 6b69  pencil_automaski
+0034f380: 6e67 5f70 6965 2720 3d20 4e6f 6e65 0a0a  ng_pie' = None..
+0034f390: 5649 4557 3344 5f4d 545f 7363 756c 7074  VIEW3D_MT_sculpt
+0034f3a0: 5f6d 6173 6b5f 6564 6974 5f70 6965 3a20  _mask_edit_pie: 
+0034f3b0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f3c0: 7733 642e 5649 4557 3344 5f4d 545f 7363  w3d.VIEW3D_MT_sc
+0034f3d0: 756c 7074 5f6d 6173 6b5f 6564 6974 5f70  ulpt_mask_edit_p
+0034f3e0: 6965 2720 3d20 4e6f 6e65 0a0a 5649 4557  ie' = None..VIEW
+0034f3f0: 3344 5f4d 545f 7363 756c 7074 5f73 6574  3D_MT_sculpt_set
+0034f400: 5f70 6976 6f74 3a20 2762 6c5f 7569 2e73  _pivot: 'bl_ui.s
+0034f410: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034f420: 3344 5f4d 545f 7363 756c 7074 5f73 6574  3D_MT_sculpt_set
+0034f430: 5f70 6976 6f74 2720 3d20 4e6f 6e65 0a0a  _pivot' = None..
+0034f440: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034f450: 5f65 6469 745f 6172 6d61 7475 7265 3a20  _edit_armature: 
+0034f460: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f470: 7733 642e 5649 4557 3344 5f4d 545f 7365  w3d.VIEW3D_MT_se
+0034f480: 6c65 6374 5f65 6469 745f 6172 6d61 7475  lect_edit_armatu
+0034f490: 7265 2720 3d20 4e6f 6e65 0a0a 5649 4557  re' = None..VIEW
+0034f4a0: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
+0034f4b0: 745f 6375 7276 653a 2027 626c 5f75 692e  t_curve: 'bl_ui.
+0034f4c0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f4d0: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034f4e0: 6974 5f63 7572 7665 2720 3d20 4e6f 6e65  it_curve' = None
+0034f4f0: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
+0034f500: 6374 5f65 6469 745f 6375 7276 6573 3a20  ct_edit_curves: 
+0034f510: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f520: 7733 642e 5649 4557 3344 5f4d 545f 7365  w3d.VIEW3D_MT_se
+0034f530: 6c65 6374 5f65 6469 745f 6375 7276 6573  lect_edit_curves
+0034f540: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f550: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f560: 6770 656e 6369 6c3a 2027 626c 5f75 692e  gpencil: 'bl_ui.
+0034f570: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f580: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034f590: 6974 5f67 7065 6e63 696c 2720 3d20 4e6f  it_gpencil' = No
+0034f5a0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034f5b0: 6c65 6374 5f65 6469 745f 6772 6561 7365  lect_edit_grease
+0034f5c0: 5f70 656e 6369 6c3a 2027 626c 5f75 692e  _pencil: 'bl_ui.
+0034f5d0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f5e0: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034f5f0: 6974 5f67 7265 6173 655f 7065 6e63 696c  it_grease_pencil
+0034f600: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f610: 5f4d 545f 7365 6c65 6374 5f65 6469 745f  _MT_select_edit_
+0034f620: 6c61 7474 6963 653a 2027 626c 5f75 692e  lattice: 'bl_ui.
+0034f630: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f640: 5733 445f 4d54 5f73 656c 6563 745f 6564  W3D_MT_select_ed
+0034f650: 6974 5f6c 6174 7469 6365 2720 3d20 4e6f  it_lattice' = No
+0034f660: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034f670: 6c65 6374 5f65 6469 745f 6d65 7368 3a20  lect_edit_mesh: 
+0034f680: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+0034f690: 7733 642e 5649 4557 3344 5f4d 545f 7365  w3d.VIEW3D_MT_se
+0034f6a0: 6c65 6374 5f65 6469 745f 6d65 7368 2720  lect_edit_mesh' 
+0034f6b0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034f6c0: 545f 7365 6c65 6374 5f65 6469 745f 6d65  T_select_edit_me
+0034f6d0: 7461 6261 6c6c 3a20 2762 6c5f 7569 2e73  taball: 'bl_ui.s
+0034f6e0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034f6f0: 3344 5f4d 545f 7365 6c65 6374 5f65 6469  3D_MT_select_edi
+0034f700: 745f 6d65 7461 6261 6c6c 2720 3d20 4e6f  t_metaball' = No
+0034f710: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034f720: 6c65 6374 5f65 6469 745f 706f 696e 745f  lect_edit_point_
+0034f730: 636c 6f75 643a 2027 626c 5f75 692e 7370  cloud: 'bl_ui.sp
+0034f740: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034f750: 445f 4d54 5f73 656c 6563 745f 6564 6974  D_MT_select_edit
+0034f760: 5f70 6f69 6e74 5f63 6c6f 7564 2720 3d20  _point_cloud' = 
+0034f770: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
+0034f780: 7365 6c65 6374 5f65 6469 745f 7375 7266  select_edit_surf
+0034f790: 6163 653a 2027 626c 5f75 692e 7370 6163  ace: 'bl_ui.spac
+0034f7a0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034f7b0: 4d54 5f73 656c 6563 745f 6564 6974 5f73  MT_select_edit_s
+0034f7c0: 7572 6661 6365 2720 3d20 4e6f 6e65 0a0a  urface' = None..
+0034f7d0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034f7e0: 5f65 6469 745f 7465 7874 3a20 2762 6c5f  _edit_text: 'bl_
+0034f7f0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034f800: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034f810: 5f65 6469 745f 7465 7874 2720 3d20 4e6f  _edit_text' = No
+0034f820: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034f830: 6c65 6374 5f6f 626a 6563 743a 2027 626c  lect_object: 'bl
 0034f840: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
 0034f850: 2e56 4945 5733 445f 4d54 5f73 656c 6563  .VIEW3D_MT_selec
-0034f860: 745f 7061 696e 745f 6d61 736b 2720 3d20  t_paint_mask' = 
-0034f870: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034f880: 7365 6c65 6374 5f70 6169 6e74 5f6d 6173  select_paint_mas
-0034f890: 6b5f 7665 7274 6578 3a20 2762 6c5f 7569  k_vertex: 'bl_ui
-0034f8a0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034f8b0: 4557 3344 5f4d 545f 7365 6c65 6374 5f70  EW3D_MT_select_p
-0034f8c0: 6169 6e74 5f6d 6173 6b5f 7665 7274 6578  aint_mask_vertex
-0034f8d0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034f8e0: 5f4d 545f 7365 6c65 6374 5f70 6172 7469  _MT_select_parti
-0034f8f0: 636c 653a 2027 626c 5f75 692e 7370 6163  cle: 'bl_ui.spac
-0034f900: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-0034f910: 4d54 5f73 656c 6563 745f 7061 7274 6963  MT_select_partic
-0034f920: 6c65 2720 3d20 4e6f 6e65 0a0a 5649 4557  le' = None..VIEW
-0034f930: 3344 5f4d 545f 7365 6c65 6374 5f70 6f73  3D_MT_select_pos
-0034f940: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-0034f950: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-0034f960: 5f73 656c 6563 745f 706f 7365 2720 3d20  _select_pose' = 
-0034f970: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034f980: 7365 6c65 6374 5f70 6f73 655f 6d6f 7265  select_pose_more
-0034f990: 5f6c 6573 733a 2027 626c 5f75 692e 7370  _less: 'bl_ui.sp
-0034f9a0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034f9b0: 445f 4d54 5f73 656c 6563 745f 706f 7365  D_MT_select_pose
-0034f9c0: 5f6d 6f72 655f 6c65 7373 2720 3d20 4e6f  _more_less' = No
-0034f9d0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
-0034f9e0: 6c65 6374 5f73 6375 6c70 745f 6375 7276  lect_sculpt_curv
-0034f9f0: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
-0034fa00: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
-0034fa10: 545f 7365 6c65 6374 5f73 6375 6c70 745f  T_select_sculpt_
-0034fa20: 6375 7276 6573 2720 3d20 4e6f 6e65 0a0a  curves' = None..
-0034fa30: 5649 4557 3344 5f4d 545f 7368 6164 696e  VIEW3D_MT_shadin
-0034fa40: 675f 6578 5f70 6965 3a20 2762 6c5f 7569  g_ex_pie: 'bl_ui
-0034fa50: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034fa60: 4557 3344 5f4d 545f 7368 6164 696e 675f  EW3D_MT_shading_
-0034fa70: 6578 5f70 6965 2720 3d20 4e6f 6e65 0a0a  ex_pie' = None..
-0034fa80: 5649 4557 3344 5f4d 545f 7368 6164 696e  VIEW3D_MT_shadin
-0034fa90: 675f 7069 653a 2027 626c 5f75 692e 7370  g_pie: 'bl_ui.sp
-0034faa0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034fab0: 445f 4d54 5f73 6861 6469 6e67 5f70 6965  D_MT_shading_pie
-0034fac0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034fad0: 5f4d 545f 736e 6170 3a20 2762 6c5f 7569  _MT_snap: 'bl_ui
-0034fae0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034faf0: 4557 3344 5f4d 545f 736e 6170 2720 3d20  EW3D_MT_snap' = 
-0034fb00: 4e6f 6e65 0a0a 5649 4557 3344 5f4d 545f  None..VIEW3D_MT_
-0034fb10: 736e 6170 5f70 6965 3a20 2762 6c5f 7569  snap_pie: 'bl_ui
-0034fb20: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-0034fb30: 4557 3344 5f4d 545f 736e 6170 5f70 6965  EW3D_MT_snap_pie
-0034fb40: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-0034fb50: 5f4d 545f 7375 7266 6163 655f 6164 643a  _MT_surface_add:
-0034fb60: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fb70: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
-0034fb80: 7572 6661 6365 5f61 6464 2720 3d20 4e6f  urface_add' = No
-0034fb90: 6e65 0a0a 5649 4557 3344 5f4d 545f 746f  ne..VIEW3D_MT_to
-0034fba0: 6f6c 735f 7072 6f6a 6563 7470 6169 6e74  ols_projectpaint
-0034fbb0: 5f63 6c6f 6e65 3a20 2762 6c5f 7569 2e70  _clone: 'bl_ui.p
-0034fbc0: 726f 7065 7274 6965 735f 7061 696e 745f  roperties_paint_
-0034fbd0: 636f 6d6d 6f6e 2e56 4945 5733 445f 4d54  common.VIEW3D_MT
-0034fbe0: 5f74 6f6f 6c73 5f70 726f 6a65 6374 7061  _tools_projectpa
-0034fbf0: 696e 745f 636c 6f6e 6527 203d 204e 6f6e  int_clone' = Non
-0034fc00: 650a 0a56 4945 5733 445f 4d54 5f74 6f6f  e..VIEW3D_MT_too
-0034fc10: 6c73 5f70 726f 6a65 6374 7061 696e 745f  ls_projectpaint_
-0034fc20: 7374 656e 6369 6c3a 2027 626c 5f75 692e  stencil: 'bl_ui.
-0034fc30: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-0034fc40: 6c62 6172 2e56 4945 5733 445f 4d54 5f74  lbar.VIEW3D_MT_t
-0034fc50: 6f6f 6c73 5f70 726f 6a65 6374 7061 696e  ools_projectpain
-0034fc60: 745f 7374 656e 6369 6c27 203d 204e 6f6e  t_stencil' = Non
-0034fc70: 650a 0a56 4945 5733 445f 4d54 5f74 6f6f  e..VIEW3D_MT_too
-0034fc80: 6c73 5f70 726f 6a65 6374 7061 696e 745f  ls_projectpaint_
-0034fc90: 7576 6c61 7965 723a 2027 626c 5f75 692e  uvlayer: 'bl_ui.
-0034fca0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-0034fcb0: 6c62 6172 2e56 4945 5733 445f 4d54 5f74  lbar.VIEW3D_MT_t
-0034fcc0: 6f6f 6c73 5f70 726f 6a65 6374 7061 696e  ools_projectpain
-0034fcd0: 745f 7576 6c61 7965 7227 203d 204e 6f6e  t_uvlayer' = Non
-0034fce0: 650a 0a56 4945 5733 445f 4d54 5f74 7261  e..VIEW3D_MT_tra
-0034fcf0: 6e73 666f 726d 3a20 2762 6c5f 7569 2e73  nsform: 'bl_ui.s
-0034fd00: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-0034fd10: 3344 5f4d 545f 7472 616e 7366 6f72 6d27  3D_MT_transform'
-0034fd20: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034fd30: 4d54 5f74 7261 6e73 666f 726d 5f61 726d  MT_transform_arm
-0034fd40: 6174 7572 653a 2027 626c 5f75 692e 7370  ature: 'bl_ui.sp
-0034fd50: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034fd60: 445f 4d54 5f74 7261 6e73 666f 726d 5f61  D_MT_transform_a
-0034fd70: 726d 6174 7572 6527 203d 204e 6f6e 650a  rmature' = None.
-0034fd80: 0a56 4945 5733 445f 4d54 5f74 7261 6e73  .VIEW3D_MT_trans
-0034fd90: 666f 726d 5f67 697a 6d6f 5f70 6965 3a20  form_gizmo_pie: 
-0034fda0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-0034fdb0: 7733 642e 5649 4557 3344 5f4d 545f 7472  w3d.VIEW3D_MT_tr
-0034fdc0: 616e 7366 6f72 6d5f 6769 7a6d 6f5f 7069  ansform_gizmo_pi
-0034fdd0: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
-0034fde0: 445f 4d54 5f74 7261 6e73 666f 726d 5f6f  D_MT_transform_o
-0034fdf0: 626a 6563 743a 2027 626c 5f75 692e 7370  bject: 'bl_ui.sp
-0034fe00: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034fe10: 445f 4d54 5f74 7261 6e73 666f 726d 5f6f  D_MT_transform_o
-0034fe20: 626a 6563 7427 203d 204e 6f6e 650a 0a56  bject' = None..V
-0034fe30: 4945 5733 445f 4d54 5f75 765f 6d61 703a  IEW3D_MT_uv_map:
-0034fe40: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034fe50: 6577 3364 2e56 4945 5733 445f 4d54 5f75  ew3d.VIEW3D_MT_u
-0034fe60: 765f 6d61 7027 203d 204e 6f6e 650a 0a56  v_map' = None..V
-0034fe70: 4945 5733 445f 4d54 5f76 6572 7465 785f  IEW3D_MT_vertex_
-0034fe80: 6772 6f75 703a 2027 626c 5f75 692e 7370  group: 'bl_ui.sp
-0034fe90: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-0034fea0: 445f 4d54 5f76 6572 7465 785f 6772 6f75  D_MT_vertex_grou
-0034feb0: 7027 203d 204e 6f6e 650a 0a56 4945 5733  p' = None..VIEW3
-0034fec0: 445f 4d54 5f76 6965 773a 2027 626c 5f75  D_MT_view: 'bl_u
-0034fed0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-0034fee0: 4945 5733 445f 4d54 5f76 6965 7727 203d  IEW3D_MT_view' =
-0034fef0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-0034ff00: 5f76 6965 775f 616c 6967 6e3a 2027 626c  _view_align: 'bl
-0034ff10: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-0034ff20: 2e56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
-0034ff30: 616c 6967 6e27 203d 204e 6f6e 650a 0a56  align' = None..V
-0034ff40: 4945 5733 445f 4d54 5f76 6965 775f 616c  IEW3D_MT_view_al
-0034ff50: 6967 6e5f 7365 6c65 6374 6564 3a20 2762  ign_selected: 'b
-0034ff60: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-0034ff70: 642e 5649 4557 3344 5f4d 545f 7669 6577  d.VIEW3D_MT_view
-0034ff80: 5f61 6c69 676e 5f73 656c 6563 7465 6427  _align_selected'
-0034ff90: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
-0034ffa0: 4d54 5f76 6965 775f 6361 6d65 7261 733a  MT_view_cameras:
-0034ffb0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-0034ffc0: 6577 3364 2e56 4945 5733 445f 4d54 5f76  ew3d.VIEW3D_MT_v
-0034ffd0: 6965 775f 6361 6d65 7261 7327 203d 204e  iew_cameras' = N
-0034ffe0: 6f6e 650a 0a56 4945 5733 445f 4d54 5f76  one..VIEW3D_MT_v
-0034fff0: 6965 775f 6c6f 6361 6c3a 2027 626c 5f75  iew_local: 'bl_u
-00350000: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00350010: 4945 5733 445f 4d54 5f76 6965 775f 6c6f  IEW3D_MT_view_lo
-00350020: 6361 6c27 203d 204e 6f6e 650a 0a56 4945  cal' = None..VIE
-00350030: 5733 445f 4d54 5f76 6965 775f 6e61 7669  W3D_MT_view_navi
-00350040: 6761 7469 6f6e 3a20 2762 6c5f 7569 2e73  gation: 'bl_ui.s
-00350050: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00350060: 3344 5f4d 545f 7669 6577 5f6e 6176 6967  3D_MT_view_navig
-00350070: 6174 696f 6e27 203d 204e 6f6e 650a 0a56  ation' = None..V
-00350080: 4945 5733 445f 4d54 5f76 6965 775f 7069  IEW3D_MT_view_pi
-00350090: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-003500a0: 7669 6577 3364 2e56 4945 5733 445f 4d54  view3d.VIEW3D_MT
-003500b0: 5f76 6965 775f 7069 6527 203d 204e 6f6e  _view_pie' = Non
-003500c0: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
-003500d0: 775f 7265 6769 6f6e 733a 2027 626c 5f75  w_regions: 'bl_u
-003500e0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-003500f0: 4945 5733 445f 4d54 5f76 6965 775f 7265  IEW3D_MT_view_re
-00350100: 6769 6f6e 7327 203d 204e 6f6e 650a 0a56  gions' = None..V
-00350110: 4945 5733 445f 4d54 5f76 6965 775f 7669  IEW3D_MT_view_vi
-00350120: 6577 706f 696e 743a 2027 626c 5f75 692e  ewpoint: 'bl_ui.
-00350130: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00350140: 5733 445f 4d54 5f76 6965 775f 7669 6577  W3D_MT_view_view
-00350150: 706f 696e 7427 203d 204e 6f6e 650a 0a56  point' = None..V
-00350160: 4945 5733 445f 4d54 5f76 6f6c 756d 655f  IEW3D_MT_volume_
-00350170: 6164 643a 2027 626c 5f75 692e 7370 6163  add: 'bl_ui.spac
-00350180: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00350190: 4d54 5f76 6f6c 756d 655f 6164 6427 203d  MT_volume_add' =
-003501a0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-003501b0: 5f77 6569 6768 745f 6770 656e 6369 6c3a  _weight_gpencil:
-003501c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003501d0: 6577 3364 2e56 4945 5733 445f 4d54 5f77  ew3d.VIEW3D_MT_w
-003501e0: 6569 6768 745f 6770 656e 6369 6c27 203d  eight_gpencil' =
-003501f0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
-00350200: 5f77 7061 696e 745f 7667 726f 7570 5f6c  _wpaint_vgroup_l
-00350210: 6f63 6b5f 7069 653a 2027 626c 5f75 692e  ock_pie: 'bl_ui.
-00350220: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00350230: 5733 445f 4d54 5f77 7061 696e 745f 7667  W3D_MT_wpaint_vg
-00350240: 726f 7570 5f6c 6f63 6b5f 7069 6527 203d  roup_lock_pie' =
-00350250: 204e 6f6e 650a 0a56 4945 5733 445f 4f54   None..VIEW3D_OT
-00350260: 5f65 6469 745f 6d65 7368 5f65 7874 7275  _edit_mesh_extru
-00350270: 6465 5f69 6e64 6976 6964 7561 6c5f 6d6f  de_individual_mo
-00350280: 7665 3a20 2762 6c5f 6f70 6572 6174 6f72  ve: 'bl_operator
-00350290: 732e 7669 6577 3364 2e56 4945 5733 445f  s.view3d.VIEW3D_
-003502a0: 4f54 5f65 6469 745f 6d65 7368 5f65 7874  OT_edit_mesh_ext
-003502b0: 7275 6465 5f69 6e64 6976 6964 7561 6c5f  rude_individual_
-003502c0: 6d6f 7665 2720 3d20 4e6f 6e65 0a0a 5649  move' = None..VI
-003502d0: 4557 3344 5f4f 545f 6564 6974 5f6d 6573  EW3D_OT_edit_mes
-003502e0: 685f 6578 7472 7564 655f 6d61 6e69 666f  h_extrude_manifo
-003502f0: 6c64 5f6e 6f72 6d61 6c3a 2027 626c 5f6f  ld_normal: 'bl_o
-00350300: 7065 7261 746f 7273 2e76 6965 7733 642e  perators.view3d.
-00350310: 5649 4557 3344 5f4f 545f 6564 6974 5f6d  VIEW3D_OT_edit_m
-00350320: 6573 685f 6578 7472 7564 655f 6d61 6e69  esh_extrude_mani
-00350330: 666f 6c64 5f6e 6f72 6d61 6c27 203d 204e  fold_normal' = N
-00350340: 6f6e 650a 0a56 4945 5733 445f 4f54 5f74  one..VIEW3D_OT_t
-00350350: 7261 6e73 666f 726d 5f67 697a 6d6f 5f73  ransform_gizmo_s
-00350360: 6574 3a20 2762 6c5f 6f70 6572 6174 6f72  et: 'bl_operator
-00350370: 732e 7669 6577 3364 2e56 4945 5733 445f  s.view3d.VIEW3D_
-00350380: 4f54 5f74 7261 6e73 666f 726d 5f67 697a  OT_transform_giz
-00350390: 6d6f 5f73 6574 2720 3d20 4e6f 6e65 0a0a  mo_set' = None..
-003503a0: 5649 4557 3344 5f50 545f 6163 7469 7665  VIEW3D_PT_active
-003503b0: 5f74 6f6f 6c3a 2027 626c 5f75 692e 7370  _tool: 'bl_ui.sp
-003503c0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003503d0: 445f 5054 5f61 6374 6976 655f 746f 6f6c  D_PT_active_tool
-003503e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003503f0: 5f50 545f 6163 7469 7665 5f74 6f6f 6c5f  _PT_active_tool_
-00350400: 6475 706c 6963 6174 653a 2027 626c 5f75  duplicate: 'bl_u
-00350410: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00350420: 4945 5733 445f 5054 5f61 6374 6976 655f  IEW3D_PT_active_
-00350430: 746f 6f6c 5f64 7570 6c69 6361 7465 2720  tool_duplicate' 
-00350440: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350450: 545f 616e 6e6f 7461 7469 6f6e 5f6f 6e69  T_annotation_oni
-00350460: 6f6e 3a20 2762 6c5f 7569 2e73 7061 6365  on: 'bl_ui.space
-00350470: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00350480: 545f 616e 6e6f 7461 7469 6f6e 5f6f 6e69  T_annotation_oni
-00350490: 6f6e 2720 3d20 4e6f 6e65 0a0a 5649 4557  on' = None..VIEW
-003504a0: 3344 5f50 545f 636f 6c6c 6563 7469 6f6e  3D_PT_collection
-003504b0: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-003504c0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-003504d0: 5f63 6f6c 6c65 6374 696f 6e73 2720 3d20  _collections' = 
-003504e0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003504f0: 636f 6e74 6578 745f 7072 6f70 6572 7469  context_properti
-00350500: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
-00350510: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00350520: 545f 636f 6e74 6578 745f 7072 6f70 6572  T_context_proper
-00350530: 7469 6573 2720 3d20 4e6f 6e65 0a0a 5649  ties' = None..VI
-00350540: 4557 3344 5f50 545f 6375 7276 6573 5f73  EW3D_PT_curves_s
-00350550: 6375 6c70 745f 6164 645f 7368 6170 653a  culpt_add_shape:
-00350560: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350570: 6577 3364 2e56 4945 5733 445f 5054 5f63  ew3d.VIEW3D_PT_c
-00350580: 7572 7665 735f 7363 756c 7074 5f61 6464  urves_sculpt_add
-00350590: 5f73 6861 7065 2720 3d20 4e6f 6e65 0a0a  _shape' = None..
-003505a0: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
-003505b0: 5f73 6375 6c70 745f 6772 6f77 5f73 6872  _sculpt_grow_shr
-003505c0: 696e 6b5f 7363 616c 696e 673a 2027 626c  ink_scaling: 'bl
-003505d0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-003505e0: 2e56 4945 5733 445f 5054 5f63 7572 7665  .VIEW3D_PT_curve
-003505f0: 735f 7363 756c 7074 5f67 726f 775f 7368  s_sculpt_grow_sh
-00350600: 7269 6e6b 5f73 6361 6c69 6e67 2720 3d20  rink_scaling' = 
-00350610: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350620: 6375 7276 6573 5f73 6375 6c70 745f 7061  curves_sculpt_pa
-00350630: 7261 6d65 7465 725f 6661 6c6c 6f66 663a  rameter_falloff:
-00350640: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350650: 6577 3364 2e56 4945 5733 445f 5054 5f63  ew3d.VIEW3D_PT_c
-00350660: 7572 7665 735f 7363 756c 7074 5f70 6172  urves_sculpt_par
-00350670: 616d 6574 6572 5f66 616c 6c6f 6666 2720  ameter_falloff' 
-00350680: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350690: 545f 6375 7276 6573 5f73 6375 6c70 745f  T_curves_sculpt_
-003506a0: 7379 6d6d 6574 7279 3a20 2762 6c5f 7569  symmetry: 'bl_ui
-003506b0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003506c0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003506d0: 6375 7276 6573 5f73 6375 6c70 745f 7379  curves_sculpt_sy
-003506e0: 6d6d 6574 7279 2720 3d20 4e6f 6e65 0a0a  mmetry' = None..
-003506f0: 5649 4557 3344 5f50 545f 6375 7276 6573  VIEW3D_PT_curves
-00350700: 5f73 6375 6c70 745f 7379 6d6d 6574 7279  _sculpt_symmetry
-00350710: 5f66 6f72 5f74 6f70 6261 723a 2027 626c  _for_topbar: 'bl
-00350720: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350730: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350740: 5054 5f63 7572 7665 735f 7363 756c 7074  PT_curves_sculpt
-00350750: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
-00350760: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
-00350770: 4557 3344 5f50 545f 6769 7a6d 6f5f 6469  EW3D_PT_gizmo_di
-00350780: 7370 6c61 793a 2027 626c 5f75 692e 7370  splay: 'bl_ui.sp
-00350790: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003507a0: 445f 5054 5f67 697a 6d6f 5f64 6973 706c  D_PT_gizmo_displ
-003507b0: 6179 2720 3d20 4e6f 6e65 0a0a 5649 4557  ay' = None..VIEW
-003507c0: 3344 5f50 545f 6770 656e 6369 6c5f 6272  3D_PT_gpencil_br
-003507d0: 7573 685f 7072 6573 6574 733a 2027 626c  ush_presets: 'bl
-003507e0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-003507f0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00350800: 5054 5f67 7065 6e63 696c 5f62 7275 7368  PT_gpencil_brush
-00350810: 5f70 7265 7365 7473 2720 3d20 4e6f 6e65  _presets' = None
-00350820: 0a0a 5649 4557 3344 5f50 545f 6770 656e  ..VIEW3D_PT_gpen
-00350830: 6369 6c5f 6375 7276 655f 6564 6974 3a20  cil_curve_edit: 
-00350840: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00350850: 7733 642e 5649 4557 3344 5f50 545f 6770  w3d.VIEW3D_PT_gp
-00350860: 656e 6369 6c5f 6375 7276 655f 6564 6974  encil_curve_edit
-00350870: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350880: 5f50 545f 6770 656e 6369 6c5f 6472 6177  _PT_gpencil_draw
-00350890: 5f63 6f6e 7465 7874 5f6d 656e 753a 2027  _context_menu: '
-003508a0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-003508b0: 3364 2e56 4945 5733 445f 5054 5f67 7065  3d.VIEW3D_PT_gpe
-003508c0: 6e63 696c 5f64 7261 775f 636f 6e74 6578  ncil_draw_contex
-003508d0: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
-003508e0: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
-003508f0: 6c5f 6775 6964 653a 2027 626c 5f75 692e  l_guide: 'bl_ui.
-00350900: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00350910: 5733 445f 5054 5f67 7065 6e63 696c 5f67  W3D_PT_gpencil_g
-00350920: 7569 6465 2720 3d20 4e6f 6e65 0a0a 5649  uide' = None..VI
+0034f860: 745f 6f62 6a65 6374 2720 3d20 4e6f 6e65  t_object' = None
+0034f870: 0a0a 5649 4557 3344 5f4d 545f 7365 6c65  ..VIEW3D_MT_sele
+0034f880: 6374 5f6f 626a 6563 745f 6d6f 7265 5f6c  ct_object_more_l
+0034f890: 6573 733a 2027 626c 5f75 692e 7370 6163  ess: 'bl_ui.spac
+0034f8a0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034f8b0: 4d54 5f73 656c 6563 745f 6f62 6a65 6374  MT_select_object
+0034f8c0: 5f6d 6f72 655f 6c65 7373 2720 3d20 4e6f  _more_less' = No
+0034f8d0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7365  ne..VIEW3D_MT_se
+0034f8e0: 6c65 6374 5f70 6169 6e74 5f6d 6173 6b3a  lect_paint_mask:
+0034f8f0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034f900: 6577 3364 2e56 4945 5733 445f 4d54 5f73  ew3d.VIEW3D_MT_s
+0034f910: 656c 6563 745f 7061 696e 745f 6d61 736b  elect_paint_mask
+0034f920: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034f930: 5f4d 545f 7365 6c65 6374 5f70 6169 6e74  _MT_select_paint
+0034f940: 5f6d 6173 6b5f 7665 7274 6578 3a20 2762  _mask_vertex: 'b
+0034f950: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034f960: 642e 5649 4557 3344 5f4d 545f 7365 6c65  d.VIEW3D_MT_sele
+0034f970: 6374 5f70 6169 6e74 5f6d 6173 6b5f 7665  ct_paint_mask_ve
+0034f980: 7274 6578 2720 3d20 4e6f 6e65 0a0a 5649  rtex' = None..VI
+0034f990: 4557 3344 5f4d 545f 7365 6c65 6374 5f70  EW3D_MT_select_p
+0034f9a0: 6172 7469 636c 653a 2027 626c 5f75 692e  article: 'bl_ui.
+0034f9b0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+0034f9c0: 5733 445f 4d54 5f73 656c 6563 745f 7061  W3D_MT_select_pa
+0034f9d0: 7274 6963 6c65 2720 3d20 4e6f 6e65 0a0a  rticle' = None..
+0034f9e0: 5649 4557 3344 5f4d 545f 7365 6c65 6374  VIEW3D_MT_select
+0034f9f0: 5f70 6f73 653a 2027 626c 5f75 692e 7370  _pose: 'bl_ui.sp
+0034fa00: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+0034fa10: 445f 4d54 5f73 656c 6563 745f 706f 7365  D_MT_select_pose
+0034fa20: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034fa30: 5f4d 545f 7365 6c65 6374 5f70 6f73 655f  _MT_select_pose_
+0034fa40: 6d6f 7265 5f6c 6573 733a 2027 626c 5f75  more_less: 'bl_u
+0034fa50: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fa60: 4945 5733 445f 4d54 5f73 656c 6563 745f  IEW3D_MT_select_
+0034fa70: 706f 7365 5f6d 6f72 655f 6c65 7373 2720  pose_more_less' 
+0034fa80: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034fa90: 545f 7365 6c65 6374 5f73 6375 6c70 745f  T_select_sculpt_
+0034faa0: 6375 7276 6573 3a20 2762 6c5f 7569 2e73  curves: 'bl_ui.s
+0034fab0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+0034fac0: 3344 5f4d 545f 7365 6c65 6374 5f73 6375  3D_MT_select_scu
+0034fad0: 6c70 745f 6375 7276 6573 2720 3d20 4e6f  lpt_curves' = No
+0034fae0: 6e65 0a0a 5649 4557 3344 5f4d 545f 7368  ne..VIEW3D_MT_sh
+0034faf0: 6164 696e 675f 6578 5f70 6965 3a20 2762  ading_ex_pie: 'b
+0034fb00: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fb10: 642e 5649 4557 3344 5f4d 545f 7368 6164  d.VIEW3D_MT_shad
+0034fb20: 696e 675f 6578 5f70 6965 2720 3d20 4e6f  ing_ex_pie' = No
+0034fb30: 6e65 0a0a 5649 4557 3344 5f4d 545f 7368  ne..VIEW3D_MT_sh
+0034fb40: 6164 696e 675f 7069 653a 2027 626c 5f75  ading_pie: 'bl_u
+0034fb50: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fb60: 4945 5733 445f 4d54 5f73 6861 6469 6e67  IEW3D_MT_shading
+0034fb70: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
+0034fb80: 4557 3344 5f4d 545f 736e 6170 3a20 2762  EW3D_MT_snap: 'b
+0034fb90: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fba0: 642e 5649 4557 3344 5f4d 545f 736e 6170  d.VIEW3D_MT_snap
+0034fbb0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+0034fbc0: 5f4d 545f 736e 6170 5f70 6965 3a20 2762  _MT_snap_pie: 'b
+0034fbd0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+0034fbe0: 642e 5649 4557 3344 5f4d 545f 736e 6170  d.VIEW3D_MT_snap
+0034fbf0: 5f70 6965 2720 3d20 4e6f 6e65 0a0a 5649  _pie' = None..VI
+0034fc00: 4557 3344 5f4d 545f 7375 7266 6163 655f  EW3D_MT_surface_
+0034fc10: 6164 643a 2027 626c 5f75 692e 7370 6163  add: 'bl_ui.spac
+0034fc20: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034fc30: 4d54 5f73 7572 6661 6365 5f61 6464 2720  MT_surface_add' 
+0034fc40: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f4d  = None..VIEW3D_M
+0034fc50: 545f 746f 6f6c 735f 7072 6f6a 6563 7470  T_tools_projectp
+0034fc60: 6169 6e74 5f63 6c6f 6e65 3a20 2762 6c5f  aint_clone: 'bl_
+0034fc70: 7569 2e70 726f 7065 7274 6965 735f 7061  ui.properties_pa
+0034fc80: 696e 745f 636f 6d6d 6f6e 2e56 4945 5733  int_common.VIEW3
+0034fc90: 445f 4d54 5f74 6f6f 6c73 5f70 726f 6a65  D_MT_tools_proje
+0034fca0: 6374 7061 696e 745f 636c 6f6e 6527 203d  ctpaint_clone' =
+0034fcb0: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034fcc0: 5f74 6f6f 6c73 5f70 726f 6a65 6374 7061  _tools_projectpa
+0034fcd0: 696e 745f 7374 656e 6369 6c3a 2027 626c  int_stencil: 'bl
+0034fce0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034fcf0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+0034fd00: 4d54 5f74 6f6f 6c73 5f70 726f 6a65 6374  MT_tools_project
+0034fd10: 7061 696e 745f 7374 656e 6369 6c27 203d  paint_stencil' =
+0034fd20: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034fd30: 5f74 6f6f 6c73 5f70 726f 6a65 6374 7061  _tools_projectpa
+0034fd40: 696e 745f 7576 6c61 7965 723a 2027 626c  int_uvlayer: 'bl
+0034fd50: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+0034fd60: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+0034fd70: 4d54 5f74 6f6f 6c73 5f70 726f 6a65 6374  MT_tools_project
+0034fd80: 7061 696e 745f 7576 6c61 7965 7227 203d  paint_uvlayer' =
+0034fd90: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+0034fda0: 5f74 7261 6e73 666f 726d 3a20 2762 6c5f  _transform: 'bl_
+0034fdb0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+0034fdc0: 5649 4557 3344 5f4d 545f 7472 616e 7366  VIEW3D_MT_transf
+0034fdd0: 6f72 6d27 203d 204e 6f6e 650a 0a56 4945  orm' = None..VIE
+0034fde0: 5733 445f 4d54 5f74 7261 6e73 666f 726d  W3D_MT_transform
+0034fdf0: 5f61 726d 6174 7572 653a 2027 626c 5f75  _armature: 'bl_u
+0034fe00: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fe10: 4945 5733 445f 4d54 5f74 7261 6e73 666f  IEW3D_MT_transfo
+0034fe20: 726d 5f61 726d 6174 7572 6527 203d 204e  rm_armature' = N
+0034fe30: 6f6e 650a 0a56 4945 5733 445f 4d54 5f74  one..VIEW3D_MT_t
+0034fe40: 7261 6e73 666f 726d 5f67 697a 6d6f 5f70  ransform_gizmo_p
+0034fe50: 6965 3a20 2762 6c5f 7569 2e73 7061 6365  ie: 'bl_ui.space
+0034fe60: 5f76 6965 7733 642e 5649 4557 3344 5f4d  _view3d.VIEW3D_M
+0034fe70: 545f 7472 616e 7366 6f72 6d5f 6769 7a6d  T_transform_gizm
+0034fe80: 6f5f 7069 6527 203d 204e 6f6e 650a 0a56  o_pie' = None..V
+0034fe90: 4945 5733 445f 4d54 5f74 7261 6e73 666f  IEW3D_MT_transfo
+0034fea0: 726d 5f6f 626a 6563 743a 2027 626c 5f75  rm_object: 'bl_u
+0034feb0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034fec0: 4945 5733 445f 4d54 5f74 7261 6e73 666f  IEW3D_MT_transfo
+0034fed0: 726d 5f6f 626a 6563 7427 203d 204e 6f6e  rm_object' = Non
+0034fee0: 650a 0a56 4945 5733 445f 4d54 5f75 765f  e..VIEW3D_MT_uv_
+0034fef0: 6d61 703a 2027 626c 5f75 692e 7370 6163  map: 'bl_ui.spac
+0034ff00: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+0034ff10: 4d54 5f75 765f 6d61 7027 203d 204e 6f6e  MT_uv_map' = Non
+0034ff20: 650a 0a56 4945 5733 445f 4d54 5f76 6572  e..VIEW3D_MT_ver
+0034ff30: 7465 785f 6772 6f75 703a 2027 626c 5f75  tex_group: 'bl_u
+0034ff40: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+0034ff50: 4945 5733 445f 4d54 5f76 6572 7465 785f  IEW3D_MT_vertex_
+0034ff60: 6772 6f75 7027 203d 204e 6f6e 650a 0a56  group' = None..V
+0034ff70: 4945 5733 445f 4d54 5f76 6965 773a 2027  IEW3D_MT_view: '
+0034ff80: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+0034ff90: 3364 2e56 4945 5733 445f 4d54 5f76 6965  3d.VIEW3D_MT_vie
+0034ffa0: 7727 203d 204e 6f6e 650a 0a56 4945 5733  w' = None..VIEW3
+0034ffb0: 445f 4d54 5f76 6965 775f 616c 6967 6e3a  D_MT_view_align:
+0034ffc0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+0034ffd0: 6577 3364 2e56 4945 5733 445f 4d54 5f76  ew3d.VIEW3D_MT_v
+0034ffe0: 6965 775f 616c 6967 6e27 203d 204e 6f6e  iew_align' = Non
+0034fff0: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
+00350000: 775f 616c 6967 6e5f 7365 6c65 6374 6564  w_align_selected
+00350010: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350020: 6965 7733 642e 5649 4557 3344 5f4d 545f  iew3d.VIEW3D_MT_
+00350030: 7669 6577 5f61 6c69 676e 5f73 656c 6563  view_align_selec
+00350040: 7465 6427 203d 204e 6f6e 650a 0a56 4945  ted' = None..VIE
+00350050: 5733 445f 4d54 5f76 6965 775f 6361 6d65  W3D_MT_view_came
+00350060: 7261 733a 2027 626c 5f75 692e 7370 6163  ras: 'bl_ui.spac
+00350070: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350080: 4d54 5f76 6965 775f 6361 6d65 7261 7327  MT_view_cameras'
+00350090: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+003500a0: 4d54 5f76 6965 775f 6c6f 6361 6c3a 2027  MT_view_local: '
+003500b0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003500c0: 3364 2e56 4945 5733 445f 4d54 5f76 6965  3d.VIEW3D_MT_vie
+003500d0: 775f 6c6f 6361 6c27 203d 204e 6f6e 650a  w_local' = None.
+003500e0: 0a56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
+003500f0: 6e61 7669 6761 7469 6f6e 3a20 2762 6c5f  navigation: 'bl_
+00350100: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00350110: 5649 4557 3344 5f4d 545f 7669 6577 5f6e  VIEW3D_MT_view_n
+00350120: 6176 6967 6174 696f 6e27 203d 204e 6f6e  avigation' = Non
+00350130: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
+00350140: 775f 7069 653a 2027 626c 5f75 692e 7370  w_pie: 'bl_ui.sp
+00350150: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350160: 445f 4d54 5f76 6965 775f 7069 6527 203d  D_MT_view_pie' =
+00350170: 204e 6f6e 650a 0a56 4945 5733 445f 4d54   None..VIEW3D_MT
+00350180: 5f76 6965 775f 7265 6769 6f6e 733a 2027  _view_regions: '
+00350190: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003501a0: 3364 2e56 4945 5733 445f 4d54 5f76 6965  3d.VIEW3D_MT_vie
+003501b0: 775f 7265 6769 6f6e 7327 203d 204e 6f6e  w_regions' = Non
+003501c0: 650a 0a56 4945 5733 445f 4d54 5f76 6965  e..VIEW3D_MT_vie
+003501d0: 775f 7669 6577 706f 696e 743a 2027 626c  w_viewpoint: 'bl
+003501e0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+003501f0: 2e56 4945 5733 445f 4d54 5f76 6965 775f  .VIEW3D_MT_view_
+00350200: 7669 6577 706f 696e 7427 203d 204e 6f6e  viewpoint' = Non
+00350210: 650a 0a56 4945 5733 445f 4d54 5f76 6f6c  e..VIEW3D_MT_vol
+00350220: 756d 655f 6164 643a 2027 626c 5f75 692e  ume_add: 'bl_ui.
+00350230: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+00350240: 5733 445f 4d54 5f76 6f6c 756d 655f 6164  W3D_MT_volume_ad
+00350250: 6427 203d 204e 6f6e 650a 0a56 4945 5733  d' = None..VIEW3
+00350260: 445f 4d54 5f77 6569 6768 745f 6770 656e  D_MT_weight_gpen
+00350270: 6369 6c3a 2027 626c 5f75 692e 7370 6163  cil: 'bl_ui.spac
+00350280: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350290: 4d54 5f77 6569 6768 745f 6770 656e 6369  MT_weight_gpenci
+003502a0: 6c27 203d 204e 6f6e 650a 0a56 4945 5733  l' = None..VIEW3
+003502b0: 445f 4d54 5f77 7061 696e 745f 7667 726f  D_MT_wpaint_vgro
+003502c0: 7570 5f6c 6f63 6b5f 7069 653a 2027 626c  up_lock_pie: 'bl
+003502d0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+003502e0: 2e56 4945 5733 445f 4d54 5f77 7061 696e  .VIEW3D_MT_wpain
+003502f0: 745f 7667 726f 7570 5f6c 6f63 6b5f 7069  t_vgroup_lock_pi
+00350300: 6527 203d 204e 6f6e 650a 0a56 4945 5733  e' = None..VIEW3
+00350310: 445f 4f54 5f65 6469 745f 6d65 7368 5f65  D_OT_edit_mesh_e
+00350320: 7874 7275 6465 5f69 6e64 6976 6964 7561  xtrude_individua
+00350330: 6c5f 6d6f 7665 3a20 2762 6c5f 6f70 6572  l_move: 'bl_oper
+00350340: 6174 6f72 732e 7669 6577 3364 2e56 4945  ators.view3d.VIE
+00350350: 5733 445f 4f54 5f65 6469 745f 6d65 7368  W3D_OT_edit_mesh
+00350360: 5f65 7874 7275 6465 5f69 6e64 6976 6964  _extrude_individ
+00350370: 7561 6c5f 6d6f 7665 2720 3d20 4e6f 6e65  ual_move' = None
+00350380: 0a0a 5649 4557 3344 5f4f 545f 6564 6974  ..VIEW3D_OT_edit
+00350390: 5f6d 6573 685f 6578 7472 7564 655f 6d61  _mesh_extrude_ma
+003503a0: 6e69 666f 6c64 5f6e 6f72 6d61 6c3a 2027  nifold_normal: '
+003503b0: 626c 5f6f 7065 7261 746f 7273 2e76 6965  bl_operators.vie
+003503c0: 7733 642e 5649 4557 3344 5f4f 545f 6564  w3d.VIEW3D_OT_ed
+003503d0: 6974 5f6d 6573 685f 6578 7472 7564 655f  it_mesh_extrude_
+003503e0: 6d61 6e69 666f 6c64 5f6e 6f72 6d61 6c27  manifold_normal'
+003503f0: 203d 204e 6f6e 650a 0a56 4945 5733 445f   = None..VIEW3D_
+00350400: 4f54 5f74 7261 6e73 666f 726d 5f67 697a  OT_transform_giz
+00350410: 6d6f 5f73 6574 3a20 2762 6c5f 6f70 6572  mo_set: 'bl_oper
+00350420: 6174 6f72 732e 7669 6577 3364 2e56 4945  ators.view3d.VIE
+00350430: 5733 445f 4f54 5f74 7261 6e73 666f 726d  W3D_OT_transform
+00350440: 5f67 697a 6d6f 5f73 6574 2720 3d20 4e6f  _gizmo_set' = No
+00350450: 6e65 0a0a 5649 4557 3344 5f50 545f 6163  ne..VIEW3D_PT_ac
+00350460: 7469 7665 5f74 6f6f 6c3a 2027 626c 5f75  tive_tool: 'bl_u
+00350470: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350480: 4945 5733 445f 5054 5f61 6374 6976 655f  IEW3D_PT_active_
+00350490: 746f 6f6c 2720 3d20 4e6f 6e65 0a0a 5649  tool' = None..VI
+003504a0: 4557 3344 5f50 545f 6163 7469 7665 5f74  EW3D_PT_active_t
+003504b0: 6f6f 6c5f 6475 706c 6963 6174 653a 2027  ool_duplicate: '
+003504c0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003504d0: 3364 2e56 4945 5733 445f 5054 5f61 6374  3d.VIEW3D_PT_act
+003504e0: 6976 655f 746f 6f6c 5f64 7570 6c69 6361  ive_tool_duplica
+003504f0: 7465 2720 3d20 4e6f 6e65 0a0a 5649 4557  te' = None..VIEW
+00350500: 3344 5f50 545f 616e 6e6f 7461 7469 6f6e  3D_PT_annotation
+00350510: 5f6f 6e69 6f6e 3a20 2762 6c5f 7569 2e73  _onion: 'bl_ui.s
+00350520: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+00350530: 3344 5f50 545f 616e 6e6f 7461 7469 6f6e  3D_PT_annotation
+00350540: 5f6f 6e69 6f6e 2720 3d20 4e6f 6e65 0a0a  _onion' = None..
+00350550: 5649 4557 3344 5f50 545f 636f 6c6c 6563  VIEW3D_PT_collec
+00350560: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
+00350570: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350580: 445f 5054 5f63 6f6c 6c65 6374 696f 6e73  D_PT_collections
+00350590: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003505a0: 5f50 545f 636f 6e74 6578 745f 7072 6f70  _PT_context_prop
+003505b0: 6572 7469 6573 3a20 2762 6c5f 7569 2e73  erties: 'bl_ui.s
+003505c0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+003505d0: 3344 5f50 545f 636f 6e74 6578 745f 7072  3D_PT_context_pr
+003505e0: 6f70 6572 7469 6573 2720 3d20 4e6f 6e65  operties' = None
+003505f0: 0a0a 5649 4557 3344 5f50 545f 6375 7276  ..VIEW3D_PT_curv
+00350600: 6573 5f73 6375 6c70 745f 6164 645f 7368  es_sculpt_add_sh
+00350610: 6170 653a 2027 626c 5f75 692e 7370 6163  ape: 'bl_ui.spac
+00350620: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350630: 5054 5f63 7572 7665 735f 7363 756c 7074  PT_curves_sculpt
+00350640: 5f61 6464 5f73 6861 7065 2720 3d20 4e6f  _add_shape' = No
+00350650: 6e65 0a0a 5649 4557 3344 5f50 545f 6375  ne..VIEW3D_PT_cu
+00350660: 7276 6573 5f73 6375 6c70 745f 6772 6f77  rves_sculpt_grow
+00350670: 5f73 6872 696e 6b5f 7363 616c 696e 673a  _shrink_scaling:
+00350680: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350690: 6577 3364 2e56 4945 5733 445f 5054 5f63  ew3d.VIEW3D_PT_c
+003506a0: 7572 7665 735f 7363 756c 7074 5f67 726f  urves_sculpt_gro
+003506b0: 775f 7368 7269 6e6b 5f73 6361 6c69 6e67  w_shrink_scaling
+003506c0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003506d0: 5f50 545f 6375 7276 6573 5f73 6375 6c70  _PT_curves_sculp
+003506e0: 745f 7061 7261 6d65 7465 725f 6661 6c6c  t_parameter_fall
+003506f0: 6f66 663a 2027 626c 5f75 692e 7370 6163  off: 'bl_ui.spac
+00350700: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350710: 5054 5f63 7572 7665 735f 7363 756c 7074  PT_curves_sculpt
+00350720: 5f70 6172 616d 6574 6572 5f66 616c 6c6f  _parameter_fallo
+00350730: 6666 2720 3d20 4e6f 6e65 0a0a 5649 4557  ff' = None..VIEW
+00350740: 3344 5f50 545f 6375 7276 6573 5f73 6375  3D_PT_curves_scu
+00350750: 6c70 745f 7379 6d6d 6574 7279 3a20 2762  lpt_symmetry: 'b
+00350760: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350770: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00350780: 5f50 545f 6375 7276 6573 5f73 6375 6c70  _PT_curves_sculp
+00350790: 745f 7379 6d6d 6574 7279 2720 3d20 4e6f  t_symmetry' = No
+003507a0: 6e65 0a0a 5649 4557 3344 5f50 545f 6375  ne..VIEW3D_PT_cu
+003507b0: 7276 6573 5f73 6375 6c70 745f 7379 6d6d  rves_sculpt_symm
+003507c0: 6574 7279 5f66 6f72 5f74 6f70 6261 723a  etry_for_topbar:
+003507d0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003507e0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+003507f0: 5733 445f 5054 5f63 7572 7665 735f 7363  W3D_PT_curves_sc
+00350800: 756c 7074 5f73 796d 6d65 7472 795f 666f  ulpt_symmetry_fo
+00350810: 725f 746f 7062 6172 2720 3d20 4e6f 6e65  r_topbar' = None
+00350820: 0a0a 5649 4557 3344 5f50 545f 6769 7a6d  ..VIEW3D_PT_gizm
+00350830: 6f5f 6469 7370 6c61 793a 2027 626c 5f75  o_display: 'bl_u
+00350840: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350850: 4945 5733 445f 5054 5f67 697a 6d6f 5f64  IEW3D_PT_gizmo_d
+00350860: 6973 706c 6179 2720 3d20 4e6f 6e65 0a0a  isplay' = None..
+00350870: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
+00350880: 6c5f 6272 7573 685f 7072 6573 6574 733a  l_brush_presets:
+00350890: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003508a0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+003508b0: 5733 445f 5054 5f67 7065 6e63 696c 5f62  W3D_PT_gpencil_b
+003508c0: 7275 7368 5f70 7265 7365 7473 2720 3d20  rush_presets' = 
+003508d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003508e0: 6770 656e 6369 6c5f 6375 7276 655f 6564  gpencil_curve_ed
+003508f0: 6974 3a20 2762 6c5f 7569 2e73 7061 6365  it: 'bl_ui.space
+00350900: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00350910: 545f 6770 656e 6369 6c5f 6375 7276 655f  T_gpencil_curve_
+00350920: 6564 6974 2720 3d20 4e6f 6e65 0a0a 5649  edit' = None..VI
 00350930: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-00350940: 6c6f 636b 3a20 2762 6c5f 7569 2e73 7061  lock: 'bl_ui.spa
-00350950: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-00350960: 5f50 545f 6770 656e 6369 6c5f 6c6f 636b  _PT_gpencil_lock
-00350970: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350980: 5f50 545f 6770 656e 6369 6c5f 6d75 6c74  _PT_gpencil_mult
-00350990: 695f 6672 616d 653a 2027 626c 5f75 692e  i_frame: 'bl_ui.
-003509a0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-003509b0: 5733 445f 5054 5f67 7065 6e63 696c 5f6d  W3D_PT_gpencil_m
-003509c0: 756c 7469 5f66 7261 6d65 2720 3d20 4e6f  ulti_frame' = No
-003509d0: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
-003509e0: 656e 6369 6c5f 6f72 6967 696e 3a20 2762  encil_origin: 'b
-003509f0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350a00: 642e 5649 4557 3344 5f50 545f 6770 656e  d.VIEW3D_PT_gpen
-00350a10: 6369 6c5f 6f72 6967 696e 2720 3d20 4e6f  cil_origin' = No
-00350a20: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
-00350a30: 656e 6369 6c5f 7363 756c 7074 5f61 7574  encil_sculpt_aut
-00350a40: 6f6d 6173 6b69 6e67 3a20 2762 6c5f 7569  omasking: 'bl_ui
-00350a50: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350a60: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
-00350a70: 7363 756c 7074 5f61 7574 6f6d 6173 6b69  sculpt_automaski
-00350a80: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
-00350a90: 3344 5f50 545f 6770 656e 6369 6c5f 7363  3D_PT_gpencil_sc
-00350aa0: 756c 7074 5f63 6f6e 7465 7874 5f6d 656e  ulpt_context_men
-00350ab0: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
-00350ac0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00350ad0: 5f67 7065 6e63 696c 5f73 6375 6c70 745f  _gpencil_sculpt_
-00350ae0: 636f 6e74 6578 745f 6d65 6e75 2720 3d20  context_menu' = 
-00350af0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00350b00: 6770 656e 6369 6c5f 7665 7274 6578 5f63  gpencil_vertex_c
-00350b10: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
-00350b20: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350b30: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
-00350b40: 696c 5f76 6572 7465 785f 636f 6e74 6578  il_vertex_contex
-00350b50: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
-00350b60: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
-00350b70: 6c5f 7765 6967 6874 5f63 6f6e 7465 7874  l_weight_context
-00350b80: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
-00350b90: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00350ba0: 445f 5054 5f67 7065 6e63 696c 5f77 6569  D_PT_gpencil_wei
-00350bb0: 6768 745f 636f 6e74 6578 745f 6d65 6e75  ght_context_menu
-00350bc0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350bd0: 5f50 545f 6772 6561 7365 5f70 656e 6369  _PT_grease_penci
-00350be0: 6c3a 2027 626c 5f75 692e 7370 6163 655f  l: 'bl_ui.space_
-00350bf0: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00350c00: 5f67 7265 6173 655f 7065 6e63 696c 2720  _grease_pencil' 
-00350c10: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350c20: 545f 6d61 736b 3a20 2762 6c5f 7569 2e73  T_mask: 'bl_ui.s
-00350c30: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00350c40: 6261 722e 5649 4557 3344 5f50 545f 6d61  bar.VIEW3D_PT_ma
-00350c50: 736b 2720 3d20 4e6f 6e65 0a0a 5649 4557  sk' = None..VIEW
-00350c60: 3344 5f50 545f 6f62 6a65 6374 5f74 7970  3D_PT_object_typ
-00350c70: 655f 7669 7369 6269 6c69 7479 3a20 2762  e_visibility: 'b
-00350c80: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00350c90: 642e 5649 4557 3344 5f50 545f 6f62 6a65  d.VIEW3D_PT_obje
-00350ca0: 6374 5f74 7970 655f 7669 7369 6269 6c69  ct_type_visibili
-00350cb0: 7479 2720 3d20 4e6f 6e65 0a0a 5649 4557  ty' = None..VIEW
-00350cc0: 3344 5f50 545f 6f76 6572 6c61 793a 2027  3D_PT_overlay: '
-00350cd0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00350ce0: 3364 2e56 4945 5733 445f 5054 5f6f 7665  3d.VIEW3D_PT_ove
-00350cf0: 726c 6179 2720 3d20 4e6f 6e65 0a0a 5649  rlay' = None..VI
-00350d00: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-00350d10: 626f 6e65 733a 2027 626c 5f75 692e 7370  bones: 'bl_ui.sp
-00350d20: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00350d30: 445f 5054 5f6f 7665 726c 6179 5f62 6f6e  D_PT_overlay_bon
-00350d40: 6573 2720 3d20 4e6f 6e65 0a0a 5649 4557  es' = None..VIEW
-00350d50: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
-00350d60: 6974 5f63 7572 7665 3a20 2762 6c5f 7569  it_curve: 'bl_ui
-00350d70: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350d80: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-00350d90: 6564 6974 5f63 7572 7665 2720 3d20 4e6f  edit_curve' = No
-00350da0: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-00350db0: 6572 6c61 795f 6564 6974 5f6d 6573 683a  erlay_edit_mesh:
-00350dc0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350dd0: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-00350de0: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
-00350df0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00350e00: 5f50 545f 6f76 6572 6c61 795f 6564 6974  _PT_overlay_edit
-00350e10: 5f6d 6573 685f 6672 6565 7374 796c 653a  _mesh_freestyle:
-00350e20: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00350e30: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
-00350e40: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
-00350e50: 5f66 7265 6573 7479 6c65 2720 3d20 4e6f  _freestyle' = No
-00350e60: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-00350e70: 6572 6c61 795f 6564 6974 5f6d 6573 685f  erlay_edit_mesh_
-00350e80: 6d65 6173 7572 656d 656e 743a 2027 626c  measurement: 'bl
-00350e90: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350ea0: 2e56 4945 5733 445f 5054 5f6f 7665 726c  .VIEW3D_PT_overl
-00350eb0: 6179 5f65 6469 745f 6d65 7368 5f6d 6561  ay_edit_mesh_mea
-00350ec0: 7375 7265 6d65 6e74 2720 3d20 4e6f 6e65  surement' = None
-00350ed0: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
-00350ee0: 6c61 795f 6564 6974 5f6d 6573 685f 6e6f  lay_edit_mesh_no
-00350ef0: 726d 616c 733a 2027 626c 5f75 692e 7370  rmals: 'bl_ui.sp
-00350f00: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00350f10: 445f 5054 5f6f 7665 726c 6179 5f65 6469  D_PT_overlay_edi
-00350f20: 745f 6d65 7368 5f6e 6f72 6d61 6c73 2720  t_mesh_normals' 
-00350f30: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00350f40: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
-00350f50: 6573 685f 7368 6164 696e 673a 2027 626c  esh_shading: 'bl
-00350f60: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00350f70: 2e56 4945 5733 445f 5054 5f6f 7665 726c  .VIEW3D_PT_overl
-00350f80: 6179 5f65 6469 745f 6d65 7368 5f73 6861  ay_edit_mesh_sha
-00350f90: 6469 6e67 2720 3d20 4e6f 6e65 0a0a 5649  ding' = None..VI
-00350fa0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-00350fb0: 6765 6f6d 6574 7279 3a20 2762 6c5f 7569  geometry: 'bl_ui
-00350fc0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00350fd0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-00350fe0: 6765 6f6d 6574 7279 2720 3d20 4e6f 6e65  geometry' = None
-00350ff0: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
-00351000: 6c61 795f 6770 656e 6369 6c5f 6f70 7469  lay_gpencil_opti
-00351010: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-00351020: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351030: 5054 5f6f 7665 726c 6179 5f67 7065 6e63  PT_overlay_gpenc
-00351040: 696c 5f6f 7074 696f 6e73 2720 3d20 4e6f  il_options' = No
-00351050: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-00351060: 6572 6c61 795f 6775 6964 6573 3a20 2762  erlay_guides: 'b
+00350940: 6472 6177 5f63 6f6e 7465 7874 5f6d 656e  draw_context_men
+00350950: 753a 2027 626c 5f75 692e 7370 6163 655f  u: 'bl_ui.space_
+00350960: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+00350970: 5f67 7065 6e63 696c 5f64 7261 775f 636f  _gpencil_draw_co
+00350980: 6e74 6578 745f 6d65 6e75 2720 3d20 4e6f  ntext_menu' = No
+00350990: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
+003509a0: 656e 6369 6c5f 6775 6964 653a 2027 626c  encil_guide: 'bl
+003509b0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+003509c0: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
+003509d0: 696c 5f67 7569 6465 2720 3d20 4e6f 6e65  il_guide' = None
+003509e0: 0a0a 5649 4557 3344 5f50 545f 6770 656e  ..VIEW3D_PT_gpen
+003509f0: 6369 6c5f 6c6f 636b 3a20 2762 6c5f 7569  cil_lock: 'bl_ui
+00350a00: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00350a10: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+00350a20: 6c6f 636b 2720 3d20 4e6f 6e65 0a0a 5649  lock' = None..VI
+00350a30: 4557 3344 5f50 545f 6770 656e 6369 6c5f  EW3D_PT_gpencil_
+00350a40: 6d75 6c74 695f 6672 616d 653a 2027 626c  multi_frame: 'bl
+00350a50: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00350a60: 2e56 4945 5733 445f 5054 5f67 7065 6e63  .VIEW3D_PT_gpenc
+00350a70: 696c 5f6d 756c 7469 5f66 7261 6d65 2720  il_multi_frame' 
+00350a80: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350a90: 545f 6770 656e 6369 6c5f 6f72 6967 696e  T_gpencil_origin
+00350aa0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350ab0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00350ac0: 6770 656e 6369 6c5f 6f72 6967 696e 2720  gpencil_origin' 
+00350ad0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350ae0: 545f 6770 656e 6369 6c5f 7363 756c 7074  T_gpencil_sculpt
+00350af0: 5f61 7574 6f6d 6173 6b69 6e67 3a20 2762  _automasking: 'b
+00350b00: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350b10: 642e 5649 4557 3344 5f50 545f 6770 656e  d.VIEW3D_PT_gpen
+00350b20: 6369 6c5f 7363 756c 7074 5f61 7574 6f6d  cil_sculpt_autom
+00350b30: 6173 6b69 6e67 2720 3d20 4e6f 6e65 0a0a  asking' = None..
+00350b40: 5649 4557 3344 5f50 545f 6770 656e 6369  VIEW3D_PT_gpenci
+00350b50: 6c5f 7363 756c 7074 5f63 6f6e 7465 7874  l_sculpt_context
+00350b60: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
+00350b70: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350b80: 445f 5054 5f67 7065 6e63 696c 5f73 6375  D_PT_gpencil_scu
+00350b90: 6c70 745f 636f 6e74 6578 745f 6d65 6e75  lpt_context_menu
+00350ba0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00350bb0: 5f50 545f 6770 656e 6369 6c5f 7665 7274  _PT_gpencil_vert
+00350bc0: 6578 5f63 6f6e 7465 7874 5f6d 656e 753a  ex_context_menu:
+00350bd0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350be0: 6577 3364 2e56 4945 5733 445f 5054 5f67  ew3d.VIEW3D_PT_g
+00350bf0: 7065 6e63 696c 5f76 6572 7465 785f 636f  pencil_vertex_co
+00350c00: 6e74 6578 745f 6d65 6e75 2720 3d20 4e6f  ntext_menu' = No
+00350c10: 6e65 0a0a 5649 4557 3344 5f50 545f 6770  ne..VIEW3D_PT_gp
+00350c20: 656e 6369 6c5f 7765 6967 6874 5f63 6f6e  encil_weight_con
+00350c30: 7465 7874 5f6d 656e 753a 2027 626c 5f75  text_menu: 'bl_u
+00350c40: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350c50: 4945 5733 445f 5054 5f67 7065 6e63 696c  IEW3D_PT_gpencil
+00350c60: 5f77 6569 6768 745f 636f 6e74 6578 745f  _weight_context_
+00350c70: 6d65 6e75 2720 3d20 4e6f 6e65 0a0a 5649  menu' = None..VI
+00350c80: 4557 3344 5f50 545f 6772 6561 7365 5f70  EW3D_PT_grease_p
+00350c90: 656e 6369 6c3a 2027 626c 5f75 692e 7370  encil: 'bl_ui.sp
+00350ca0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+00350cb0: 445f 5054 5f67 7265 6173 655f 7065 6e63  D_PT_grease_penc
+00350cc0: 696c 2720 3d20 4e6f 6e65 0a0a 5649 4557  il' = None..VIEW
+00350cd0: 3344 5f50 545f 6d61 736b 3a20 2762 6c5f  3D_PT_mask: 'bl_
+00350ce0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00350cf0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00350d00: 545f 6d61 736b 2720 3d20 4e6f 6e65 0a0a  T_mask' = None..
+00350d10: 5649 4557 3344 5f50 545f 6f62 6a65 6374  VIEW3D_PT_object
+00350d20: 5f74 7970 655f 7669 7369 6269 6c69 7479  _type_visibility
+00350d30: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00350d40: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00350d50: 6f62 6a65 6374 5f74 7970 655f 7669 7369  object_type_visi
+00350d60: 6269 6c69 7479 2720 3d20 4e6f 6e65 0a0a  bility' = None..
+00350d70: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
+00350d80: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
+00350d90: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
+00350da0: 5f6f 7665 726c 6179 2720 3d20 4e6f 6e65  _overlay' = None
+00350db0: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
+00350dc0: 6c61 795f 626f 6e65 733a 2027 626c 5f75  lay_bones: 'bl_u
+00350dd0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350de0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+00350df0: 5f62 6f6e 6573 2720 3d20 4e6f 6e65 0a0a  _bones' = None..
+00350e00: 5649 4557 3344 5f50 545f 6f76 6572 6c61  VIEW3D_PT_overla
+00350e10: 795f 6564 6974 5f63 7572 7665 3a20 2762  y_edit_curve: 'b
+00350e20: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00350e30: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
+00350e40: 6c61 795f 6564 6974 5f63 7572 7665 2720  lay_edit_curve' 
+00350e50: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350e60: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
+00350e70: 6573 683a 2027 626c 5f75 692e 7370 6163  esh: 'bl_ui.spac
+00350e80: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350e90: 5054 5f6f 7665 726c 6179 5f65 6469 745f  PT_overlay_edit_
+00350ea0: 6d65 7368 2720 3d20 4e6f 6e65 0a0a 5649  mesh' = None..VI
+00350eb0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
+00350ec0: 6564 6974 5f6d 6573 685f 6672 6565 7374  edit_mesh_freest
+00350ed0: 796c 653a 2027 626c 5f75 692e 7370 6163  yle: 'bl_ui.spac
+00350ee0: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00350ef0: 5054 5f6f 7665 726c 6179 5f65 6469 745f  PT_overlay_edit_
+00350f00: 6d65 7368 5f66 7265 6573 7479 6c65 2720  mesh_freestyle' 
+00350f10: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00350f20: 545f 6f76 6572 6c61 795f 6564 6974 5f6d  T_overlay_edit_m
+00350f30: 6573 685f 6d65 6173 7572 656d 656e 743a  esh_measurement:
+00350f40: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00350f50: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+00350f60: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+00350f70: 5f6d 6561 7375 7265 6d65 6e74 2720 3d20  _measurement' = 
+00350f80: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00350f90: 6f76 6572 6c61 795f 6564 6974 5f6d 6573  overlay_edit_mes
+00350fa0: 685f 6e6f 726d 616c 733a 2027 626c 5f75  h_normals: 'bl_u
+00350fb0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00350fc0: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+00350fd0: 5f65 6469 745f 6d65 7368 5f6e 6f72 6d61  _edit_mesh_norma
+00350fe0: 6c73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ls' = None..VIEW
+00350ff0: 3344 5f50 545f 6f76 6572 6c61 795f 6564  3D_PT_overlay_ed
+00351000: 6974 5f6d 6573 685f 7368 6164 696e 673a  it_mesh_shading:
+00351010: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351020: 6577 3364 2e56 4945 5733 445f 5054 5f6f  ew3d.VIEW3D_PT_o
+00351030: 7665 726c 6179 5f65 6469 745f 6d65 7368  verlay_edit_mesh
+00351040: 5f73 6861 6469 6e67 2720 3d20 4e6f 6e65  _shading' = None
+00351050: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
+00351060: 6c61 795f 6765 6f6d 6574 7279 3a20 2762  lay_geometry: 'b
 00351070: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
 00351080: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-00351090: 6c61 795f 6775 6964 6573 2720 3d20 4e6f  lay_guides' = No
-003510a0: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-003510b0: 6572 6c61 795f 6d6f 7469 6f6e 5f74 7261  erlay_motion_tra
-003510c0: 636b 696e 673a 2027 626c 5f75 692e 7370  cking: 'bl_ui.sp
-003510d0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003510e0: 445f 5054 5f6f 7665 726c 6179 5f6d 6f74  D_PT_overlay_mot
-003510f0: 696f 6e5f 7472 6163 6b69 6e67 2720 3d20  ion_tracking' = 
-00351100: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351110: 6f76 6572 6c61 795f 6f62 6a65 6374 3a20  overlay_object: 
-00351120: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00351130: 7733 642e 5649 4557 3344 5f50 545f 6f76  w3d.VIEW3D_PT_ov
-00351140: 6572 6c61 795f 6f62 6a65 6374 2720 3d20  erlay_object' = 
-00351150: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00351160: 6f76 6572 6c61 795f 7363 756c 7074 3a20  overlay_sculpt: 
-00351170: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00351180: 7733 642e 5649 4557 3344 5f50 545f 6f76  w3d.VIEW3D_PT_ov
-00351190: 6572 6c61 795f 7363 756c 7074 2720 3d20  erlay_sculpt' = 
-003511a0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003511b0: 6f76 6572 6c61 795f 7363 756c 7074 5f63  overlay_sculpt_c
-003511c0: 7572 7665 733a 2027 626c 5f75 692e 7370  urves: 'bl_ui.sp
-003511d0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003511e0: 445f 5054 5f6f 7665 726c 6179 5f73 6375  D_PT_overlay_scu
-003511f0: 6c70 745f 6375 7276 6573 2720 3d20 4e6f  lpt_curves' = No
-00351200: 6e65 0a0a 5649 4557 3344 5f50 545f 6f76  ne..VIEW3D_PT_ov
-00351210: 6572 6c61 795f 7465 7874 7572 655f 7061  erlay_texture_pa
-00351220: 696e 743a 2027 626c 5f75 692e 7370 6163  int: 'bl_ui.spac
-00351230: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
-00351240: 5054 5f6f 7665 726c 6179 5f74 6578 7475  PT_overlay_textu
-00351250: 7265 5f70 6169 6e74 2720 3d20 4e6f 6e65  re_paint' = None
-00351260: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
-00351270: 6c61 795f 7665 7274 6578 5f70 6169 6e74  lay_vertex_paint
-00351280: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351290: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
-003512a0: 6f76 6572 6c61 795f 7665 7274 6578 5f70  overlay_vertex_p
-003512b0: 6169 6e74 2720 3d20 4e6f 6e65 0a0a 5649  aint' = None..VI
-003512c0: 4557 3344 5f50 545f 6f76 6572 6c61 795f  EW3D_PT_overlay_
-003512d0: 7765 6967 6874 5f70 6169 6e74 3a20 2762  weight_paint: 'b
-003512e0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003512f0: 642e 5649 4557 3344 5f50 545f 6f76 6572  d.VIEW3D_PT_over
-00351300: 6c61 795f 7765 6967 6874 5f70 6169 6e74  lay_weight_paint
-00351310: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351320: 5f50 545f 7061 696e 745f 7465 7874 7572  _PT_paint_textur
-00351330: 655f 636f 6e74 6578 745f 6d65 6e75 3a20  e_context_menu: 
-00351340: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00351350: 7733 642e 5649 4557 3344 5f50 545f 7061  w3d.VIEW3D_PT_pa
-00351360: 696e 745f 7465 7874 7572 655f 636f 6e74  int_texture_cont
-00351370: 6578 745f 6d65 6e75 2720 3d20 4e6f 6e65  ext_menu' = None
-00351380: 0a0a 5649 4557 3344 5f50 545f 7061 696e  ..VIEW3D_PT_pain
-00351390: 745f 7665 7274 6578 5f63 6f6e 7465 7874  t_vertex_context
-003513a0: 5f6d 656e 753a 2027 626c 5f75 692e 7370  _menu: 'bl_ui.sp
-003513b0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-003513c0: 445f 5054 5f70 6169 6e74 5f76 6572 7465  D_PT_paint_verte
-003513d0: 785f 636f 6e74 6578 745f 6d65 6e75 2720  x_context_menu' 
-003513e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003513f0: 545f 7061 696e 745f 7765 6967 6874 5f63  T_paint_weight_c
-00351400: 6f6e 7465 7874 5f6d 656e 753a 2027 626c  ontext_menu: 'bl
-00351410: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00351420: 2e56 4945 5733 445f 5054 5f70 6169 6e74  .VIEW3D_PT_paint
-00351430: 5f77 6569 6768 745f 636f 6e74 6578 745f  _weight_context_
-00351440: 6d65 6e75 2720 3d20 4e6f 6e65 0a0a 5649  menu' = None..VI
-00351450: 4557 3344 5f50 545f 7072 6f70 6f72 7469  EW3D_PT_proporti
-00351460: 6f6e 616c 5f65 6469 743a 2027 626c 5f75  onal_edit: 'bl_u
-00351470: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00351480: 4945 5733 445f 5054 5f70 726f 706f 7274  IEW3D_PT_proport
-00351490: 696f 6e61 6c5f 6564 6974 2720 3d20 4e6f  ional_edit' = No
-003514a0: 6e65 0a0a 5649 4557 3344 5f50 545f 7175  ne..VIEW3D_PT_qu
-003514b0: 6164 5f76 6965 773a 2027 626c 5f75 692e  ad_view: 'bl_ui.
-003514c0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-003514d0: 5733 445f 5054 5f71 7561 645f 7669 6577  W3D_PT_quad_view
-003514e0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-003514f0: 5f50 545f 7363 756c 7074 5f61 7574 6f6d  _PT_sculpt_autom
-00351500: 6173 6b69 6e67 3a20 2762 6c5f 7569 2e73  asking: 'bl_ui.s
-00351510: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00351520: 3344 5f50 545f 7363 756c 7074 5f61 7574  3D_PT_sculpt_aut
-00351530: 6f6d 6173 6b69 6e67 2720 3d20 4e6f 6e65  omasking' = None
-00351540: 0a0a 5649 4557 3344 5f50 545f 7363 756c  ..VIEW3D_PT_scul
-00351550: 7074 5f63 6f6e 7465 7874 5f6d 656e 753a  pt_context_menu:
-00351560: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351570: 6577 3364 2e56 4945 5733 445f 5054 5f73  ew3d.VIEW3D_PT_s
-00351580: 6375 6c70 745f 636f 6e74 6578 745f 6d65  culpt_context_me
-00351590: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
-003515a0: 3344 5f50 545f 7363 756c 7074 5f64 796e  3D_PT_sculpt_dyn
-003515b0: 746f 706f 3a20 2762 6c5f 7569 2e73 7061  topo: 'bl_ui.spa
-003515c0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-003515d0: 722e 5649 4557 3344 5f50 545f 7363 756c  r.VIEW3D_PT_scul
-003515e0: 7074 5f64 796e 746f 706f 2720 3d20 4e6f  pt_dyntopo' = No
-003515f0: 6e65 0a0a 5649 4557 3344 5f50 545f 7363  ne..VIEW3D_PT_sc
-00351600: 756c 7074 5f6f 7074 696f 6e73 3a20 2762  ulpt_options: 'b
-00351610: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351620: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00351630: 5f50 545f 7363 756c 7074 5f6f 7074 696f  _PT_sculpt_optio
-00351640: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-00351650: 3344 5f50 545f 7363 756c 7074 5f6f 7074  3D_PT_sculpt_opt
-00351660: 696f 6e73 5f67 7261 7669 7479 3a20 2762  ions_gravity: 'b
-00351670: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351680: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00351690: 5f50 545f 7363 756c 7074 5f6f 7074 696f  _PT_sculpt_optio
-003516a0: 6e73 5f67 7261 7669 7479 2720 3d20 4e6f  ns_gravity' = No
-003516b0: 6e65 0a0a 5649 4557 3344 5f50 545f 7363  ne..VIEW3D_PT_sc
-003516c0: 756c 7074 5f73 796d 6d65 7472 793a 2027  ulpt_symmetry: '
-003516d0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-003516e0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-003516f0: 445f 5054 5f73 6375 6c70 745f 7379 6d6d  D_PT_sculpt_symm
-00351700: 6574 7279 2720 3d20 4e6f 6e65 0a0a 5649  etry' = None..VI
-00351710: 4557 3344 5f50 545f 7363 756c 7074 5f73  EW3D_PT_sculpt_s
-00351720: 796d 6d65 7472 795f 666f 725f 746f 7062  ymmetry_for_topb
-00351730: 6172 3a20 2762 6c5f 7569 2e73 7061 6365  ar: 'bl_ui.space
-00351740: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00351750: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
-00351760: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
-00351770: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
-00351780: 4557 3344 5f50 545f 7363 756c 7074 5f76  EW3D_PT_sculpt_v
-00351790: 6f78 656c 5f72 656d 6573 683a 2027 626c  oxel_remesh: 'bl
-003517a0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-003517b0: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-003517c0: 5054 5f73 6375 6c70 745f 766f 7865 6c5f  PT_sculpt_voxel_
-003517d0: 7265 6d65 7368 2720 3d20 4e6f 6e65 0a0a  remesh' = None..
-003517e0: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
-003517f0: 673a 2027 626c 5f75 692e 7370 6163 655f  g: 'bl_ui.space_
-00351800: 7669 6577 3364 2e56 4945 5733 445f 5054  view3d.VIEW3D_PT
-00351810: 5f73 6861 6469 6e67 2720 3d20 4e6f 6e65  _shading' = None
-00351820: 0a0a 5649 4557 3344 5f50 545f 7368 6164  ..VIEW3D_PT_shad
-00351830: 696e 675f 636f 6c6f 723a 2027 626c 5f75  ing_color: 'bl_u
-00351840: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00351850: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
-00351860: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
-00351870: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
-00351880: 675f 636f 6d70 6f73 6974 6f72 3a20 2762  g_compositor: 'b
-00351890: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003518a0: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
-003518b0: 696e 675f 636f 6d70 6f73 6974 6f72 2720  ing_compositor' 
-003518c0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-003518d0: 545f 7368 6164 696e 675f 6c69 6768 7469  T_shading_lighti
-003518e0: 6e67 3a20 2762 6c5f 7569 2e73 7061 6365  ng: 'bl_ui.space
-003518f0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
-00351900: 545f 7368 6164 696e 675f 6c69 6768 7469  T_shading_lighti
-00351910: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
-00351920: 3344 5f50 545f 7368 6164 696e 675f 6f70  3D_PT_shading_op
-00351930: 7469 6f6e 733a 2027 626c 5f75 692e 7370  tions: 'bl_ui.sp
-00351940: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
-00351950: 445f 5054 5f73 6861 6469 6e67 5f6f 7074  D_PT_shading_opt
-00351960: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00351970: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
-00351980: 6f70 7469 6f6e 735f 7368 6164 6f77 3a20  options_shadow: 
-00351990: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003519a0: 7733 642e 5649 4557 3344 5f50 545f 7368  w3d.VIEW3D_PT_sh
-003519b0: 6164 696e 675f 6f70 7469 6f6e 735f 7368  ading_options_sh
-003519c0: 6164 6f77 2720 3d20 4e6f 6e65 0a0a 5649  adow' = None..VI
-003519d0: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
-003519e0: 6f70 7469 6f6e 735f 7373 616f 3a20 2762  options_ssao: 'b
-003519f0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00351a00: 642e 5649 4557 3344 5f50 545f 7368 6164  d.VIEW3D_PT_shad
-00351a10: 696e 675f 6f70 7469 6f6e 735f 7373 616f  ing_options_ssao
-00351a20: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351a30: 5f50 545f 7368 6164 696e 675f 7265 6e64  _PT_shading_rend
-00351a40: 6572 5f70 6173 733a 2027 626c 5f75 692e  er_pass: 'bl_ui.
-00351a50: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00351a60: 5733 445f 5054 5f73 6861 6469 6e67 5f72  W3D_PT_shading_r
-00351a70: 656e 6465 725f 7061 7373 2720 3d20 4e6f  ender_pass' = No
-00351a80: 6e65 0a0a 5649 4557 3344 5f50 545f 736c  ne..VIEW3D_PT_sl
-00351a90: 6f74 735f 7061 696e 745f 6361 6e76 6173  ots_paint_canvas
+00351090: 6c61 795f 6765 6f6d 6574 7279 2720 3d20  lay_geometry' = 
+003510a0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003510b0: 6f76 6572 6c61 795f 6770 656e 6369 6c5f  overlay_gpencil_
+003510c0: 6f70 7469 6f6e 733a 2027 626c 5f75 692e  options: 'bl_ui.
+003510d0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+003510e0: 5733 445f 5054 5f6f 7665 726c 6179 5f67  W3D_PT_overlay_g
+003510f0: 7065 6e63 696c 5f6f 7074 696f 6e73 2720  pencil_options' 
+00351100: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351110: 545f 6f76 6572 6c61 795f 6775 6964 6573  T_overlay_guides
+00351120: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00351130: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00351140: 6f76 6572 6c61 795f 6775 6964 6573 2720  overlay_guides' 
+00351150: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351160: 545f 6f76 6572 6c61 795f 6d6f 7469 6f6e  T_overlay_motion
+00351170: 5f74 7261 636b 696e 673a 2027 626c 5f75  _tracking: 'bl_u
+00351180: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00351190: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+003511a0: 5f6d 6f74 696f 6e5f 7472 6163 6b69 6e67  _motion_tracking
+003511b0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003511c0: 5f50 545f 6f76 6572 6c61 795f 6f62 6a65  _PT_overlay_obje
+003511d0: 6374 3a20 2762 6c5f 7569 2e73 7061 6365  ct: 'bl_ui.space
+003511e0: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+003511f0: 545f 6f76 6572 6c61 795f 6f62 6a65 6374  T_overlay_object
+00351200: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351210: 5f50 545f 6f76 6572 6c61 795f 7363 756c  _PT_overlay_scul
+00351220: 7074 3a20 2762 6c5f 7569 2e73 7061 6365  pt: 'bl_ui.space
+00351230: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00351240: 545f 6f76 6572 6c61 795f 7363 756c 7074  T_overlay_sculpt
+00351250: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00351260: 5f50 545f 6f76 6572 6c61 795f 7363 756c  _PT_overlay_scul
+00351270: 7074 5f63 7572 7665 733a 2027 626c 5f75  pt_curves: 'bl_u
+00351280: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00351290: 4945 5733 445f 5054 5f6f 7665 726c 6179  IEW3D_PT_overlay
+003512a0: 5f73 6375 6c70 745f 6375 7276 6573 2720  _sculpt_curves' 
+003512b0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003512c0: 545f 6f76 6572 6c61 795f 7465 7874 7572  T_overlay_textur
+003512d0: 655f 7061 696e 743a 2027 626c 5f75 692e  e_paint: 'bl_ui.
+003512e0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
+003512f0: 5733 445f 5054 5f6f 7665 726c 6179 5f74  W3D_PT_overlay_t
+00351300: 6578 7475 7265 5f70 6169 6e74 2720 3d20  exture_paint' = 
+00351310: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351320: 6f76 6572 6c61 795f 7665 7274 6578 5f70  overlay_vertex_p
+00351330: 6169 6e74 3a20 2762 6c5f 7569 2e73 7061  aint: 'bl_ui.spa
+00351340: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
+00351350: 5f50 545f 6f76 6572 6c61 795f 7665 7274  _PT_overlay_vert
+00351360: 6578 5f70 6169 6e74 2720 3d20 4e6f 6e65  ex_paint' = None
+00351370: 0a0a 5649 4557 3344 5f50 545f 6f76 6572  ..VIEW3D_PT_over
+00351380: 6c61 795f 7765 6967 6874 5f70 6169 6e74  lay_weight_paint
+00351390: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003513a0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+003513b0: 6f76 6572 6c61 795f 7765 6967 6874 5f70  overlay_weight_p
+003513c0: 6169 6e74 2720 3d20 4e6f 6e65 0a0a 5649  aint' = None..VI
+003513d0: 4557 3344 5f50 545f 7061 696e 745f 7465  EW3D_PT_paint_te
+003513e0: 7874 7572 655f 636f 6e74 6578 745f 6d65  xture_context_me
+003513f0: 6e75 3a20 2762 6c5f 7569 2e73 7061 6365  nu: 'bl_ui.space
+00351400: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00351410: 545f 7061 696e 745f 7465 7874 7572 655f  T_paint_texture_
+00351420: 636f 6e74 6578 745f 6d65 6e75 2720 3d20  context_menu' = 
+00351430: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351440: 7061 696e 745f 7665 7274 6578 5f63 6f6e  paint_vertex_con
+00351450: 7465 7874 5f6d 656e 753a 2027 626c 5f75  text_menu: 'bl_u
+00351460: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00351470: 4945 5733 445f 5054 5f70 6169 6e74 5f76  IEW3D_PT_paint_v
+00351480: 6572 7465 785f 636f 6e74 6578 745f 6d65  ertex_context_me
+00351490: 6e75 2720 3d20 4e6f 6e65 0a0a 5649 4557  nu' = None..VIEW
+003514a0: 3344 5f50 545f 7061 696e 745f 7765 6967  3D_PT_paint_weig
+003514b0: 6874 5f63 6f6e 7465 7874 5f6d 656e 753a  ht_context_menu:
+003514c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003514d0: 6577 3364 2e56 4945 5733 445f 5054 5f70  ew3d.VIEW3D_PT_p
+003514e0: 6169 6e74 5f77 6569 6768 745f 636f 6e74  aint_weight_cont
+003514f0: 6578 745f 6d65 6e75 2720 3d20 4e6f 6e65  ext_menu' = None
+00351500: 0a0a 5649 4557 3344 5f50 545f 7072 6f70  ..VIEW3D_PT_prop
+00351510: 6f72 7469 6f6e 616c 5f65 6469 743a 2027  ortional_edit: '
+00351520: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351530: 3364 2e56 4945 5733 445f 5054 5f70 726f  3d.VIEW3D_PT_pro
+00351540: 706f 7274 696f 6e61 6c5f 6564 6974 2720  portional_edit' 
+00351550: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351560: 545f 7175 6164 5f76 6965 773a 2027 626c  T_quad_view: 'bl
+00351570: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00351580: 2e56 4945 5733 445f 5054 5f71 7561 645f  .VIEW3D_PT_quad_
+00351590: 7669 6577 2720 3d20 4e6f 6e65 0a0a 5649  view' = None..VI
+003515a0: 4557 3344 5f50 545f 7363 756c 7074 5f61  EW3D_PT_sculpt_a
+003515b0: 7574 6f6d 6173 6b69 6e67 3a20 2762 6c5f  utomasking: 'bl_
+003515c0: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+003515d0: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
+003515e0: 5f61 7574 6f6d 6173 6b69 6e67 2720 3d20  _automasking' = 
+003515f0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351600: 7363 756c 7074 5f63 6f6e 7465 7874 5f6d  sculpt_context_m
+00351610: 656e 753a 2027 626c 5f75 692e 7370 6163  enu: 'bl_ui.spac
+00351620: 655f 7669 6577 3364 2e56 4945 5733 445f  e_view3d.VIEW3D_
+00351630: 5054 5f73 6375 6c70 745f 636f 6e74 6578  PT_sculpt_contex
+00351640: 745f 6d65 6e75 2720 3d20 4e6f 6e65 0a0a  t_menu' = None..
+00351650: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
+00351660: 5f64 796e 746f 706f 3a20 2762 6c5f 7569  _dyntopo: 'bl_ui
+00351670: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00351680: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00351690: 7363 756c 7074 5f64 796e 746f 706f 2720  sculpt_dyntopo' 
+003516a0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003516b0: 545f 7363 756c 7074 5f6f 7074 696f 6e73  T_sculpt_options
+003516c0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+003516d0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+003516e0: 4557 3344 5f50 545f 7363 756c 7074 5f6f  EW3D_PT_sculpt_o
+003516f0: 7074 696f 6e73 2720 3d20 4e6f 6e65 0a0a  ptions' = None..
+00351700: 5649 4557 3344 5f50 545f 7363 756c 7074  VIEW3D_PT_sculpt
+00351710: 5f6f 7074 696f 6e73 5f67 7261 7669 7479  _options_gravity
+00351720: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00351730: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00351740: 4557 3344 5f50 545f 7363 756c 7074 5f6f  EW3D_PT_sculpt_o
+00351750: 7074 696f 6e73 5f67 7261 7669 7479 2720  ptions_gravity' 
+00351760: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351770: 545f 7363 756c 7074 5f73 796d 6d65 7472  T_sculpt_symmetr
+00351780: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
+00351790: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+003517a0: 4945 5733 445f 5054 5f73 6375 6c70 745f  IEW3D_PT_sculpt_
+003517b0: 7379 6d6d 6574 7279 2720 3d20 4e6f 6e65  symmetry' = None
+003517c0: 0a0a 5649 4557 3344 5f50 545f 7363 756c  ..VIEW3D_PT_scul
+003517d0: 7074 5f73 796d 6d65 7472 795f 666f 725f  pt_symmetry_for_
+003517e0: 746f 7062 6172 3a20 2762 6c5f 7569 2e73  topbar: 'bl_ui.s
+003517f0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00351800: 6261 722e 5649 4557 3344 5f50 545f 7363  bar.VIEW3D_PT_sc
+00351810: 756c 7074 5f73 796d 6d65 7472 795f 666f  ulpt_symmetry_fo
+00351820: 725f 746f 7062 6172 2720 3d20 4e6f 6e65  r_topbar' = None
+00351830: 0a0a 5649 4557 3344 5f50 545f 7363 756c  ..VIEW3D_PT_scul
+00351840: 7074 5f76 6f78 656c 5f72 656d 6573 683a  pt_voxel_remesh:
+00351850: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351860: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00351870: 5733 445f 5054 5f73 6375 6c70 745f 766f  W3D_PT_sculpt_vo
+00351880: 7865 6c5f 7265 6d65 7368 2720 3d20 4e6f  xel_remesh' = No
+00351890: 6e65 0a0a 5649 4557 3344 5f50 545f 7368  ne..VIEW3D_PT_sh
+003518a0: 6164 696e 673a 2027 626c 5f75 692e 7370  ading: 'bl_ui.sp
+003518b0: 6163 655f 7669 6577 3364 2e56 4945 5733  ace_view3d.VIEW3
+003518c0: 445f 5054 5f73 6861 6469 6e67 2720 3d20  D_PT_shading' = 
+003518d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003518e0: 7368 6164 696e 675f 636f 6c6f 723a 2027  shading_color: '
+003518f0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00351900: 3364 2e56 4945 5733 445f 5054 5f73 6861  3d.VIEW3D_PT_sha
+00351910: 6469 6e67 5f63 6f6c 6f72 2720 3d20 4e6f  ding_color' = No
+00351920: 6e65 0a0a 5649 4557 3344 5f50 545f 7368  ne..VIEW3D_PT_sh
+00351930: 6164 696e 675f 636f 6d70 6f73 6974 6f72  ading_compositor
+00351940: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00351950: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00351960: 7368 6164 696e 675f 636f 6d70 6f73 6974  shading_composit
+00351970: 6f72 2720 3d20 4e6f 6e65 0a0a 5649 4557  or' = None..VIEW
+00351980: 3344 5f50 545f 7368 6164 696e 675f 6c69  3D_PT_shading_li
+00351990: 6768 7469 6e67 3a20 2762 6c5f 7569 2e73  ghting: 'bl_ui.s
+003519a0: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
+003519b0: 3344 5f50 545f 7368 6164 696e 675f 6c69  3D_PT_shading_li
+003519c0: 6768 7469 6e67 2720 3d20 4e6f 6e65 0a0a  ghting' = None..
+003519d0: 5649 4557 3344 5f50 545f 7368 6164 696e  VIEW3D_PT_shadin
+003519e0: 675f 6f70 7469 6f6e 733a 2027 626c 5f75  g_options: 'bl_u
+003519f0: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
+00351a00: 4945 5733 445f 5054 5f73 6861 6469 6e67  IEW3D_PT_shading
+00351a10: 5f6f 7074 696f 6e73 2720 3d20 4e6f 6e65  _options' = None
+00351a20: 0a0a 5649 4557 3344 5f50 545f 7368 6164  ..VIEW3D_PT_shad
+00351a30: 696e 675f 6f70 7469 6f6e 735f 7368 6164  ing_options_shad
+00351a40: 6f77 3a20 2762 6c5f 7569 2e73 7061 6365  ow: 'bl_ui.space
+00351a50: 5f76 6965 7733 642e 5649 4557 3344 5f50  _view3d.VIEW3D_P
+00351a60: 545f 7368 6164 696e 675f 6f70 7469 6f6e  T_shading_option
+00351a70: 735f 7368 6164 6f77 2720 3d20 4e6f 6e65  s_shadow' = None
+00351a80: 0a0a 5649 4557 3344 5f50 545f 7368 6164  ..VIEW3D_PT_shad
+00351a90: 696e 675f 6f70 7469 6f6e 735f 7373 616f  ing_options_ssao
 00351aa0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351ab0: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00351ac0: 4557 3344 5f50 545f 736c 6f74 735f 7061  EW3D_PT_slots_pa
-00351ad0: 696e 745f 6361 6e76 6173 2720 3d20 4e6f  int_canvas' = No
-00351ae0: 6e65 0a0a 5649 4557 3344 5f50 545f 736c  ne..VIEW3D_PT_sl
-00351af0: 6f74 735f 7072 6f6a 6563 7470 6169 6e74  ots_projectpaint
-00351b00: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00351b10: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00351b20: 4557 3344 5f50 545f 736c 6f74 735f 7072  EW3D_PT_slots_pr
-00351b30: 6f6a 6563 7470 6169 6e74 2720 3d20 4e6f  ojectpaint' = No
-00351b40: 6e65 0a0a 5649 4557 3344 5f50 545f 736e  ne..VIEW3D_PT_sn
-00351b50: 6170 7069 6e67 3a20 2762 6c5f 7569 2e73  apping: 'bl_ui.s
-00351b60: 7061 6365 5f76 6965 7733 642e 5649 4557  pace_view3d.VIEW
-00351b70: 3344 5f50 545f 736e 6170 7069 6e67 2720  3D_PT_snapping' 
-00351b80: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
-00351b90: 545f 7374 656e 6369 6c5f 7072 6f6a 6563  T_stencil_projec
-00351ba0: 7470 6169 6e74 3a20 2762 6c5f 7569 2e73  tpaint: 'bl_ui.s
-00351bb0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00351bc0: 6261 722e 5649 4557 3344 5f50 545f 7374  bar.VIEW3D_PT_st
-00351bd0: 656e 6369 6c5f 7072 6f6a 6563 7470 6169  encil_projectpai
-00351be0: 6e74 2720 3d20 4e6f 6e65 0a0a 5649 4557  nt' = None..VIEW
-00351bf0: 3344 5f50 545f 746f 6f6c 735f 6163 7469  3D_PT_tools_acti
-00351c00: 7665 3a20 2762 6c5f 7569 2e73 7061 6365  ve: 'bl_ui.space
-00351c10: 5f74 6f6f 6c73 7973 7465 6d5f 746f 6f6c  _toolsystem_tool
-00351c20: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00351c30: 6f6c 735f 6163 7469 7665 2720 3d20 4e6f  ols_active' = No
-00351c40: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00351c50: 6f6c 735f 6172 6d61 7475 7265 6564 6974  ols_armatureedit
-00351c60: 5f6f 7074 696f 6e73 3a20 2762 6c5f 7569  _options: 'bl_ui
-00351c70: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00351c80: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00351c90: 746f 6f6c 735f 6172 6d61 7475 7265 6564  tools_armatureed
-00351ca0: 6974 5f6f 7074 696f 6e73 2720 3d20 4e6f  it_options' = No
-00351cb0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00351cc0: 6f6c 735f 6272 7573 685f 636c 6f6e 653a  ols_brush_clone:
-00351cd0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351ce0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00351cf0: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
-00351d00: 7368 5f63 6c6f 6e65 2720 3d20 4e6f 6e65  sh_clone' = None
-00351d10: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00351d20: 735f 6272 7573 685f 636f 6c6f 723a 2027  s_brush_color: '
-00351d30: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351d40: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00351d50: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00351d60: 5f63 6f6c 6f72 2720 3d20 4e6f 6e65 0a0a  _color' = None..
-00351d70: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00351d80: 6272 7573 685f 6469 7370 6c61 793a 2027  brush_display: '
-00351d90: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00351da0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00351db0: 445f 5054 5f74 6f6f 6c73 5f62 7275 7368  D_PT_tools_brush
-00351dc0: 5f64 6973 706c 6179 2720 3d20 4e6f 6e65  _display' = None
-00351dd0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00351de0: 735f 6272 7573 685f 6661 6c6c 6f66 663a  s_brush_falloff:
-00351df0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-00351e00: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-00351e10: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
-00351e20: 7368 5f66 616c 6c6f 6666 2720 3d20 4e6f  sh_falloff' = No
-00351e30: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00351e40: 6f6c 735f 6272 7573 685f 6661 6c6c 6f66  ols_brush_fallof
-00351e50: 665f 6672 6f6e 7466 6163 653a 2027 626c  f_frontface: 'bl
-00351e60: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00351e70: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00351e80: 5054 5f74 6f6f 6c73 5f62 7275 7368 5f66  PT_tools_brush_f
-00351e90: 616c 6c6f 6666 5f66 726f 6e74 6661 6365  alloff_frontface
-00351ea0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351eb0: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00351ec0: 6661 6c6c 6f66 665f 6e6f 726d 616c 3a20  falloff_normal: 
-00351ed0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00351ee0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00351ef0: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
-00351f00: 685f 6661 6c6c 6f66 665f 6e6f 726d 616c  h_falloff_normal
-00351f10: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351f20: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00351f30: 7365 6c65 6374 3a20 2762 6c5f 7569 2e73  select: 'bl_ui.s
-00351f40: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
-00351f50: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
-00351f60: 6f6c 735f 6272 7573 685f 7365 6c65 6374  ols_brush_select
-00351f70: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00351f80: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
-00351f90: 7365 7474 696e 6773 3a20 2762 6c5f 7569  settings: 'bl_ui
-00351fa0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00351fb0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00351fc0: 746f 6f6c 735f 6272 7573 685f 7365 7474  tools_brush_sett
-00351fd0: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
-00351fe0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-00351ff0: 7573 685f 7365 7474 696e 6773 5f61 6476  ush_settings_adv
-00352000: 616e 6365 643a 2027 626c 5f75 692e 7370  anced: 'bl_ui.sp
-00352010: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00352020: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00352030: 6c73 5f62 7275 7368 5f73 6574 7469 6e67  ls_brush_setting
-00352040: 735f 6164 7661 6e63 6564 2720 3d20 4e6f  s_advanced' = No
-00352050: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00352060: 6f6c 735f 6272 7573 685f 7374 726f 6b65  ols_brush_stroke
-00352070: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00352080: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00352090: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
-003520a0: 7573 685f 7374 726f 6b65 2720 3d20 4e6f  ush_stroke' = No
-003520b0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003520c0: 6f6c 735f 6272 7573 685f 7374 726f 6b65  ols_brush_stroke
-003520d0: 5f73 6d6f 6f74 685f 7374 726f 6b65 3a20  _smooth_stroke: 
-003520e0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003520f0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352100: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
-00352110: 685f 7374 726f 6b65 5f73 6d6f 6f74 685f  h_stroke_smooth_
-00352120: 7374 726f 6b65 2720 3d20 4e6f 6e65 0a0a  stroke' = None..
-00352130: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352140: 6272 7573 685f 7377 6174 6368 6573 3a20  brush_swatches: 
-00352150: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00352160: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352170: 3344 5f50 545f 746f 6f6c 735f 6272 7573  3D_PT_tools_brus
-00352180: 685f 7377 6174 6368 6573 2720 3d20 4e6f  h_swatches' = No
-00352190: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003521a0: 6f6c 735f 6272 7573 685f 7465 7874 7572  ols_brush_textur
-003521b0: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
-003521c0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-003521d0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
-003521e0: 7275 7368 5f74 6578 7475 7265 2720 3d20  rush_texture' = 
-003521f0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352200: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00352210: 6369 6c5f 6272 7573 685f 6164 7661 6e63  cil_brush_advanc
-00352220: 6564 3a20 2762 6c5f 7569 2e73 7061 6365  ed: 'bl_ui.space
-00352230: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00352240: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00352250: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
-00352260: 7573 685f 6164 7661 6e63 6564 2720 3d20  ush_advanced' = 
-00352270: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-00352280: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00352290: 6369 6c5f 6272 7573 685f 6761 705f 636c  cil_brush_gap_cl
-003522a0: 6f73 7572 653a 2027 626c 5f75 692e 7370  osure: 'bl_ui.sp
-003522b0: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-003522c0: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-003522d0: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-003522e0: 5f62 7275 7368 5f67 6170 5f63 6c6f 7375  _brush_gap_closu
-003522f0: 7265 2720 3d20 4e6f 6e65 0a0a 5649 4557  re' = None..VIEW
-00352300: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352310: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00352320: 6d69 785f 7061 6c65 7474 653a 2027 626c  mix_palette: 'bl
-00352330: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00352340: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00352350: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352360: 7065 6e63 696c 5f62 7275 7368 5f6d 6978  pencil_brush_mix
-00352370: 5f70 616c 6574 7465 2720 3d20 4e6f 6e65  _palette' = None
-00352380: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352390: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-003523a0: 6272 7573 685f 6d69 7863 6f6c 6f72 3a20  brush_mixcolor: 
-003523b0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003523c0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-003523d0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003523e0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-003523f0: 6d69 7863 6f6c 6f72 2720 3d20 4e6f 6e65  mixcolor' = None
-00352400: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352410: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352420: 6272 7573 685f 7061 696e 745f 6661 6c6c  brush_paint_fall
-00352430: 6f66 663a 2027 626c 5f75 692e 7370 6163  off: 'bl_ui.spac
-00352440: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00352450: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00352460: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
-00352470: 7275 7368 5f70 6169 6e74 5f66 616c 6c6f  rush_paint_fallo
-00352480: 6666 2720 3d20 4e6f 6e65 0a0a 5649 4557  ff' = None..VIEW
-00352490: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003524a0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-003524b0: 706f 7374 5f70 726f 6365 7373 696e 673a  post_processing:
-003524c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003524d0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-003524e0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-003524f0: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
-00352500: 5f70 6f73 745f 7072 6f63 6573 7369 6e67  _post_processing
-00352510: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00352520: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00352530: 5f70 656e 6369 6c5f 6272 7573 685f 7261  _pencil_brush_ra
-00352540: 6e64 6f6d 3a20 2762 6c5f 7569 2e73 7061  ndom: 'bl_ui.spa
-00352550: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352560: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352570: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352580: 6272 7573 685f 7261 6e64 6f6d 2720 3d20  brush_random' = 
-00352590: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003525a0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-003525b0: 6369 6c5f 6272 7573 685f 7363 756c 7074  cil_brush_sculpt
-003525c0: 5f66 616c 6c6f 6666 3a20 2762 6c5f 7569  _falloff: 'bl_ui
-003525d0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003525e0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003525f0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00352600: 6369 6c5f 6272 7573 685f 7363 756c 7074  cil_brush_sculpt
-00352610: 5f66 616c 6c6f 6666 2720 3d20 4e6f 6e65  _falloff' = None
-00352620: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352630: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352640: 6272 7573 685f 7365 6c65 6374 3a20 2762  brush_select: 'b
-00352650: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00352660: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00352670: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00352680: 5f70 656e 6369 6c5f 6272 7573 685f 7365  _pencil_brush_se
-00352690: 6c65 6374 2720 3d20 4e6f 6e65 0a0a 5649  lect' = None..VI
-003526a0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-003526b0: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
-003526c0: 685f 7365 7474 696e 6773 3a20 2762 6c5f  h_settings: 'bl_
-003526d0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
-003526e0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
-003526f0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
-00352700: 656e 6369 6c5f 6272 7573 685f 7365 7474  encil_brush_sett
-00352710: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
+00351ab0: 6965 7733 642e 5649 4557 3344 5f50 545f  iew3d.VIEW3D_PT_
+00351ac0: 7368 6164 696e 675f 6f70 7469 6f6e 735f  shading_options_
+00351ad0: 7373 616f 2720 3d20 4e6f 6e65 0a0a 5649  ssao' = None..VI
+00351ae0: 4557 3344 5f50 545f 7368 6164 696e 675f  EW3D_PT_shading_
+00351af0: 7265 6e64 6572 5f70 6173 733a 2027 626c  render_pass: 'bl
+00351b00: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00351b10: 2e56 4945 5733 445f 5054 5f73 6861 6469  .VIEW3D_PT_shadi
+00351b20: 6e67 5f72 656e 6465 725f 7061 7373 2720  ng_render_pass' 
+00351b30: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351b40: 545f 736c 6f74 735f 7061 696e 745f 6361  T_slots_paint_ca
+00351b50: 6e76 6173 3a20 2762 6c5f 7569 2e73 7061  nvas: 'bl_ui.spa
+00351b60: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00351b70: 722e 5649 4557 3344 5f50 545f 736c 6f74  r.VIEW3D_PT_slot
+00351b80: 735f 7061 696e 745f 6361 6e76 6173 2720  s_paint_canvas' 
+00351b90: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351ba0: 545f 736c 6f74 735f 7072 6f6a 6563 7470  T_slots_projectp
+00351bb0: 6169 6e74 3a20 2762 6c5f 7569 2e73 7061  aint: 'bl_ui.spa
+00351bc0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00351bd0: 722e 5649 4557 3344 5f50 545f 736c 6f74  r.VIEW3D_PT_slot
+00351be0: 735f 7072 6f6a 6563 7470 6169 6e74 2720  s_projectpaint' 
+00351bf0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351c00: 545f 736e 6170 7069 6e67 3a20 2762 6c5f  T_snapping: 'bl_
+00351c10: 7569 2e73 7061 6365 5f76 6965 7733 642e  ui.space_view3d.
+00351c20: 5649 4557 3344 5f50 545f 736e 6170 7069  VIEW3D_PT_snappi
+00351c30: 6e67 2720 3d20 4e6f 6e65 0a0a 5649 4557  ng' = None..VIEW
+00351c40: 3344 5f50 545f 7374 656e 6369 6c5f 7072  3D_PT_stencil_pr
+00351c50: 6f6a 6563 7470 6169 6e74 3a20 2762 6c5f  ojectpaint: 'bl_
+00351c60: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00351c70: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00351c80: 545f 7374 656e 6369 6c5f 7072 6f6a 6563  T_stencil_projec
+00351c90: 7470 6169 6e74 2720 3d20 4e6f 6e65 0a0a  tpaint' = None..
+00351ca0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00351cb0: 6163 7469 7665 3a20 2762 6c5f 7569 2e73  active: 'bl_ui.s
+00351cc0: 7061 6365 5f74 6f6f 6c73 7973 7465 6d5f  pace_toolsystem_
+00351cd0: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00351ce0: 545f 746f 6f6c 735f 6163 7469 7665 2720  T_tools_active' 
+00351cf0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351d00: 545f 746f 6f6c 735f 6172 6d61 7475 7265  T_tools_armature
+00351d10: 6564 6974 5f6f 7074 696f 6e73 3a20 2762  edit_options: 'b
+00351d20: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00351d30: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00351d40: 5f50 545f 746f 6f6c 735f 6172 6d61 7475  _PT_tools_armatu
+00351d50: 7265 6564 6974 5f6f 7074 696f 6e73 2720  reedit_options' 
+00351d60: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351d70: 545f 746f 6f6c 735f 6272 7573 685f 636c  T_tools_brush_cl
+00351d80: 6f6e 653a 2027 626c 5f75 692e 7370 6163  one: 'bl_ui.spac
+00351d90: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00351da0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00351db0: 5f62 7275 7368 5f63 6c6f 6e65 2720 3d20  _brush_clone' = 
+00351dc0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351dd0: 746f 6f6c 735f 6272 7573 685f 636f 6c6f  tools_brush_colo
+00351de0: 723a 2027 626c 5f75 692e 7370 6163 655f  r: 'bl_ui.space_
+00351df0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00351e00: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
+00351e10: 7275 7368 5f63 6f6c 6f72 2720 3d20 4e6f  rush_color' = No
+00351e20: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00351e30: 6f6c 735f 6272 7573 685f 6469 7370 6c61  ols_brush_displa
+00351e40: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
+00351e50: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00351e60: 4945 5733 445f 5054 5f74 6f6f 6c73 5f62  IEW3D_PT_tools_b
+00351e70: 7275 7368 5f64 6973 706c 6179 2720 3d20  rush_display' = 
+00351e80: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00351e90: 746f 6f6c 735f 6272 7573 685f 6661 6c6c  tools_brush_fall
+00351ea0: 6f66 663a 2027 626c 5f75 692e 7370 6163  off: 'bl_ui.spac
+00351eb0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00351ec0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+00351ed0: 5f62 7275 7368 5f66 616c 6c6f 6666 2720  _brush_falloff' 
+00351ee0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00351ef0: 545f 746f 6f6c 735f 6272 7573 685f 6661  T_tools_brush_fa
+00351f00: 6c6c 6f66 665f 6672 6f6e 7466 6163 653a  lloff_frontface:
+00351f10: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00351f20: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00351f30: 5733 445f 5054 5f74 6f6f 6c73 5f62 7275  W3D_PT_tools_bru
+00351f40: 7368 5f66 616c 6c6f 6666 5f66 726f 6e74  sh_falloff_front
+00351f50: 6661 6365 2720 3d20 4e6f 6e65 0a0a 5649  face' = None..VI
+00351f60: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00351f70: 7573 685f 6661 6c6c 6f66 665f 6e6f 726d  ush_falloff_norm
+00351f80: 616c 3a20 2762 6c5f 7569 2e73 7061 6365  al: 'bl_ui.space
+00351f90: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00351fa0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00351fb0: 6272 7573 685f 6661 6c6c 6f66 665f 6e6f  brush_falloff_no
+00351fc0: 726d 616c 2720 3d20 4e6f 6e65 0a0a 5649  rmal' = None..VI
+00351fd0: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00351fe0: 7573 685f 7365 6c65 6374 3a20 2762 6c5f  ush_select: 'bl_
+00351ff0: 7569 2e73 7061 6365 5f76 6965 7733 645f  ui.space_view3d_
+00352000: 746f 6f6c 6261 722e 5649 4557 3344 5f50  toolbar.VIEW3D_P
+00352010: 545f 746f 6f6c 735f 6272 7573 685f 7365  T_tools_brush_se
+00352020: 6c65 6374 2720 3d20 4e6f 6e65 0a0a 5649  lect' = None..VI
+00352030: 4557 3344 5f50 545f 746f 6f6c 735f 6272  EW3D_PT_tools_br
+00352040: 7573 685f 7365 7474 696e 6773 3a20 2762  ush_settings: 'b
+00352050: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352060: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00352070: 5f50 545f 746f 6f6c 735f 6272 7573 685f  _PT_tools_brush_
+00352080: 7365 7474 696e 6773 2720 3d20 4e6f 6e65  settings' = None
+00352090: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003520a0: 735f 6272 7573 685f 7365 7474 696e 6773  s_brush_settings
+003520b0: 5f61 6476 616e 6365 643a 2027 626c 5f75  _advanced: 'bl_u
+003520c0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+003520d0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+003520e0: 5f74 6f6f 6c73 5f62 7275 7368 5f73 6574  _tools_brush_set
+003520f0: 7469 6e67 735f 6164 7661 6e63 6564 2720  tings_advanced' 
+00352100: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00352110: 545f 746f 6f6c 735f 6272 7573 685f 7374  T_tools_brush_st
+00352120: 726f 6b65 3a20 2762 6c5f 7569 2e73 7061  roke: 'bl_ui.spa
+00352130: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00352140: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00352150: 735f 6272 7573 685f 7374 726f 6b65 2720  s_brush_stroke' 
+00352160: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00352170: 545f 746f 6f6c 735f 6272 7573 685f 7374  T_tools_brush_st
+00352180: 726f 6b65 5f73 6d6f 6f74 685f 7374 726f  roke_smooth_stro
+00352190: 6b65 3a20 2762 6c5f 7569 2e73 7061 6365  ke: 'bl_ui.space
+003521a0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+003521b0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003521c0: 6272 7573 685f 7374 726f 6b65 5f73 6d6f  brush_stroke_smo
+003521d0: 6f74 685f 7374 726f 6b65 2720 3d20 4e6f  oth_stroke' = No
+003521e0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+003521f0: 6f6c 735f 6272 7573 685f 7377 6174 6368  ols_brush_swatch
+00352200: 6573 3a20 2762 6c5f 7569 2e73 7061 6365  es: 'bl_ui.space
+00352210: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00352220: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352230: 6272 7573 685f 7377 6174 6368 6573 2720  brush_swatches' 
+00352240: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00352250: 545f 746f 6f6c 735f 6272 7573 685f 7465  T_tools_brush_te
+00352260: 7874 7572 653a 2027 626c 5f75 692e 7370  xture: 'bl_ui.sp
+00352270: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00352280: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00352290: 6c73 5f62 7275 7368 5f74 6578 7475 7265  ls_brush_texture
+003522a0: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+003522b0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003522c0: 5f70 656e 6369 6c5f 6272 7573 685f 6164  _pencil_brush_ad
+003522d0: 7661 6e63 6564 3a20 2762 6c5f 7569 2e73  vanced: 'bl_ui.s
+003522e0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+003522f0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00352300: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
+00352310: 6c5f 6272 7573 685f 6164 7661 6e63 6564  l_brush_advanced
+00352320: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00352330: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00352340: 5f70 656e 6369 6c5f 6272 7573 685f 6761  _pencil_brush_ga
+00352350: 705f 636c 6f73 7572 653a 2027 626c 5f75  p_closure: 'bl_u
+00352360: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352370: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352380: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352390: 6e63 696c 5f62 7275 7368 5f67 6170 5f63  ncil_brush_gap_c
+003523a0: 6c6f 7375 7265 2720 3d20 4e6f 6e65 0a0a  losure' = None..
+003523b0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003523c0: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
+003523d0: 7573 685f 6d69 785f 7061 6c65 7474 653a  ush_mix_palette:
+003523e0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+003523f0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00352400: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00352410: 6173 655f 7065 6e63 696c 5f62 7275 7368  ase_pencil_brush
+00352420: 5f6d 6978 5f70 616c 6574 7465 2720 3d20  _mix_palette' = 
+00352430: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00352440: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352450: 6369 6c5f 6272 7573 685f 6d69 7863 6f6c  cil_brush_mixcol
+00352460: 6f72 3a20 2762 6c5f 7569 2e73 7061 6365  or: 'bl_ui.space
+00352470: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00352480: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352490: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
+003524a0: 7573 685f 6d69 7863 6f6c 6f72 2720 3d20  ush_mixcolor' = 
+003524b0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003524c0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003524d0: 6369 6c5f 6272 7573 685f 7061 696e 745f  cil_brush_paint_
+003524e0: 6661 6c6c 6f66 663a 2027 626c 5f75 692e  falloff: 'bl_ui.
+003524f0: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00352500: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00352510: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+00352520: 696c 5f62 7275 7368 5f70 6169 6e74 5f66  il_brush_paint_f
+00352530: 616c 6c6f 6666 2720 3d20 4e6f 6e65 0a0a  alloff' = None..
+00352540: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352550: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
+00352560: 7573 685f 706f 7374 5f70 726f 6365 7373  ush_post_process
+00352570: 696e 673a 2027 626c 5f75 692e 7370 6163  ing: 'bl_ui.spac
+00352580: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00352590: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003525a0: 5f67 7265 6173 655f 7065 6e63 696c 5f62  _grease_pencil_b
+003525b0: 7275 7368 5f70 6f73 745f 7072 6f63 6573  rush_post_proces
+003525c0: 7369 6e67 2720 3d20 4e6f 6e65 0a0a 5649  sing' = None..VI
+003525d0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+003525e0: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+003525f0: 685f 7261 6e64 6f6d 3a20 2762 6c5f 7569  h_random: 'bl_ui
+00352600: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352610: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352620: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352630: 6369 6c5f 6272 7573 685f 7261 6e64 6f6d  cil_brush_random
+00352640: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00352650: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00352660: 5f70 656e 6369 6c5f 6272 7573 685f 7363  _pencil_brush_sc
+00352670: 756c 7074 5f66 616c 6c6f 6666 3a20 2762  ulpt_falloff: 'b
+00352680: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352690: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+003526a0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003526b0: 5f70 656e 6369 6c5f 6272 7573 685f 7363  _pencil_brush_sc
+003526c0: 756c 7074 5f66 616c 6c6f 6666 2720 3d20  ulpt_falloff' = 
+003526d0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003526e0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003526f0: 6369 6c5f 6272 7573 685f 7365 6c65 6374  cil_brush_select
+00352700: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352710: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
 00352720: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
 00352730: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
-00352740: 685f 7374 6162 696c 697a 6572 3a20 2762  h_stabilizer: 'b
-00352750: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00352760: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00352770: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00352780: 5f70 656e 6369 6c5f 6272 7573 685f 7374  _pencil_brush_st
-00352790: 6162 696c 697a 6572 2720 3d20 4e6f 6e65  abilizer' = None
-003527a0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-003527b0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-003527c0: 6272 7573 685f 7374 726f 6b65 3a20 2762  brush_stroke: 'b
-003527d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-003527e0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-003527f0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00352800: 5f70 656e 6369 6c5f 6272 7573 685f 7374  _pencil_brush_st
-00352810: 726f 6b65 2720 3d20 4e6f 6e65 0a0a 5649  roke' = None..VI
+00352740: 685f 7365 6c65 6374 2720 3d20 4e6f 6e65  h_select' = None
+00352750: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352760: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352770: 6272 7573 685f 7365 7474 696e 6773 3a20  brush_settings: 
+00352780: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
+00352790: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
+003527a0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
+003527b0: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
+003527c0: 7365 7474 696e 6773 2720 3d20 4e6f 6e65  settings' = None
+003527d0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003527e0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003527f0: 6272 7573 685f 7374 6162 696c 697a 6572  brush_stabilizer
+00352800: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352810: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
 00352820: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
 00352830: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
-00352840: 685f 7665 7274 6578 5f63 6f6c 6f72 3a20  h_vertex_color: 
-00352850: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00352860: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352870: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352880: 7365 5f70 656e 6369 6c5f 6272 7573 685f  se_pencil_brush_
-00352890: 7665 7274 6578 5f63 6f6c 6f72 2720 3d20  vertex_color' = 
-003528a0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003528b0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-003528c0: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
-003528d0: 5f66 616c 6c6f 6666 3a20 2762 6c5f 7569  _falloff: 'bl_ui
-003528e0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003528f0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00352900: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00352910: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
-00352920: 5f66 616c 6c6f 6666 2720 3d20 4e6f 6e65  _falloff' = None
-00352930: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352940: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352950: 6272 7573 685f 7665 7274 6578 5f70 616c  brush_vertex_pal
-00352960: 6574 7465 3a20 2762 6c5f 7569 2e73 7061  ette: 'bl_ui.spa
-00352970: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352980: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352990: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-003529a0: 6272 7573 685f 7665 7274 6578 5f70 616c  brush_vertex_pal
-003529b0: 6574 7465 2720 3d20 4e6f 6e65 0a0a 5649  ette' = None..VI
-003529c0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-003529d0: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
-003529e0: 685f 7765 6967 6874 5f66 616c 6c6f 6666  h_weight_falloff
-003529f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00352a00: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00352a10: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00352a20: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
-00352a30: 685f 7765 6967 6874 5f66 616c 6c6f 6666  h_weight_falloff
-00352a40: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00352a50: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
-00352a60: 5f70 656e 6369 6c5f 7061 696e 745f 6170  _pencil_paint_ap
-00352a70: 7065 6172 616e 6365 3a20 2762 6c5f 7569  pearance: 'bl_ui
-00352a80: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00352a90: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00352aa0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
-00352ab0: 6369 6c5f 7061 696e 745f 6170 7065 6172  cil_paint_appear
-00352ac0: 616e 6365 2720 3d20 4e6f 6e65 0a0a 5649  ance' = None..VI
-00352ad0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00352ae0: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
-00352af0: 7074 5f61 7070 6561 7261 6e63 653a 2027  pt_appearance: '
-00352b00: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00352b10: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00352b20: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-00352b30: 655f 7065 6e63 696c 5f73 6375 6c70 745f  e_pencil_sculpt_
-00352b40: 6170 7065 6172 616e 6365 2720 3d20 4e6f  appearance' = No
-00352b50: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00352b60: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-00352b70: 6c5f 7363 756c 7074 5f62 7275 7368 5f61  l_sculpt_brush_a
-00352b80: 6476 616e 6365 643a 2027 626c 5f75 692e  dvanced: 'bl_ui.
-00352b90: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
-00352ba0: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
-00352bb0: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
-00352bc0: 696c 5f73 6375 6c70 745f 6272 7573 685f  il_sculpt_brush_
-00352bd0: 6164 7661 6e63 6564 2720 3d20 4e6f 6e65  advanced' = None
-00352be0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352bf0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352c00: 7363 756c 7074 5f62 7275 7368 5f70 6f70  sculpt_brush_pop
-00352c10: 6f76 6572 3a20 2762 6c5f 7569 2e73 7061  over: 'bl_ui.spa
-00352c20: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00352c30: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00352c40: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352c50: 7363 756c 7074 5f62 7275 7368 5f70 6f70  sculpt_brush_pop
-00352c60: 6f76 6572 2720 3d20 4e6f 6e65 0a0a 5649  over' = None..VI
-00352c70: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00352c80: 6561 7365 5f70 656e 6369 6c5f 7363 756c  ease_pencil_scul
-00352c90: 7074 5f73 656c 6563 743a 2027 626c 5f75  pt_select: 'bl_u
-00352ca0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00352cb0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00352cc0: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
-00352cd0: 6e63 696c 5f73 6375 6c70 745f 7365 6c65  ncil_sculpt_sele
-00352ce0: 6374 2720 3d20 4e6f 6e65 0a0a 5649 4557  ct' = None..VIEW
-00352cf0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352d00: 7365 5f70 656e 6369 6c5f 7363 756c 7074  se_pencil_sculpt
-00352d10: 5f73 6574 7469 6e67 733a 2027 626c 5f75  _settings: 'bl_u
-00352d20: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00352d30: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00352d40: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
-00352d50: 6e63 696c 5f73 6375 6c70 745f 7365 7474  ncil_sculpt_sett
-00352d60: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
-00352d70: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00352d80: 6561 7365 5f70 656e 6369 6c5f 7665 7274  ease_pencil_vert
-00352d90: 6578 5f61 7070 6561 7261 6e63 653a 2027  ex_appearance: '
-00352da0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00352db0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00352dc0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
-00352dd0: 655f 7065 6e63 696c 5f76 6572 7465 785f  e_pencil_vertex_
-00352de0: 6170 7065 6172 616e 6365 2720 3d20 4e6f  appearance' = No
-00352df0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00352e00: 6f6c 735f 6772 6561 7365 5f70 656e 6369  ols_grease_penci
-00352e10: 6c5f 7665 7274 6578 5f70 6169 6e74 5f73  l_vertex_paint_s
-00352e20: 656c 6563 743a 2027 626c 5f75 692e 7370  elect: 'bl_ui.sp
-00352e30: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
-00352e40: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
-00352e50: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
-00352e60: 5f76 6572 7465 785f 7061 696e 745f 7365  _vertex_paint_se
-00352e70: 6c65 6374 2720 3d20 4e6f 6e65 0a0a 5649  lect' = None..VI
-00352e80: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
-00352e90: 6561 7365 5f70 656e 6369 6c5f 7665 7274  ease_pencil_vert
-00352ea0: 6578 5f70 6169 6e74 5f73 6574 7469 6e67  ex_paint_setting
-00352eb0: 733a 2027 626c 5f75 692e 7370 6163 655f  s: 'bl_ui.space_
-00352ec0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-00352ed0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
-00352ee0: 7265 6173 655f 7065 6e63 696c 5f76 6572  rease_pencil_ver
-00352ef0: 7465 785f 7061 696e 745f 7365 7474 696e  tex_paint_settin
-00352f00: 6773 2720 3d20 4e6f 6e65 0a0a 5649 4557  gs' = None..VIEW
-00352f10: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352f20: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
-00352f30: 5f61 7070 6561 7261 6e63 653a 2027 626c  _appearance: 'bl
-00352f40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00352f50: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00352f60: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
-00352f70: 7065 6e63 696c 5f77 6569 6768 745f 6170  pencil_weight_ap
-00352f80: 7065 6172 616e 6365 2720 3d20 4e6f 6e65  pearance' = None
-00352f90: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00352fa0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00352fb0: 7765 6967 6874 5f6f 7074 696f 6e73 3a20  weight_options: 
-00352fc0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00352fd0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00352fe0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-00352ff0: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
-00353000: 5f6f 7074 696f 6e73 2720 3d20 4e6f 6e65  _options' = None
-00353010: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
-00353020: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
-00353030: 7765 6967 6874 5f70 6169 6e74 5f73 656c  weight_paint_sel
-00353040: 6563 743a 2027 626c 5f75 692e 7370 6163  ect: 'bl_ui.spac
-00353050: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-00353060: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353070: 5f67 7265 6173 655f 7065 6e63 696c 5f77  _grease_pencil_w
-00353080: 6569 6768 745f 7061 696e 745f 7365 6c65  eight_paint_sele
-00353090: 6374 2720 3d20 4e6f 6e65 0a0a 5649 4557  ct' = None..VIEW
-003530a0: 3344 5f50 545f 746f 6f6c 735f 6772 6561  3D_PT_tools_grea
-003530b0: 7365 5f70 656e 6369 6c5f 7765 6967 6874  se_pencil_weight
-003530c0: 5f70 6169 6e74 5f73 6574 7469 6e67 733a  _paint_settings:
-003530d0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003530e0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-003530f0: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
-00353100: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
-00353110: 745f 7061 696e 745f 7365 7474 696e 6773  t_paint_settings
-00353120: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00353130: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
-00353140: 6169 6e74 5f6f 7074 696f 6e73 3a20 2762  aint_options: 'b
-00353150: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00353160: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00353170: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
-00353180: 6169 6e74 5f6f 7074 696f 6e73 2720 3d20  aint_options' = 
-00353190: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003531a0: 746f 6f6c 735f 696d 6167 6570 6169 6e74  tools_imagepaint
-003531b0: 5f6f 7074 696f 6e73 5f63 6176 6974 793a  _options_cavity:
-003531c0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
-003531d0: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
-003531e0: 5733 445f 5054 5f74 6f6f 6c73 5f69 6d61  W3D_PT_tools_ima
-003531f0: 6765 7061 696e 745f 6f70 7469 6f6e 735f  gepaint_options_
-00353200: 6361 7669 7479 2720 3d20 4e6f 6e65 0a0a  cavity' = None..
-00353210: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00353220: 696d 6167 6570 6169 6e74 5f6f 7074 696f  imagepaint_optio
-00353230: 6e73 5f65 7874 6572 6e61 6c3a 2027 626c  ns_external: 'bl
-00353240: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00353250: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
-00353260: 5054 5f74 6f6f 6c73 5f69 6d61 6765 7061  PT_tools_imagepa
-00353270: 696e 745f 6f70 7469 6f6e 735f 6578 7465  int_options_exte
-00353280: 726e 616c 2720 3d20 4e6f 6e65 0a0a 5649  rnal' = None..VI
-00353290: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
-003532a0: 6167 6570 6169 6e74 5f73 796d 6d65 7472  agepaint_symmetr
-003532b0: 793a 2027 626c 5f75 692e 7370 6163 655f  y: 'bl_ui.space_
-003532c0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
-003532d0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f69  IEW3D_PT_tools_i
-003532e0: 6d61 6765 7061 696e 745f 7379 6d6d 6574  magepaint_symmet
-003532f0: 7279 2720 3d20 4e6f 6e65 0a0a 5649 4557  ry' = None..VIEW
-00353300: 3344 5f50 545f 746f 6f6c 735f 6d61 736b  3D_PT_tools_mask
-00353310: 5f74 6578 7475 7265 3a20 2762 6c5f 7569  _texture: 'bl_ui
-00353320: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00353330: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00353340: 746f 6f6c 735f 6d61 736b 5f74 6578 7475  tools_mask_textu
-00353350: 7265 2720 3d20 4e6f 6e65 0a0a 5649 4557  re' = None..VIEW
-00353360: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
-00353370: 6564 6974 5f6f 7074 696f 6e73 3a20 2762  edit_options: 'b
-00353380: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00353390: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-003533a0: 5f50 545f 746f 6f6c 735f 6d65 7368 6564  _PT_tools_meshed
-003533b0: 6974 5f6f 7074 696f 6e73 2720 3d20 4e6f  it_options' = No
-003533c0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003533d0: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
-003533e0: 696f 6e73 5f74 7261 6e73 666f 726d 3a20  ions_transform: 
-003533f0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00353400: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-00353410: 3344 5f50 545f 746f 6f6c 735f 6d65 7368  3D_PT_tools_mesh
-00353420: 6564 6974 5f6f 7074 696f 6e73 5f74 7261  edit_options_tra
-00353430: 6e73 666f 726d 2720 3d20 4e6f 6e65 0a0a  nsform' = None..
-00353440: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00353450: 6d65 7368 6564 6974 5f6f 7074 696f 6e73  meshedit_options
-00353460: 5f75 7673 3a20 2762 6c5f 7569 2e73 7061  _uvs: 'bl_ui.spa
-00353470: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
-00353480: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
-00353490: 735f 6d65 7368 6564 6974 5f6f 7074 696f  s_meshedit_optio
-003534a0: 6e73 5f75 7673 2720 3d20 4e6f 6e65 0a0a  ns_uvs' = None..
-003534b0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-003534c0: 6f62 6a65 6374 5f6f 7074 696f 6e73 3a20  object_options: 
-003534d0: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-003534e0: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-003534f0: 3344 5f50 545f 746f 6f6c 735f 6f62 6a65  3D_PT_tools_obje
-00353500: 6374 5f6f 7074 696f 6e73 2720 3d20 4e6f  ct_options' = No
-00353510: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00353520: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
-00353530: 6e73 5f74 7261 6e73 666f 726d 3a20 2762  ns_transform: 'b
-00353540: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
-00353550: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
-00353560: 5f50 545f 746f 6f6c 735f 6f62 6a65 6374  _PT_tools_object
-00353570: 5f6f 7074 696f 6e73 5f74 7261 6e73 666f  _options_transfo
-00353580: 726d 2720 3d20 4e6f 6e65 0a0a 5649 4557  rm' = None..VIEW
-00353590: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
-003535a0: 6963 6c65 6d6f 6465 3a20 2762 6c5f 7569  iclemode: 'bl_ui
-003535b0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003535c0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003535d0: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-003535e0: 6465 2720 3d20 4e6f 6e65 0a0a 5649 4557  de' = None..VIEW
-003535f0: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
-00353600: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
-00353610: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
-00353620: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
-00353630: 4557 3344 5f50 545f 746f 6f6c 735f 7061  EW3D_PT_tools_pa
-00353640: 7274 6963 6c65 6d6f 6465 5f6f 7074 696f  rticlemode_optio
-00353650: 6e73 2720 3d20 4e6f 6e65 0a0a 5649 4557  ns' = None..VIEW
-00353660: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
-00353670: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
-00353680: 5f64 6973 706c 6179 3a20 2762 6c5f 7569  _display: 'bl_ui
-00353690: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-003536a0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-003536b0: 746f 6f6c 735f 7061 7274 6963 6c65 6d6f  tools_particlemo
-003536c0: 6465 5f6f 7074 696f 6e73 5f64 6973 706c  de_options_displ
-003536d0: 6179 2720 3d20 4e6f 6e65 0a0a 5649 4557  ay' = None..VIEW
-003536e0: 3344 5f50 545f 746f 6f6c 735f 7061 7274  3D_PT_tools_part
-003536f0: 6963 6c65 6d6f 6465 5f6f 7074 696f 6e73  iclemode_options
-00353700: 5f73 6861 7065 6375 743a 2027 626c 5f75  _shapecut: 'bl_u
-00353710: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00353720: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00353730: 5f74 6f6f 6c73 5f70 6172 7469 636c 656d  _tools_particlem
-00353740: 6f64 655f 6f70 7469 6f6e 735f 7368 6170  ode_options_shap
-00353750: 6563 7574 2720 3d20 4e6f 6e65 0a0a 5649  ecut' = None..VI
-00353760: 4557 3344 5f50 545f 746f 6f6c 735f 706f  EW3D_PT_tools_po
-00353770: 7365 6d6f 6465 5f6f 7074 696f 6e73 3a20  semode_options: 
-00353780: 2762 6c5f 7569 2e73 7061 6365 5f76 6965  'bl_ui.space_vie
-00353790: 7733 645f 746f 6f6c 6261 722e 5649 4557  w3d_toolbar.VIEW
-003537a0: 3344 5f50 545f 746f 6f6c 735f 706f 7365  3D_PT_tools_pose
-003537b0: 6d6f 6465 5f6f 7074 696f 6e73 2720 3d20  mode_options' = 
-003537c0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
-003537d0: 746f 6f6c 735f 7665 7274 6578 7061 696e  tools_vertexpain
-003537e0: 745f 6f70 7469 6f6e 733a 2027 626c 5f75  t_options: 'bl_u
-003537f0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00353800: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00353810: 5f74 6f6f 6c73 5f76 6572 7465 7870 6169  _tools_vertexpai
-00353820: 6e74 5f6f 7074 696f 6e73 2720 3d20 4e6f  nt_options' = No
-00353830: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-00353840: 6f6c 735f 7665 7274 6578 7061 696e 745f  ols_vertexpaint_
-00353850: 7379 6d6d 6574 7279 3a20 2762 6c5f 7569  symmetry: 'bl_ui
-00353860: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
-00353870: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
-00353880: 746f 6f6c 735f 7665 7274 6578 7061 696e  tools_vertexpain
-00353890: 745f 7379 6d6d 6574 7279 2720 3d20 4e6f  t_symmetry' = No
-003538a0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
-003538b0: 6f6c 735f 7665 7274 6578 7061 696e 745f  ols_vertexpaint_
-003538c0: 7379 6d6d 6574 7279 5f66 6f72 5f74 6f70  symmetry_for_top
-003538d0: 6261 723a 2027 626c 5f75 692e 7370 6163  bar: 'bl_ui.spac
-003538e0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-003538f0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-00353900: 5f76 6572 7465 7870 6169 6e74 5f73 796d  _vertexpaint_sym
-00353910: 6d65 7472 795f 666f 725f 746f 7062 6172  metry_for_topbar
-00353920: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
-00353930: 5f50 545f 746f 6f6c 735f 7765 6967 6874  _PT_tools_weight
-00353940: 5f67 7261 6469 656e 743a 2027 626c 5f75  _gradient: 'bl_u
-00353950: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
-00353960: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
-00353970: 5f74 6f6f 6c73 5f77 6569 6768 745f 6772  _tools_weight_gr
-00353980: 6164 6965 6e74 2720 3d20 4e6f 6e65 0a0a  adient' = None..
-00353990: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-003539a0: 7765 6967 6874 7061 696e 745f 6f70 7469  weightpaint_opti
-003539b0: 6f6e 733a 2027 626c 5f75 692e 7370 6163  ons: 'bl_ui.spac
-003539c0: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
-003539d0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
-003539e0: 5f77 6569 6768 7470 6169 6e74 5f6f 7074  _weightpaint_opt
-003539f0: 696f 6e73 2720 3d20 4e6f 6e65 0a0a 5649  ions' = None..VI
-00353a00: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
-00353a10: 6967 6874 7061 696e 745f 7379 6d6d 6574  ightpaint_symmet
-00353a20: 7279 3a20 2762 6c5f 7569 2e73 7061 6365  ry: 'bl_ui.space
-00353a30: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
-00353a40: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
-00353a50: 7765 6967 6874 7061 696e 745f 7379 6d6d  weightpaint_symm
-00353a60: 6574 7279 2720 3d20 4e6f 6e65 0a0a 5649  etry' = None..VI
-00353a70: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
-00353a80: 6967 6874 7061 696e 745f 7379 6d6d 6574  ightpaint_symmet
-00353a90: 7279 5f66 6f72 5f74 6f70 6261 723a 2027  ry_for_topbar: '
-00353aa0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-00353ab0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
-00353ac0: 445f 5054 5f74 6f6f 6c73 5f77 6569 6768  D_PT_tools_weigh
-00353ad0: 7470 6169 6e74 5f73 796d 6d65 7472 795f  tpaint_symmetry_
-00353ae0: 666f 725f 746f 7062 6172 2720 3d20 4e6f  for_topbar' = No
-00353af0: 6e65 0a0a 5649 4557 3344 5f50 545f 7472  ne..VIEW3D_PT_tr
-00353b00: 616e 7366 6f72 6d5f 6f72 6965 6e74 6174  ansform_orientat
-00353b10: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
-00353b20: 6365 5f76 6965 7733 642e 5649 4557 3344  ce_view3d.VIEW3D
-00353b30: 5f50 545f 7472 616e 7366 6f72 6d5f 6f72  _PT_transform_or
-00353b40: 6965 6e74 6174 696f 6e73 2720 3d20 4e6f  ientations' = No
-00353b50: 6e65 0a0a 5649 4557 3344 5f50 545f 7669  ne..VIEW3D_PT_vi
-00353b60: 6577 3364 5f63 7572 736f 723a 2027 626c  ew3d_cursor: 'bl
-00353b70: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
-00353b80: 2e56 4945 5733 445f 5054 5f76 6965 7733  .VIEW3D_PT_view3
-00353b90: 645f 6375 7273 6f72 2720 3d20 4e6f 6e65  d_cursor' = None
-00353ba0: 0a0a 5649 4557 3344 5f50 545f 7669 6577  ..VIEW3D_PT_view
-00353bb0: 3364 5f6c 6f63 6b3a 2027 626c 5f75 692e  3d_lock: 'bl_ui.
-00353bc0: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00353bd0: 5733 445f 5054 5f76 6965 7733 645f 6c6f  W3D_PT_view3d_lo
-00353be0: 636b 2720 3d20 4e6f 6e65 0a0a 5649 4557  ck' = None..VIEW
-00353bf0: 3344 5f50 545f 7669 6577 3364 5f70 726f  3D_PT_view3d_pro
-00353c00: 7065 7274 6965 733a 2027 626c 5f75 692e  perties: 'bl_ui.
-00353c10: 7370 6163 655f 7669 6577 3364 2e56 4945  space_view3d.VIE
-00353c20: 5733 445f 5054 5f76 6965 7733 645f 7072  W3D_PT_view3d_pr
-00353c30: 6f70 6572 7469 6573 2720 3d20 4e6f 6e65  operties' = None
-00353c40: 0a0a 5649 4557 3344 5f50 545f 7669 6577  ..VIEW3D_PT_view
-00353c50: 3364 5f73 7465 7265 6f3a 2027 626c 5f75  3d_stereo: 'bl_u
-00353c60: 692e 7370 6163 655f 7669 6577 3364 2e56  i.space_view3d.V
-00353c70: 4945 5733 445f 5054 5f76 6965 7733 645f  IEW3D_PT_view3d_
-00353c80: 7374 6572 656f 2720 3d20 4e6f 6e65 0a0a  stereo' = None..
-00353c90: 5649 4557 3344 5f50 545f 7669 6577 706f  VIEW3D_PT_viewpo
-00353ca0: 7274 5f64 6562 7567 3a20 2762 6c5f 7569  rt_debug: 'bl_ui
-00353cb0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
-00353cc0: 4557 3344 5f50 545f 7669 6577 706f 7274  EW3D_PT_viewport
-00353cd0: 5f64 6562 7567 2720 3d20 4e6f 6e65 0a0a  _debug' = None..
-00353ce0: 5649 4557 4c41 5945 525f 4d54 5f6c 6967  VIEWLAYER_MT_lig
-00353cf0: 6874 6772 6f75 705f 7379 6e63 3a20 2762  htgroup_sync: 'b
-00353d00: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00353d10: 7669 6577 5f6c 6179 6572 2e56 4945 574c  view_layer.VIEWL
-00353d20: 4159 4552 5f4d 545f 6c69 6768 7467 726f  AYER_MT_lightgro
-00353d30: 7570 5f73 796e 6327 203d 204e 6f6e 650a  up_sync' = None.
-00353d40: 0a56 4945 574c 4159 4552 5f50 545f 6565  .VIEWLAYER_PT_ee
-00353d50: 7665 655f 6c61 7965 725f 7061 7373 6573  vee_layer_passes
-00353d60: 5f64 6174 613a 2027 626c 5f75 692e 7072  _data: 'bl_ui.pr
-00353d70: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-00353d80: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
-00353d90: 5f65 6576 6565 5f6c 6179 6572 5f70 6173  _eevee_layer_pas
-00353da0: 7365 735f 6461 7461 2720 3d20 4e6f 6e65  ses_data' = None
-00353db0: 0a0a 5649 4557 4c41 5945 525f 5054 5f65  ..VIEWLAYER_PT_e
-00353dc0: 6576 6565 5f6c 6179 6572 5f70 6173 7365  evee_layer_passe
-00353dd0: 735f 6566 6665 6374 733a 2027 626c 5f75  s_effects: 'bl_u
-00353de0: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
-00353df0: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
-00353e00: 525f 5054 5f65 6576 6565 5f6c 6179 6572  R_PT_eevee_layer
-00353e10: 5f70 6173 7365 735f 6566 6665 6374 7327  _passes_effects'
-00353e20: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-00353e30: 4552 5f50 545f 6565 7665 655f 6c61 7965  ER_PT_eevee_laye
-00353e40: 725f 7061 7373 6573 5f6c 6967 6874 3a20  r_passes_light: 
-00353e50: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00353e60: 735f 7669 6577 5f6c 6179 6572 2e56 4945  s_view_layer.VIE
-00353e70: 574c 4159 4552 5f50 545f 6565 7665 655f  WLAYER_PT_eevee_
-00353e80: 6c61 7965 725f 7061 7373 6573 5f6c 6967  layer_passes_lig
-00353e90: 6874 2720 3d20 4e6f 6e65 0a0a 5649 4557  ht' = None..VIEW
-00353ea0: 4c41 5945 525f 5054 5f65 6576 6565 5f6e  LAYER_PT_eevee_n
-00353eb0: 6578 745f 6c61 7965 725f 7061 7373 6573  ext_layer_passes
-00353ec0: 5f64 6174 613a 2027 626c 5f75 692e 7072  _data: 'bl_ui.pr
-00353ed0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-00353ee0: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
-00353ef0: 5f65 6576 6565 5f6e 6578 745f 6c61 7965  _eevee_next_laye
-00353f00: 725f 7061 7373 6573 5f64 6174 6127 203d  r_passes_data' =
-00353f10: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00353f20: 5f50 545f 6672 6565 7374 796c 653a 2027  _PT_freestyle: '
-00353f30: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00353f40: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
-00353f50: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00353f60: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
-00353f70: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00353f80: 655f 6564 6765 5f64 6574 6563 7469 6f6e  e_edge_detection
-00353f90: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00353fa0: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
-00353fb0: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
-00353fc0: 7479 6c65 5f65 6467 655f 6465 7465 6374  tyle_edge_detect
-00353fd0: 696f 6e27 203d 204e 6f6e 650a 0a56 4945  ion' = None..VIE
-00353fe0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00353ff0: 796c 655f 6c69 6e65 7365 743a 2027 626c  yle_lineset: 'bl
-00354000: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-00354010: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
-00354020: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-00354030: 6c69 6e65 7365 7427 203d 204e 6f6e 650a  lineset' = None.
-00354040: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00354050: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
-00354060: 636f 6c6c 6563 7469 6f6e 3a20 2762 6c5f  collection: 'bl_
-00354070: 7569 2e70 726f 7065 7274 6965 735f 6672  ui.properties_fr
-00354080: 6565 7374 796c 652e 5649 4557 4c41 5945  eestyle.VIEWLAYE
-00354090: 525f 5054 5f66 7265 6573 7479 6c65 5f6c  R_PT_freestyle_l
-003540a0: 696e 6573 6574 5f63 6f6c 6c65 6374 696f  ineset_collectio
-003540b0: 6e27 203d 204e 6f6e 650a 0a56 4945 574c  n' = None..VIEWL
-003540c0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-003540d0: 655f 6c69 6e65 7365 745f 6564 6765 7479  e_lineset_edgety
-003540e0: 7065 3a20 2762 6c5f 7569 2e70 726f 7065  pe: 'bl_ui.prope
-003540f0: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-00354100: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00354110: 6573 7479 6c65 5f6c 696e 6573 6574 5f65  estyle_lineset_e
-00354120: 6467 6574 7970 6527 203d 204e 6f6e 650a  dgetype' = None.
-00354130: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00354140: 6565 7374 796c 655f 6c69 6e65 7365 745f  eestyle_lineset_
-00354150: 6661 6365 6d61 726b 733a 2027 626c 5f75  facemarks: 'bl_u
-00354160: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00354170: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00354180: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00354190: 6e65 7365 745f 6661 6365 6d61 726b 7327  neset_facemarks'
-003541a0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-003541b0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003541c0: 6c69 6e65 7365 745f 7669 7369 6269 6c74  lineset_visibilt
-003541d0: 793a 2027 626c 5f75 692e 7072 6f70 6572  y: 'bl_ui.proper
-003541e0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-003541f0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00354200: 7374 796c 655f 6c69 6e65 7365 745f 7669  style_lineset_vi
-00354210: 7369 6269 6c74 7927 203d 204e 6f6e 650a  sibilty' = None.
-00354220: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
-00354230: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
-00354240: 655f 616c 7068 613a 2027 626c 5f75 692e  e_alpha: 'bl_ui.
-00354250: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00354260: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00354270: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-00354280: 7374 796c 655f 616c 7068 6127 203d 204e  style_alpha' = N
-00354290: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-003542a0: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-003542b0: 7374 796c 655f 636f 6c6f 723a 2027 626c  style_color: 'bl
-003542c0: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-003542d0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
-003542e0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003542f0: 6c69 6e65 7374 796c 655f 636f 6c6f 7227  linestyle_color'
-00354300: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
-00354310: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-00354320: 6c69 6e65 7374 796c 655f 6765 6f6d 6574  linestyle_geomet
-00354330: 7279 3a20 2762 6c5f 7569 2e70 726f 7065  ry: 'bl_ui.prope
-00354340: 7274 6965 735f 6672 6565 7374 796c 652e  rties_freestyle.
-00354350: 5649 4557 4c41 5945 525f 5054 5f66 7265  VIEWLAYER_PT_fre
-00354360: 6573 7479 6c65 5f6c 696e 6573 7479 6c65  estyle_linestyle
-00354370: 5f67 656f 6d65 7472 7927 203d 204e 6f6e  _geometry' = Non
-00354380: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00354390: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-003543a0: 796c 655f 7374 726f 6b65 733a 2027 626c  yle_strokes: 'bl
-003543b0: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
-003543c0: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
-003543d0: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
-003543e0: 6c69 6e65 7374 796c 655f 7374 726f 6b65  linestyle_stroke
-003543f0: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
-00354400: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00354410: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-00354420: 6b65 735f 6368 6169 6e69 6e67 3a20 2762  kes_chaining: 'b
-00354430: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00354440: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
-00354450: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
-00354460: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
-00354470: 6573 5f63 6861 696e 696e 6727 203d 204e  es_chaining' = N
-00354480: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00354490: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-003544a0: 7374 796c 655f 7374 726f 6b65 735f 6461  style_strokes_da
-003544b0: 7368 6564 6c69 6e65 3a20 2762 6c5f 7569  shedline: 'bl_ui
-003544c0: 2e70 726f 7065 7274 6965 735f 6672 6565  .properties_free
-003544d0: 7374 796c 652e 5649 4557 4c41 5945 525f  style.VIEWLAYER_
-003544e0: 5054 5f66 7265 6573 7479 6c65 5f6c 696e  PT_freestyle_lin
-003544f0: 6573 7479 6c65 5f73 7472 6f6b 6573 5f64  estyle_strokes_d
-00354500: 6173 6865 646c 696e 6527 203d 204e 6f6e  ashedline' = Non
-00354510: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00354520: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-00354530: 796c 655f 7374 726f 6b65 735f 7365 6c65  yle_strokes_sele
-00354540: 6374 696f 6e3a 2027 626c 5f75 692e 7072  ction: 'bl_ui.pr
-00354550: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
-00354560: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
-00354570: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-00354580: 796c 655f 7374 726f 6b65 735f 7365 6c65  yle_strokes_sele
-00354590: 6374 696f 6e27 203d 204e 6f6e 650a 0a56  ction' = None..V
-003545a0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-003545b0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-003545c0: 7374 726f 6b65 735f 736f 7274 696e 673a  strokes_sorting:
-003545d0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-003545e0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
-003545f0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
-00354600: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
-00354610: 726f 6b65 735f 736f 7274 696e 6727 203d  rokes_sorting' =
-00354620: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00354630: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00354640: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
-00354650: 7370 6c69 7474 696e 673a 2027 626c 5f75  splitting: 'bl_u
-00354660: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00354670: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00354680: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-00354690: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
-003546a0: 7370 6c69 7474 696e 6727 203d 204e 6f6e  splitting' = Non
-003546b0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-003546c0: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
-003546d0: 796c 655f 7374 726f 6b65 735f 7370 6c69  yle_strokes_spli
-003546e0: 7474 696e 675f 7061 7474 6572 6e3a 2027  tting_pattern: '
-003546f0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00354700: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
-00354710: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
-00354720: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
-00354730: 6b65 735f 7370 6c69 7474 696e 675f 7061  kes_splitting_pa
-00354740: 7474 6572 6e27 203d 204e 6f6e 650a 0a56  ttern' = None..V
-00354750: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00354760: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00354770: 7465 7874 7572 653a 2027 626c 5f75 692e  texture: 'bl_ui.
-00354780: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00354790: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-003547a0: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
-003547b0: 7374 796c 655f 7465 7874 7572 6527 203d  style_texture' =
-003547c0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-003547d0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
-003547e0: 6e65 7374 796c 655f 7468 6963 6b6e 6573  nestyle_thicknes
-003547f0: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
-00354800: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
-00354810: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
-00354820: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
-00354830: 7468 6963 6b6e 6573 7327 203d 204e 6f6e  thickness' = Non
-00354840: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-00354850: 6672 6565 7374 796c 655f 7374 796c 655f  freestyle_style_
-00354860: 6d6f 6475 6c65 733a 2027 626c 5f75 692e  modules: 'bl_ui.
-00354870: 7072 6f70 6572 7469 6573 5f66 7265 6573  properties_frees
-00354880: 7479 6c65 2e56 4945 574c 4159 4552 5f50  tyle.VIEWLAYER_P
-00354890: 545f 6672 6565 7374 796c 655f 7374 796c  T_freestyle_styl
-003548a0: 655f 6d6f 6475 6c65 7327 203d 204e 6f6e  e_modules' = Non
-003548b0: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
-003548c0: 6c61 7965 723a 2027 626c 5f75 692e 7072  layer: 'bl_ui.pr
-003548d0: 6f70 6572 7469 6573 5f76 6965 775f 6c61  operties_view_la
-003548e0: 7965 722e 5649 4557 4c41 5945 525f 5054  yer.VIEWLAYER_PT
-003548f0: 5f6c 6179 6572 2720 3d20 4e6f 6e65 0a0a  _layer' = None..
-00354900: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
-00354910: 6572 5f63 7573 746f 6d5f 7072 6f70 733a  er_custom_props:
-00354920: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00354930: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
-00354940: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
-00354950: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
+00352840: 685f 7374 6162 696c 697a 6572 2720 3d20  h_stabilizer' = 
+00352850: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00352860: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352870: 6369 6c5f 6272 7573 685f 7374 726f 6b65  cil_brush_stroke
+00352880: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00352890: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+003528a0: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+003528b0: 6561 7365 5f70 656e 6369 6c5f 6272 7573  ease_pencil_brus
+003528c0: 685f 7374 726f 6b65 2720 3d20 4e6f 6e65  h_stroke' = None
+003528d0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+003528e0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+003528f0: 6272 7573 685f 7665 7274 6578 5f63 6f6c  brush_vertex_col
+00352900: 6f72 3a20 2762 6c5f 7569 2e73 7061 6365  or: 'bl_ui.space
+00352910: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00352920: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352930: 6772 6561 7365 5f70 656e 6369 6c5f 6272  grease_pencil_br
+00352940: 7573 685f 7665 7274 6578 5f63 6f6c 6f72  ush_vertex_color
+00352950: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00352960: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00352970: 5f70 656e 6369 6c5f 6272 7573 685f 7665  _pencil_brush_ve
+00352980: 7274 6578 5f66 616c 6c6f 6666 3a20 2762  rtex_falloff: 'b
+00352990: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003529a0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+003529b0: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+003529c0: 5f70 656e 6369 6c5f 6272 7573 685f 7665  _pencil_brush_ve
+003529d0: 7274 6578 5f66 616c 6c6f 6666 2720 3d20  rtex_falloff' = 
+003529e0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003529f0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352a00: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
+00352a10: 5f70 616c 6574 7465 3a20 2762 6c5f 7569  _palette: 'bl_ui
+00352a20: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352a30: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352a40: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352a50: 6369 6c5f 6272 7573 685f 7665 7274 6578  cil_brush_vertex
+00352a60: 5f70 616c 6574 7465 2720 3d20 4e6f 6e65  _palette' = None
+00352a70: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352a80: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352a90: 6272 7573 685f 7765 6967 6874 5f66 616c  brush_weight_fal
+00352aa0: 6c6f 6666 3a20 2762 6c5f 7569 2e73 7061  loff: 'bl_ui.spa
+00352ab0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+00352ac0: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+00352ad0: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352ae0: 6272 7573 685f 7765 6967 6874 5f66 616c  brush_weight_fal
+00352af0: 6c6f 6666 2720 3d20 4e6f 6e65 0a0a 5649  loff' = None..VI
+00352b00: 4557 3344 5f50 545f 746f 6f6c 735f 6772  EW3D_PT_tools_gr
+00352b10: 6561 7365 5f70 656e 6369 6c5f 7061 696e  ease_pencil_pain
+00352b20: 745f 6170 7065 6172 616e 6365 3a20 2762  t_appearance: 'b
+00352b30: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00352b40: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00352b50: 5f50 545f 746f 6f6c 735f 6772 6561 7365  _PT_tools_grease
+00352b60: 5f70 656e 6369 6c5f 7061 696e 745f 6170  _pencil_paint_ap
+00352b70: 7065 6172 616e 6365 2720 3d20 4e6f 6e65  pearance' = None
+00352b80: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352b90: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352ba0: 7363 756c 7074 5f61 7070 6561 7261 6e63  sculpt_appearanc
+00352bb0: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+00352bc0: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00352bd0: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352be0: 7265 6173 655f 7065 6e63 696c 5f73 6375  rease_pencil_scu
+00352bf0: 6c70 745f 6170 7065 6172 616e 6365 2720  lpt_appearance' 
+00352c00: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00352c10: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
+00352c20: 656e 6369 6c5f 7363 756c 7074 5f62 7275  encil_sculpt_bru
+00352c30: 7368 5f61 6476 616e 6365 643a 2027 626c  sh_advanced: 'bl
+00352c40: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00352c50: 5f74 6f6f 6c62 6172 2e56 4945 5733 445f  _toolbar.VIEW3D_
+00352c60: 5054 5f74 6f6f 6c73 5f67 7265 6173 655f  PT_tools_grease_
+00352c70: 7065 6e63 696c 5f73 6375 6c70 745f 6272  pencil_sculpt_br
+00352c80: 7573 685f 6164 7661 6e63 6564 2720 3d20  ush_advanced' = 
+00352c90: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00352ca0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352cb0: 6369 6c5f 7363 756c 7074 5f62 7275 7368  cil_sculpt_brush
+00352cc0: 5f70 6f70 6f76 6572 3a20 2762 6c5f 7569  _popover: 'bl_ui
+00352cd0: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00352ce0: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00352cf0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00352d00: 6369 6c5f 7363 756c 7074 5f62 7275 7368  cil_sculpt_brush
+00352d10: 5f70 6f70 6f76 6572 2720 3d20 4e6f 6e65  _popover' = None
+00352d20: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352d30: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352d40: 7363 756c 7074 5f73 656c 6563 743a 2027  sculpt_select: '
+00352d50: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352d60: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00352d70: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352d80: 655f 7065 6e63 696c 5f73 6375 6c70 745f  e_pencil_sculpt_
+00352d90: 7365 6c65 6374 2720 3d20 4e6f 6e65 0a0a  select' = None..
+00352da0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352db0: 6772 6561 7365 5f70 656e 6369 6c5f 7363  grease_pencil_sc
+00352dc0: 756c 7074 5f73 6574 7469 6e67 733a 2027  ulpt_settings: '
+00352dd0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00352de0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00352df0: 445f 5054 5f74 6f6f 6c73 5f67 7265 6173  D_PT_tools_greas
+00352e00: 655f 7065 6e63 696c 5f73 6375 6c70 745f  e_pencil_sculpt_
+00352e10: 7365 7474 696e 6773 2720 3d20 4e6f 6e65  settings' = None
+00352e20: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352e30: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352e40: 7665 7274 6578 5f61 7070 6561 7261 6e63  vertex_appearanc
+00352e50: 653a 2027 626c 5f75 692e 7370 6163 655f  e: 'bl_ui.space_
+00352e60: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00352e70: 4945 5733 445f 5054 5f74 6f6f 6c73 5f67  IEW3D_PT_tools_g
+00352e80: 7265 6173 655f 7065 6e63 696c 5f76 6572  rease_pencil_ver
+00352e90: 7465 785f 6170 7065 6172 616e 6365 2720  tex_appearance' 
+00352ea0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00352eb0: 545f 746f 6f6c 735f 6772 6561 7365 5f70  T_tools_grease_p
+00352ec0: 656e 6369 6c5f 7665 7274 6578 5f70 6169  encil_vertex_pai
+00352ed0: 6e74 5f73 656c 6563 743a 2027 626c 5f75  nt_select: 'bl_u
+00352ee0: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00352ef0: 6f6f 6c62 6172 2e56 4945 5733 445f 5054  oolbar.VIEW3D_PT
+00352f00: 5f74 6f6f 6c73 5f67 7265 6173 655f 7065  _tools_grease_pe
+00352f10: 6e63 696c 5f76 6572 7465 785f 7061 696e  ncil_vertex_pain
+00352f20: 745f 7365 6c65 6374 2720 3d20 4e6f 6e65  t_select' = None
+00352f30: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00352f40: 735f 6772 6561 7365 5f70 656e 6369 6c5f  s_grease_pencil_
+00352f50: 7665 7274 6578 5f70 6169 6e74 5f73 6574  vertex_paint_set
+00352f60: 7469 6e67 733a 2027 626c 5f75 692e 7370  tings: 'bl_ui.sp
+00352f70: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00352f80: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00352f90: 6c73 5f67 7265 6173 655f 7065 6e63 696c  ls_grease_pencil
+00352fa0: 5f76 6572 7465 785f 7061 696e 745f 7365  _vertex_paint_se
+00352fb0: 7474 696e 6773 2720 3d20 4e6f 6e65 0a0a  ttings' = None..
+00352fc0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00352fd0: 6772 6561 7365 5f70 656e 6369 6c5f 7765  grease_pencil_we
+00352fe0: 6967 6874 5f61 7070 6561 7261 6e63 653a  ight_appearance:
+00352ff0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353000: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353010: 5733 445f 5054 5f74 6f6f 6c73 5f67 7265  W3D_PT_tools_gre
+00353020: 6173 655f 7065 6e63 696c 5f77 6569 6768  ase_pencil_weigh
+00353030: 745f 6170 7065 6172 616e 6365 2720 3d20  t_appearance' = 
+00353040: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00353050: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+00353060: 6369 6c5f 7765 6967 6874 5f6f 7074 696f  cil_weight_optio
+00353070: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
+00353080: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00353090: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003530a0: 6772 6561 7365 5f70 656e 6369 6c5f 7765  grease_pencil_we
+003530b0: 6967 6874 5f6f 7074 696f 6e73 2720 3d20  ight_options' = 
+003530c0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+003530d0: 746f 6f6c 735f 6772 6561 7365 5f70 656e  tools_grease_pen
+003530e0: 6369 6c5f 7765 6967 6874 5f70 6169 6e74  cil_weight_paint
+003530f0: 5f73 656c 6563 743a 2027 626c 5f75 692e  _select: 'bl_ui.
+00353100: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00353110: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00353120: 6f6f 6c73 5f67 7265 6173 655f 7065 6e63  ools_grease_penc
+00353130: 696c 5f77 6569 6768 745f 7061 696e 745f  il_weight_paint_
+00353140: 7365 6c65 6374 2720 3d20 4e6f 6e65 0a0a  select' = None..
+00353150: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353160: 6772 6561 7365 5f70 656e 6369 6c5f 7765  grease_pencil_we
+00353170: 6967 6874 5f70 6169 6e74 5f73 6574 7469  ight_paint_setti
+00353180: 6e67 733a 2027 626c 5f75 692e 7370 6163  ngs: 'bl_ui.spac
+00353190: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+003531a0: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003531b0: 5f67 7265 6173 655f 7065 6e63 696c 5f77  _grease_pencil_w
+003531c0: 6569 6768 745f 7061 696e 745f 7365 7474  eight_paint_sett
+003531d0: 696e 6773 2720 3d20 4e6f 6e65 0a0a 5649  ings' = None..VI
+003531e0: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
+003531f0: 6167 6570 6169 6e74 5f6f 7074 696f 6e73  agepaint_options
+00353200: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00353210: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00353220: 4557 3344 5f50 545f 746f 6f6c 735f 696d  EW3D_PT_tools_im
+00353230: 6167 6570 6169 6e74 5f6f 7074 696f 6e73  agepaint_options
+00353240: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00353250: 5f50 545f 746f 6f6c 735f 696d 6167 6570  _PT_tools_imagep
+00353260: 6169 6e74 5f6f 7074 696f 6e73 5f63 6176  aint_options_cav
+00353270: 6974 793a 2027 626c 5f75 692e 7370 6163  ity: 'bl_ui.spac
+00353280: 655f 7669 6577 3364 5f74 6f6f 6c62 6172  e_view3d_toolbar
+00353290: 2e56 4945 5733 445f 5054 5f74 6f6f 6c73  .VIEW3D_PT_tools
+003532a0: 5f69 6d61 6765 7061 696e 745f 6f70 7469  _imagepaint_opti
+003532b0: 6f6e 735f 6361 7669 7479 2720 3d20 4e6f  ons_cavity' = No
+003532c0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+003532d0: 6f6c 735f 696d 6167 6570 6169 6e74 5f6f  ols_imagepaint_o
+003532e0: 7074 696f 6e73 5f65 7874 6572 6e61 6c3a  ptions_external:
+003532f0: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353300: 6577 3364 5f74 6f6f 6c62 6172 2e56 4945  ew3d_toolbar.VIE
+00353310: 5733 445f 5054 5f74 6f6f 6c73 5f69 6d61  W3D_PT_tools_ima
+00353320: 6765 7061 696e 745f 6f70 7469 6f6e 735f  gepaint_options_
+00353330: 6578 7465 726e 616c 2720 3d20 4e6f 6e65  external' = None
+00353340: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00353350: 735f 696d 6167 6570 6169 6e74 5f73 796d  s_imagepaint_sym
+00353360: 6d65 7472 793a 2027 626c 5f75 692e 7370  metry: 'bl_ui.sp
+00353370: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00353380: 6172 2e56 4945 5733 445f 5054 5f74 6f6f  ar.VIEW3D_PT_too
+00353390: 6c73 5f69 6d61 6765 7061 696e 745f 7379  ls_imagepaint_sy
+003533a0: 6d6d 6574 7279 2720 3d20 4e6f 6e65 0a0a  mmetry' = None..
+003533b0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003533c0: 6d61 736b 5f74 6578 7475 7265 3a20 2762  mask_texture: 'b
+003533d0: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+003533e0: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+003533f0: 5f50 545f 746f 6f6c 735f 6d61 736b 5f74  _PT_tools_mask_t
+00353400: 6578 7475 7265 2720 3d20 4e6f 6e65 0a0a  exture' = None..
+00353410: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353420: 6d65 7368 6564 6974 5f6f 7074 696f 6e73  meshedit_options
+00353430: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00353440: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00353450: 4557 3344 5f50 545f 746f 6f6c 735f 6d65  EW3D_PT_tools_me
+00353460: 7368 6564 6974 5f6f 7074 696f 6e73 2720  shedit_options' 
+00353470: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00353480: 545f 746f 6f6c 735f 6d65 7368 6564 6974  T_tools_meshedit
+00353490: 5f6f 7074 696f 6e73 5f74 7261 6e73 666f  _options_transfo
+003534a0: 726d 3a20 2762 6c5f 7569 2e73 7061 6365  rm: 'bl_ui.space
+003534b0: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+003534c0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003534d0: 6d65 7368 6564 6974 5f6f 7074 696f 6e73  meshedit_options
+003534e0: 5f74 7261 6e73 666f 726d 2720 3d20 4e6f  _transform' = No
+003534f0: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00353500: 6f6c 735f 6d65 7368 6564 6974 5f6f 7074  ols_meshedit_opt
+00353510: 696f 6e73 5f75 7673 3a20 2762 6c5f 7569  ions_uvs: 'bl_ui
+00353520: 2e73 7061 6365 5f76 6965 7733 645f 746f  .space_view3d_to
+00353530: 6f6c 6261 722e 5649 4557 3344 5f50 545f  olbar.VIEW3D_PT_
+00353540: 746f 6f6c 735f 6d65 7368 6564 6974 5f6f  tools_meshedit_o
+00353550: 7074 696f 6e73 5f75 7673 2720 3d20 4e6f  ptions_uvs' = No
+00353560: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00353570: 6f6c 735f 6f62 6a65 6374 5f6f 7074 696f  ols_object_optio
+00353580: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
+00353590: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+003535a0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003535b0: 6f62 6a65 6374 5f6f 7074 696f 6e73 2720  object_options' 
+003535c0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003535d0: 545f 746f 6f6c 735f 6f62 6a65 6374 5f6f  T_tools_object_o
+003535e0: 7074 696f 6e73 5f74 7261 6e73 666f 726d  ptions_transform
+003535f0: 3a20 2762 6c5f 7569 2e73 7061 6365 5f76  : 'bl_ui.space_v
+00353600: 6965 7733 645f 746f 6f6c 6261 722e 5649  iew3d_toolbar.VI
+00353610: 4557 3344 5f50 545f 746f 6f6c 735f 6f62  EW3D_PT_tools_ob
+00353620: 6a65 6374 5f6f 7074 696f 6e73 5f74 7261  ject_options_tra
+00353630: 6e73 666f 726d 2720 3d20 4e6f 6e65 0a0a  nsform' = None..
+00353640: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353650: 7061 7274 6963 6c65 6d6f 6465 3a20 2762  particlemode: 'b
+00353660: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353670: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00353680: 5f50 545f 746f 6f6c 735f 7061 7274 6963  _PT_tools_partic
+00353690: 6c65 6d6f 6465 2720 3d20 4e6f 6e65 0a0a  lemode' = None..
+003536a0: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003536b0: 7061 7274 6963 6c65 6d6f 6465 5f6f 7074  particlemode_opt
+003536c0: 696f 6e73 3a20 2762 6c5f 7569 2e73 7061  ions: 'bl_ui.spa
+003536d0: 6365 5f76 6965 7733 645f 746f 6f6c 6261  ce_view3d_toolba
+003536e0: 722e 5649 4557 3344 5f50 545f 746f 6f6c  r.VIEW3D_PT_tool
+003536f0: 735f 7061 7274 6963 6c65 6d6f 6465 5f6f  s_particlemode_o
+00353700: 7074 696f 6e73 2720 3d20 4e6f 6e65 0a0a  ptions' = None..
+00353710: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353720: 7061 7274 6963 6c65 6d6f 6465 5f6f 7074  particlemode_opt
+00353730: 696f 6e73 5f64 6973 706c 6179 3a20 2762  ions_display: 'b
+00353740: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353750: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00353760: 5f50 545f 746f 6f6c 735f 7061 7274 6963  _PT_tools_partic
+00353770: 6c65 6d6f 6465 5f6f 7074 696f 6e73 5f64  lemode_options_d
+00353780: 6973 706c 6179 2720 3d20 4e6f 6e65 0a0a  isplay' = None..
+00353790: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+003537a0: 7061 7274 6963 6c65 6d6f 6465 5f6f 7074  particlemode_opt
+003537b0: 696f 6e73 5f73 6861 7065 6375 743a 2027  ions_shapecut: '
+003537c0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003537d0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003537e0: 445f 5054 5f74 6f6f 6c73 5f70 6172 7469  D_PT_tools_parti
+003537f0: 636c 656d 6f64 655f 6f70 7469 6f6e 735f  clemode_options_
+00353800: 7368 6170 6563 7574 2720 3d20 4e6f 6e65  shapecut' = None
+00353810: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00353820: 735f 706f 7365 6d6f 6465 5f6f 7074 696f  s_posemode_optio
+00353830: 6e73 3a20 2762 6c5f 7569 2e73 7061 6365  ns: 'bl_ui.space
+00353840: 5f76 6965 7733 645f 746f 6f6c 6261 722e  _view3d_toolbar.
+00353850: 5649 4557 3344 5f50 545f 746f 6f6c 735f  VIEW3D_PT_tools_
+00353860: 706f 7365 6d6f 6465 5f6f 7074 696f 6e73  posemode_options
+00353870: 2720 3d20 4e6f 6e65 0a0a 5649 4557 3344  ' = None..VIEW3D
+00353880: 5f50 545f 746f 6f6c 735f 7665 7274 6578  _PT_tools_vertex
+00353890: 7061 696e 745f 6f70 7469 6f6e 733a 2027  paint_options: '
+003538a0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+003538b0: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+003538c0: 445f 5054 5f74 6f6f 6c73 5f76 6572 7465  D_PT_tools_verte
+003538d0: 7870 6169 6e74 5f6f 7074 696f 6e73 2720  xpaint_options' 
+003538e0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+003538f0: 545f 746f 6f6c 735f 7665 7274 6578 7061  T_tools_vertexpa
+00353900: 696e 745f 7379 6d6d 6574 7279 3a20 2762  int_symmetry: 'b
+00353910: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353920: 645f 746f 6f6c 6261 722e 5649 4557 3344  d_toolbar.VIEW3D
+00353930: 5f50 545f 746f 6f6c 735f 7665 7274 6578  _PT_tools_vertex
+00353940: 7061 696e 745f 7379 6d6d 6574 7279 2720  paint_symmetry' 
+00353950: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00353960: 545f 746f 6f6c 735f 7665 7274 6578 7061  T_tools_vertexpa
+00353970: 696e 745f 7379 6d6d 6574 7279 5f66 6f72  int_symmetry_for
+00353980: 5f74 6f70 6261 723a 2027 626c 5f75 692e  _topbar: 'bl_ui.
+00353990: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+003539a0: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+003539b0: 6f6f 6c73 5f76 6572 7465 7870 6169 6e74  ools_vertexpaint
+003539c0: 5f73 796d 6d65 7472 795f 666f 725f 746f  _symmetry_for_to
+003539d0: 7062 6172 2720 3d20 4e6f 6e65 0a0a 5649  pbar' = None..VI
+003539e0: 4557 3344 5f50 545f 746f 6f6c 735f 7765  EW3D_PT_tools_we
+003539f0: 6967 6874 5f67 7261 6469 656e 743a 2027  ight_gradient: '
+00353a00: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00353a10: 3364 5f74 6f6f 6c62 6172 2e56 4945 5733  3d_toolbar.VIEW3
+00353a20: 445f 5054 5f74 6f6f 6c73 5f77 6569 6768  D_PT_tools_weigh
+00353a30: 745f 6772 6164 6965 6e74 2720 3d20 4e6f  t_gradient' = No
+00353a40: 6e65 0a0a 5649 4557 3344 5f50 545f 746f  ne..VIEW3D_PT_to
+00353a50: 6f6c 735f 7765 6967 6874 7061 696e 745f  ols_weightpaint_
+00353a60: 6f70 7469 6f6e 733a 2027 626c 5f75 692e  options: 'bl_ui.
+00353a70: 7370 6163 655f 7669 6577 3364 5f74 6f6f  space_view3d_too
+00353a80: 6c62 6172 2e56 4945 5733 445f 5054 5f74  lbar.VIEW3D_PT_t
+00353a90: 6f6f 6c73 5f77 6569 6768 7470 6169 6e74  ools_weightpaint
+00353aa0: 5f6f 7074 696f 6e73 2720 3d20 4e6f 6e65  _options' = None
+00353ab0: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00353ac0: 735f 7765 6967 6874 7061 696e 745f 7379  s_weightpaint_sy
+00353ad0: 6d6d 6574 7279 3a20 2762 6c5f 7569 2e73  mmetry: 'bl_ui.s
+00353ae0: 7061 6365 5f76 6965 7733 645f 746f 6f6c  pace_view3d_tool
+00353af0: 6261 722e 5649 4557 3344 5f50 545f 746f  bar.VIEW3D_PT_to
+00353b00: 6f6c 735f 7765 6967 6874 7061 696e 745f  ols_weightpaint_
+00353b10: 7379 6d6d 6574 7279 2720 3d20 4e6f 6e65  symmetry' = None
+00353b20: 0a0a 5649 4557 3344 5f50 545f 746f 6f6c  ..VIEW3D_PT_tool
+00353b30: 735f 7765 6967 6874 7061 696e 745f 7379  s_weightpaint_sy
+00353b40: 6d6d 6574 7279 5f66 6f72 5f74 6f70 6261  mmetry_for_topba
+00353b50: 723a 2027 626c 5f75 692e 7370 6163 655f  r: 'bl_ui.space_
+00353b60: 7669 6577 3364 5f74 6f6f 6c62 6172 2e56  view3d_toolbar.V
+00353b70: 4945 5733 445f 5054 5f74 6f6f 6c73 5f77  IEW3D_PT_tools_w
+00353b80: 6569 6768 7470 6169 6e74 5f73 796d 6d65  eightpaint_symme
+00353b90: 7472 795f 666f 725f 746f 7062 6172 2720  try_for_topbar' 
+00353ba0: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00353bb0: 545f 7472 616e 7366 6f72 6d5f 6f72 6965  T_transform_orie
+00353bc0: 6e74 6174 696f 6e73 3a20 2762 6c5f 7569  ntations: 'bl_ui
+00353bd0: 2e73 7061 6365 5f76 6965 7733 642e 5649  .space_view3d.VI
+00353be0: 4557 3344 5f50 545f 7472 616e 7366 6f72  EW3D_PT_transfor
+00353bf0: 6d5f 6f72 6965 6e74 6174 696f 6e73 2720  m_orientations' 
+00353c00: 3d20 4e6f 6e65 0a0a 5649 4557 3344 5f50  = None..VIEW3D_P
+00353c10: 545f 7669 6577 3364 5f63 7572 736f 723a  T_view3d_cursor:
+00353c20: 2027 626c 5f75 692e 7370 6163 655f 7669   'bl_ui.space_vi
+00353c30: 6577 3364 2e56 4945 5733 445f 5054 5f76  ew3d.VIEW3D_PT_v
+00353c40: 6965 7733 645f 6375 7273 6f72 2720 3d20  iew3d_cursor' = 
+00353c50: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00353c60: 7669 6577 3364 5f6c 6f63 6b3a 2027 626c  view3d_lock: 'bl
+00353c70: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00353c80: 2e56 4945 5733 445f 5054 5f76 6965 7733  .VIEW3D_PT_view3
+00353c90: 645f 6c6f 636b 2720 3d20 4e6f 6e65 0a0a  d_lock' = None..
+00353ca0: 5649 4557 3344 5f50 545f 7669 6577 3364  VIEW3D_PT_view3d
+00353cb0: 5f70 726f 7065 7274 6965 733a 2027 626c  _properties: 'bl
+00353cc0: 5f75 692e 7370 6163 655f 7669 6577 3364  _ui.space_view3d
+00353cd0: 2e56 4945 5733 445f 5054 5f76 6965 7733  .VIEW3D_PT_view3
+00353ce0: 645f 7072 6f70 6572 7469 6573 2720 3d20  d_properties' = 
+00353cf0: 4e6f 6e65 0a0a 5649 4557 3344 5f50 545f  None..VIEW3D_PT_
+00353d00: 7669 6577 3364 5f73 7465 7265 6f3a 2027  view3d_stereo: '
+00353d10: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
+00353d20: 3364 2e56 4945 5733 445f 5054 5f76 6965  3d.VIEW3D_PT_vie
+00353d30: 7733 645f 7374 6572 656f 2720 3d20 4e6f  w3d_stereo' = No
+00353d40: 6e65 0a0a 5649 4557 3344 5f50 545f 7669  ne..VIEW3D_PT_vi
+00353d50: 6577 706f 7274 5f64 6562 7567 3a20 2762  ewport_debug: 'b
+00353d60: 6c5f 7569 2e73 7061 6365 5f76 6965 7733  l_ui.space_view3
+00353d70: 642e 5649 4557 3344 5f50 545f 7669 6577  d.VIEW3D_PT_view
+00353d80: 706f 7274 5f64 6562 7567 2720 3d20 4e6f  port_debug' = No
+00353d90: 6e65 0a0a 5649 4557 4c41 5945 525f 4d54  ne..VIEWLAYER_MT
+00353da0: 5f6c 6967 6874 6772 6f75 705f 7379 6e63  _lightgroup_sync
+00353db0: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+00353dc0: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
+00353dd0: 4945 574c 4159 4552 5f4d 545f 6c69 6768  IEWLAYER_MT_ligh
+00353de0: 7467 726f 7570 5f73 796e 6327 203d 204e  tgroup_sync' = N
+00353df0: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00353e00: 545f 6565 7665 655f 6c61 7965 725f 7061  T_eevee_layer_pa
+00353e10: 7373 6573 5f64 6174 613a 2027 626c 5f75  sses_data: 'bl_u
+00353e20: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+00353e30: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
+00353e40: 525f 5054 5f65 6576 6565 5f6c 6179 6572  R_PT_eevee_layer
+00353e50: 5f70 6173 7365 735f 6461 7461 2720 3d20  _passes_data' = 
+00353e60: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
+00353e70: 5054 5f65 6576 6565 5f6c 6179 6572 5f70  PT_eevee_layer_p
+00353e80: 6173 7365 735f 6566 6665 6374 733a 2027  asses_effects: '
+00353e90: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00353ea0: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
+00353eb0: 4c41 5945 525f 5054 5f65 6576 6565 5f6c  LAYER_PT_eevee_l
+00353ec0: 6179 6572 5f70 6173 7365 735f 6566 6665  ayer_passes_effe
+00353ed0: 6374 7327 203d 204e 6f6e 650a 0a56 4945  cts' = None..VIE
+00353ee0: 574c 4159 4552 5f50 545f 6565 7665 655f  WLAYER_PT_eevee_
+00353ef0: 6c61 7965 725f 7061 7373 6573 5f6c 6967  layer_passes_lig
+00353f00: 6874 3a20 2762 6c5f 7569 2e70 726f 7065  ht: 'bl_ui.prope
+00353f10: 7274 6965 735f 7669 6577 5f6c 6179 6572  rties_view_layer
+00353f20: 2e56 4945 574c 4159 4552 5f50 545f 6565  .VIEWLAYER_PT_ee
+00353f30: 7665 655f 6c61 7965 725f 7061 7373 6573  vee_layer_passes
+00353f40: 5f6c 6967 6874 2720 3d20 4e6f 6e65 0a0a  _light' = None..
+00353f50: 5649 4557 4c41 5945 525f 5054 5f65 6576  VIEWLAYER_PT_eev
+00353f60: 6565 5f6e 6578 745f 6c61 7965 725f 7061  ee_next_layer_pa
+00353f70: 7373 6573 5f64 6174 613a 2027 626c 5f75  sses_data: 'bl_u
+00353f80: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+00353f90: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
+00353fa0: 525f 5054 5f65 6576 6565 5f6e 6578 745f  R_PT_eevee_next_
+00353fb0: 6c61 7965 725f 7061 7373 6573 5f64 6174  layer_passes_dat
+00353fc0: 6127 203d 204e 6f6e 650a 0a56 4945 574c  a' = None..VIEWL
+00353fd0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00353fe0: 653a 2027 626c 5f75 692e 7072 6f70 6572  e: 'bl_ui.proper
+00353ff0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+00354000: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00354010: 7374 796c 6527 203d 204e 6f6e 650a 0a56  style' = None..V
+00354020: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00354030: 7374 796c 655f 6564 6765 5f64 6574 6563  style_edge_detec
+00354040: 7469 6f6e 3a20 2762 6c5f 7569 2e70 726f  tion: 'bl_ui.pro
+00354050: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
+00354060: 652e 5649 4557 4c41 5945 525f 5054 5f66  e.VIEWLAYER_PT_f
+00354070: 7265 6573 7479 6c65 5f65 6467 655f 6465  reestyle_edge_de
+00354080: 7465 6374 696f 6e27 203d 204e 6f6e 650a  tection' = None.
+00354090: 0a56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+003540a0: 6565 7374 796c 655f 6c69 6e65 7365 743a  eestyle_lineset:
+003540b0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+003540c0: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+003540d0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003540e0: 796c 655f 6c69 6e65 7365 7427 203d 204e  yle_lineset' = N
+003540f0: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+00354100: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00354110: 7365 745f 636f 6c6c 6563 7469 6f6e 3a20  set_collection: 
+00354120: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354130: 735f 6672 6565 7374 796c 652e 5649 4557  s_freestyle.VIEW
+00354140: 4c41 5945 525f 5054 5f66 7265 6573 7479  LAYER_PT_freesty
+00354150: 6c65 5f6c 696e 6573 6574 5f63 6f6c 6c65  le_lineset_colle
+00354160: 6374 696f 6e27 203d 204e 6f6e 650a 0a56  ction' = None..V
+00354170: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+00354180: 7374 796c 655f 6c69 6e65 7365 745f 6564  style_lineset_ed
+00354190: 6765 7479 7065 3a20 2762 6c5f 7569 2e70  getype: 'bl_ui.p
+003541a0: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
+003541b0: 796c 652e 5649 4557 4c41 5945 525f 5054  yle.VIEWLAYER_PT
+003541c0: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+003541d0: 6574 5f65 6467 6574 7970 6527 203d 204e  et_edgetype' = N
+003541e0: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+003541f0: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+00354200: 7365 745f 6661 6365 6d61 726b 733a 2027  set_facemarks: '
+00354210: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00354220: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00354230: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00354240: 655f 6c69 6e65 7365 745f 6661 6365 6d61  e_lineset_facema
+00354250: 726b 7327 203d 204e 6f6e 650a 0a56 4945  rks' = None..VIE
+00354260: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+00354270: 796c 655f 6c69 6e65 7365 745f 7669 7369  yle_lineset_visi
+00354280: 6269 6c74 793a 2027 626c 5f75 692e 7072  bilty: 'bl_ui.pr
+00354290: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+003542a0: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
+003542b0: 6672 6565 7374 796c 655f 6c69 6e65 7365  freestyle_linese
+003542c0: 745f 7669 7369 6269 6c74 7927 203d 204e  t_visibilty' = N
+003542d0: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
+003542e0: 545f 6672 6565 7374 796c 655f 6c69 6e65  T_freestyle_line
+003542f0: 7374 796c 655f 616c 7068 613a 2027 626c  style_alpha: 'bl
+00354300: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+00354310: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+00354320: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00354330: 6c69 6e65 7374 796c 655f 616c 7068 6127  linestyle_alpha'
+00354340: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00354350: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00354360: 6c69 6e65 7374 796c 655f 636f 6c6f 723a  linestyle_color:
+00354370: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00354380: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+00354390: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003543a0: 796c 655f 6c69 6e65 7374 796c 655f 636f  yle_linestyle_co
+003543b0: 6c6f 7227 203d 204e 6f6e 650a 0a56 4945  lor' = None..VIE
+003543c0: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+003543d0: 796c 655f 6c69 6e65 7374 796c 655f 6765  yle_linestyle_ge
+003543e0: 6f6d 6574 7279 3a20 2762 6c5f 7569 2e70  ometry: 'bl_ui.p
+003543f0: 726f 7065 7274 6965 735f 6672 6565 7374  roperties_freest
+00354400: 796c 652e 5649 4557 4c41 5945 525f 5054  yle.VIEWLAYER_PT
+00354410: 5f66 7265 6573 7479 6c65 5f6c 696e 6573  _freestyle_lines
+00354420: 7479 6c65 5f67 656f 6d65 7472 7927 203d  tyle_geometry' =
+00354430: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00354440: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00354450: 6e65 7374 796c 655f 7374 726f 6b65 733a  nestyle_strokes:
+00354460: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00354470: 6573 5f66 7265 6573 7479 6c65 2e56 4945  es_freestyle.VIE
+00354480: 574c 4159 4552 5f50 545f 6672 6565 7374  WLAYER_PT_freest
+00354490: 796c 655f 6c69 6e65 7374 796c 655f 7374  yle_linestyle_st
+003544a0: 726f 6b65 7327 203d 204e 6f6e 650a 0a56  rokes' = None..V
+003544b0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+003544c0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+003544d0: 7374 726f 6b65 735f 6368 6169 6e69 6e67  strokes_chaining
+003544e0: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
+003544f0: 6965 735f 6672 6565 7374 796c 652e 5649  ies_freestyle.VI
+00354500: 4557 4c41 5945 525f 5054 5f66 7265 6573  EWLAYER_PT_frees
+00354510: 7479 6c65 5f6c 696e 6573 7479 6c65 5f73  tyle_linestyle_s
+00354520: 7472 6f6b 6573 5f63 6861 696e 696e 6727  trokes_chaining'
+00354530: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00354540: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00354550: 6c69 6e65 7374 796c 655f 7374 726f 6b65  linestyle_stroke
+00354560: 735f 6461 7368 6564 6c69 6e65 3a20 2762  s_dashedline: 'b
+00354570: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+00354580: 6672 6565 7374 796c 652e 5649 4557 4c41  freestyle.VIEWLA
+00354590: 5945 525f 5054 5f66 7265 6573 7479 6c65  YER_PT_freestyle
+003545a0: 5f6c 696e 6573 7479 6c65 5f73 7472 6f6b  _linestyle_strok
+003545b0: 6573 5f64 6173 6865 646c 696e 6527 203d  es_dashedline' =
+003545c0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+003545d0: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+003545e0: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+003545f0: 7365 6c65 6374 696f 6e3a 2027 626c 5f75  selection: 'bl_u
+00354600: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
+00354610: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
+00354620: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00354630: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00354640: 7365 6c65 6374 696f 6e27 203d 204e 6f6e  selection' = Non
+00354650: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00354660: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00354670: 796c 655f 7374 726f 6b65 735f 736f 7274  yle_strokes_sort
+00354680: 696e 673a 2027 626c 5f75 692e 7072 6f70  ing: 'bl_ui.prop
+00354690: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
+003546a0: 2e56 4945 574c 4159 4552 5f50 545f 6672  .VIEWLAYER_PT_fr
+003546b0: 6565 7374 796c 655f 6c69 6e65 7374 796c  eestyle_linestyl
+003546c0: 655f 7374 726f 6b65 735f 736f 7274 696e  e_strokes_sortin
+003546d0: 6727 203d 204e 6f6e 650a 0a56 4945 574c  g' = None..VIEWL
+003546e0: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+003546f0: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00354700: 6b65 735f 7370 6c69 7474 696e 673a 2027  kes_splitting: '
+00354710: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00354720: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00354730: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00354740: 655f 6c69 6e65 7374 796c 655f 7374 726f  e_linestyle_stro
+00354750: 6b65 735f 7370 6c69 7474 696e 6727 203d  kes_splitting' =
+00354760: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00354770: 5f50 545f 6672 6565 7374 796c 655f 6c69  _PT_freestyle_li
+00354780: 6e65 7374 796c 655f 7374 726f 6b65 735f  nestyle_strokes_
+00354790: 7370 6c69 7474 696e 675f 7061 7474 6572  splitting_patter
+003547a0: 6e3a 2027 626c 5f75 692e 7072 6f70 6572  n: 'bl_ui.proper
+003547b0: 7469 6573 5f66 7265 6573 7479 6c65 2e56  ties_freestyle.V
+003547c0: 4945 574c 4159 4552 5f50 545f 6672 6565  IEWLAYER_PT_free
+003547d0: 7374 796c 655f 6c69 6e65 7374 796c 655f  style_linestyle_
+003547e0: 7374 726f 6b65 735f 7370 6c69 7474 696e  strokes_splittin
+003547f0: 675f 7061 7474 6572 6e27 203d 204e 6f6e  g_pattern' = Non
+00354800: 650a 0a56 4945 574c 4159 4552 5f50 545f  e..VIEWLAYER_PT_
+00354810: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+00354820: 796c 655f 7465 7874 7572 653a 2027 626c  yle_texture: 'bl
+00354830: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+00354840: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+00354850: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00354860: 6c69 6e65 7374 796c 655f 7465 7874 7572  linestyle_textur
+00354870: 6527 203d 204e 6f6e 650a 0a56 4945 574c  e' = None..VIEWL
+00354880: 4159 4552 5f50 545f 6672 6565 7374 796c  AYER_PT_freestyl
+00354890: 655f 6c69 6e65 7374 796c 655f 7468 6963  e_linestyle_thic
+003548a0: 6b6e 6573 733a 2027 626c 5f75 692e 7072  kness: 'bl_ui.pr
+003548b0: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+003548c0: 6c65 2e56 4945 574c 4159 4552 5f50 545f  le.VIEWLAYER_PT_
+003548d0: 6672 6565 7374 796c 655f 6c69 6e65 7374  freestyle_linest
+003548e0: 796c 655f 7468 6963 6b6e 6573 7327 203d  yle_thickness' =
+003548f0: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
+00354900: 5f50 545f 6672 6565 7374 796c 655f 7374  _PT_freestyle_st
+00354910: 796c 655f 6d6f 6475 6c65 733a 2027 626c  yle_modules: 'bl
+00354920: 5f75 692e 7072 6f70 6572 7469 6573 5f66  _ui.properties_f
+00354930: 7265 6573 7479 6c65 2e56 4945 574c 4159  reestyle.VIEWLAY
+00354940: 4552 5f50 545f 6672 6565 7374 796c 655f  ER_PT_freestyle_
+00354950: 7374 796c 655f 6d6f 6475 6c65 7327 203d  style_modules' =
 00354960: 204e 6f6e 650a 0a56 4945 574c 4159 4552   None..VIEWLAYER
-00354970: 5f50 545f 6c61 7965 725f 7061 7373 6573  _PT_layer_passes
-00354980: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00354990: 6965 735f 7669 6577 5f6c 6179 6572 2e56  ies_view_layer.V
-003549a0: 4945 574c 4159 4552 5f50 545f 6c61 7965  IEWLAYER_PT_laye
-003549b0: 725f 7061 7373 6573 2720 3d20 4e6f 6e65  r_passes' = None
-003549c0: 0a0a 5649 4557 4c41 5945 525f 5054 5f6c  ..VIEWLAYER_PT_l
-003549d0: 6179 6572 5f70 6173 7365 735f 616f 763a  ayer_passes_aov:
-003549e0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-003549f0: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
-00354a00: 4557 4c41 5945 525f 5054 5f6c 6179 6572  EWLAYER_PT_layer
-00354a10: 5f70 6173 7365 735f 616f 7627 203d 204e  _passes_aov' = N
-00354a20: 6f6e 650a 0a56 4945 574c 4159 4552 5f50  one..VIEWLAYER_P
-00354a30: 545f 6c61 7965 725f 7061 7373 6573 5f63  T_layer_passes_c
-00354a40: 7279 7074 6f6d 6174 7465 3a20 2762 6c5f  ryptomatte: 'bl_
-00354a50: 7569 2e70 726f 7065 7274 6965 735f 7669  ui.properties_vi
-00354a60: 6577 5f6c 6179 6572 2e56 4945 574c 4159  ew_layer.VIEWLAY
-00354a70: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
-00354a80: 6573 5f63 7279 7074 6f6d 6174 7465 2720  es_cryptomatte' 
-00354a90: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
-00354aa0: 525f 5054 5f6c 6179 6572 5f70 6173 7365  R_PT_layer_passe
-00354ab0: 735f 6c69 6768 7467 726f 7570 733a 2027  s_lightgroups: '
-00354ac0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00354ad0: 5f76 6965 775f 6c61 7965 722e 5649 4557  _view_layer.VIEW
-00354ae0: 4c41 5945 525f 5054 5f6c 6179 6572 5f70  LAYER_PT_layer_p
-00354af0: 6173 7365 735f 6c69 6768 7467 726f 7570  asses_lightgroup
-00354b00: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
-00354b10: 4159 4552 5f55 4c5f 616f 763a 2027 626c  AYER_UL_aov: 'bl
-00354b20: 5f75 692e 7072 6f70 6572 7469 6573 5f76  _ui.properties_v
-00354b30: 6965 775f 6c61 7965 722e 5649 4557 4c41  iew_layer.VIEWLA
-00354b40: 5945 525f 554c 5f61 6f76 2720 3d20 4e6f  YER_UL_aov' = No
-00354b50: 6e65 0a0a 5649 4557 4c41 5945 525f 554c  ne..VIEWLAYER_UL
-00354b60: 5f6c 696e 6573 6574 733a 2027 626c 5f75  _linesets: 'bl_u
-00354b70: 692e 7072 6f70 6572 7469 6573 5f66 7265  i.properties_fre
-00354b80: 6573 7479 6c65 2e56 4945 574c 4159 4552  estyle.VIEWLAYER
-00354b90: 5f55 4c5f 6c69 6e65 7365 7473 2720 3d20  _UL_linesets' = 
-00354ba0: 4e6f 6e65 0a0a 564f 4c55 4d45 5f55 4c5f  None..VOLUME_UL_
-00354bb0: 6772 6964 733a 2027 626c 5f75 692e 7072  grids: 'bl_ui.pr
-00354bc0: 6f70 6572 7469 6573 5f64 6174 615f 766f  operties_data_vo
-00354bd0: 6c75 6d65 2e56 4f4c 554d 455f 554c 5f67  lume.VOLUME_UL_g
-00354be0: 7269 6473 2720 3d20 4e6f 6e65 0a0a 574d  rids' = None..WM
-00354bf0: 5f4d 545f 6f70 6572 6174 6f72 5f70 7265  _MT_operator_pre
-00354c00: 7365 7473 3a20 2762 6c5f 6f70 6572 6174  sets: 'bl_operat
-00354c10: 6f72 732e 7072 6573 6574 732e 574d 5f4d  ors.presets.WM_M
-00354c20: 545f 6f70 6572 6174 6f72 5f70 7265 7365  T_operator_prese
-00354c30: 7473 2720 3d20 4e6f 6e65 0a0a 574d 5f4d  ts' = None..WM_M
-00354c40: 545f 7370 6c61 7368 3a20 2762 6c5f 6f70  T_splash: 'bl_op
-00354c50: 6572 6174 6f72 732e 776d 2e57 4d5f 4d54  erators.wm.WM_MT
-00354c60: 5f73 706c 6173 6827 203d 204e 6f6e 650a  _splash' = None.
-00354c70: 0a57 4d5f 4d54 5f73 706c 6173 685f 6162  .WM_MT_splash_ab
-00354c80: 6f75 743a 2027 626c 5f6f 7065 7261 746f  out: 'bl_operato
-00354c90: 7273 2e77 6d2e 574d 5f4d 545f 7370 6c61  rs.wm.WM_MT_spla
-00354ca0: 7368 5f61 626f 7574 2720 3d20 4e6f 6e65  sh_about' = None
-00354cb0: 0a0a 574d 5f4d 545f 7370 6c61 7368 5f71  ..WM_MT_splash_q
-00354cc0: 7569 636b 5f73 6574 7570 3a20 2762 6c5f  uick_setup: 'bl_
-00354cd0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00354ce0: 4d54 5f73 706c 6173 685f 7175 6963 6b5f  MT_splash_quick_
-00354cf0: 7365 7475 7027 203d 204e 6f6e 650a 0a57  setup' = None..W
-00354d00: 4d5f 4d54 5f74 6f6f 6c73 7973 7465 6d5f  M_MT_toolsystem_
-00354d10: 7375 626d 656e 753a 2027 626c 5f75 692e  submenu: 'bl_ui.
-00354d20: 7370 6163 655f 746f 6f6c 7379 7374 656d  space_toolsystem
-00354d30: 5f63 6f6d 6d6f 6e2e 574d 5f4d 545f 746f  _common.WM_MT_to
-00354d40: 6f6c 7379 7374 656d 5f73 7562 6d65 6e75  olsystem_submenu
-00354d50: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00354d60: 6261 7463 685f 7265 6e61 6d65 3a20 2762  batch_rename: 'b
-00354d70: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00354d80: 4d5f 4f54 5f62 6174 6368 5f72 656e 616d  M_OT_batch_renam
-00354d90: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
-00354da0: 5f62 6c65 6e64 5f73 7472 696e 6773 5f75  _blend_strings_u
-00354db0: 7466 385f 7661 6c69 6461 7465 3a20 2762  tf8_validate: 'b
-00354dc0: 6c5f 6f70 6572 6174 6f72 732e 6669 6c65  l_operators.file
-00354dd0: 2e57 4d5f 4f54 5f62 6c65 6e64 5f73 7472  .WM_OT_blend_str
-00354de0: 696e 6773 5f75 7466 385f 7661 6c69 6461  ings_utf8_valida
-00354df0: 7465 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  te' = None..WM_O
-00354e00: 545f 636f 6e74 6578 745f 636f 6c6c 6563  T_context_collec
-00354e10: 7469 6f6e 5f62 6f6f 6c65 616e 5f73 6574  tion_boolean_set
+00354970: 5f50 545f 6c61 7965 723a 2027 626c 5f75  _PT_layer: 'bl_u
+00354980: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+00354990: 775f 6c61 7965 722e 5649 4557 4c41 5945  w_layer.VIEWLAYE
+003549a0: 525f 5054 5f6c 6179 6572 2720 3d20 4e6f  R_PT_layer' = No
+003549b0: 6e65 0a0a 5649 4557 4c41 5945 525f 5054  ne..VIEWLAYER_PT
+003549c0: 5f6c 6179 6572 5f63 7573 746f 6d5f 7072  _layer_custom_pr
+003549d0: 6f70 733a 2027 626c 5f75 692e 7072 6f70  ops: 'bl_ui.prop
+003549e0: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
+003549f0: 722e 5649 4557 4c41 5945 525f 5054 5f6c  r.VIEWLAYER_PT_l
+00354a00: 6179 6572 5f63 7573 746f 6d5f 7072 6f70  ayer_custom_prop
+00354a10: 7327 203d 204e 6f6e 650a 0a56 4945 574c  s' = None..VIEWL
+00354a20: 4159 4552 5f50 545f 6c61 7965 725f 7061  AYER_PT_layer_pa
+00354a30: 7373 6573 3a20 2762 6c5f 7569 2e70 726f  sses: 'bl_ui.pro
+00354a40: 7065 7274 6965 735f 7669 6577 5f6c 6179  perties_view_lay
+00354a50: 6572 2e56 4945 574c 4159 4552 5f50 545f  er.VIEWLAYER_PT_
+00354a60: 6c61 7965 725f 7061 7373 6573 2720 3d20  layer_passes' = 
+00354a70: 4e6f 6e65 0a0a 5649 4557 4c41 5945 525f  None..VIEWLAYER_
+00354a80: 5054 5f6c 6179 6572 5f70 6173 7365 735f  PT_layer_passes_
+00354a90: 616f 763a 2027 626c 5f75 692e 7072 6f70  aov: 'bl_ui.prop
+00354aa0: 6572 7469 6573 5f76 6965 775f 6c61 7965  erties_view_laye
+00354ab0: 722e 5649 4557 4c41 5945 525f 5054 5f6c  r.VIEWLAYER_PT_l
+00354ac0: 6179 6572 5f70 6173 7365 735f 616f 7627  ayer_passes_aov'
+00354ad0: 203d 204e 6f6e 650a 0a56 4945 574c 4159   = None..VIEWLAY
+00354ae0: 4552 5f50 545f 6c61 7965 725f 7061 7373  ER_PT_layer_pass
+00354af0: 6573 5f63 7279 7074 6f6d 6174 7465 3a20  es_cryptomatte: 
+00354b00: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00354b10: 735f 7669 6577 5f6c 6179 6572 2e56 4945  s_view_layer.VIE
+00354b20: 574c 4159 4552 5f50 545f 6c61 7965 725f  WLAYER_PT_layer_
+00354b30: 7061 7373 6573 5f63 7279 7074 6f6d 6174  passes_cryptomat
+00354b40: 7465 2720 3d20 4e6f 6e65 0a0a 5649 4557  te' = None..VIEW
+00354b50: 4c41 5945 525f 5054 5f6c 6179 6572 5f70  LAYER_PT_layer_p
+00354b60: 6173 7365 735f 6c69 6768 7467 726f 7570  asses_lightgroup
+00354b70: 733a 2027 626c 5f75 692e 7072 6f70 6572  s: 'bl_ui.proper
+00354b80: 7469 6573 5f76 6965 775f 6c61 7965 722e  ties_view_layer.
+00354b90: 5649 4557 4c41 5945 525f 5054 5f6c 6179  VIEWLAYER_PT_lay
+00354ba0: 6572 5f70 6173 7365 735f 6c69 6768 7467  er_passes_lightg
+00354bb0: 726f 7570 7327 203d 204e 6f6e 650a 0a56  roups' = None..V
+00354bc0: 4945 574c 4159 4552 5f55 4c5f 616f 763a  IEWLAYER_UL_aov:
+00354bd0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
+00354be0: 6573 5f76 6965 775f 6c61 7965 722e 5649  es_view_layer.VI
+00354bf0: 4557 4c41 5945 525f 554c 5f61 6f76 2720  EWLAYER_UL_aov' 
+00354c00: 3d20 4e6f 6e65 0a0a 5649 4557 4c41 5945  = None..VIEWLAYE
+00354c10: 525f 554c 5f6c 696e 6573 6574 733a 2027  R_UL_linesets: '
+00354c20: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00354c30: 5f66 7265 6573 7479 6c65 2e56 4945 574c  _freestyle.VIEWL
+00354c40: 4159 4552 5f55 4c5f 6c69 6e65 7365 7473  AYER_UL_linesets
+00354c50: 2720 3d20 4e6f 6e65 0a0a 564f 4c55 4d45  ' = None..VOLUME
+00354c60: 5f55 4c5f 6772 6964 733a 2027 626c 5f75  _UL_grids: 'bl_u
+00354c70: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00354c80: 615f 766f 6c75 6d65 2e56 4f4c 554d 455f  a_volume.VOLUME_
+00354c90: 554c 5f67 7269 6473 2720 3d20 4e6f 6e65  UL_grids' = None
+00354ca0: 0a0a 574d 5f4d 545f 6f70 6572 6174 6f72  ..WM_MT_operator
+00354cb0: 5f70 7265 7365 7473 3a20 2762 6c5f 6f70  _presets: 'bl_op
+00354cc0: 6572 6174 6f72 732e 7072 6573 6574 732e  erators.presets.
+00354cd0: 574d 5f4d 545f 6f70 6572 6174 6f72 5f70  WM_MT_operator_p
+00354ce0: 7265 7365 7473 2720 3d20 4e6f 6e65 0a0a  resets' = None..
+00354cf0: 574d 5f4d 545f 7370 6c61 7368 3a20 2762  WM_MT_splash: 'b
+00354d00: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00354d10: 4d5f 4d54 5f73 706c 6173 6827 203d 204e  M_MT_splash' = N
+00354d20: 6f6e 650a 0a57 4d5f 4d54 5f73 706c 6173  one..WM_MT_splas
+00354d30: 685f 6162 6f75 743a 2027 626c 5f6f 7065  h_about: 'bl_ope
+00354d40: 7261 746f 7273 2e77 6d2e 574d 5f4d 545f  rators.wm.WM_MT_
+00354d50: 7370 6c61 7368 5f61 626f 7574 2720 3d20  splash_about' = 
+00354d60: 4e6f 6e65 0a0a 574d 5f4d 545f 7370 6c61  None..WM_MT_spla
+00354d70: 7368 5f71 7569 636b 5f73 6574 7570 3a20  sh_quick_setup: 
+00354d80: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00354d90: 2e57 4d5f 4d54 5f73 706c 6173 685f 7175  .WM_MT_splash_qu
+00354da0: 6963 6b5f 7365 7475 7027 203d 204e 6f6e  ick_setup' = Non
+00354db0: 650a 0a57 4d5f 4d54 5f74 6f6f 6c73 7973  e..WM_MT_toolsys
+00354dc0: 7465 6d5f 7375 626d 656e 753a 2027 626c  tem_submenu: 'bl
+00354dd0: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
+00354de0: 7374 656d 5f63 6f6d 6d6f 6e2e 574d 5f4d  stem_common.WM_M
+00354df0: 545f 746f 6f6c 7379 7374 656d 5f73 7562  T_toolsystem_sub
+00354e00: 6d65 6e75 2720 3d20 4e6f 6e65 0a0a 574d  menu' = None..WM
+00354e10: 5f4f 545f 6261 7463 685f 7265 6e61 6d65  _OT_batch_rename
 00354e20: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00354e30: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
-00354e40: 5f63 6f6c 6c65 6374 696f 6e5f 626f 6f6c  _collection_bool
-00354e50: 6561 6e5f 7365 7427 203d 204e 6f6e 650a  ean_set' = None.
-00354e60: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
-00354e70: 7963 6c65 5f61 7272 6179 3a20 2762 6c5f  ycle_array: 'bl_
-00354e80: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00354e90: 4f54 5f63 6f6e 7465 7874 5f63 7963 6c65  OT_context_cycle
-00354ea0: 5f61 7272 6179 2720 3d20 4e6f 6e65 0a0a  _array' = None..
-00354eb0: 574d 5f4f 545f 636f 6e74 6578 745f 6379  WM_OT_context_cy
-00354ec0: 636c 655f 656e 756d 3a20 2762 6c5f 6f70  cle_enum: 'bl_op
-00354ed0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00354ee0: 5f63 6f6e 7465 7874 5f63 7963 6c65 5f65  _context_cycle_e
-00354ef0: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
-00354f00: 4f54 5f63 6f6e 7465 7874 5f63 7963 6c65  OT_context_cycle
-00354f10: 5f69 6e74 3a20 2762 6c5f 6f70 6572 6174  _int: 'bl_operat
-00354f20: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00354f30: 7465 7874 5f63 7963 6c65 5f69 6e74 2720  text_cycle_int' 
-00354f40: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-00354f50: 6e74 6578 745f 6d65 6e75 5f65 6e75 6d3a  ntext_menu_enum:
-00354f60: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00354f70: 6d2e 574d 5f4f 545f 636f 6e74 6578 745f  m.WM_OT_context_
-00354f80: 6d65 6e75 5f65 6e75 6d27 203d 204e 6f6e  menu_enum' = Non
-00354f90: 650a 0a57 4d5f 4f54 5f63 6f6e 7465 7874  e..WM_OT_context
-00354fa0: 5f6d 6f64 616c 5f6d 6f75 7365 3a20 2762  _modal_mouse: 'b
-00354fb0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00354fc0: 4d5f 4f54 5f63 6f6e 7465 7874 5f6d 6f64  M_OT_context_mod
-00354fd0: 616c 5f6d 6f75 7365 2720 3d20 4e6f 6e65  al_mouse' = None
-00354fe0: 0a0a 574d 5f4f 545f 636f 6e74 6578 745f  ..WM_OT_context_
-00354ff0: 7069 655f 656e 756d 3a20 2762 6c5f 6f70  pie_enum: 'bl_op
-00355000: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00355010: 5f63 6f6e 7465 7874 5f70 6965 5f65 6e75  _context_pie_enu
-00355020: 6d27 203d 204e 6f6e 650a 0a57 4d5f 4f54  m' = None..WM_OT
-00355030: 5f63 6f6e 7465 7874 5f73 6361 6c65 5f66  _context_scale_f
-00355040: 6c6f 6174 3a20 2762 6c5f 6f70 6572 6174  loat: 'bl_operat
-00355050: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00355060: 7465 7874 5f73 6361 6c65 5f66 6c6f 6174  text_scale_float
-00355070: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00355080: 636f 6e74 6578 745f 7363 616c 655f 696e  context_scale_in
-00355090: 743a 2027 626c 5f6f 7065 7261 746f 7273  t: 'bl_operators
-003550a0: 2e77 6d2e 574d 5f4f 545f 636f 6e74 6578  .wm.WM_OT_contex
-003550b0: 745f 7363 616c 655f 696e 7427 203d 204e  t_scale_int' = N
-003550c0: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
-003550d0: 7874 5f73 6574 5f62 6f6f 6c65 616e 3a20  xt_set_boolean: 
-003550e0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-003550f0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
-00355100: 6574 5f62 6f6f 6c65 616e 2720 3d20 4e6f  et_boolean' = No
-00355110: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-00355120: 745f 7365 745f 656e 756d 3a20 2762 6c5f  t_set_enum: 'bl_
-00355130: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00355140: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f65  OT_context_set_e
-00355150: 6e75 6d27 203d 204e 6f6e 650a 0a57 4d5f  num' = None..WM_
-00355160: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f66  OT_context_set_f
-00355170: 6c6f 6174 3a20 2762 6c5f 6f70 6572 6174  loat: 'bl_operat
-00355180: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
-00355190: 7465 7874 5f73 6574 5f66 6c6f 6174 2720  text_set_float' 
-003551a0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
-003551b0: 6e74 6578 745f 7365 745f 6964 3a20 2762  ntext_set_id: 'b
-003551c0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-003551d0: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-003551e0: 5f69 6427 203d 204e 6f6e 650a 0a57 4d5f  _id' = None..WM_
-003551f0: 4f54 5f63 6f6e 7465 7874 5f73 6574 5f69  OT_context_set_i
-00355200: 6e74 3a20 2762 6c5f 6f70 6572 6174 6f72  nt: 'bl_operator
-00355210: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
-00355220: 7874 5f73 6574 5f69 6e74 2720 3d20 4e6f  xt_set_int' = No
-00355230: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
-00355240: 745f 7365 745f 7374 7269 6e67 3a20 2762  t_set_string: 'b
-00355250: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
-00355260: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
-00355270: 5f73 7472 696e 6727 203d 204e 6f6e 650a  _string' = None.
-00355280: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
-00355290: 6574 5f76 616c 7565 3a20 2762 6c5f 6f70  et_value: 'bl_op
-003552a0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-003552b0: 5f63 6f6e 7465 7874 5f73 6574 5f76 616c  _context_set_val
-003552c0: 7565 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  ue' = None..WM_O
-003552d0: 545f 636f 6e74 6578 745f 746f 6767 6c65  T_context_toggle
-003552e0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003552f0: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
-00355300: 5f74 6f67 676c 6527 203d 204e 6f6e 650a  _toggle' = None.
-00355310: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f74  .WM_OT_context_t
-00355320: 6f67 676c 655f 656e 756d 3a20 2762 6c5f  oggle_enum: 'bl_
-00355330: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
-00355340: 4f54 5f63 6f6e 7465 7874 5f74 6f67 676c  OT_context_toggl
-00355350: 655f 656e 756d 2720 3d20 4e6f 6e65 0a0a  e_enum' = None..
-00355360: 574d 5f4f 545f 646f 635f 7669 6577 3a20  WM_OT_doc_view: 
-00355370: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00355380: 2e57 4d5f 4f54 5f64 6f63 5f76 6965 7727  .WM_OT_doc_view'
-00355390: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f64   = None..WM_OT_d
-003553a0: 6f63 5f76 6965 775f 6d61 6e75 616c 3a20  oc_view_manual: 
-003553b0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-003553c0: 2e57 4d5f 4f54 5f64 6f63 5f76 6965 775f  .WM_OT_doc_view_
-003553d0: 6d61 6e75 616c 2720 3d20 4e6f 6e65 0a0a  manual' = None..
-003553e0: 574d 5f4f 545f 6472 6f70 5f62 6c65 6e64  WM_OT_drop_blend
-003553f0: 5f66 696c 653a 2027 626c 5f6f 7065 7261  _file: 'bl_opera
-00355400: 746f 7273 2e77 6d2e 574d 5f4f 545f 6472  tors.wm.WM_OT_dr
-00355410: 6f70 5f62 6c65 6e64 5f66 696c 6527 203d  op_blend_file' =
-00355420: 204e 6f6e 650a 0a57 4d5f 4f54 5f6f 7065   None..WM_OT_ope
-00355430: 7261 746f 725f 6368 6561 745f 7368 6565  rator_cheat_shee
-00355440: 743a 2027 626c 5f6f 7065 7261 746f 7273  t: 'bl_operators
-00355450: 2e77 6d2e 574d 5f4f 545f 6f70 6572 6174  .wm.WM_OT_operat
-00355460: 6f72 5f63 6865 6174 5f73 6865 6574 2720  or_cheat_sheet' 
-00355470: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 6f70  = None..WM_OT_op
-00355480: 6572 6174 6f72 5f70 6965 5f65 6e75 6d3a  erator_pie_enum:
-00355490: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-003554a0: 6d2e 574d 5f4f 545f 6f70 6572 6174 6f72  m.WM_OT_operator
-003554b0: 5f70 6965 5f65 6e75 6d27 203d 204e 6f6e  _pie_enum' = Non
-003554c0: 650a 0a57 4d5f 4f54 5f6f 776e 6572 5f64  e..WM_OT_owner_d
-003554d0: 6973 6162 6c65 3a20 2762 6c5f 6f70 6572  isable: 'bl_oper
-003554e0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f6f  ators.wm.WM_OT_o
-003554f0: 776e 6572 5f64 6973 6162 6c65 2720 3d20  wner_disable' = 
-00355500: 4e6f 6e65 0a0a 574d 5f4f 545f 6f77 6e65  None..WM_OT_owne
-00355510: 725f 656e 6162 6c65 3a20 2762 6c5f 6f70  r_enable: 'bl_op
-00355520: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
-00355530: 5f6f 776e 6572 5f65 6e61 626c 6527 203d  _owner_enable' =
-00355540: 204e 6f6e 650a 0a57 4d5f 4f54 5f70 6174   None..WM_OT_pat
-00355550: 685f 6f70 656e 3a20 2762 6c5f 6f70 6572  h_open: 'bl_oper
-00355560: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f70  ators.wm.WM_OT_p
-00355570: 6174 685f 6f70 656e 2720 3d20 4e6f 6e65  ath_open' = None
-00355580: 0a0a 574d 5f4f 545f 7072 6576 6965 7773  ..WM_OT_previews
-00355590: 5f62 6174 6368 5f63 6c65 6172 3a20 2762  _batch_clear: 'b
-003555a0: 6c5f 6f70 6572 6174 6f72 732e 6669 6c65  l_operators.file
-003555b0: 2e57 4d5f 4f54 5f70 7265 7669 6577 735f  .WM_OT_previews_
-003555c0: 6261 7463 685f 636c 6561 7227 203d 204e  batch_clear' = N
-003555d0: 6f6e 650a 0a57 4d5f 4f54 5f70 7265 7669  one..WM_OT_previ
-003555e0: 6577 735f 6261 7463 685f 6765 6e65 7261  ews_batch_genera
-003555f0: 7465 3a20 2762 6c5f 6f70 6572 6174 6f72  te: 'bl_operator
-00355600: 732e 6669 6c65 2e57 4d5f 4f54 5f70 7265  s.file.WM_OT_pre
-00355610: 7669 6577 735f 6261 7463 685f 6765 6e65  views_batch_gene
-00355620: 7261 7465 2720 3d20 4e6f 6e65 0a0a 574d  rate' = None..WM
-00355630: 5f4f 545f 7072 6f70 6572 7469 6573 5f61  _OT_properties_a
-00355640: 6464 3a20 2762 6c5f 6f70 6572 6174 6f72  dd: 'bl_operator
-00355650: 732e 776d 2e57 4d5f 4f54 5f70 726f 7065  s.wm.WM_OT_prope
-00355660: 7274 6965 735f 6164 6427 203d 204e 6f6e  rties_add' = Non
-00355670: 650a 0a57 4d5f 4f54 5f70 726f 7065 7274  e..WM_OT_propert
-00355680: 6965 735f 636f 6e74 6578 745f 6368 616e  ies_context_chan
-00355690: 6765 3a20 2762 6c5f 6f70 6572 6174 6f72  ge: 'bl_operator
-003556a0: 732e 776d 2e57 4d5f 4f54 5f70 726f 7065  s.wm.WM_OT_prope
-003556b0: 7274 6965 735f 636f 6e74 6578 745f 6368  rties_context_ch
-003556c0: 616e 6765 2720 3d20 4e6f 6e65 0a0a 574d  ange' = None..WM
-003556d0: 5f4f 545f 7072 6f70 6572 7469 6573 5f65  _OT_properties_e
-003556e0: 6469 743a 2027 626c 5f6f 7065 7261 746f  dit: 'bl_operato
-003556f0: 7273 2e77 6d2e 574d 5f4f 545f 7072 6f70  rs.wm.WM_OT_prop
-00355700: 6572 7469 6573 5f65 6469 7427 203d 204e  erties_edit' = N
-00355710: 6f6e 650a 0a57 4d5f 4f54 5f70 726f 7065  one..WM_OT_prope
-00355720: 7274 6965 735f 6564 6974 5f76 616c 7565  rties_edit_value
-00355730: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-00355740: 776d 2e57 4d5f 4f54 5f70 726f 7065 7274  wm.WM_OT_propert
-00355750: 6965 735f 6564 6974 5f76 616c 7565 2720  ies_edit_value' 
-00355760: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 7072  = None..WM_OT_pr
-00355770: 6f70 6572 7469 6573 5f72 656d 6f76 653a  operties_remove:
-00355780: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
-00355790: 6d2e 574d 5f4f 545f 7072 6f70 6572 7469  m.WM_OT_properti
-003557a0: 6573 5f72 656d 6f76 6527 203d 204e 6f6e  es_remove' = Non
-003557b0: 650a 0a57 4d5f 4f54 5f73 7973 696e 666f  e..WM_OT_sysinfo
-003557c0: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
-003557d0: 776d 2e57 4d5f 4f54 5f73 7973 696e 666f  wm.WM_OT_sysinfo
-003557e0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-003557f0: 746f 6f6c 5f73 6574 5f62 795f 6964 3a20  tool_set_by_id: 
-00355800: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
-00355810: 2e57 4d5f 4f54 5f74 6f6f 6c5f 7365 745f  .WM_OT_tool_set_
-00355820: 6279 5f69 6427 203d 204e 6f6e 650a 0a57  by_id' = None..W
-00355830: 4d5f 4f54 5f74 6f6f 6c5f 7365 745f 6279  M_OT_tool_set_by
-00355840: 5f69 6e64 6578 3a20 2762 6c5f 6f70 6572  _index: 'bl_oper
-00355850: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
-00355860: 6f6f 6c5f 7365 745f 6279 5f69 6e64 6578  ool_set_by_index
-00355870: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
-00355880: 746f 6f6c 6261 723a 2027 626c 5f6f 7065  toolbar: 'bl_ope
-00355890: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
-003558a0: 746f 6f6c 6261 7227 203d 204e 6f6e 650a  toolbar' = None.
-003558b0: 0a57 4d5f 4f54 5f74 6f6f 6c62 6172 5f66  .WM_OT_toolbar_f
-003558c0: 616c 6c62 6163 6b5f 7069 653a 2027 626c  allback_pie: 'bl
-003558d0: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
-003558e0: 5f4f 545f 746f 6f6c 6261 725f 6661 6c6c  _OT_toolbar_fall
-003558f0: 6261 636b 5f70 6965 2720 3d20 4e6f 6e65  back_pie' = None
-00355900: 0a0a 574d 5f4f 545f 746f 6f6c 6261 725f  ..WM_OT_toolbar_
-00355910: 7072 6f6d 7074 3a20 2762 6c5f 6f70 6572  prompt: 'bl_oper
-00355920: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f74  ators.wm.WM_OT_t
-00355930: 6f6f 6c62 6172 5f70 726f 6d70 7427 203d  oolbar_prompt' =
-00355940: 204e 6f6e 650a 0a57 4d5f 4f54 5f75 726c   None..WM_OT_url
-00355950: 5f6f 7065 6e3a 2027 626c 5f6f 7065 7261  _open: 'bl_opera
-00355960: 746f 7273 2e77 6d2e 574d 5f4f 545f 7572  tors.wm.WM_OT_ur
-00355970: 6c5f 6f70 656e 2720 3d20 4e6f 6e65 0a0a  l_open' = None..
-00355980: 574d 5f4f 545f 7572 6c5f 6f70 656e 5f70  WM_OT_url_open_p
-00355990: 7265 7365 743a 2027 626c 5f6f 7065 7261  reset: 'bl_opera
-003559a0: 746f 7273 2e77 6d2e 574d 5f4f 545f 7572  tors.wm.WM_OT_ur
-003559b0: 6c5f 6f70 656e 5f70 7265 7365 7427 203d  l_open_preset' =
-003559c0: 204e 6f6e 650a 0a57 4f52 4b53 5041 4345   None..WORKSPACE
-003559d0: 5f50 545f 6164 646f 6e73 3a20 2762 6c5f  _PT_addons: 'bl_
-003559e0: 7569 2e70 726f 7065 7274 6965 735f 776f  ui.properties_wo
-003559f0: 726b 7370 6163 652e 574f 524b 5350 4143  rkspace.WORKSPAC
-00355a00: 455f 5054 5f61 6464 6f6e 7327 203d 204e  E_PT_addons' = N
-00355a10: 6f6e 650a 0a57 4f52 4b53 5041 4345 5f50  one..WORKSPACE_P
-00355a20: 545f 6375 7374 6f6d 5f70 726f 7073 3a20  T_custom_props: 
-00355a30: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00355a40: 735f 776f 726b 7370 6163 652e 574f 524b  s_workspace.WORK
-00355a50: 5350 4143 455f 5054 5f63 7573 746f 6d5f  SPACE_PT_custom_
-00355a60: 7072 6f70 7327 203d 204e 6f6e 650a 0a57  props' = None..W
-00355a70: 4f52 4b53 5041 4345 5f50 545f 6d61 696e  ORKSPACE_PT_main
-00355a80: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00355a90: 6965 735f 776f 726b 7370 6163 652e 574f  ies_workspace.WO
-00355aa0: 524b 5350 4143 455f 5054 5f6d 6169 6e27  RKSPACE_PT_main'
-00355ab0: 203d 204e 6f6e 650a 0a57 4f52 4c44 5f50   = None..WORLD_P
-00355ac0: 545f 636f 6e74 6578 745f 776f 726c 643a  T_context_world:
-00355ad0: 2027 626c 5f75 692e 7072 6f70 6572 7469   'bl_ui.properti
-00355ae0: 6573 5f77 6f72 6c64 2e57 4f52 4c44 5f50  es_world.WORLD_P
-00355af0: 545f 636f 6e74 6578 745f 776f 726c 6427  T_context_world'
-00355b00: 203d 204e 6f6e 650a 0a57 4f52 4c44 5f50   = None..WORLD_P
-00355b10: 545f 6375 7374 6f6d 5f70 726f 7073 3a20  T_custom_props: 
-00355b20: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
-00355b30: 735f 776f 726c 642e 574f 524c 445f 5054  s_world.WORLD_PT
-00355b40: 5f63 7573 746f 6d5f 7072 6f70 7327 203d  _custom_props' =
-00355b50: 204e 6f6e 650a 0a57 4f52 4c44 5f50 545f   None..WORLD_PT_
-00355b60: 7669 6577 706f 7274 5f64 6973 706c 6179  viewport_display
-00355b70: 3a20 2762 6c5f 7569 2e70 726f 7065 7274  : 'bl_ui.propert
-00355b80: 6965 735f 776f 726c 642e 574f 524c 445f  ies_world.WORLD_
-00355b90: 5054 5f76 6965 7770 6f72 745f 6469 7370  PT_viewport_disp
-00355ba0: 6c61 7927 203d 204e 6f6e 650a            lay' = None.
+00354e30: 776d 2e57 4d5f 4f54 5f62 6174 6368 5f72  wm.WM_OT_batch_r
+00354e40: 656e 616d 6527 203d 204e 6f6e 650a 0a57  ename' = None..W
+00354e50: 4d5f 4f54 5f62 6c65 6e64 5f73 7472 696e  M_OT_blend_strin
+00354e60: 6773 5f75 7466 385f 7661 6c69 6461 7465  gs_utf8_validate
+00354e70: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00354e80: 6669 6c65 2e57 4d5f 4f54 5f62 6c65 6e64  file.WM_OT_blend
+00354e90: 5f73 7472 696e 6773 5f75 7466 385f 7661  _strings_utf8_va
+00354ea0: 6c69 6461 7465 2720 3d20 4e6f 6e65 0a0a  lidate' = None..
+00354eb0: 574d 5f4f 545f 636f 6e74 6578 745f 636f  WM_OT_context_co
+00354ec0: 6c6c 6563 7469 6f6e 5f62 6f6f 6c65 616e  llection_boolean
+00354ed0: 5f73 6574 3a20 2762 6c5f 6f70 6572 6174  _set: 'bl_operat
+00354ee0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+00354ef0: 7465 7874 5f63 6f6c 6c65 6374 696f 6e5f  text_collection_
+00354f00: 626f 6f6c 6561 6e5f 7365 7427 203d 204e  boolean_set' = N
+00354f10: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00354f20: 7874 5f63 7963 6c65 5f61 7272 6179 3a20  xt_cycle_array: 
+00354f30: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+00354f40: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
+00354f50: 7963 6c65 5f61 7272 6179 2720 3d20 4e6f  ycle_array' = No
+00354f60: 6e65 0a0a 574d 5f4f 545f 636f 6e74 6578  ne..WM_OT_contex
+00354f70: 745f 6379 636c 655f 656e 756d 3a20 2762  t_cycle_enum: 'b
+00354f80: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00354f90: 4d5f 4f54 5f63 6f6e 7465 7874 5f63 7963  M_OT_context_cyc
+00354fa0: 6c65 5f65 6e75 6d27 203d 204e 6f6e 650a  le_enum' = None.
+00354fb0: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f63  .WM_OT_context_c
+00354fc0: 7963 6c65 5f69 6e74 3a20 2762 6c5f 6f70  ycle_int: 'bl_op
+00354fd0: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00354fe0: 5f63 6f6e 7465 7874 5f63 7963 6c65 5f69  _context_cycle_i
+00354ff0: 6e74 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  nt' = None..WM_O
+00355000: 545f 636f 6e74 6578 745f 6d65 6e75 5f65  T_context_menu_e
+00355010: 6e75 6d3a 2027 626c 5f6f 7065 7261 746f  num: 'bl_operato
+00355020: 7273 2e77 6d2e 574d 5f4f 545f 636f 6e74  rs.wm.WM_OT_cont
+00355030: 6578 745f 6d65 6e75 5f65 6e75 6d27 203d  ext_menu_enum' =
+00355040: 204e 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e   None..WM_OT_con
+00355050: 7465 7874 5f6d 6f64 616c 5f6d 6f75 7365  text_modal_mouse
+00355060: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00355070: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00355080: 5f6d 6f64 616c 5f6d 6f75 7365 2720 3d20  _modal_mouse' = 
+00355090: 4e6f 6e65 0a0a 574d 5f4f 545f 636f 6e74  None..WM_OT_cont
+003550a0: 6578 745f 7069 655f 656e 756d 3a20 2762  ext_pie_enum: 'b
+003550b0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+003550c0: 4d5f 4f54 5f63 6f6e 7465 7874 5f70 6965  M_OT_context_pie
+003550d0: 5f65 6e75 6d27 203d 204e 6f6e 650a 0a57  _enum' = None..W
+003550e0: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6361  M_OT_context_sca
+003550f0: 6c65 5f66 6c6f 6174 3a20 2762 6c5f 6f70  le_float: 'bl_op
+00355100: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00355110: 5f63 6f6e 7465 7874 5f73 6361 6c65 5f66  _context_scale_f
+00355120: 6c6f 6174 2720 3d20 4e6f 6e65 0a0a 574d  loat' = None..WM
+00355130: 5f4f 545f 636f 6e74 6578 745f 7363 616c  _OT_context_scal
+00355140: 655f 696e 743a 2027 626c 5f6f 7065 7261  e_int: 'bl_opera
+00355150: 746f 7273 2e77 6d2e 574d 5f4f 545f 636f  tors.wm.WM_OT_co
+00355160: 6e74 6578 745f 7363 616c 655f 696e 7427  ntext_scale_int'
+00355170: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f63   = None..WM_OT_c
+00355180: 6f6e 7465 7874 5f73 6574 5f62 6f6f 6c65  ontext_set_boole
+00355190: 616e 3a20 2762 6c5f 6f70 6572 6174 6f72  an: 'bl_operator
+003551a0: 732e 776d 2e57 4d5f 4f54 5f63 6f6e 7465  s.wm.WM_OT_conte
+003551b0: 7874 5f73 6574 5f62 6f6f 6c65 616e 2720  xt_set_boolean' 
+003551c0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
+003551d0: 6e74 6578 745f 7365 745f 656e 756d 3a20  ntext_set_enum: 
+003551e0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+003551f0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
+00355200: 6574 5f65 6e75 6d27 203d 204e 6f6e 650a  et_enum' = None.
+00355210: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
+00355220: 6574 5f66 6c6f 6174 3a20 2762 6c5f 6f70  et_float: 'bl_op
+00355230: 6572 6174 6f72 732e 776d 2e57 4d5f 4f54  erators.wm.WM_OT
+00355240: 5f63 6f6e 7465 7874 5f73 6574 5f66 6c6f  _context_set_flo
+00355250: 6174 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  at' = None..WM_O
+00355260: 545f 636f 6e74 6578 745f 7365 745f 6964  T_context_set_id
+00355270: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00355280: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00355290: 5f73 6574 5f69 6427 203d 204e 6f6e 650a  _set_id' = None.
+003552a0: 0a57 4d5f 4f54 5f63 6f6e 7465 7874 5f73  .WM_OT_context_s
+003552b0: 6574 5f69 6e74 3a20 2762 6c5f 6f70 6572  et_int: 'bl_oper
+003552c0: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f63  ators.wm.WM_OT_c
+003552d0: 6f6e 7465 7874 5f73 6574 5f69 6e74 2720  ontext_set_int' 
+003552e0: 3d20 4e6f 6e65 0a0a 574d 5f4f 545f 636f  = None..WM_OT_co
+003552f0: 6e74 6578 745f 7365 745f 7374 7269 6e67  ntext_set_string
+00355300: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00355310: 776d 2e57 4d5f 4f54 5f63 6f6e 7465 7874  wm.WM_OT_context
+00355320: 5f73 6574 5f73 7472 696e 6727 203d 204e  _set_string' = N
+00355330: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+00355340: 7874 5f73 6574 5f76 616c 7565 3a20 2762  xt_set_value: 'b
+00355350: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+00355360: 4d5f 4f54 5f63 6f6e 7465 7874 5f73 6574  M_OT_context_set
+00355370: 5f76 616c 7565 2720 3d20 4e6f 6e65 0a0a  _value' = None..
+00355380: 574d 5f4f 545f 636f 6e74 6578 745f 746f  WM_OT_context_to
+00355390: 6767 6c65 3a20 2762 6c5f 6f70 6572 6174  ggle: 'bl_operat
+003553a0: 6f72 732e 776d 2e57 4d5f 4f54 5f63 6f6e  ors.wm.WM_OT_con
+003553b0: 7465 7874 5f74 6f67 676c 6527 203d 204e  text_toggle' = N
+003553c0: 6f6e 650a 0a57 4d5f 4f54 5f63 6f6e 7465  one..WM_OT_conte
+003553d0: 7874 5f74 6f67 676c 655f 656e 756d 3a20  xt_toggle_enum: 
+003553e0: 2762 6c5f 6f70 6572 6174 6f72 732e 776d  'bl_operators.wm
+003553f0: 2e57 4d5f 4f54 5f63 6f6e 7465 7874 5f74  .WM_OT_context_t
+00355400: 6f67 676c 655f 656e 756d 2720 3d20 4e6f  oggle_enum' = No
+00355410: 6e65 0a0a 574d 5f4f 545f 646f 635f 7669  ne..WM_OT_doc_vi
+00355420: 6577 3a20 2762 6c5f 6f70 6572 6174 6f72  ew: 'bl_operator
+00355430: 732e 776d 2e57 4d5f 4f54 5f64 6f63 5f76  s.wm.WM_OT_doc_v
+00355440: 6965 7727 203d 204e 6f6e 650a 0a57 4d5f  iew' = None..WM_
+00355450: 4f54 5f64 6f63 5f76 6965 775f 6d61 6e75  OT_doc_view_manu
+00355460: 616c 3a20 2762 6c5f 6f70 6572 6174 6f72  al: 'bl_operator
+00355470: 732e 776d 2e57 4d5f 4f54 5f64 6f63 5f76  s.wm.WM_OT_doc_v
+00355480: 6965 775f 6d61 6e75 616c 2720 3d20 4e6f  iew_manual' = No
+00355490: 6e65 0a0a 574d 5f4f 545f 6472 6f70 5f62  ne..WM_OT_drop_b
+003554a0: 6c65 6e64 5f66 696c 653a 2027 626c 5f6f  lend_file: 'bl_o
+003554b0: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+003554c0: 545f 6472 6f70 5f62 6c65 6e64 5f66 696c  T_drop_blend_fil
+003554d0: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
+003554e0: 5f6f 7065 7261 746f 725f 6368 6561 745f  _operator_cheat_
+003554f0: 7368 6565 743a 2027 626c 5f6f 7065 7261  sheet: 'bl_opera
+00355500: 746f 7273 2e77 6d2e 574d 5f4f 545f 6f70  tors.wm.WM_OT_op
+00355510: 6572 6174 6f72 5f63 6865 6174 5f73 6865  erator_cheat_she
+00355520: 6574 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  et' = None..WM_O
+00355530: 545f 6f70 6572 6174 6f72 5f70 6965 5f65  T_operator_pie_e
+00355540: 6e75 6d3a 2027 626c 5f6f 7065 7261 746f  num: 'bl_operato
+00355550: 7273 2e77 6d2e 574d 5f4f 545f 6f70 6572  rs.wm.WM_OT_oper
+00355560: 6174 6f72 5f70 6965 5f65 6e75 6d27 203d  ator_pie_enum' =
+00355570: 204e 6f6e 650a 0a57 4d5f 4f54 5f6f 776e   None..WM_OT_own
+00355580: 6572 5f64 6973 6162 6c65 3a20 2762 6c5f  er_disable: 'bl_
+00355590: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+003555a0: 4f54 5f6f 776e 6572 5f64 6973 6162 6c65  OT_owner_disable
+003555b0: 2720 3d20 4e6f 6e65 0a0a 574d 5f4f 545f  ' = None..WM_OT_
+003555c0: 6f77 6e65 725f 656e 6162 6c65 3a20 2762  owner_enable: 'b
+003555d0: 6c5f 6f70 6572 6174 6f72 732e 776d 2e57  l_operators.wm.W
+003555e0: 4d5f 4f54 5f6f 776e 6572 5f65 6e61 626c  M_OT_owner_enabl
+003555f0: 6527 203d 204e 6f6e 650a 0a57 4d5f 4f54  e' = None..WM_OT
+00355600: 5f70 6174 685f 6f70 656e 3a20 2762 6c5f  _path_open: 'bl_
+00355610: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00355620: 4f54 5f70 6174 685f 6f70 656e 2720 3d20  OT_path_open' = 
+00355630: 4e6f 6e65 0a0a 574d 5f4f 545f 7072 6576  None..WM_OT_prev
+00355640: 6965 7773 5f62 6174 6368 5f63 6c65 6172  iews_batch_clear
+00355650: 3a20 2762 6c5f 6f70 6572 6174 6f72 732e  : 'bl_operators.
+00355660: 6669 6c65 2e57 4d5f 4f54 5f70 7265 7669  file.WM_OT_previ
+00355670: 6577 735f 6261 7463 685f 636c 6561 7227  ews_batch_clear'
+00355680: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f70   = None..WM_OT_p
+00355690: 7265 7669 6577 735f 6261 7463 685f 6765  reviews_batch_ge
+003556a0: 6e65 7261 7465 3a20 2762 6c5f 6f70 6572  nerate: 'bl_oper
+003556b0: 6174 6f72 732e 6669 6c65 2e57 4d5f 4f54  ators.file.WM_OT
+003556c0: 5f70 7265 7669 6577 735f 6261 7463 685f  _previews_batch_
+003556d0: 6765 6e65 7261 7465 2720 3d20 4e6f 6e65  generate' = None
+003556e0: 0a0a 574d 5f4f 545f 7072 6f70 6572 7469  ..WM_OT_properti
+003556f0: 6573 5f61 6464 3a20 2762 6c5f 6f70 6572  es_add: 'bl_oper
+00355700: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f70  ators.wm.WM_OT_p
+00355710: 726f 7065 7274 6965 735f 6164 6427 203d  roperties_add' =
+00355720: 204e 6f6e 650a 0a57 4d5f 4f54 5f70 726f   None..WM_OT_pro
+00355730: 7065 7274 6965 735f 636f 6e74 6578 745f  perties_context_
+00355740: 6368 616e 6765 3a20 2762 6c5f 6f70 6572  change: 'bl_oper
+00355750: 6174 6f72 732e 776d 2e57 4d5f 4f54 5f70  ators.wm.WM_OT_p
+00355760: 726f 7065 7274 6965 735f 636f 6e74 6578  roperties_contex
+00355770: 745f 6368 616e 6765 2720 3d20 4e6f 6e65  t_change' = None
+00355780: 0a0a 574d 5f4f 545f 7072 6f70 6572 7469  ..WM_OT_properti
+00355790: 6573 5f65 6469 743a 2027 626c 5f6f 7065  es_edit: 'bl_ope
+003557a0: 7261 746f 7273 2e77 6d2e 574d 5f4f 545f  rators.wm.WM_OT_
+003557b0: 7072 6f70 6572 7469 6573 5f65 6469 7427  properties_edit'
+003557c0: 203d 204e 6f6e 650a 0a57 4d5f 4f54 5f70   = None..WM_OT_p
+003557d0: 726f 7065 7274 6965 735f 6564 6974 5f76  roperties_edit_v
+003557e0: 616c 7565 3a20 2762 6c5f 6f70 6572 6174  alue: 'bl_operat
+003557f0: 6f72 732e 776d 2e57 4d5f 4f54 5f70 726f  ors.wm.WM_OT_pro
+00355800: 7065 7274 6965 735f 6564 6974 5f76 616c  perties_edit_val
+00355810: 7565 2720 3d20 4e6f 6e65 0a0a 574d 5f4f  ue' = None..WM_O
+00355820: 545f 7072 6f70 6572 7469 6573 5f72 656d  T_properties_rem
+00355830: 6f76 653a 2027 626c 5f6f 7065 7261 746f  ove: 'bl_operato
+00355840: 7273 2e77 6d2e 574d 5f4f 545f 7072 6f70  rs.wm.WM_OT_prop
+00355850: 6572 7469 6573 5f72 656d 6f76 6527 203d  erties_remove' =
+00355860: 204e 6f6e 650a 0a57 4d5f 4f54 5f73 7973   None..WM_OT_sys
+00355870: 696e 666f 3a20 2762 6c5f 6f70 6572 6174  info: 'bl_operat
+00355880: 6f72 732e 776d 2e57 4d5f 4f54 5f73 7973  ors.wm.WM_OT_sys
+00355890: 696e 666f 2720 3d20 4e6f 6e65 0a0a 574d  info' = None..WM
+003558a0: 5f4f 545f 746f 6f6c 5f73 6574 5f62 795f  _OT_tool_set_by_
+003558b0: 6964 3a20 2762 6c5f 6f70 6572 6174 6f72  id: 'bl_operator
+003558c0: 732e 776d 2e57 4d5f 4f54 5f74 6f6f 6c5f  s.wm.WM_OT_tool_
+003558d0: 7365 745f 6279 5f69 6427 203d 204e 6f6e  set_by_id' = Non
+003558e0: 650a 0a57 4d5f 4f54 5f74 6f6f 6c5f 7365  e..WM_OT_tool_se
+003558f0: 745f 6279 5f69 6e64 6578 3a20 2762 6c5f  t_by_index: 'bl_
+00355900: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+00355910: 4f54 5f74 6f6f 6c5f 7365 745f 6279 5f69  OT_tool_set_by_i
+00355920: 6e64 6578 2720 3d20 4e6f 6e65 0a0a 574d  ndex' = None..WM
+00355930: 5f4f 545f 746f 6f6c 6261 723a 2027 626c  _OT_toolbar: 'bl
+00355940: 5f6f 7065 7261 746f 7273 2e77 6d2e 574d  _operators.wm.WM
+00355950: 5f4f 545f 746f 6f6c 6261 7227 203d 204e  _OT_toolbar' = N
+00355960: 6f6e 650a 0a57 4d5f 4f54 5f74 6f6f 6c62  one..WM_OT_toolb
+00355970: 6172 5f66 616c 6c62 6163 6b5f 7069 653a  ar_fallback_pie:
+00355980: 2027 626c 5f6f 7065 7261 746f 7273 2e77   'bl_operators.w
+00355990: 6d2e 574d 5f4f 545f 746f 6f6c 6261 725f  m.WM_OT_toolbar_
+003559a0: 6661 6c6c 6261 636b 5f70 6965 2720 3d20  fallback_pie' = 
+003559b0: 4e6f 6e65 0a0a 574d 5f4f 545f 746f 6f6c  None..WM_OT_tool
+003559c0: 6261 725f 7072 6f6d 7074 3a20 2762 6c5f  bar_prompt: 'bl_
+003559d0: 6f70 6572 6174 6f72 732e 776d 2e57 4d5f  operators.wm.WM_
+003559e0: 4f54 5f74 6f6f 6c62 6172 5f70 726f 6d70  OT_toolbar_promp
+003559f0: 7427 203d 204e 6f6e 650a 0a57 4d5f 4f54  t' = None..WM_OT
+00355a00: 5f75 726c 5f6f 7065 6e3a 2027 626c 5f6f  _url_open: 'bl_o
+00355a10: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00355a20: 545f 7572 6c5f 6f70 656e 2720 3d20 4e6f  T_url_open' = No
+00355a30: 6e65 0a0a 574d 5f4f 545f 7572 6c5f 6f70  ne..WM_OT_url_op
+00355a40: 656e 5f70 7265 7365 743a 2027 626c 5f6f  en_preset: 'bl_o
+00355a50: 7065 7261 746f 7273 2e77 6d2e 574d 5f4f  perators.wm.WM_O
+00355a60: 545f 7572 6c5f 6f70 656e 5f70 7265 7365  T_url_open_prese
+00355a70: 7427 203d 204e 6f6e 650a 0a57 4f52 4b53  t' = None..WORKS
+00355a80: 5041 4345 5f50 545f 6164 646f 6e73 3a20  PACE_PT_addons: 
+00355a90: 2762 6c5f 7569 2e70 726f 7065 7274 6965  'bl_ui.propertie
+00355aa0: 735f 776f 726b 7370 6163 652e 574f 524b  s_workspace.WORK
+00355ab0: 5350 4143 455f 5054 5f61 6464 6f6e 7327  SPACE_PT_addons'
+00355ac0: 203d 204e 6f6e 650a 0a57 4f52 4b53 5041   = None..WORKSPA
+00355ad0: 4345 5f50 545f 6375 7374 6f6d 5f70 726f  CE_PT_custom_pro
+00355ae0: 7073 3a20 2762 6c5f 7569 2e70 726f 7065  ps: 'bl_ui.prope
+00355af0: 7274 6965 735f 776f 726b 7370 6163 652e  rties_workspace.
+00355b00: 574f 524b 5350 4143 455f 5054 5f63 7573  WORKSPACE_PT_cus
+00355b10: 746f 6d5f 7072 6f70 7327 203d 204e 6f6e  tom_props' = Non
+00355b20: 650a 0a57 4f52 4b53 5041 4345 5f50 545f  e..WORKSPACE_PT_
+00355b30: 6d61 696e 3a20 2762 6c5f 7569 2e70 726f  main: 'bl_ui.pro
+00355b40: 7065 7274 6965 735f 776f 726b 7370 6163  perties_workspac
+00355b50: 652e 574f 524b 5350 4143 455f 5054 5f6d  e.WORKSPACE_PT_m
+00355b60: 6169 6e27 203d 204e 6f6e 650a 0a57 4f52  ain' = None..WOR
+00355b70: 4c44 5f50 545f 636f 6e74 6578 745f 776f  LD_PT_context_wo
+00355b80: 726c 643a 2027 626c 5f75 692e 7072 6f70  rld: 'bl_ui.prop
+00355b90: 6572 7469 6573 5f77 6f72 6c64 2e57 4f52  erties_world.WOR
+00355ba0: 4c44 5f50 545f 636f 6e74 6578 745f 776f  LD_PT_context_wo
+00355bb0: 726c 6427 203d 204e 6f6e 650a 0a57 4f52  rld' = None..WOR
+00355bc0: 4c44 5f50 545f 6375 7374 6f6d 5f70 726f  LD_PT_custom_pro
+00355bd0: 7073 3a20 2762 6c5f 7569 2e70 726f 7065  ps: 'bl_ui.prope
+00355be0: 7274 6965 735f 776f 726c 642e 574f 524c  rties_world.WORL
+00355bf0: 445f 5054 5f63 7573 746f 6d5f 7072 6f70  D_PT_custom_prop
+00355c00: 7327 203d 204e 6f6e 650a 0a57 4f52 4c44  s' = None..WORLD
+00355c10: 5f50 545f 7669 6577 706f 7274 5f64 6973  _PT_viewport_dis
+00355c20: 706c 6179 3a20 2762 6c5f 7569 2e70 726f  play: 'bl_ui.pro
+00355c30: 7065 7274 6965 735f 776f 726c 642e 574f  perties_world.WO
+00355c40: 524c 445f 5054 5f76 6965 7770 6f72 745f  RLD_PT_viewport_
+00355c50: 6469 7370 6c61 7927 203d 204e 6f6e 650a  display' = None.
```

### Comparing `fake-bpy-module-latest-20230628/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230629/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import units
 from . import previews
+from . import units
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230628/bpy/utils/previews.py` & `fake-bpy-module-latest-20230629/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy/utils/units.py` & `fake-bpy-module-latest-20230629/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/anim_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230629/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230629/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/bpy_types.py` & `fake-bpy-module-latest-20230629/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230628
+Version: 20230629
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230628/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230629/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230629/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/functions.py` & `fake-bpy-module-latest-20230629/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/predicates.py` & `fake-bpy-module-latest-20230629/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/shaders.py` & `fake-bpy-module-latest-20230629/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/types.py` & `fake-bpy-module-latest-20230629/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230629/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230629/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/capabilities.py` & `fake-bpy-module-latest-20230629/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/matrix.py` & `fake-bpy-module-latest-20230629/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/platform.py` & `fake-bpy-module-latest-20230629/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/shader.py` & `fake-bpy-module-latest-20230629/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/state.py` & `fake-bpy-module-latest-20230629/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/texture.py` & `fake-bpy-module-latest-20230629/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu/types.py` & `fake-bpy-module-latest-20230629/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu_extras/batch.py` & `fake-bpy-module-latest-20230629/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/gpu_extras/presets.py` & `fake-bpy-module-latest-20230629/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/idprop/types.py` & `fake-bpy-module-latest-20230629/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/imbuf/__init__.py` & `fake-bpy-module-latest-20230629/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/imbuf/types.py` & `fake-bpy-module-latest-20230629/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/keyingsets_builtins.py` & `fake-bpy-module-latest-20230629/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/keyingsets_utils.py` & `fake-bpy-module-latest-20230629/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/mathutils/__init__.py` & `fake-bpy-module-latest-20230629/mathutils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import typing
-from . import interpolate
-from . import bvhtree
+from . import geometry
 from . import kdtree
 from . import noise
-from . import geometry
+from . import interpolate
+from . import bvhtree
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class Color:
     ''' This object gives access to Colors in Blender. Most colors returned by Blender APIs are in scene linear color space, as defined by the OpenColorIO configuration. The notable exception is user interface theming colors, which are in sRGB color space. :arg rgb: (r, g, b) color values :type rgb: 3d vector
     '''
```

### Comparing `fake-bpy-module-latest-20230628/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230629/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/mathutils/geometry.py` & `fake-bpy-module-latest-20230629/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/mathutils/kdtree.py` & `fake-bpy-module-latest-20230629/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/mathutils/noise.py` & `fake-bpy-module-latest-20230629/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/nodeitems_builtins.py` & `fake-bpy-module-latest-20230629/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/nodeitems_utils.py` & `fake-bpy-module-latest-20230629/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/rna_info.py` & `fake-bpy-module-latest-20230629/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/rna_keymap_ui.py` & `fake-bpy-module-latest-20230629/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/rna_prop_ui.py` & `fake-bpy-module-latest-20230629/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/rna_xml.py` & `fake-bpy-module-latest-20230629/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230628/setup.py` & `fake-bpy-module-latest-20230629/setup.py`

 * *Files identical despite different names*

