# Comparing `tmp/electricalsim-0.0.6.8.tar.gz` & `tmp/electricalsim-0.0.6.9.tar.gz`

## Comparing `electricalsim-0.0.6.8.tar` & `electricalsim-0.0.6.9.tar`

### file list

```diff
@@ -1,135 +1,83 @@
--rw-r--r--   0        0        0    17417 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/README.md
--rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/10_PF4.png
--rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/11_PF_tooltips.png
--rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/12_App_settings.png
--rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/13_Disabling_nodes.png
--rw-r--r--   0        0        0    63575 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/14_Context_menu.png
--rw-r--r--   0        0        0    97038 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/1_Main_Window.png
--rw-r--r--   0        0        0    95822 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/1_Main_Window_dark.png
--rw-r--r--   0        0        0   136326 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/2_Dialogs.png
--rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/3_Widgets.png
--rw-r--r--   0        0        0    84286 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/4_Pandapower_DataFrames.png
--rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/5_Connections_angle_b.png
--rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/5_Connections_curved_b.png
--rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/5_Connections_straight_b.png
--rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/6_Line_and_transformer_nodes.png
--rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/7_PF1.png
--rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/8_PF2.png
--rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/9_PF3.png
--rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/img/app_icon.png
--rw-r--r--   0        0        0    20968 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/Electrical_Grid_Simulator.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/__init__.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/config.ini
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/egs_create_shortcut.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/egs_run.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/version.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/electricalsim.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/modules.xml
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/workspace.xml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/__init__.py
--rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/constants.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/errors.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/pkg_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/__init__.py
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/commands.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/factory.py
--rw-r--r--   0        0        0    91881 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/graph.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/menu.py
--rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/model.py
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/node.py
--rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/base/port.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/__init__.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/nodes_tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0        0        0    19685 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/__init__.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/backdrop_node.py
--rw-r--r--   0        0        0    21685 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/base_node.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/base_node_circle.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/group_node.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/nodes/port_node.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/__init__.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_abstract.py
--rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_backdrop.py
--rw-r--r--   0        0        0    35668 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_base.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_circle.py
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_group.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_port_in.py
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_port_out.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/node_text_item.py
--rw-r--r--   0        0        0    16695 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/pipe.py
--rw-r--r--   0        0        0    10257 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/port.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/qgraphics/slicer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/__init__.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/actions.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/dialogs.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/node_graph.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/node_widgets.py
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/scene.py
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/tab_search.py
--rw-r--r--   0        0        0    45942 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/viewer.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/viewer_nav.py
--rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/NodeGraphQt/widgets/icons/node_base.png
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/hotkeys/hotkey_functions.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/hotkeys/hotkeys.json
--rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
--rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.ico
--rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.png
--rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.svg
--rw-r--r--   0        0        0    29502 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/lib/auxiliary.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/lib/calculations.py
--rw-r--r--   0        0        0   204596 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/lib/electricalGraph.py
--rw-r--r--   0        0        0    83266 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/lib/main_components.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/lib/table_widget.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/about_dialog.ui
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/aload_dialog.ui
--rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/asgen_dialog.ui
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/bus_dialog.ui
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/choose_bus_switch.ui
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/choose_generator_type.ui
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/choose_line_type.ui
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/choose_load_type.ui
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/choose_transformer_type.ui
--rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/dcline_dialog.ui
--rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/dialogs.py
--rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/ext_grid_dialog.ui
--rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/gen_dialog.ui
--rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/impedance_dialog.ui
--rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/line_dialog.ui
--rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/load_dialog.ui
--rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/main_window.ui
--rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/main_window_backup.ui
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/motor_dialog.ui
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/network_settings_dialog.ui
--rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/pf_settings_widget.ui
--rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/power_flow_dialog.ui
--rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/settings_dialog.ui
--rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/sgen_dialog.ui
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/shunt_dialog.ui
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/stdline_dialog.ui
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/stdtransformer3w_dialog.ui
--rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/stdtransformer_dialog.ui
--rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/storage_dialog.ui
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/switch_dialog.ui
--rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/transformer3w_dialog.ui
--rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/transformer_dialog.ui
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/ward_dialog.ui
--rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/src/electricalsim/ui/xward_dialog.ui
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/LICENSE
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/README_PyPI.md
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/pyproject.toml
--rw-r--r--   0        0        0    13034 2020-02-02 00:00:00.000000 electricalsim-0.0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/README.md
+-rw-r--r--   0        0        0    84223 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/10_PF4.png
+-rw-r--r--   0        0        0    54206 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/11_PF_tooltips.png
+-rw-r--r--   0        0        0    88072 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/12_App_settings.png
+-rw-r--r--   0        0        0    50389 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/13_Disabling_nodes.png
+-rw-r--r--   0        0        0    69759 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/14_Context_menu.png
+-rw-r--r--   0        0        0    97038 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/1_Main_Window.png
+-rw-r--r--   0        0        0    95822 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/1_Main_Window_dark.png
+-rw-r--r--   0        0        0   136326 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/2_Dialogs.png
+-rw-r--r--   0        0        0    25172 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/3_Widgets.png
+-rw-r--r--   0        0        0    84286 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/4_Pandapower_DataFrames.png
+-rw-r--r--   0        0        0    16870 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_angle_b.png
+-rw-r--r--   0        0        0    21425 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_curved_b.png
+-rw-r--r--   0        0        0    21864 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/5_Connections_straight_b.png
+-rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/6_Line_and_transformer_nodes.png
+-rw-r--r--   0        0        0   136386 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/7_PF1.png
+-rw-r--r--   0        0        0   144782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/8_PF2.png
+-rw-r--r--   0        0        0    83704 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/9_PF3.png
+-rwxr-xr-x   0        0        0    51862 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/Logo_CIESE_2021 y UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/img/app_icon.png
+-rw-r--r--   0        0        0    22462 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/Electrical_Grid_Simulator.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/__init__.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/config.ini
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/egs_create_shortcut.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/egs_run.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/version.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/electricalsim.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/modules.xml
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/workspace.xml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/extensions/extension_classes.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkey_functions.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkeys.json
+-rwxr-xr-x   0        0        0    82539 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png
+-rw-r--r--   0        0        0    33031 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.ico
+-rw-r--r--   0        0        0    33067 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.png
+-rwxr-xr-x   0        0        0    14363 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.svg
+-rw-r--r--   0        0        0    30015 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/auxiliary.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/calculations.py
+-rw-r--r--   0        0        0   208285 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/electricalGraph.py
+-rw-r--r--   0        0        0    83266 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/main_components.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/lib/table_widget.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/about_dialog.ui
+-rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/aload_dialog.ui
+-rw-r--r--   0        0        0    17419 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/asgen_dialog.ui
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/bus_dialog.ui
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_bus_switch.ui
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_generator_type.ui
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_line_type.ui
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_load_type.ui
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/choose_transformer_type.ui
+-rw-r--r--   0        0        0    23084 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/dcline_dialog.ui
+-rw-r--r--   0        0        0   138693 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/dialogs.py
+-rw-r--r--   0        0        0    35106 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/ext_grid_dialog.ui
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/extension.ui
+-rw-r--r--   0        0        0    33034 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/gen_dialog.ui
+-rw-r--r--   0        0        0    16772 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/impedance_dialog.ui
+-rw-r--r--   0        0        0    31104 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/line_dialog.ui
+-rw-r--r--   0        0        0    25616 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/load_dialog.ui
+-rw-r--r--   0        0        0    12940 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/main_window.ui
+-rw-r--r--   0        0        0    12741 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/main_window_backup.ui
+-rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/motor_dialog.ui
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/network_settings_dialog.ui
+-rw-r--r--   0        0        0    34604 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/pf_settings_widget.ui
+-rw-r--r--   0        0        0    50076 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/power_flow_dialog.ui
+-rw-r--r--   0        0        0    14082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/settings_dialog.ui
+-rw-r--r--   0        0        0    38654 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/sgen_dialog.ui
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/shunt_dialog.ui
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdline_dialog.ui
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer3w_dialog.ui
+-rw-r--r--   0        0        0    30234 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer_dialog.ui
+-rw-r--r--   0        0        0    26339 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/storage_dialog.ui
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/switch_dialog.ui
+-rw-r--r--   0        0        0    65860 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/transformer3w_dialog.ui
+-rw-r--r--   0        0        0    56751 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/transformer_dialog.ui
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/ward_dialog.ui
+-rw-r--r--   0        0        0    15494 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/src/electricalsim/ui/xward_dialog.ui
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/LICENSE
+-rw-r--r--   0        0        0    12030 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/README_PyPI.md
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/pyproject.toml
+-rw-r--r--   0        0        0    13259 2020-02-02 00:00:00.000000 electricalsim-0.0.6.9/PKG-INFO
```

