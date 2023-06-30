# Comparing `tmp/pydivkit-25.6.0.tar.gz` & `tmp/pydivkit-25.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-25.6.0.tar", max compression
+gzip compressed data, was "pydivkit-25.7.0.tar", max compression
```

## Comparing `pydivkit-25.6.0.tar` & `pydivkit-25.7.0.tar`

### file list

```diff
@@ -1,128 +1,131 @@
--rw-r--r--   0        0        0     9446 2023-06-27 11:05:18.333821 pydivkit-25.6.0/README.md
--rw-r--r--   0        0        0      700 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    13558 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      884 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      898 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      863 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3263 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     3671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0      285 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3038 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9833 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1697 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0    17322 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0     1861 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1292 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10752 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2915 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     2952 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1228 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     1385 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      827 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      271 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      686 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3313 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1090 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     3026 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      258 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_font_family.py
--rw-r--r--   0        0        0      300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    14582 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14431 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12886 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    16177 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2552 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13998 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    15687 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      403 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      671 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1249 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1590 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1548 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    13014 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1950 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      357 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1136 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1156 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13936 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    13054 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0      424 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    15030 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13360 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20599 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25719 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2796 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2923 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      566 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    13711 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_video.py
--rw-r--r--   0        0        0     2826 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     2956 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      866 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      872 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      860 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      882 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2023-06-27 11:05:18.333821 pydivkit-25.6.0/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-25.6.0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2023-06-30 11:32:05.700599 pydivkit-25.7.0/README.md
+-rw-r--r--   0        0        0      700 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    13901 2023-06-30 11:32:46.030344 pydivkit-25.7.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      884 2023-06-30 11:32:45.781249 pydivkit-25.7.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      898 2023-06-30 11:32:45.781447 pydivkit-25.7.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      879 2023-06-30 11:32:45.781901 pydivkit-25.7.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2023-06-30 11:32:45.768330 pydivkit-25.7.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2023-06-30 11:32:45.773659 pydivkit-25.7.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3285 2023-06-30 11:32:45.782394 pydivkit-25.7.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     3671 2023-06-30 11:32:45.783346 pydivkit-25.7.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0      285 2023-06-30 11:32:45.782543 pydivkit-25.7.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2023-06-30 11:32:45.788687 pydivkit-25.7.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3038 2023-06-30 11:32:45.797990 pydivkit-25.7.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2023-06-30 11:32:45.789016 pydivkit-25.7.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2023-06-30 11:32:45.791548 pydivkit-25.7.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2023-06-30 11:32:45.788125 pydivkit-25.7.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2023-06-30 11:32:45.790196 pydivkit-25.7.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2023-06-30 11:32:45.790066 pydivkit-25.7.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9833 2023-06-30 11:32:45.809339 pydivkit-25.7.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2023-06-30 11:32:45.796876 pydivkit-25.7.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2023-06-30 11:32:45.799481 pydivkit-25.7.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1697 2023-06-30 11:32:45.798774 pydivkit-25.7.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2023-06-30 11:32:45.802893 pydivkit-25.7.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2023-06-30 11:32:45.801312 pydivkit-25.7.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2023-06-30 11:32:45.797743 pydivkit-25.7.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2023-06-30 11:32:45.808208 pydivkit-25.7.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0    17693 2023-06-30 11:32:45.856440 pydivkit-25.7.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      396 2023-06-30 11:32:45.806978 pydivkit-25.7.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2023-06-30 11:32:45.807227 pydivkit-25.7.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2023-06-30 11:32:45.813508 pydivkit-25.7.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2023-06-30 11:32:45.806726 pydivkit-25.7.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1292 2023-06-30 11:32:45.813258 pydivkit-25.7.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10752 2023-06-30 11:32:45.851666 pydivkit-25.7.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2915 2023-06-30 11:32:45.818082 pydivkit-25.7.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2023-06-30 11:32:45.817813 pydivkit-25.7.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2023-06-30 11:32:45.815439 pydivkit-25.7.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     2970 2023-06-30 11:32:45.823213 pydivkit-25.7.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1228 2023-06-30 11:32:45.821063 pydivkit-25.7.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2023-06-30 11:32:45.821876 pydivkit-25.7.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     1385 2023-06-30 11:32:45.827364 pydivkit-25.7.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      827 2023-06-30 11:32:45.828612 pydivkit-25.7.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2023-06-30 11:32:45.835158 pydivkit-25.7.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      271 2023-06-30 11:32:45.829825 pydivkit-25.7.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      686 2023-06-30 11:32:45.832012 pydivkit-25.7.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3313 2023-06-30 11:32:45.841142 pydivkit-25.7.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1090 2023-06-30 11:32:45.841686 pydivkit-25.7.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     3026 2023-06-30 11:32:45.842834 pydivkit-25.7.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2023-06-30 11:32:45.838220 pydivkit-25.7.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    14582 2023-06-30 11:32:45.876045 pydivkit-25.7.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14431 2023-06-30 11:32:45.879042 pydivkit-25.7.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12886 2023-06-30 11:32:45.877903 pydivkit-25.7.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    16177 2023-06-30 11:32:45.886837 pydivkit-25.7.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2552 2023-06-30 11:32:45.857177 pydivkit-25.7.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2023-06-30 11:32:45.853746 pydivkit-25.7.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13998 2023-06-30 11:32:45.890014 pydivkit-25.7.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2023-06-30 11:32:45.860161 pydivkit-25.7.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2023-06-30 11:32:45.865772 pydivkit-25.7.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16458 2023-06-30 11:32:45.930319 pydivkit-25.7.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      403 2023-06-30 11:32:45.867781 pydivkit-25.7.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      671 2023-06-30 11:32:45.872367 pydivkit-25.7.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2023-06-30 11:32:45.874811 pydivkit-25.7.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1323 2023-06-30 11:32:45.882317 pydivkit-25.7.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1765 2023-06-30 11:32:45.888107 pydivkit-25.7.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1697 2023-06-30 11:32:45.888091 pydivkit-25.7.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2023-06-30 11:32:45.885163 pydivkit-25.7.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2023-06-30 11:32:45.888410 pydivkit-25.7.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2023-06-30 11:32:45.894475 pydivkit-25.7.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2023-06-30 11:32:45.895232 pydivkit-25.7.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2023-06-30 11:32:45.897606 pydivkit-25.7.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2023-06-30 11:32:45.898273 pydivkit-25.7.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0    13014 2023-06-30 11:32:45.924238 pydivkit-25.7.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2023-06-30 11:32:45.893109 pydivkit-25.7.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1950 2023-06-30 11:32:45.905630 pydivkit-25.7.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2023-06-30 11:32:45.904332 pydivkit-25.7.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      357 2023-06-30 11:32:45.899756 pydivkit-25.7.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1136 2023-06-30 11:32:45.904950 pydivkit-25.7.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2023-06-30 11:32:45.907253 pydivkit-25.7.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2023-06-30 11:32:45.904791 pydivkit-25.7.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2023-06-30 11:32:45.913307 pydivkit-25.7.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2023-06-30 11:32:45.910337 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1156 2023-06-30 11:32:45.916966 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2023-06-30 11:32:45.912141 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2023-06-30 11:32:45.915905 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2023-06-30 11:32:45.917465 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2023-06-30 11:32:45.923814 pydivkit-25.7.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2023-06-30 11:32:45.930929 pydivkit-25.7.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13890 2023-06-30 11:32:45.956362 pydivkit-25.7.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    13054 2023-06-30 11:32:45.952789 pydivkit-25.7.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2023-06-30 11:32:45.924609 pydivkit-25.7.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2023-06-30 11:32:45.922132 pydivkit-25.7.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2023-06-30 11:32:45.934871 pydivkit-25.7.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2165 2023-06-30 11:32:45.936122 pydivkit-25.7.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2023-06-30 11:32:45.930235 pydivkit-25.7.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2023-06-30 11:32:45.933138 pydivkit-25.7.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2023-06-30 11:32:45.943727 pydivkit-25.7.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    15030 2023-06-30 11:32:45.980307 pydivkit-25.7.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2023-06-30 11:32:45.940072 pydivkit-25.7.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13360 2023-06-30 11:32:45.981759 pydivkit-25.7.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2023-06-30 11:32:45.945288 pydivkit-25.7.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2023-06-30 11:32:45.948881 pydivkit-25.7.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20553 2023-06-30 11:32:46.013984 pydivkit-25.7.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25644 2023-06-30 11:32:46.018547 pydivkit-25.7.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2023-06-30 11:32:45.950652 pydivkit-25.7.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2023-06-30 11:32:45.956329 pydivkit-25.7.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2023-06-30 11:32:45.960020 pydivkit-25.7.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2796 2023-06-30 11:32:45.963845 pydivkit-25.7.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2923 2023-06-30 11:32:45.974324 pydivkit-25.7.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2023-06-30 11:32:45.966110 pydivkit-25.7.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2023-06-30 11:32:45.969969 pydivkit-25.7.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2023-06-30 11:32:45.975480 pydivkit-25.7.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2023-06-30 11:32:45.976638 pydivkit-25.7.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2023-06-30 11:32:45.984727 pydivkit-25.7.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      613 2023-06-30 11:32:45.980644 pydivkit-25.7.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    13675 2023-06-30 11:32:46.027816 pydivkit-25.7.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0     2331 2023-06-30 11:32:45.990717 pydivkit-25.7.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2023-06-30 11:32:45.987531 pydivkit-25.7.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     2956 2023-06-30 11:32:45.992519 pydivkit-25.7.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2023-06-30 11:32:45.995316 pydivkit-25.7.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      866 2023-06-30 11:32:45.996831 pydivkit-25.7.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      872 2023-06-30 11:32:45.998793 pydivkit-25.7.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      860 2023-06-30 11:32:46.001820 pydivkit-25.7.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      882 2023-06-30 11:32:46.005354 pydivkit-25.7.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-25.7.0/PKG-INFO
```

### Comparing `pydivkit-25.6.0/README.md` & `pydivkit-25.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/__init__.py` & `pydivkit-25.7.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/core/entities.py` & `pydivkit-25.7.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/core/fields.py` & `pydivkit-25.7.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/core/types/union.py` & `pydivkit-25.7.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/__init__.py` & `pydivkit-25.7.0/pydivkit/div/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Generated code. Do not modify.
 # flake8: noqa: F405
 
 from .boolean_variable import BooleanVariable
 from .color_variable import ColorVariable