### Comparing `electricalsim-0.0.6.8/README.md` & `electricalsim-0.0.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,16 @@
 | ```R``` | Flip the selected nodes (works only with nodes that have only one port) |
 | ```Ctrl++``` | Zoom in |
 | ```Ctrl+-``` | Zoom out |
 | ```=``` | Reset zoom |
 | ```F``` | Adjust the zoom level according to the selection |
 | ```V``` | Change selected nodes to the vertical layout |
 | ```H``` | Change selected nodes to the horizontal layout |
+| ```Shift+V``` | Apply a vertical alignment to selected nodes |
+| ```Shift+H``` | Apply a horizontal alignment to selected nodes |
 
 > __Note__ <br>
 > * ```Undo``` and ```Redo``` only work for simple actions.
 > * Pressing ```F``` without selected nodes will adjust the zoom level to show all the grid.
 > * Pressing ```D``` will change the bool value for the ```in_service``` parameter in the **Data model**. This works for every component, except for switches.
 > * For selecting nodes in the **Graph** you can use the left mouse button (```LMB```). Just click with the ```LMB```, hold and drag to mark the selection area.
 > * Clicking with the ```LMB``` on the background will unselect all.
```

### Comparing `electricalsim-0.0.6.8/img/10_PF4.png` & `electricalsim-0.0.6.9/img/10_PF4.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/11_PF_tooltips.png` & `electricalsim-0.0.6.9/img/11_PF_tooltips.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/12_App_settings.png` & `electricalsim-0.0.6.9/img/12_App_settings.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/13_Disabling_nodes.png` & `electricalsim-0.0.6.9/img/13_Disabling_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/1_Main_Window.png` & `electricalsim-0.0.6.9/img/1_Main_Window.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/1_Main_Window_dark.png` & `electricalsim-0.0.6.9/img/1_Main_Window_dark.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/2_Dialogs.png` & `electricalsim-0.0.6.9/img/2_Dialogs.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/3_Widgets.png` & `electricalsim-0.0.6.9/img/3_Widgets.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/4_Pandapower_DataFrames.png` & `electricalsim-0.0.6.9/img/4_Pandapower_DataFrames.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/5_Connections_angle_b.png` & `electricalsim-0.0.6.9/img/5_Connections_angle_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/5_Connections_curved_b.png` & `electricalsim-0.0.6.9/img/5_Connections_curved_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/5_Connections_straight_b.png` & `electricalsim-0.0.6.9/img/5_Connections_straight_b.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/6_Line_and_transformer_nodes.png` & `electricalsim-0.0.6.9/img/6_Line_and_transformer_nodes.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/7_PF1.png` & `electricalsim-0.0.6.9/img/7_PF1.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/8_PF2.png` & `electricalsim-0.0.6.9/img/8_PF2.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/9_PF3.png` & `electricalsim-0.0.6.9/img/9_PF3.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/Logo_CIESE_2021 y UTN_Sta_Fe.png` & `electricalsim-0.0.6.9/img/Logo_CIESE_2021 y UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/img/app_icon.png` & `electricalsim-0.0.6.9/img/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/Electrical_Grid_Simulator.py` & `electricalsim-0.0.6.9/src/electricalsim/Electrical_Grid_Simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import sys
 import os
+import importlib
 
 from Qt import QtWidgets, QtCompat, QtGui, QtCore
 import qdarktheme  # Always import after Qt
 import qtawesome as qta
 
 from lib.electricalGraph import ElectricalGraph
 from lib.table_widget import TableWidget
 from lib.auxiliary import QVLine, QMainWindow2, return_config
 from lib.calculations import Run_PF
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 
 def main():
     """
     Execute the Electrical Grid Simulator (GUI).
     """
     directory = os.path.dirname(__file__)
     os.chdir(directory)
@@ -32,16 +38,25 @@
     
     ui_file = os.path.join(directory, 'ui', 'main_window.ui')
     main_window = QtCompat.loadUi(uifile=ui_file, baseinstance=QMainWindow2())
     
     icon_path = os.path.join(directory, 'icons', 'app_icon.png')
     main_window.setWindowIcon(QtGui.QIcon(icon_path))
     main_window.setWindowTitle('Electrical Grid Simulator')
-    
-    graph = ElectricalGraph(config, config_file_path, main_window=main_window)
+
+    # Loading extensions:
+    extensions = entry_points(group='electricalsim.extensions')
+    extensions_dict = dict()
+    for ex in extensions:
+        extension_module = importlib.import_module(f'electricalsim_{ex.name}.extension')
+        extensions_dict[ex.name] = extension_module
+    
+    graph = ElectricalGraph(config, config_file_path,
+                            main_window=main_window,
+                            extensions_dict=extensions_dict)
     
     # Toolbar settings------------------------------
     addBus_action = QtWidgets.QAction('addBus')
     addBus_action.setText('Bus')
     addBus_action.setToolTip('Add a bus')
     addBus_action.triggered.connect(graph.add_bus)
     addBus_action.setIcon(qta.icon('ph.git-commit'))
@@ -228,14 +243,31 @@
     
     run_pf_btn = QtWidgets.QToolButton(main_window)
     run_pf_btn.setToolTip('Balanced AC power flow')
     run_pf_btn.setIconSize(icon_size)
     run_pf_btn.setIcon(qta.icon('mdi6.play-outline'))
     main_window.layout_upper_toolbar.addWidget(run_pf_btn)
     run_pf_btn.clicked.connect(Run_PF(graph))
+
+    main_window.layout_upper_toolbar.addStretch()
+
+    extensions_label = QtWidgets.QLabel(main_window)
+    extensions_label.setText('Extensions:')
+    extensions_combobox = QtWidgets.QComboBox(main_window)
+    extensions_combobox.setObjectName('extension_selector')
+    extensions_combobox.setMinimumSize(250, 0)
+    extension_run_btn = QtWidgets.QToolButton(main_window)
+    extension_run_btn.setObjectName('extension_run_btn')
+    extension_run_btn.setToolTip('Execute the selected extension')
+    extension_run_btn.setIconSize(icon_size)
+    extension_run_btn.setIcon(qta.icon('mdi6.puzzle-outline'))
+    main_window.layout_upper_toolbar.addWidget(extensions_label)
+    main_window.layout_upper_toolbar.addWidget(extensions_combobox)
+    main_window.layout_upper_toolbar.addWidget(extension_run_btn)
+    extension_run_btn.clicked.connect(graph.execute_extension)
     
     main_window.layout_upper_toolbar.addStretch()
     
     net_settings = QtWidgets.QToolButton(main_window)
     net_settings.setToolTip('Basic network settings')
     net_settings.setIconSize(icon_size)
     net_settings.setIcon(qta.icon('mdi6.grid'))
@@ -433,15 +465,19 @@
             old_switch_table = main_window.layout_switch.itemAt(0).widget()
             old_switch_table.setParent(None)
             df_switch_widget = TableWidget(graph.net.switch.copy(deep=True))
             main_window.layout_switch.addWidget(df_switch_widget)
             
     main_window.toolBox.currentChanged.connect(page_changed_on_toolbox)
     graph.page_changed_on_toolbox = page_changed_on_toolbox
-    
+
+    # Update the extensions list in the UI (combobox selector):
+    graph.update_extensions_list()
+
     # Show main window:
     main_window.show()
+
     app.exec_()
 
 
-if __name__=='__main__':
+if __name__ == '__main__':
     main()
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/config.ini` & `electricalsim-0.0.6.9/src/electricalsim/config.ini`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/egs_create_shortcut.py` & `electricalsim-0.0.6.9/src/electricalsim/egs_create_shortcut.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.6.9/src/electricalsim/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `electricalsim-0.0.6.8/src/electricalsim/.idea/workspace.xml` & `electricalsim-0.0.6.9/src/electricalsim/.idea/workspace.xml`

```diff
@@ -12,22 +12,22 @@
   </component>
   <component name="ProjectId" id="2MKCBopZy5dPlZhrEXWU7Iz8rBU"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showExcludedFiles" value="false"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/home/usuario/Documentos/Inquietudes/Electrical Grid Simulation/src/electricalsim/Electrical_Grid_Simulator.py",