+from .dict_variable import DictVariable
 from .div import Div
 from .div_absolute_edge_insets import DivAbsoluteEdgeInsets
 from .div_accessibility import (
     DivAccessibility, DivAccessibilityMode, DivAccessibilityType,
 )
 from .div_action import DivAction, DivActionMenuItem, DivActionTarget
 from .div_alignment_horizontal import DivAlignmentHorizontal
@@ -25,14 +26,16 @@
 from .div_change_set_transition import DivChangeSetTransition
 from .div_change_transition import DivChangeTransition
 from .div_circle_shape import DivCircleShape
 from .div_container import (
     DivContainer, DivContainerLayoutMode, DivContainerOrientation,
     DivContainerSeparator,
 )
+from .div_content_alignment_horizontal import DivContentAlignmentHorizontal
+from .div_content_alignment_vertical import DivContentAlignmentVertical
 from .div_corners_radius import DivCornersRadius
 from .div_count import DivCount
 from .div_currency_input_mask import DivCurrencyInputMask
 from .div_custom import DivCustom
 from .div_data import DivData, DivDataState
 from .div_default_indicator_item_placement import (
     DivDefaultIndicatorItemPlacement,
@@ -47,15 +50,14 @@
 from .div_filter import DivFilter
 from .div_fixed_count import DivFixedCount
 from .div_fixed_length_input_mask import (
     DivFixedLengthInputMask, DivFixedLengthInputMaskPatternElement,
 )
 from .div_fixed_size import DivFixedSize
 from .div_focus import DivFocus, DivFocusNextFocusIds
-from .div_font_family import DivFontFamily
 from .div_font_weight import DivFontWeight
 from .div_gallery import (
     DivGallery, DivGalleryCrossContentAlignment, DivGalleryOrientation,
     DivGalleryScrollMode,
 )
 from .div_gif_image import DivGifImage
 from .div_grid import DivGrid
@@ -99,14 +101,15 @@
 from .div_select import DivSelect, DivSelectOption
 from .div_separator import (
     DelimiterStyleOrientation, DivSeparator, DivSeparatorDelimiterStyle,
 )
 from .div_shadow import DivShadow
 from .div_shape import DivShape
 from .div_shape_drawable import DivShapeDrawable
+from .div_sight_action import DivSightAction
 from .div_size import DivSize
 from .div_size_unit import DivSizeUnit
 from .div_slide_transition import DivSlideTransition, DivSlideTransitionEdge
 from .div_slider import DivSlider, DivSliderTextStyle
 from .div_solid_background import DivSolidBackground
 from .div_state import DivState, DivStateState
 from .div_stretch_indicator_item_placement import (
@@ -141,14 +144,15 @@
 from .number_variable import NumberVariable
 from .string_variable import StringVariable
 from .url_variable import UrlVariable
 
 
 BooleanVariable.update_forward_refs()
 ColorVariable.update_forward_refs()
+DictVariable.update_forward_refs()
 DivAbsoluteEdgeInsets.update_forward_refs()
 DivAccessibility.update_forward_refs()
 DivAction.update_forward_refs()
 DivActionMenuItem.update_forward_refs()
 DivAnimation.update_forward_refs()
 DivAppearanceSetTransition.update_forward_refs()
 DivAspect.update_forward_refs()
@@ -211,14 +215,15 @@
 DivScaleTransition.update_forward_refs()
 DivSelect.update_forward_refs()
 DivSelectOption.update_forward_refs()
 DivSeparator.update_forward_refs()
 DivSeparatorDelimiterStyle.update_forward_refs()
 DivShadow.update_forward_refs()
 DivShapeDrawable.update_forward_refs()
+DivSightAction.update_forward_refs()
 DivSlideTransition.update_forward_refs()
 DivSlider.update_forward_refs()
 DivSliderTextStyle.update_forward_refs()
 DivSolidBackground.update_forward_refs()
 DivState.update_forward_refs()
 DivStateState.update_forward_refs()
 DivStretchIndicatorItemPlacement.update_forward_refs()
@@ -243,8 +248,8 @@
 DivWrapContentSize.update_forward_refs()
 DivWrapContentSizeConstraintSize.update_forward_refs()
 IntegerVariable.update_forward_refs()
 NumberVariable.update_forward_refs()
 StringVariable.update_forward_refs()
 UrlVariable.update_forward_refs()
 
-__all__ = ("BooleanVariable", "ColorVariable", "DelimiterStyleOrientation", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionMenuItem", "DivActionTarget", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontFamily", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivVariable", "DivVideo", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerVariable", "NumberVariable", "StringVariable", "TabTitleStyleAnimationType", "UrlVariable")
+__all__ = ("BooleanVariable", "ColorVariable", "DelimiterStyleOrientation", "DictVariable", "Div", "DivAbsoluteEdgeInsets", "DivAccessibility", "DivAccessibilityMode", "DivAccessibilityType", "DivAction", "DivActionMenuItem", "DivActionTarget", "DivAlignmentHorizontal", "DivAlignmentVertical", "DivAnimation", "DivAnimationInterpolator", "DivAnimationName", "DivAppearanceSetTransition", "DivAppearanceTransition", "DivAspect", "DivBackground", "DivBase", "DivBlendMode", "DivBlur", "DivBorder", "DivChangeBoundsTransition", "DivChangeSetTransition", "DivChangeTransition", "DivCircleShape", "DivContainer", "DivContainerLayoutMode", "DivContainerOrientation", "DivContainerSeparator", "DivContentAlignmentHorizontal", "DivContentAlignmentVertical", "DivCornersRadius", "DivCount", "DivCurrencyInputMask", "DivCustom", "DivData", "DivDataState", "DivDefaultIndicatorItemPlacement", "DivDimension", "DivDisappearAction", "DivDownloadCallbacks", "DivDrawable", "DivEdgeInsets", "DivExtension", "DivFadeTransition", "DivFilter", "DivFixedCount", "DivFixedLengthInputMask", "DivFixedLengthInputMaskPatternElement", "DivFixedSize", "DivFocus", "DivFocusNextFocusIds", "DivFontWeight", "DivGallery", "DivGalleryCrossContentAlignment", "DivGalleryOrientation", "DivGalleryScrollMode", "DivGifImage", "DivGrid", "DivImage", "DivImageBackground", "DivImageScale", "DivIndicator", "DivIndicatorAnimation", "DivIndicatorItemPlacement", "DivInfinityCount", "DivInput", "DivInputKeyboardType", "DivInputMask", "DivInputMaskBase", "DivInputNativeInterface", "DivInputValidator", "DivInputValidatorBase", "DivInputValidatorExpression", "DivInputValidatorRegex", "DivLineStyle", "DivLinearGradient", "DivMatchParentSize", "DivNeighbourPageSize", "DivNinePatchBackground", "DivPageSize", "DivPager", "DivPagerLayoutMode", "DivPagerOrientation", "DivPatch", "DivPatchChange", "DivPatchMode", "DivPercentageSize", "DivPivot", "DivPivotFixed", "DivPivotPercentage", "DivPoint", "DivRadialGradient", "DivRadialGradientCenter", "DivRadialGradientFixedCenter", "DivRadialGradientRadius", "DivRadialGradientRelativeCenter", "DivRadialGradientRelativeRadius", "DivRadialGradientRelativeRadiusValue", "DivRoundedRectangleShape", "DivScaleTransition", "DivSelect", "DivSelectOption", "DivSeparator", "DivSeparatorDelimiterStyle", "DivShadow", "DivShape", "DivShapeDrawable", "DivSightAction", "DivSize", "DivSizeUnit", "DivSlideTransition", "DivSlideTransitionEdge", "DivSlider", "DivSliderTextStyle", "DivSolidBackground", "DivState", "DivStateState", "DivStretchIndicatorItemPlacement", "DivStroke", "DivTabs", "DivTabsItem", "DivTabsTabTitleStyle", "DivText", "DivTextEllipsis", "DivTextGradient", "DivTextImage", "DivTextRange", "DivTextRangeBackground", "DivTextRangeBorder", "DivTextTruncate", "DivTimer", "DivTooltip", "DivTooltipPosition", "DivTransform", "DivTransitionBase", "DivTransitionSelector", "DivTransitionTrigger", "DivTrigger", "DivTriggerMode", "DivVariable", "DivVideo", "DivVideoSource", "DivVideoSourceResolution", "DivVisibility", "DivVisibilityAction", "DivWrapContentSize", "DivWrapContentSizeConstraintSize", "IntegerVariable", "NumberVariable", "StringVariable", "TabTitleStyleAnimationType", "UrlVariable")
```

### Comparing `pydivkit-25.6.0/pydivkit/div/boolean_variable.py` & `pydivkit-25.7.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/color_variable.py` & `pydivkit-25.7.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div.py` & `pydivkit-25.7.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-25.7.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_accessibility.py` & `pydivkit-25.7.0/pydivkit/div/div_accessibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,10 +90,11 @@
     BUTTON = "button"
     IMAGE = "image"
     TEXT = "text"
     EDIT_TEXT = "edit_text"
     HEADER = "header"
     TAB_BAR = "tab_bar"
     LIST = "list"
+    SELECT = "select"
 
 
 DivAccessibility.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_action.py` & `pydivkit-25.7.0/pydivkit/div/div_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_animation.py` & `pydivkit-25.7.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_appearance_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_aspect.py` & `pydivkit-25.7.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_background.py` & `pydivkit-25.7.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_base.py` & `pydivkit-25.7.0/pydivkit/div/div_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_blur.py` & `pydivkit-25.7.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_border.py` & `pydivkit-25.7.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_change_set_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_circle_shape.py` & `pydivkit-25.7.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_container.py` & `pydivkit-25.7.0/pydivkit/div/div_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_animation, div_appearance_transition,
     div_aspect, div_background, div_border, div_change_transition,
+    div_content_alignment_horizontal, div_content_alignment_vertical,
     div_disappear_action, div_drawable, div_edge_insets, div_extension,
     div_focus, div_size, div_tooltip, div_transform, div_transition_trigger,
     div_visibility, div_visibility_action,
 )
 
 
 # Container. It contains other elements and is responsible for their location. It
@@ -33,16 +34,16 @@
         alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
         alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
         alpha: typing.Optional[typing.Union[Expr, float]] = None,
         aspect: typing.Optional[div_aspect.DivAspect] = None,
         background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
         column_span: typing.Optional[typing.Union[Expr, int]] = None,
-        content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
-        content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
+        content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_content_alignment_horizontal.DivContentAlignmentHorizontal]] = None,
+        content_alignment_vertical: typing.Optional[typing.Union[Expr, div_content_alignment_vertical.DivContentAlignmentVertical]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         height: typing.Optional[div_size.DivSize] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
         items: typing.Optional[typing.Sequence[div.Div]] = None,
@@ -166,21 +167,21 @@
     )
     column_span: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Merges cells in a column of the [grid](div-grid.md) "
             "element."
         ),
     )