-    "settings.editor.selected.configurable": "preferences.keymap"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/usuario/Documentos/Inquietudes/EGS-arcflash/src/electricalsim_arcflash&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;preferences.general&quot;
   }
-}]]></component>
+}</component>
   <component name="RunManager">
     <configuration name="EGS" type="PythonConfigurationType" factoryName="Python">
       <module name="electricalsim"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim-0.0.6.9/src/electricalsim/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/hotkeys/hotkey_functions.py` & `electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkey_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -206,7 +206,31 @@
 def flip_nodes(graph):
     """
     Flip the selected nodes.
     """
     selected = graph.selected_nodes()
     for node in selected:
         node.flip()
+
+
+def horizontal_alignment(graph):
+    """
+    Apply a horizontal alignment to selected nodes.
+    """
+    selected = graph.selected_nodes()
+    if selected:
+        last_node = selected[-1]
+        pos = last_node.y_pos()
+        for node in selected[:-1]:
+            node.set_y_pos(pos)
+
+
+def vertical_alignment(graph):
+    """
+    Apply a vertical alignment to selected nodes.
+    """
+    selected = graph.selected_nodes()
+    if selected:
+        last_node = selected[-1]
+        pos = last_node.x_pos()
+        for node in selected[:-1]:
+            node.set_x_pos(pos)
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/hotkeys/hotkeys.json` & `electricalsim-0.0.6.9/src/electricalsim/hotkeys/hotkeys.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {'2': "{'items': {insert: [(2, OrderedDict([('type', 'separator')])), (3, OrderedDict([('type', "*

 * *      "'command'), ('label', 'Vertical alignment'), ('file', './hotkeys/hotkey_functions.py'), "*

 * *      "('function_name', 'vertical_alignment'), ('shortcut', 'Shift+V')])), (4, "*

 * *      "OrderedDict([('type', 'command'), ('label', 'Horizontal alignment'), ('file', "*

 * *      "'./hotkeys/hotkey_functions.py'), ('function_name', 'horizontal_alignment'), ('shortcut', "*

 * *      "'Shift+H')]))]}}"}*