-    content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
+    content_alignment_horizontal: typing.Optional[typing.Union[Expr, div_content_alignment_horizontal.DivContentAlignmentHorizontal]] = Field(
         description=(
             "Horizontal element alignment. For child elements, it can be "
             "redefined using the`alignment_horizontal` property."
         ),
     )
-    content_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
+    content_alignment_vertical: typing.Optional[typing.Union[Expr, div_content_alignment_vertical.DivContentAlignmentVertical]] = Field(
         description=(
             "Vertical element alignment. The `baseline` value aligns "
             "elements along their ownspecified baseline (for text and "
             "other elements that have a baseline). Elementsthat don\'t "
             "have their baseline value specified are aligned along the "
             "top edge.For child elements, it can be redefined using the "
             "`alignment_vertical` property."
@@ -355,28 +356,33 @@
     OVERLAP = "overlap"
 
 
 class DivContainerSeparator(BaseDiv):
 
     def __init__(
         self, *,
+        margins: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         show_at_end: typing.Optional[typing.Union[Expr, bool]] = None,
         show_at_start: typing.Optional[typing.Union[Expr, bool]] = None,
         show_between: typing.Optional[typing.Union[Expr, bool]] = None,
         style: typing.Optional[div_drawable.DivDrawable] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
+            margins=margins,
             show_at_end=show_at_end,
             show_at_start=show_at_start,
             show_between=show_between,
             style=style,
             **kwargs,
         )
 
+    margins: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
+        description="External margins from the element stroke.",
+    )
     show_at_end: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Enables displaying the separator after the last item.",
     )
     show_at_start: typing.Optional[typing.Union[Expr, bool]] = Field(
         description="Enables displaying the separator before the first item.",
     )
     show_between: typing.Optional[typing.Union[Expr, bool]] = Field(
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_corners_radius.py` & `pydivkit-25.7.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_currency_input_mask.py` & `pydivkit-25.7.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_custom.py` & `pydivkit-25.7.0/pydivkit/div/div_custom.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_data.py` & `pydivkit-25.7.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-25.7.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_dimension.py` & `pydivkit-25.7.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_disappear_action.py` & `pydivkit-25.7.0/pydivkit/div/div_disappear_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import div_download_callbacks
 
 
-# Actions performed when an element becomes invisible.
+# Actions performed when an element is no longer visible.
 class DivDisappearAction(BaseDiv):
 
     def __init__(
         self, *,
         disappear_duration: typing.Optional[typing.Union[Expr, int]] = None,
         download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = None,
         log_id: typing.Optional[typing.Union[Expr, str]] = None,
@@ -37,15 +37,15 @@
             visibility_percentage=visibility_percentage,
             **kwargs,
         )
 
     disappear_duration: typing.Optional[typing.Union[Expr, int]] = Field(
         description=(
             "Time in milliseconds during which an element must be "
-            "invisible to trigger`disappear-action`."
+            "outside the visible area totrigger `disappear-action`."
         ),
     )
     download_callbacks: typing.Optional[div_download_callbacks.DivDownloadCallbacks] = Field(
         description=(
             "Callbacks that are called after "
             "[dataloading](../../interaction.dita#loading-data)."
         ),
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_download_callbacks.py` & `pydivkit-25.7.0/pydivkit/div/div_download_callbacks.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_edge_insets.py` & `pydivkit-25.7.0/pydivkit/div/div_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_extension.py` & `pydivkit-25.7.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_fade_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_fixed_count.py` & `pydivkit-25.7.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-25.7.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_fixed_size.py` & `pydivkit-25.7.0/pydivkit/div/div_fixed_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_focus.py` & `pydivkit-25.7.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_gallery.py` & `pydivkit-25.7.0/pydivkit/div/div_gallery.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_gif_image.py` & `pydivkit-25.7.0/pydivkit/div/div_gif_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_grid.py` & `pydivkit-25.7.0/pydivkit/div/div_grid.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_image.py` & `pydivkit-25.7.0/pydivkit/div/div_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_image_background.py` & `pydivkit-25.7.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_indicator.py` & `pydivkit-25.7.0/pydivkit/div/div_indicator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_infinity_count.py` & `pydivkit-25.7.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_input.py` & `pydivkit-25.7.0/pydivkit/div/div_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
     div_border, div_change_transition, div_disappear_action, div_edge_insets,
-    div_extension, div_focus, div_font_family, div_font_weight, div_input_mask,
+    div_extension, div_focus, div_font_weight, div_input_mask,
     div_input_validator, div_size, div_size_unit, div_tooltip, div_transform,
     div_transition_trigger, div_visibility, div_visibility_action,
 )
 
 
 # Text input element.
 class DivInput(BaseDiv):
@@ -30,15 +30,15 @@
         alpha: typing.Optional[typing.Union[Expr, float]] = None,
         background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
         column_span: typing.Optional[typing.Union[Expr, int]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
-        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_family: typing.Optional[typing.Union[Expr, str]] = None,
         font_size: typing.Optional[typing.Union[Expr, int]] = None,
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
         highlight_color: typing.Optional[typing.Union[Expr, str]] = None,
         hint_color: typing.Optional[typing.Union[Expr, str]] = None,
         hint_text: typing.Optional[typing.Union[Expr, str]] = None,
@@ -50,14 +50,16 @@
         mask: typing.Optional[div_input_mask.DivInputMask] = None,
         max_visible_lines: typing.Optional[typing.Union[Expr, int]] = None,
         native_interface: typing.Optional[DivInputNativeInterface] = None,
         paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = None,
         row_span: typing.Optional[typing.Union[Expr, int]] = None,
         select_all_on_focus: typing.Optional[typing.Union[Expr, bool]] = None,
         selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
+        text_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = None,
+        text_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = None,
         text_color: typing.Optional[typing.Union[Expr, str]] = None,
         text_variable: typing.Optional[typing.Union[Expr, str]] = None,
         tooltips: typing.Optional[typing.Sequence[div_tooltip.DivTooltip]] = None,
         transform: typing.Optional[div_transform.DivTransform] = None,
         transition_change: typing.Optional[div_change_transition.DivChangeTransition] = None,
         transition_in: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
         transition_out: typing.Optional[div_appearance_transition.DivAppearanceTransition] = None,
@@ -97,14 +99,16 @@
             mask=mask,
             max_visible_lines=max_visible_lines,
             native_interface=native_interface,
             paddings=paddings,
             row_span=row_span,
             select_all_on_focus=select_all_on_focus,
             selected_actions=selected_actions,
+            text_alignment_horizontal=text_alignment_horizontal,
+            text_alignment_vertical=text_alignment_vertical,
             text_color=text_color,
             text_variable=text_variable,
             tooltips=tooltips,
             transform=transform,
             transition_change=transition_change,
             transition_in=transition_in,
             transition_out=transition_out,
@@ -162,15 +166,16 @@
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
-    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+    font_family: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
     font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Font size.",
@@ -258,14 +263,20 @@
     selected_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
             "List of [actions](div-action.md) to be executed when "
             "selecting an element in[pager](div-pager.md)."
         ),
     )
+    text_alignment_horizontal: typing.Optional[typing.Union[Expr, div_alignment_horizontal.DivAlignmentHorizontal]] = Field(
+        description="Horizontal text alignment.",
+    )
+    text_alignment_vertical: typing.Optional[typing.Union[Expr, div_alignment_vertical.DivAlignmentVertical]] = Field(
+        description="Vertical text alignment.",
+    )
     text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Text color.",
     )
     text_variable: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Name of text storage variable.",
@@ -310,15 +321,18 @@
         description=(
             "Animation starting triggers. Default value: `[state_change, "
             "visibility_change]`."
         ),
     )
     validators: typing.Optional[typing.Sequence[div_input_validator.DivInputValidator]] = Field(
         min_items=1, 
-        description="Validators for text value.",
+        description=(
+            "Validator that checks that the field value meets the "
+            "specified conditions."
+        ),
     )
     visibility: typing.Optional[typing.Union[Expr, div_visibility.DivVisibility]] = Field(
         description="Element visibility.",
     )
     visibility_action: typing.Optional[div_visibility_action.DivVisibilityAction] = Field(
         description=(
             "Tracking visibility of a single element. Not used if the "
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_input_mask_base.py` & `pydivkit-25.7.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_input_validator_base.py` & `pydivkit-25.7.0/pydivkit/div/dict_variable.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,40 +5,35 @@
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 
-class DivInputValidatorBase(BaseDiv):
+# An arbitrary object in JSON format.
+class DictVariable(BaseDiv):
 
     def __init__(
         self, *,
-        allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
-        label_id: typing.Optional[typing.Union[Expr, str]] = None,
-        variable: typing.Optional[typing.Union[Expr, str]] = None,
+        type: str = "dict",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Dict[str, typing.Any]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
-            allow_empty=allow_empty,
-            label_id=label_id,
-            variable=variable,
+            type=type,
+            name=name,
+            value=value,
             **kwargs,
         )
 
-    allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
-        description="Whether an empty value is correct. By default, false.",
-    )
-    label_id: typing.Optional[typing.Union[Expr, str]] = Field(
+    type: str = Field(default="dict")
+    name: typing.Union[Expr, str] = Field(
         min_length=1, 
-        description=(
-            "ID of the text div containing the error message, which will "
-            "also be used foraccessibility."
-        ),
+        description="Variable name.",
     )
-    variable: typing.Optional[typing.Union[Expr, str]] = Field(
-        min_length=1, 
-        description="Name of validation storage variable.",
+    value: typing.Dict[str, typing.Any] = Field(
+        description="Value.",
     )
 
 
-DivInputValidatorBase.update_forward_refs()
+DictVariable.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_input_validator_expression.py` & `pydivkit-25.7.0/pydivkit/div/div_input_validator_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,50 +5,43 @@
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 
-# Expression validator.
-class DivInputValidatorExpression(BaseDiv):
+class DivInputValidatorBase(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "expression",
         allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
-        condition: typing.Optional[typing.Union[Expr, str]] = None,
         label_id: typing.Optional[typing.Union[Expr, str]] = None,
         variable: typing.Optional[typing.Union[Expr, str]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
-            type=type,
             allow_empty=allow_empty,
-            condition=condition,
             label_id=label_id,
             variable=variable,
             **kwargs,
         )
 
-    type: str = Field(default="expression")
     allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
-        description="Whether an empty value is correct. By default, false.",
+        description="Determines whether the empty field value is valid.",
     )
-    condition: typing.Union[Expr, str] = Field(
-        min_length=1, 
-        description="Expression condition for evaluating.",
-    )
-    label_id: typing.Union[Expr, str] = Field(
+    label_id: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
-            "ID of the text div containing the error message, which will "
-            "also be used foraccessibility."
+            "ID of the text element containing the error message. The "
+            "message will also beused for providing access."
         ),
     )
-    variable: typing.Union[Expr, str] = Field(
+    variable: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
-        description="Name of validation storage variable.",
+        description=(
+            "The name of the variable that stores the calculation "
+            "results."
+        ),
     )
 
 
-DivInputValidatorExpression.update_forward_refs()
+DivInputValidatorBase.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_input_validator_regex.py` & `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,51 +4,41 @@
 from __future__ import annotations
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
+from . import div_size_unit
 
-# Regex validator.
-class DivInputValidatorRegex(BaseDiv):
+
+# Fixed coordinates of the central point of the gradient.
+class DivRadialGradientFixedCenter(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "regex",
-        allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
-        label_id: typing.Optional[typing.Union[Expr, str]] = None,
-        pattern: typing.Optional[typing.Union[Expr, str]] = None,
-        variable: typing.Optional[typing.Union[Expr, str]] = None,
+        type: str = "fixed",
+        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        value: typing.Optional[typing.Union[Expr, int]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            allow_empty=allow_empty,
-            label_id=label_id,
-            pattern=pattern,
-            variable=variable,
+            unit=unit,
+            value=value,
             **kwargs,
         )
 
-    type: str = Field(default="regex")
-    allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
-        description="Whether an empty value is correct. By default, false.",
-    )
-    label_id: typing.Union[Expr, str] = Field(
-        min_length=1, 
+    type: str = Field(default="fixed")
+    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
         description=(
-            "ID of the text div containing the error message, which will "
-            "also be used foraccessibility."
+            "Unit of measurement. To learn more about units of size "
+            "measurement, see [Layoutinside the "
+            "card](../../layout.dita)."
         ),
     )
-    pattern: typing.Union[Expr, str] = Field(
-        min_length=1, 
-        description="Regex pattern for matching.",
-    )
-    variable: typing.Union[Expr, str] = Field(
-        min_length=1, 
-        description="Name of validation storage variable.",
+    value: typing.Union[Expr, int] = Field(
+        description="Coordinate value.",
     )
 
 
-DivInputValidatorRegex.update_forward_refs()
+DivRadialGradientFixedCenter.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_linear_gradient.py` & `pydivkit-25.7.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_match_parent_size.py` & `pydivkit-25.7.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-25.7.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_nine_patch_background.py` & `pydivkit-25.7.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_page_size.py` & `pydivkit-25.7.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_pager.py` & `pydivkit-25.7.0/pydivkit/div/div_pager.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_patch.py` & `pydivkit-25.7.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_percentage_size.py` & `pydivkit-25.7.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-25.7.0/pydivkit/div/div_pivot_fixed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-25.7.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_point.py` & `pydivkit-25.7.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_radial_gradient.py` & `pydivkit-25.7.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-25.7.0/pydivkit/div/integer_variable.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,41 +4,36 @@
 from __future__ import annotations
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_size_unit
 
-
-# Fixed coordinates of the central point of the gradient.
-class DivRadialGradientFixedCenter(BaseDiv):
+# An integer variable.
+class IntegerVariable(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "fixed",
-        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        type: str = "integer",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
         value: typing.Optional[typing.Union[Expr, int]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            unit=unit,
+            name=name,
             value=value,
             **kwargs,
         )
 
-    type: str = Field(default="fixed")
-    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
-        description=(
-            "Unit of measurement. To learn more about units of size "
-            "measurement, see [Layoutinside the "
-            "card](../../layout.dita)."
-        ),
+    type: str = Field(default="integer")
+    name: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Variable name.",
     )
     value: typing.Union[Expr, int] = Field(
-        description="Coordinate value.",
+        description="Value.",
     )
 
 
-DivRadialGradientFixedCenter.update_forward_refs()
+IntegerVariable.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-25.7.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_scale_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_select.py` & `pydivkit-25.7.0/pydivkit/div/div_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
     div_border, div_change_transition, div_disappear_action, div_edge_insets,
-    div_extension, div_focus, div_font_family, div_font_weight, div_size,
-    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_extension, div_focus, div_font_weight, div_size, div_size_unit,
+    div_tooltip, div_transform, div_transition_trigger, div_visibility,
+    div_visibility_action,
 )
 
 
 # List of options with only one to be selected.
 class DivSelect(BaseDiv):
 
     def __init__(
@@ -30,15 +30,15 @@
         alpha: typing.Optional[typing.Union[Expr, float]] = None,
         background: typing.Optional[typing.Sequence[div_background.DivBackground]] = None,
         border: typing.Optional[div_border.DivBorder] = None,
         column_span: typing.Optional[typing.Union[Expr, int]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
-        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_family: typing.Optional[typing.Union[Expr, str]] = None,
         font_size: typing.Optional[typing.Union[Expr, int]] = None,
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
         hint_color: typing.Optional[typing.Union[Expr, str]] = None,
         hint_text: typing.Optional[typing.Union[Expr, str]] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
@@ -150,15 +150,16 @@
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
-    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+    font_family: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
     font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Font size.",
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_separator.py` & `pydivkit-25.7.0/pydivkit/div/div_separator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_shadow.py` & `pydivkit-25.7.0/pydivkit/div/div_shadow.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_shape_drawable.py` & `pydivkit-25.7.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_slide_transition.py` & `pydivkit-25.7.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_slider.py` & `pydivkit-25.7.0/pydivkit/div/div_slider.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_solid_background.py` & `pydivkit-25.7.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_state.py` & `pydivkit-25.7.0/pydivkit/div/div_state.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-25.7.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_stroke.py` & `pydivkit-25.7.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_tabs.py` & `pydivkit-25.7.0/pydivkit/div/div_tabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div, div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_appearance_transition, div_background,
     div_border, div_change_transition, div_corners_radius, div_disappear_action,
-    div_edge_insets, div_extension, div_focus, div_font_family, div_font_weight,
-    div_size, div_size_unit, div_tooltip, div_transform, div_transition_trigger,
+    div_edge_insets, div_extension, div_focus, div_font_weight, div_size,
+    div_size_unit, div_tooltip, div_transform, div_transition_trigger,
     div_visibility, div_visibility_action,
 )
 
 
 # Tabs. Height of the first tab is determined by its contents, and height of the
 # remaining [depends on the platform](../../location.dita#tabs).
 class DivTabs(BaseDiv):
@@ -344,15 +344,15 @@
         active_background_color: typing.Optional[typing.Union[Expr, str]] = None,
         active_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         active_text_color: typing.Optional[typing.Union[Expr, str]] = None,
         animation_duration: typing.Optional[typing.Union[Expr, int]] = None,
         animation_type: typing.Optional[typing.Union[Expr, TabTitleStyleAnimationType]] = None,
         corner_radius: typing.Optional[typing.Union[Expr, int]] = None,
         corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = None,
-        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_family: typing.Optional[typing.Union[Expr, str]] = None,
         font_size: typing.Optional[typing.Union[Expr, int]] = None,
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         inactive_background_color: typing.Optional[typing.Union[Expr, str]] = None,
         inactive_font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         inactive_text_color: typing.Optional[typing.Union[Expr, str]] = None,
         item_spacing: typing.Optional[typing.Union[Expr, int]] = None,
@@ -409,15 +409,16 @@
     )
     corners_radius: typing.Optional[div_corners_radius.DivCornersRadius] = Field(
         description=(
             "Rounding radii of corners of multiple titles. Empty values "
             "are replaced by`corner_radius`."
         ),
     )
-    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+    font_family: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
     font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Title font size.",
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_text.py` & `pydivkit-25.7.0/pydivkit/div/div_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
     div_accessibility, div_action, div_alignment_horizontal,
     div_alignment_vertical, div_animation, div_appearance_transition,
     div_background, div_blend_mode, div_border, div_change_transition,
     div_disappear_action, div_edge_insets, div_extension, div_fixed_size,
-    div_focus, div_font_family, div_font_weight, div_line_style, div_size,
-    div_size_unit, div_text_gradient, div_text_range_background,
-    div_text_range_border, div_tooltip, div_transform, div_transition_trigger,
-    div_visibility, div_visibility_action,
+    div_focus, div_font_weight, div_line_style, div_size, div_size_unit,
+    div_text_gradient, div_text_range_background, div_text_range_border,
+    div_tooltip, div_transform, div_transition_trigger, div_visibility,
+    div_visibility_action,
 )
 
 
 # Text.
 class DivText(BaseDiv):
 
     def __init__(
@@ -39,15 +39,15 @@
         column_span: typing.Optional[typing.Union[Expr, int]] = None,
         disappear_actions: typing.Optional[typing.Sequence[div_disappear_action.DivDisappearAction]] = None,
         doubletap_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         ellipsis: typing.Optional[DivTextEllipsis] = None,
         extensions: typing.Optional[typing.Sequence[div_extension.DivExtension]] = None,
         focus: typing.Optional[div_focus.DivFocus] = None,
         focused_text_color: typing.Optional[typing.Union[Expr, str]] = None,
-        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_family: typing.Optional[typing.Union[Expr, str]] = None,
         font_size: typing.Optional[typing.Union[Expr, int]] = None,
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         height: typing.Optional[div_size.DivSize] = None,
         id: typing.Optional[typing.Union[Expr, str]] = None,
         images: typing.Optional[typing.Sequence[DivTextImage]] = None,
         letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
@@ -217,15 +217,16 @@
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     focused_text_color: typing.Optional[typing.Union[Expr, str]] = Field(
         format="color", 
         description="Text color when focusing on the element.",
     )
-    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+    font_family: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
     font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Font size.",
@@ -503,15 +504,15 @@
 
     def __init__(
         self, *,
         actions: typing.Optional[typing.Sequence[div_action.DivAction]] = None,
         background: typing.Optional[div_text_range_background.DivTextRangeBackground] = None,
         border: typing.Optional[div_text_range_border.DivTextRangeBorder] = None,
         end: typing.Optional[typing.Union[Expr, int]] = None,
-        font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = None,
+        font_family: typing.Optional[typing.Union[Expr, str]] = None,
         font_size: typing.Optional[typing.Union[Expr, int]] = None,
         font_size_unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
         font_weight: typing.Optional[typing.Union[Expr, div_font_weight.DivFontWeight]] = None,
         letter_spacing: typing.Optional[typing.Union[Expr, float]] = None,
         line_height: typing.Optional[typing.Union[Expr, int]] = None,
         start: typing.Optional[typing.Union[Expr, int]] = None,
         strike: typing.Optional[typing.Union[Expr, div_line_style.DivLineStyle]] = None,
@@ -551,15 +552,16 @@
     )
     end: typing.Union[Expr, int] = Field(
         description=(
             "Ordinal number of the last character to be included in the "
             "range."
         ),
     )
-    font_family: typing.Optional[typing.Union[Expr, div_font_family.DivFontFamily]] = Field(
+    font_family: typing.Optional[typing.Union[Expr, str]] = Field(
+        min_length=1, 
         description=(
             "Font family:`text` — a standard text font;`display` — a "
             "family of fonts with alarge font size."
         ),
     )
     font_size: typing.Optional[typing.Union[Expr, int]] = Field(
         description="Font size.",
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_text_range_border.py` & `pydivkit-25.7.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_timer.py` & `pydivkit-25.7.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_tooltip.py` & `pydivkit-25.7.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_transform.py` & `pydivkit-25.7.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_transition_base.py` & `pydivkit-25.7.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_trigger.py` & `pydivkit-25.7.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_variable.py` & `pydivkit-25.7.0/pydivkit/div/div_variable.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import enum
 import typing
 from typing import Union
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 from . import (
-    boolean_variable, color_variable, integer_variable, number_variable,
-    string_variable, url_variable,
+    boolean_variable, color_variable, dict_variable, integer_variable,
+    number_variable, string_variable, url_variable,
 )
 
 
 DivVariable = Union[
     string_variable.StringVariable,
     number_variable.NumberVariable,
     integer_variable.IntegerVariable,
     boolean_variable.BooleanVariable,
     color_variable.ColorVariable,
     url_variable.UrlVariable,
+    dict_variable.DictVariable,
 ]
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_video.py` & `pydivkit-25.7.0/pydivkit/div/div_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,16 @@
             "list of extensions isgiven in "
             "[DivExtension](../../extensions.dita)."
         ),
     )
     fatal_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
         description=(
-            "Actions that are performed when it is impossible to "
-            "continue playback due to anerror in the player."
+            "Actions performed when playback can\'t be continued due to "
+            "a player error."
         ),
     )
     focus: typing.Optional[div_focus.DivFocus] = Field(
         description="Parameters when focusing on an element or losing focus.",
     )
     height: typing.Optional[div_size.DivSize] = Field(
         description=(
@@ -207,15 +207,15 @@
         description="This option mutes video.",
     )
     paddings: typing.Optional[div_edge_insets.DivEdgeInsets] = Field(
         description="Internal margins from the element stroke.",
     )
     pause_actions: typing.Optional[typing.Sequence[div_action.DivAction]] = Field(
         min_items=1, 
-        description="Actions that are performed when a playback is paused.",
+        description="Actions performed when playback is paused.",
     )
     player_settings_payload: typing.Optional[typing.Dict[str, typing.Any]] = Field(
         description="Additional information that can be used in the player.",
     )
     preview: typing.Optional[typing.Union[Expr, str]] = Field(
         min_length=1, 
         description=(
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_video_source.py` & `pydivkit-25.7.0/pydivkit/div/div_input_validator_regex.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,92 +5,56 @@
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 
-class DivVideoSource(BaseDiv):
+# Regex validator.
+class DivInputValidatorRegex(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "video_source",
-        bitrate: typing.Optional[typing.Union[Expr, int]] = None,
-        mime_type: typing.Optional[typing.Union[Expr, str]] = None,
-        resolution: typing.Optional[DivVideoSourceResolution] = None,
-        url: typing.Optional[typing.Union[Expr, str]] = None,
+        type: str = "regex",
+        allow_empty: typing.Optional[typing.Union[Expr, bool]] = None,
+        label_id: typing.Optional[typing.Union[Expr, str]] = None,
+        pattern: typing.Optional[typing.Union[Expr, str]] = None,
+        variable: typing.Optional[typing.Union[Expr, str]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
-            bitrate=bitrate,
-            mime_type=mime_type,
-            resolution=resolution,
-            url=url,
+            allow_empty=allow_empty,
+            label_id=label_id,
+            pattern=pattern,
+            variable=variable,
             **kwargs,
         )
 
-    type: str = Field(default="video_source")
-    bitrate: typing.Optional[typing.Union[Expr, int]] = Field(
-        description=(
-            "Properties of the media file that determines the data "
-            "transfer rate in the videostream. Bitrate is measured in "
-            "kilobits per second (kbps) and indicates how muchdata is "
-            "transmitted per unit of time."
-        ),
-    )
-    mime_type: typing.Union[Expr, str] = Field(
-        description=(
-            "The property defines the MIME type (Multipurpose Internet "
-            "Mail Extensions) forthe media file. A MIME type is a string "
-            "that indicates the type of file contentand is used to "
-            "determine the type of file and its correct processing."
-        ),
+    type: str = Field(default="regex")
+    allow_empty: typing.Optional[typing.Union[Expr, bool]] = Field(
+        description="Determines whether the empty field value is valid.",
     )
-    resolution: typing.Optional[DivVideoSourceResolution] = Field(
-        description="Media file Resolution.",
-    )
-    url: typing.Union[Expr, str] = Field(
-        format="uri", 
+    label_id: typing.Union[Expr, str] = Field(
+        min_length=1, 
         description=(
-            "The property contains a link to a media file available for "
-            "playback or download."
+            "ID of the text element containing the error message. The "
+            "message will also beused for providing access."
         ),
     )
-
-
-# Media file Resolution.
-class DivVideoSourceResolution(BaseDiv):
-
-    def __init__(
-        self, *,
-        type: str = "resolution",
-        height: typing.Optional[typing.Union[Expr, int]] = None,
-        width: typing.Optional[typing.Union[Expr, int]] = None,
-        **kwargs: typing.Any,
-    ):
-        super().__init__(
-            type=type,
-            height=height,
-            width=width,
-            **kwargs,
-        )
-
-    type: str = Field(default="resolution")
-    height: typing.Union[Expr, int] = Field(
+    pattern: typing.Union[Expr, str] = Field(
+        min_length=1, 
         description=(
-            "Contains information about the resolution height of the "
-            "Media file."
+            "A regular expression (pattern) that the field value must "
+            "match."
         ),
     )
-    width: typing.Union[Expr, int] = Field(
+    variable: typing.Union[Expr, str] = Field(
+        min_length=1, 
         description=(
-            "Contains information about the resolution width of the "
-            "video file."
+            "The name of the variable that stores the calculation "
+            "results."
         ),
     )
 
 
-DivVideoSourceResolution.update_forward_refs()
-
-
-DivVideoSource.update_forward_refs()
+DivInputValidatorRegex.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/div_visibility_action.py` & `pydivkit-25.7.0/pydivkit/div/div_visibility_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/div_wrap_content_size.py` & `pydivkit-25.7.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/integer_variable.py` & `pydivkit-25.7.0/pydivkit/div/string_variable.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
 
-# An integer variable.
-class IntegerVariable(BaseDiv):
+# A string variable.
+class StringVariable(BaseDiv):
 
     def __init__(
         self, *,
-        type: str = "integer",
+        type: str = "string",
         name: typing.Optional[typing.Union[Expr, str]] = None,
-        value: typing.Optional[typing.Union[Expr, int]] = None,
+        value: typing.Optional[typing.Union[Expr, str]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
             type=type,
             name=name,
             value=value,
             **kwargs,
         )
 
-    type: str = Field(default="integer")
+    type: str = Field(default="string")
     name: typing.Union[Expr, str] = Field(
         min_length=1, 
         description="Variable name.",
     )
-    value: typing.Union[Expr, int] = Field(
+    value: typing.Union[Expr, str] = Field(
         description="Value.",
     )
 
 
-IntegerVariable.update_forward_refs()
+StringVariable.update_forward_refs()
```

### Comparing `pydivkit-25.6.0/pydivkit/div/number_variable.py` & `pydivkit-25.7.0/pydivkit/div/number_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pydivkit/div/url_variable.py` & `pydivkit-25.7.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.6.0/pyproject.toml` & `pydivkit-25.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "25.6.0"
+version = "25.7.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-25.6.0/PKG-INFO` & `pydivkit-25.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 25.6.0
+Version: 25.7.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