```diff
@@ -105,13 +105,30 @@
             },
             {
                 "file": "./hotkeys/hotkey_functions.py",
                 "function_name": "horizontal_layout",
                 "label": "Horizontal layout",
                 "shortcut": "H",
                 "type": "command"
+            },
+            {
+                "type": "separator"
+            },
+            {
+                "file": "./hotkeys/hotkey_functions.py",
+                "function_name": "vertical_alignment",
+                "label": "Vertical alignment",
+                "shortcut": "Shift+V",
+                "type": "command"
+            },
+            {
+                "file": "./hotkeys/hotkey_functions.py",
+                "function_name": "horizontal_alignment",
+                "label": "Horizontal alignment",
+                "shortcut": "Shift+H",
+                "type": "command"
             }
         ],
         "label": "&Format",
         "type": "menu"
     }
 ]
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png` & `electricalsim-0.0.6.9/src/electricalsim/icons/CIESE_UTN_Sta_Fe.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.ico` & `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.ico`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.png` & `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/icons/app_icon.svg` & `electricalsim-0.0.6.9/src/electricalsim/icons/app_icon.svg`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/lib/auxiliary.py` & `electricalsim-0.0.6.9/src/electricalsim/lib/auxiliary.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import configparser
 
 from Qt import QtWidgets
 import qtawesome as qta
 from pynput.keyboard import Key, Controller
 from platformdirs import user_config_dir
 
+directory = os.path.dirname(__file__)
+root_dir, _ = os.path.split(directory)
+
 
 def show_WIP(window_parent):
     """
     Show a warning popup dialog which indicates work in progress,
     so that option is not available yet.
     """
     title = 'Work in progress'
@@ -25,14 +28,39 @@
     
     This is used for avoiding freezes due to a Qt error with
     open/save dialogs (workaround).
     """
     keyboard = Controller()
     keyboard.press(Key.esc)
     keyboard.release(Key.esc)
+    
+
+def simulate_H_key():
+    """
+    Simulate the press and release of H key.
+    """
+    keyboard = Controller()
+    keyboard.press('h')
+    keyboard.release('h')
+
+
+def simulate_V_key():
+    """
+    Simulate the press and release of V key.
+    """
+    keyboard = Controller()
+    keyboard.press('v')
+    keyboard.release('v')
+
+
+def egs_path():
+    """
+    Returns the EGS installation path (directory).
+    """
+    return root_dir
 
 
 class QMainWindow2(QtWidgets.QMainWindow):
     """
     Same as default QMainWindow, but ask for permission before closing.
     """
     def __init__(self, **kwargs):
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/lib/electricalGraph.py` & `electricalsim-0.0.6.9/src/electricalsim/lib/electricalGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # -*- coding: utf-8 -*-
 
 import os
 import warnings
 from math import isnan, nan
 import pickle
 
-from Qt import QtGui, QtWidgets
+from Qt import QtGui, QtWidgets, QtCore
 
 from NodeGraphQt import NodeGraph, errors
 from NodeGraphQt.constants import PortTypeEnum, PipeLayoutEnum
 import pandapower as pp
-from pandapower.toolbox import drop_from_groups
+# from pandapower.toolbox import drop_from_groups
+from pandapower.toolbox import drop_elements
 import numpy as np
 
 from lib.main_components import (BusNode, LineNode, StdLineNode, DCLineNode,
                                  ImpedanceNode, TrafoNode, StdTrafoNode,
                                  Trafo3wNode, StdTrafo3wNode, GenNode,
                                  SGenNode, ASGenNode, ExtGridNode,
                                  LoadNode, ALoadNode, ShuntNode, MotorNode,
                                  WardNode, XWardNode, StorageNode,
                                  SwitchNode)
 from lib.auxiliary import (NodeMovedCmd, StatusMessageUnsaved,
-                     simulate_ESC_key)  # , show_WIP)
+                           simulate_ESC_key)  # , show_WIP)
 from ui.dialogs import (bus_dialog, choose_line_dialog, line_dialog,
                         stdline_dialog,
                         dcline_dialog, impedance_dialog,
                         choose_transformer_dialog, transformer_dialog,
                         stdtransformer_dialog,
                         transformer3w_dialog, stdtransformer3w_dialog,
                         choose_generator_dialog, gen_dialog,
                         sgen_dialog, asgen_dialog, ext_grid_dialog,
                         choose_load_dialog, load_dialog, aload_dialog,
                         shunt_dialog, motor_dialog, about_dialog,
                         ward_dialog, xward_dialog, storage_dialog,
                         choose_bus_switch_dialog, switch_dialog,
                         network_settings_dialog, Settings_Dialog)
+from extensions.extension_classes import ExtensionWorker
 
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 directory = os.path.dirname(__file__)
 root_directory, _ = os.path.split(directory)
 icon_path = os.path.join(root_directory, 'icons', 'app_icon.png')
 
@@ -120,18 +122,16 @@
 
         self.node_double_clicked.connect(self.open_options_dialog)
         self._viewer.connection_changed.connect(self.connection_changed)
         self.port_disconnected.connect(self.disconnect_component)
 
         self.saved_file_path = None  # None if the session was never saved
 
-        if 'main_window' in kwargs:
-            self.main_window = kwargs['main_window']
-        else:
-            self.main_window = None  # QMainWindow2 reference to the main window
+        self.main_window = kwargs.get('main_window')  # QMainWindow2 reference to the main window
+        self.extensions_dict = kwargs.get('extensions_dict', dict())
 
         # When something in the graph changed:
         self.property_changed.connect(self.session_change_warning)
         self.message_unsaved = StatusMessageUnsaved()
         self.main_window.statusbar.addWidget(self.message_unsaved)
         self.message_unsaved.hide()
 
@@ -370,22 +370,33 @@
             self.message_unsaved.hide()
             # self.update_tooltips()
             
             for node in self.all_nodes():
                 layout_vert = node.get_property('layout_vert')
                 if layout_vert is not None and layout_vert is True:
                     node.set_layout_direction(1)
-                    if self.config['general']['theme']=='light':
-                        node.model.set_property('text_color', (0, 0, 0, 255))  # black
-                    else:
-                        node.model.set_property('text_color', (255, 255, 255, 180))  # default color
-                    node.update()
+                    
+                #     if self.config['general']['theme']=='light':
+                #         node.model.set_property('text_color', (0, 0, 0, 255))  # black
+                #     else:
+                #         node.model.set_property('text_color', (255, 255, 255, 180))  # default color
+                #     node.update()
+            
+            # for node in self.all_nodes():
+            #     layout_vert = node.get_property('layout_vert')
+            #     if layout_vert is not None and layout_vert is True:
+            #         node.set_selected()
+            # horizontal_layout(self)
+            # vertical_layout(self)
+            # self.clear_selection()
             
             if self.main_window.toolBox.currentIndex()==1:
                 self.page_changed_on_toolbox(index=1)
+                
+            
 
         simulate_ESC_key()
 
     def new_session(self):
         """
         Clear the session (graph and pandapower network) and creates a new one.
         """
@@ -3549,33 +3560,35 @@
         node in the graph is removed.
         """
         line_name = node.get_property('name')
         line_row = self.net.dcline[self.net.dcline['name']==line_name]
         if not line_row.empty:
             line_index = line_row.index[0]
             lines = [line_index]
-            drop_from_groups(self.net, "dcline", lines)
-            self.net["dcline"].drop(lines, inplace=True)
-            res_dclines = self.net.res_dcline.index.intersection(lines)
-            self.net["res_dcline"].drop(res_dclines, inplace=True)
+            # drop_from_groups(self.net, "dcline", lines)
+            drop_elements(self.net, "dcline", lines)
+            # self.net["dcline"].drop(lines, inplace=True)
+            # res_dclines = self.net.res_dcline.index.intersection(lines)
+            # self.net["res_dcline"].drop(res_dclines, inplace=True)
 
     def remove_impedance(self, node):
         """
         Remove an impedance from the pandapower network when its corresponding
         node in the graph is removed.
         """
         impedance_name = node.get_property('name')
         impedance_row = self.net.impedance[self.net.impedance['name']==impedance_name]
         if not impedance_row.empty:
             impedance_index = impedance_row.index[0]
             impedances = [impedance_index]
-            drop_from_groups(self.net, "impedace", impedances)
-            self.net["impedance"].drop(impedances, inplace=True)
-            res_impedances = self.net.res_impedance.index.intersection(impedances)
-            self.net["res_impedance"].drop(res_impedances, inplace=True)
+            # drop_from_groups(self.net, "impedace", impedances)
+            drop_elements(self.net, "impedace", impedances)
+            # self.net["impedance"].drop(impedances, inplace=True)
+            # res_impedances = self.net.res_impedance.index.intersection(impedances)
+            # self.net["res_impedance"].drop(res_impedances, inplace=True)
 
     def remove_trafo(self, node, directly_removed=True):
         """
         Remove a two-winding transformer from the pandapower network when its corresponding
         node in the graph is removed.
         """
         if directly_removed:
@@ -3613,137 +3626,162 @@
         node in the graph is removed.
         """
         gen_name = node.get_property('name')
         gen_row = self.net.gen[self.net.gen['name']==gen_name]
         if not gen_row.empty:
             gen_index = gen_row.index[0]
             gens = [gen_index]
-            drop_from_groups(self.net, "gen", gens)
-            self.net["gen"].drop(gens, inplace=True)
-            res_gens = self.net.res_gen.index.intersection(gens)
-            self.net["res_gen"].drop(res_gens, inplace=True)
+            # drop_from_groups(self.net, "gen", gens)
+            drop_elements(self.net, "gen", gens)
+            # self.net["gen"].drop(gens, inplace=True)
+            # res_gens = self.net.res_gen.index.intersection(gens)
+            # self.net["res_gen"].drop(res_gens, inplace=True)
 
     def remove_sgen(self, node):
         """
         Remove a static generator from the pandapower network when its
         corresponding node in the graph is removed.
         """
         gen_name = node.get_property('name')
         gen_row = self.net.sgen[self.net.sgen['name']==gen_name]
         if not gen_row.empty:
             gen_index = gen_row.index[0]
             gens = [gen_index]
-            drop_from_groups(self.net, "sgen", gens)
-            self.net["sgen"].drop(gens, inplace=True)
-            res_sgens = self.net.res_sgen.index.intersection(gens)
-            self.net["res_sgen"].drop(res_sgens, inplace=True)
+            # drop_from_groups(self.net, "sgen", gens)
+            drop_elements(self.net, "sgen", gens)
+            # self.net["sgen"].drop(gens, inplace=True)
+            # res_sgens = self.net.res_sgen.index.intersection(gens)
+            # self.net["res_sgen"].drop(res_sgens, inplace=True)
 
     def remove_asgen(self, node):
         """
         Remove an asymmetric static generator from the pandapower network when its
         corresponding node in the graph is removed.
         """
         gen_name = node.get_property('name')
         gen_row = self.net.asymmetric_sgen[self.net.asymmetric_sgen['name']==gen_name]
         if not gen_row.empty:
             gen_index = gen_row.index[0]
             gens = [gen_index]
-            drop_from_groups(self.net, "asymmetric_sgen", gens)
-            self.net["asymmetric_sgen"].drop(gens, inplace=True)
-
-            res_asgens = self.net.res_asymmetric_sgen.index.intersection(gens)
-            self.net["res_asymmetric_sgen"].drop(res_asgens, inplace=True)
+            # drop_from_groups(self.net, "asymmetric_sgen", gens)
+            drop_elements(self.net, "asymmetric_sgen", gens)
+            # self.net["asymmetric_sgen"].drop(gens, inplace=True)
+            #
+            # res_asgens = self.net.res_asymmetric_sgen.index.intersection(gens)
+            # self.net["res_asymmetric_sgen"].drop(res_asgens, inplace=True)
 
             res_asgens2 = self.net.res_asymmetric_sgen_3ph.index.intersection(gens)
             self.net["res_asymmetric_sgen_3ph"].drop(res_asgens2, inplace=True)
 
     def remove_ext_grid(self, node):
         """
         Remove an external grid from the pandapower network when its
         corresponding node in the graph is removed.
         """
         grid_name = node.get_property('name')
         grid_row = self.net.ext_grid[self.net.ext_grid['name']==grid_name]
         if not grid_row.empty:
             grid_index = grid_row.index[0]
             grids = [grid_index]
-            drop_from_groups(self.net, "ext_grid", grids)
-            self.net["ext_grid"].drop(grids, inplace=True)
+            # drop_from_groups(self.net, "ext_grid", grids)
+            drop_elements(self.net, "ext_grid", grids)
+            # self.net["ext_grid"].drop(grids, inplace=True)
 
-            res_grids = self.net.res_ext_grid.index.intersection(grids)
-            self.net["res_ext_grid"].drop(res_grids, inplace=True)
+            # res_grids = self.net.res_ext_grid.index.intersection(grids)
+            # self.net["res_ext_grid"].drop(res_grids, inplace=True)
 
             res_grids2 = self.net.res_ext_grid_3ph.index.intersection(grids)
             self.net["res_ext_grid_3ph"].drop(res_grids2, inplace=True)
 
             res_grids3 = self.net.res_ext_grid_sc.index.intersection(grids)
             self.net["res_ext_grid_sc"].drop(res_grids3, inplace=True)
 
     def remove_load(self, node):
         """
         Remove a symmetric load from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        load_index = node.get_property('load_index')
-        if load_index is not None:
-            pp.drop_elements_simple(self.net, 'load', load_index)
+        load_name = node.get_property('name')
+        load_row = self.net.load[self.net.load['name'] == load_name]
+        if not load_row.empty:
+            load_index = node.get_property('load_index')
+            if load_index is not None:
+                pp.drop_elements_simple(self.net, 'load', load_index)
 
     def remove_aload(self, node):
         """
         Remove an asymmetric load from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        load_index = node.get_property('load_index')
-        if load_index is not None:
-            pp.drop_elements_simple(self.net, 'asymmetric_load', load_index)
+        load_name = node.get_property('name')
+        load_row = self.net.asymmetric_load[self.net.asymmetric_load['name'] == load_name]
+        if not load_row.empty:
+            load_index = node.get_property('load_index')
+            if load_index is not None:
+                pp.drop_elements_simple(self.net, 'asymmetric_load', load_index)
 
     def remove_shunt(self, node):
         """
         Remove a shunt element from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        shunt_index = node.get_property('shunt_index')
-        if shunt_index is not None:
-            pp.drop_elements_simple(self.net, 'shunt', shunt_index)
+        shunt_name = node.get_property('name')
+        shunt_row = self.net.shunt[self.net.shunt['name'] == shunt_name]
+        if not shunt_row.empty:
+            shunt_index = node.get_property('shunt_index')
+            if shunt_index is not None:
+                pp.drop_elements_simple(self.net, 'shunt', shunt_index)
 
     def remove_motor(self, node):
         """
         Remove a motor from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        motor_index = node.get_property('motor_index')
-        if motor_index is not None:
-            pp.drop_elements_simple(self.net, 'motor', motor_index)
+        motor_name = node.get_property('name')
+        motor_row = self.net.motor[self.net.motor['name'] == motor_name]
+        if not motor_row.empty:
+            motor_index = node.get_property('motor_index')
+            if motor_index is not None:
+                pp.drop_elements_simple(self.net, 'motor', motor_index)
 
     def remove_ward(self, node):
         """
         Remove a ward from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        ward_index = node.get_property('ward_index')
-        if ward_index is not None:
-            pp.drop_elements_simple(self.net, 'ward', ward_index)
+        ward_name = node.get_property('name')
+        ward_row = self.net.ward[self.net.ward['name'] == ward_name]
+        if not ward_row.empty:
+            ward_index = node.get_property('ward_index')
+            if ward_index is not None:
+                pp.drop_elements_simple(self.net, 'ward', ward_index)
 
     def remove_xward(self, node):
         """
         Remove an extended ward from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        ward_index = node.get_property('ward_index')
-        if ward_index is not None:
-            pp.drop_elements_simple(self.net, 'xward', ward_index)
+        xward_name = node.get_property('name')
+        xward_row = self.net.xward[self.net.xward['name'] == xward_name]
+        if not xward_row.empty:
+            ward_index = node.get_property('ward_index')
+            if ward_index is not None:
+                pp.drop_elements_simple(self.net, 'xward', ward_index)
 
     def remove_storage(self, node):
         """
         Remove a storage from the pandapower network when its corresponding
         node in the graph is removed.
         """
-        storage_index = node.get_property('storage_index')
-        if storage_index is not None and storage_index in self.net.storage.index:
-            pp.drop_elements_simple(self.net, 'storage', storage_index)
+        storage_name = node.get_property('name')
+        storage_row = self.net.storage[self.net.storage['name'] == storage_name]
+        if not storage_row.empty:
+            storage_index = node.get_property('storage_index')
+            if storage_index is not None and storage_index in self.net.storage.index:
+                pp.drop_elements_simple(self.net, 'storage', storage_index)
             
     def remove_switch(self, node, directly_removed=True):
         """
         Remove a switch from the pandapower network when its corresponding
         node in the graph is removed.
         """
         node.set_locked(False)  # Necessary to remove the node
@@ -3760,7 +3798,62 @@
             trafos = node.node_trafo_connected()
             for trafo_node in trafos:
                 self.remove_trafo(trafo_node, directly_removed=False)
             
             trafos3w = node.node_trafo3w_connected()
             for trafo3w_node in trafos3w:
                 self.remove_trafo3w(trafo3w_node, directly_removed=False)
+
+    def run_extension(self, name):
+        """
+        Run an extension.
+
+        Args:
+            name: Extension name
+
+        Returns: None
+
+        """
+        ex_mod = self.extensions_dict[name]
+        ex_obj = ex_mod.Extension(graph=self)
+        ex_obj.set_name(name)
+
+        if ex_obj.extension_window() is True:
+            ex_obj.show_dialog()
+        else:
+            ex_obj.before_running()
+            if ex_obj.separate_thread() is True:
+                ex_wkr = ExtensionWorker(ex_obj)
+                ex_wkr.signals.finished.connect(ex_obj.finish)
+                ex_threadpool = QtCore.QThreadPool()
+                ex_threadpool.start(ex_wkr)
+            else:
+                ex_obj()
+                ex_obj.finish()
+
+    def execute_extension(self):
+        """
+        Execute the selected extension.
+
+        Returns: None
+
+        """
+        selector = self.main_window.findChild(QtWidgets.QComboBox, 'extension_selector')
+        extension_name = selector.currentText()
+        self.run_extension(extension_name)
+
+    def update_extensions_list(self):
+        """
+        Update the extensions list in the combobox selector.
+
+        Returns: None
+
+        """
+        selector = self.main_window.findChild(QtWidgets.QComboBox, 'extension_selector')
+        btn = self.main_window.findChild(QtWidgets.QToolButton, 'extension_run_btn')
+        selector.clear()
+        if self.extensions_dict:
+            selector.addItems(sorted(self.extensions_dict.keys()))
+            btn.setEnabled(True)
+        else:
+            selector.addItem('<No extensions available>')
+            btn.setEnabled(False)
```

### Comparing `electricalsim-0.0.6.8/src/electricalsim/lib/main_components.py` & `electricalsim-0.0.6.9/src/electricalsim/lib/main_components.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/lib/table_widget.py` & `electricalsim-0.0.6.9/src/electricalsim/lib/table_widget.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/about_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/aload_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/aload_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/asgen_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/asgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/bus_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/bus_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/choose_bus_switch.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/choose_bus_switch.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/choose_generator_type.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/choose_generator_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/choose_line_type.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/choose_line_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/choose_load_type.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/choose_load_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/choose_transformer_type.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/choose_transformer_type.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/dcline_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/dcline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/dialogs.py` & `electricalsim-0.0.6.9/src/electricalsim/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/ext_grid_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/ext_grid_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/gen_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/gen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/impedance_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/impedance_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/line_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/line_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/load_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/load_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/main_window.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/main_window_backup.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/main_window_backup.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/motor_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/motor_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/network_settings_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/network_settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/pf_settings_widget.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/pf_settings_widget.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/power_flow_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/power_flow_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/settings_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/sgen_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/sgen_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/shunt_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/shunt_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/stdline_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/stdline_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/stdtransformer3w_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/stdtransformer_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/stdtransformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/storage_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/storage_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/switch_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/switch_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/transformer3w_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/transformer3w_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/transformer_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/transformer_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/ward_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/ward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/src/electricalsim/ui/xward_dialog.ui` & `electricalsim-0.0.6.9/src/electricalsim/ui/xward_dialog.ui`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/LICENSE` & `electricalsim-0.0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim-0.0.6.8/README_PyPI.md` & `electricalsim-0.0.6.9/README_PyPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 | ```R``` | Flip the selected nodes (works only with nodes that have only one port) |
 | ```Ctrl++``` | Zoom in |
 | ```Ctrl+-``` | Zoom out |
 | ```=``` | Reset zoom |
 | ```F``` | Adjust the zoom level according to the selection |
 | ```V``` | Change selected nodes to the vertical layout |
 | ```H``` | Change selected nodes to the horizontal layout |
+| ```Shift+V``` | Apply a vertical alignment to selected nodes |
+| ```Shift+H``` | Apply a horizontal alignment to selected nodes |
 
 > __Note__ <br>
 > * ```Undo``` and ```Redo``` only work for simple actions.
 > * Pressing ```F``` without selected nodes will adjust the zoom level to show all the grid.
 > * Pressing ```D``` will change the bool value for the ```in_service``` parameter in the **Data model**. This works for every component, except for switches.
 > * For selecting nodes in the **Graph** you can use the left mouse button (```LMB```). Just click with the ```LMB```, hold and drag to mark the selection area.
 > * Clicking with the ```LMB``` on the background will unselect all.
```

### Comparing `electricalsim-0.0.6.8/pyproject.toml` & `electricalsim-0.0.6.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim"
-version = "0.0.6.8"
+version = "0.0.6.9"
 author = "PhD Ariel S. Loyarte"
 authors = [
   { name="PhD Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
-description = "Graphical user interface for simulating electrical networks based on pandapower library"
+description = "Graphical user interface for simulating electrical networks based on the pandapower library"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 dependencies = [
   "PySide2>=5.15",
   "Qt.py>=1.3.7",
-  "pandapower>=2.11.1",
+  "pandapower>=2.13.1",
   "numba>=0.56.4",
   "pyqtdarktheme>=2.1.0",
   "qtawesome>=1.2.2",
   "pynput>=1.7.6",
   "lightsim2grid>=0.7.1",
   "matplotlib>=3.6.0",
   "platformdirs>=3.0.0",
   "qtpy>=2.3.0",
   "pyshortcuts>=1.8.3",
+  "importlib_metadata>=4.11.3",
+  "NodeGraphQt>=0.6.1",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = ["electrical networks", "simulation", "energy", "power systems"]
+license = {text = "MIT"}
 
 [project.urls]
 "Homepage" = "https://github.com/aloytag/electrical-grid-simulator"
 "Bug Tracker" = "https://github.com/aloytag/electrical-grid-simulator/issues"
 "Repository" = "https://github.com/aloytag/electrical-grid-simulator"
 
 [project.scripts]
```

### Comparing `electricalsim-0.0.6.8/PKG-INFO` & `electricalsim-0.0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: electricalsim
-Version: 0.0.6.8
-Summary: Graphical user interface for simulating electrical networks based on pandapower library
+Version: 0.0.6.9
+Summary: Graphical user interface for simulating electrical networks based on the pandapower library
 Project-URL: Homepage, https://github.com/aloytag/electrical-grid-simulator
 Project-URL: Bug Tracker, https://github.com/aloytag/electrical-grid-simulator/issues
 Project-URL: Repository, https://github.com/aloytag/electrical-grid-simulator
 Author-email: "PhD Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
+License: MIT
 License-File: LICENSE
 Keywords: electrical networks,energy,power systems,simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: importlib-metadata>=4.11.3
 Requires-Dist: lightsim2grid>=0.7.1
 Requires-Dist: matplotlib>=3.6.0
+Requires-Dist: nodegraphqt>=0.6.1
 Requires-Dist: numba>=0.56.4
-Requires-Dist: pandapower>=2.11.1
+Requires-Dist: pandapower>=2.13.1
 Requires-Dist: platformdirs>=3.0.0
 Requires-Dist: pynput>=1.7.6
 Requires-Dist: pyqtdarktheme>=2.1.0
 Requires-Dist: pyshortcuts>=1.8.3
 Requires-Dist: pyside2>=5.15
 Requires-Dist: qt-py>=1.3.7
 Requires-Dist: qtawesome>=1.2.2
@@ -132,14 +135,16 @@
 | ```R``` | Flip the selected nodes (works only with nodes that have only one port) |
 | ```Ctrl++``` | Zoom in |
 | ```Ctrl+-``` | Zoom out |
 | ```=``` | Reset zoom |
 | ```F``` | Adjust the zoom level according to the selection |
 | ```V``` | Change selected nodes to the vertical layout |
 | ```H``` | Change selected nodes to the horizontal layout |
+| ```Shift+V``` | Apply a vertical alignment to selected nodes |
+| ```Shift+H``` | Apply a horizontal alignment to selected nodes |
 
 > __Note__ <br>
 > * ```Undo``` and ```Redo``` only work for simple actions.
 > * Pressing ```F``` without selected nodes will adjust the zoom level to show all the grid.
 > * Pressing ```D``` will change the bool value for the ```in_service``` parameter in the **Data model**. This works for every component, except for switches.
 > * For selecting nodes in the **Graph** you can use the left mouse button (```LMB```). Just click with the ```LMB```, hold and drag to mark the selection area.
 > * Clicking with the ```LMB``` on the background will unselect all.
```

