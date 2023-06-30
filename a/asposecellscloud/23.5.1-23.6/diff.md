# Comparing `tmp/asposecellscloud-23.5.1.tar.gz` & `tmp/asposecellscloud-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\asposecellscloud-23.5.1.tar", last modified: Thu May 25 13:08:44 2023, max compression
+gzip compressed data, was "dist\asposecellscloud-23.6.tar", last modified: Fri Jun 30 00:06:04 2023, max compression
```

## Comparing `asposecellscloud-23.5.1.tar` & `asposecellscloud-23.6.tar`

### file list

```diff
@@ -1,640 +1,746 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:44.382692 asposecellscloud-23.5.1/
--rw-rw-rw-   0        0        0     1092 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/LICENSE
--rw-rw-rw-   0        0        0      900 2023-05-25 13:08:44.380698 asposecellscloud-23.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6827 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:37.724389 asposecellscloud-23.5.1/asposecellscloud/
--rw-rw-rw-   0        0        0    15740 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/__init__.py
--rw-rw-rw-   0        0        0    30491 2023-05-25 13:07:11.000000 asposecellscloud-23.5.1/asposecellscloud/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:37.782392 asposecellscloud-23.5.1/asposecellscloud/apis/
--rw-rw-rw-   0        0        0      128 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/apis/__init__.py
--rw-rw-rw-   0        0        0  2591815 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/apis/cells_api.py
--rw-rw-rw-   0        0        0    98544 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/apis/light_cells_api.py
--rw-rw-rw-   0        0        0    86342 2022-01-24 09:49:53.000000 asposecellscloud-23.5.1/asposecellscloud/apis/lite_cells_api.py
--rw-rw-rw-   0        0        0     8706 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:40.832996 asposecellscloud-23.5.1/asposecellscloud/models/
--rw-rw-rw-   0        0        0    13630 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/models/__init__.py
--rw-rw-rw-   0        0        0     7878 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/above_average.py
--rw-rw-rw-   0        0        0    10430 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/access_token_response.py
--rw-rw-rw-   0        0        0     8340 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/area.py
--rw-rw-rw-   0        0        0     6499 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_filter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_filter_response.py
--rw-rw-rw-   0        0        0     6636 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_fitter_options.py
--rw-rw-rw-   0        0        0    30150 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_shape.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_shape_response.py
--rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_shapes.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/auto_shapes_response.py
--rw-rw-rw-   0        0        0    30674 2022-12-08 06:28:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/axis.py
--rw-rw-rw-   0        0        0     4464 2022-12-08 06:28:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/axis_response.py
--rw-rw-rw-   0        0        0     6075 2022-12-08 06:52:13.000000 asposecellscloud-23.5.1/asposecellscloud/models/barcode_response.py
--rw-rw-rw-   0        0        0     4577 2022-05-26 05:48:42.000000 asposecellscloud-23.5.1/asposecellscloud/models/barcode_response_list.py
--rw-rw-rw-   0        0        0     9409 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/batch_convert_request.py
--rw-rw-rw-   0        0        0     5784 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/border.py
--rw-rw-rw-   0        0        0     7101 2022-01-09 23:56:52.000000 asposecellscloud-23.5.1/asposecellscloud/models/calculation_options.py
--rw-rw-rw-   0        0        0    17986 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cell.py
--rw-rw-rw-   0        0        0     6979 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cell_area.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cell_response.py
--rw-rw-rw-   0        0        0     7712 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cell_value.py
--rw-rw-rw-   0        0        0     8817 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells.py
--rw-rw-rw-   0        0        0     6537 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_cloud_file_info.py
--rw-rw-rw-   0        0        0     5207 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_cloud_response.py
--rw-rw-rw-   0        0        0     7300 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_color.py
--rw-rw-rw-   0        0        0     5567 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_document_properties.py
--rw-rw-rw-   0        0        0     5010 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_document_properties_response.py
--rw-rw-rw-   0        0        0     9807 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_document_property.py
--rw-rw-rw-   0        0        0     4944 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_document_property_response.py
--rw-rw-rw-   0        0        0     6787 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_error.py
--rw-rw-rw-   0        0        0     6872 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_object_operate_task_parameter.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/cells_response.py
--rw-rw-rw-   0        0        0    42900 2022-01-09 23:56:53.000000 asposecellscloud-23.5.1/asposecellscloud/models/chart.py
--rw-rw-rw-   0        0        0    13338 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/chart_area.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/chart_area_response.py
--rw-rw-rw-   0        0        0    13399 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/chart_frame.py
--rw-rw-rw-   0        0        0    11252 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/chart_operate_parameter.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/charts.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/charts_response.py
--rw-rw-rw-   0        0        0     6206 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/color.py
--rw-rw-rw-   0        0        0     7856 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/color_filter.py
--rw-rw-rw-   0        0        0     6284 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/color_filter_request.py
--rw-rw-rw-   0        0        0     9488 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/color_scale.py
--rw-rw-rw-   0        0        0     7595 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/column.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/column_response.py
--rw-rw-rw-   0        0        0     6821 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/columns.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:54.000000 asposecellscloud-23.5.1/asposecellscloud/models/columns_response.py
--rw-rw-rw-   0        0        0    12495 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/comment.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/comment_response.py
--rw-rw-rw-   0        0        0     5143 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/comments.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/comments_response.py
--rw-rw-rw-   0        0        0     6091 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting.py
--rw-rw-rw-   0        0        0     6615 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_icon.py
--rw-rw-rw-   0        0        0     5044 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_response.py
--rw-rw-rw-   0        0        0     7124 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_value.py
--rw-rw-rw-   0        0        0     6424 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formattings.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/conditional_formattings_response.py
--rw-rw-rw-   0        0        0     6330 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/convert_task_parameter.py
--rw-rw-rw-   0        0        0    10343 2021-01-25 09:55:40.000000 asposecellscloud-23.5.1/asposecellscloud/models/convert_worksheet_task_parameter.py
--rw-rw-rw-   0        0        0    10822 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/copy_options.py
--rw-rw-rw-   0        0        0     9904 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/create_pivot_table_request.py
--rw-rw-rw-   0        0        0     5389 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/custom_filter.py
--rw-rw-rw-   0        0        0     6181 2022-01-09 23:56:55.000000 asposecellscloud-23.5.1/asposecellscloud/models/custom_parser_config.py
--rw-rw-rw-   0        0        0    14799 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/data_bar.py
--rw-rw-rw-   0        0        0     5420 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/data_bar_border.py
--rw-rw-rw-   0        0        0     6904 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/data_sorter.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/dif_save_options.py
--rw-rw-rw-   0        0        0     5507 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:18.000000 asposecellscloud-23.5.1/asposecellscloud/models/docx_save_options.py
--rw-rw-rw-   0        0        0     6036 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/dynamic_filter.py
--rw-rw-rw-   0        0        0     5319 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/error_details.py
--rw-rw-rw-   0        0        0     5975 2021-07-06 12:22:32.000000 asposecellscloud-23.5.1/asposecellscloud/models/file_info.py
--rw-rw-rw-   0        0        0     5302 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/file_source.py
--rw-rw-rw-   0        0        0     5596 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/file_version.py
--rw-rw-rw-   0        0        0     4514 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4535 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/files_list.py
--rw-rw-rw-   0        0        0     4424 2021-07-06 12:22:32.000000 asposecellscloud-23.5.1/asposecellscloud/models/files_result.py
--rw-rw-rw-   0        0        0     5357 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     8516 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/fill_format.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/fill_format_response.py
--rw-rw-rw-   0        0        0    11145 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/filter_column.py
--rw-rw-rw-   0        0        0    10480 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/font.py
--rw-rw-rw-   0        0        0     7369 2022-01-09 23:56:56.000000 asposecellscloud-23.5.1/asposecellscloud/models/font_setting.py
--rw-rw-rw-   0        0        0    15284 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/format_condition.py
--rw-rw-rw-   0        0        0     6793 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/gradient_fill.py
--rw-rw-rw-   0        0        0     6156 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/gradient_fill_stop.py
--rw-rw-rw-   0        0        0     6286 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_break.py
--rw-rw-rw-   0        0        0     4997 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_break_response.py
--rw-rw-rw-   0        0        0     5601 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_breaks.py
--rw-rw-rw-   0        0        0     5030 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_breaks_response.py
--rw-rw-rw-   0        0        0    35831 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/html_save_options.py
--rw-rw-rw-   0        0        0     7164 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/hyperlink.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/hyperlink_response.py
--rw-rw-rw-   0        0        0     5931 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/hyperlinks.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/hyperlinks_response.py
--rw-rw-rw-   0        0        0     5303 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/icon_filter.py
--rw-rw-rw-   0        0        0     9489 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/icon_set.py
--rw-rw-rw-   0        0        0    14318 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/image_save_options.py
--rw-rw-rw-   0        0        0     4682 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_batch_data_option.py
--rw-rw-rw-   0        0        0     8921 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_csv_data_option.py
--rw-rw-rw-   0        0        0     6508 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_data_task_parameter.py
--rw-rw-rw-   0        0        0     6936 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_double_array_option.py
--rw-rw-rw-   0        0        0     6864 2022-01-09 23:56:57.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_int_array_option.py
--rw-rw-rw-   0        0        0     6953 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_option.py
--rw-rw-rw-   0        0        0     9052 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_picture_option.py
--rw-rw-rw-   0        0        0     5368 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_position.py
--rw-rw-rw-   0        0        0     6930 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_string_array_option.py
--rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/models/import_xml_request.py
--rw-rw-rw-   0        0        0     6968 2022-07-25 09:20:20.000000 asposecellscloud-23.5.1/asposecellscloud/models/json_save_options.py
--rw-rw-rw-   0        0        0    14632 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/legend.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/legend_response.py
--rw-rw-rw-   0        0        0    17404 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/line.py
--rw-rw-rw-   0        0        0    17619 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/line_format.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/line_response.py
--rw-rw-rw-   0        0        0     6045 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/link.py
--rw-rw-rw-   0        0        0     4374 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/link_element.py
--rw-rw-rw-   0        0        0     7020 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_column.py
--rw-rw-rw-   0        0        0    18926 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_object.py
--rw-rw-rw-   0        0        0     4753 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_object_operate_parameter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_object_response.py
--rw-rw-rw-   0        0        0     5261 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_objects.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/list_objects_response.py
--rw-rw-rw-   0        0        0    15529 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/m_html_save_options.py
--rw-rw-rw-   0        0        0     6279 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/markdown_save_options.py
--rw-rw-rw-   0        0        0     5643 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/match_condition_request.py
--rw-rw-rw-   0        0        0     7627 2022-01-09 23:56:58.000000 asposecellscloud-23.5.1/asposecellscloud/models/merged_cell.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/merged_cell_response.py
--rw-rw-rw-   0        0        0     5987 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/merged_cells.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/merged_cells_response.py
--rw-rw-rw-   0        0        0     3801 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/multiple_filter.py
--rw-rw-rw-   0        0        0     5541 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/multiple_filters.py
--rw-rw-rw-   0        0        0     9541 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/name.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/name_response.py
--rw-rw-rw-   0        0        0     5746 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/names.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/names_response.py
--rw-rw-rw-   0        0        0     7728 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/negative_bar_format.py
--rw-rw-rw-   0        0        0     5540 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ods_save_options.py
--rw-rw-rw-   0        0        0    35679 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ole_object.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ole_object_response.py
--rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ole_objects.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ole_objects_response.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/ooxml_save_options.py
--rw-rw-rw-   0        0        0     5436 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/operate_object.py
--rw-rw-rw-   0        0        0     8551 2022-01-09 23:56:59.000000 asposecellscloud-23.5.1/asposecellscloud/models/operate_object_position.py
--rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/operate_parameter.py
--rw-rw-rw-   0        0        0     8394 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_break_operate_parameter.py
--rw-rw-rw-   0        0        0     8214 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_section.py
--rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_sections_response.py
--rw-rw-rw-   0        0        0    36653 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_setup.py
--rw-rw-rw-   0        0        0     4720 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_setup_operate_parameter.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/page_setup_response.py
--rw-rw-rw-   0        0        0     4487 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/password_request.py
--rw-rw-rw-   0        0        0     6858 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/paste_options.py
--rw-rw-rw-   0        0        0     9851 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/pattern_fill.py
--rw-rw-rw-   0        0        0    12225 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/pdf_save_options.py
--rw-rw-rw-   0        0        0    14691 2022-01-09 23:57:00.000000 asposecellscloud-23.5.1/asposecellscloud/models/pdf_security_options.py
--rw-rw-rw-   0        0        0     7612 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pic_format_option.py
--rw-rw-rw-   0        0        0    34670 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/picture.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/picture_response.py
--rw-rw-rw-   0        0        0     5143 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pictures.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pictures_response.py
--rw-rw-rw-   0        0        0    35618 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_field.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_field_response.py
--rw-rw-rw-   0        0        0    11803 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_filter.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_filter_response.py
--rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_filters_response.py
--rw-rw-rw-   0        0        0     6544 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_item.py
--rw-rw-rw-   0        0        0    62471 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_table.py
--rw-rw-rw-   0        0        0     4488 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_field_request.py
--rw-rw-rw-   0        0        0    11025 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_operate_parameter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_response.py
--rw-rw-rw-   0        0        0     5261 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_tables.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.5.1/asposecellscloud/models/pivot_tables_response.py
--rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:24.000000 asposecellscloud-23.5.1/asposecellscloud/models/pptx_save_options.py
--rw-rw-rw-   0        0        0    19154 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/protect_sheet_parameter.py
--rw-rw-rw-   0        0        0    11570 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/range.py
--rw-rw-rw-   0        0        0     6655 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/range_copy_request.py
--rw-rw-rw-   0        0        0     7038 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/range_set_outline_border_request.py
--rw-rw-rw-   0        0        0     5147 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/range_set_style_request.py
--rw-rw-rw-   0        0        0     4661 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/range_value_response.py
--rw-rw-rw-   0        0        0     4469 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/ranges.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/ranges_response.py
--rw-rw-rw-   0        0        0     6184 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/result_destination.py
--rw-rw-rw-   0        0        0     9021 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/row.py
--rw-rw-rw-   0        0        0     4431 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/row_response.py
--rw-rw-rw-   0        0        0     6572 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/rows.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/rows_response.py
--rw-rw-rw-   0        0        0    11282 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/save_options.py
--rw-rw-rw-   0        0        0     4621 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/save_response.py
--rw-rw-rw-   0        0        0     4525 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/save_result.py
--rw-rw-rw-   0        0        0     5706 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/save_result_task_parameter.py
--rw-rw-rw-   0        0        0     8516 2022-01-09 23:57:02.000000 asposecellscloud-23.5.1/asposecellscloud/models/shadow_effect.py
--rw-rw-rw-   0        0        0    29570 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/shape.py
--rw-rw-rw-   0        0        0     4569 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/shape_operate_parameter.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/shape_response.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/shapes.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/shapes_response.py
--rw-rw-rw-   0        0        0     5135 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/single_value.py
--rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/single_value_response.py
--rw-rw-rw-   0        0        0     6559 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/smart_marker_task_parameter.py
--rw-rw-rw-   0        0        0     5903 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/solid_fill.py
--rw-rw-rw-   0        0        0     7683 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sort_key.py
--rw-rw-rw-   0        0        0     5887 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sparkline.py
--rw-rw-rw-   0        0        0    27947 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sparkline_group.py
--rw-rw-rw-   0        0        0     4813 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sparkline_group_response.py
--rw-rw-rw-   0        0        0     4776 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sparkline_groups.py
--rw-rw-rw-   0        0        0     4846 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/sparkline_groups_response.py
--rw-rw-rw-   0        0        0     4534 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/split_result.py
--rw-rw-rw-   0        0        0     5141 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/split_result_document.py
--rw-rw-rw-   0        0        0     4683 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/split_result_response.py
--rw-rw-rw-   0        0        0     9690 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/split_workbook_task_parameter.py
--rw-rw-rw-   0        0        0     6924 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/spreadsheet_ml2003_save_options.py
--rw-rw-rw-   0        0        0    14315 2022-07-25 09:20:26.000000 asposecellscloud-23.5.1/asposecellscloud/models/sql_script_save_options.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7638 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/storage_file.py
--rw-rw-rw-   0        0        0    21950 2022-01-09 23:57:03.000000 asposecellscloud-23.5.1/asposecellscloud/models/style.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/style_response.py
--rw-rw-rw-   0        0        0     4592 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/svg_save_options.py
--rw-rw-rw-   0        0        0     6423 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/table_total_request.py
--rw-rw-rw-   0        0        0     4418 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/task_data.py
--rw-rw-rw-   0        0        0     5358 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/task_description.py
--rw-rw-rw-   0        0        0     3796 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/task_parameter.py
--rw-rw-rw-   0        0        0     4942 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/text_item.py
--rw-rw-rw-   0        0        0     5186 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/text_items.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/text_items_response.py
--rw-rw-rw-   0        0        0    14978 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/text_options.py
--rw-rw-rw-   0        0        0     7524 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/text_water_marker_request.py
--rw-rw-rw-   0        0        0     8184 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/texture_fill.py
--rw-rw-rw-   0        0        0     5090 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/theme_color.py
--rw-rw-rw-   0        0        0    12409 2022-12-08 06:28:10.000000 asposecellscloud-23.5.1/asposecellscloud/models/tick_labels.py
--rw-rw-rw-   0        0        0     8508 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/tile_pic_option.py
--rw-rw-rw-   0        0        0    18670 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/title.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/title_response.py
--rw-rw-rw-   0        0        0     6735 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/top10.py
--rw-rw-rw-   0        0        0     6759 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/top10_filter.py
--rw-rw-rw-   0        0        0     6950 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/txt_save_options.py
--rw-rw-rw-   0        0        0    18950 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/validation.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/validation_response.py
--rw-rw-rw-   0        0        0     5968 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/validations.py
--rw-rw-rw-   0        0        0     4695 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/validations_response.py
--rw-rw-rw-   0        0        0     3776 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/value_type.py
--rw-rw-rw-   0        0        0     6189 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_break.py
--rw-rw-rw-   0        0        0     4931 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_break_response.py
--rw-rw-rw-   0        0        0     5529 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_breaks.py
--rw-rw-rw-   0        0        0     4964 2022-01-09 23:57:04.000000 asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_breaks_response.py
--rw-rw-rw-   0        0        0    11948 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook.py
--rw-rw-rw-   0        0        0     6539 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_encryption_request.py
--rw-rw-rw-   0        0        0     3936 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_operate_parameter.py
--rw-rw-rw-   0        0        0     5709 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_protection_request.py
--rw-rw-rw-   0        0        0     5491 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_replace_response.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_response.py
--rw-rw-rw-   0        0        0    52420 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings.py
--rw-rw-rw-   0        0        0     4951 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings_operate_parameter.py
--rw-rw-rw-   0        0        0     4700 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings_response.py
--rw-rw-rw-   0        0        0    32067 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheet.py
--rw-rw-rw-   0        0        0     5720 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheet_moving_request.py
--rw-rw-rw-   0        0        0     7026 2021-05-13 06:59:25.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheet_operate_parameter.py
--rw-rw-rw-   0        0        0     5525 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheet_replace_response.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheet_response.py
--rw-rw-rw-   0        0        0     5209 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheets.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/worksheets_response.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/xls_save_options.py
--rw-rw-rw-   0        0        0     3862 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/xlsb_save_options.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.5.1/asposecellscloud/models/xps_save_options.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:44.149883 asposecellscloud-23.5.1/asposecellscloud/requests/
--rw-rw-rw-   0        0        0    33472 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/__init__.py
--rw-rw-rw-   0        0        0     4290 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/copy_file_request.py
--rw-rw-rw-   0        0        0     4137 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/copy_folder_request.py
--rw-rw-rw-   0        0        0     3513 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/create_folder_request.py
--rw-rw-rw-   0        0        0     4058 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_decrypt_workbook_request.py
--rw-rw-rw-   0        0        0     3715 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_properties_request.py
--rw-rw-rw-   0        0        0     4246 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_property_request.py
--rw-rw-rw-   0        0        0     3745 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py
--rw-rw-rw-   0        0        0     3671 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_file_request.py
--rw-rw-rw-   0        0        0     3674 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_folder_request.py
--rw-rw-rw-   0        0        0     4092 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_header_footer_request.py
--rw-rw-rw-   0        0        0     4450 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4241 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_horizontal_page_breaks_request.py
--rw-rw-rw-   0        0        0     4087 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_metadata_request.py
--rw-rw-rw-   0        0        0     5464 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_un_protect_workbook_request.py
--rw-rw-rw-   0        0        0     4518 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_unprotect_worksheet_request.py
--rw-rw-rw-   0        0        0     4438 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4249 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_vertical_page_breaks_request.py
--rw-rw-rw-   0        0        0     3707 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_background_request.py
--rw-rw-rw-   0        0        0     4049 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_name_request.py
--rw-rw-rw-   0        0        0     3687 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_names_request.py
--rw-rw-rw-   0        0        0     4103 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_background_request.py
--rw-rw-rw-   0        0        0     4785 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_cells_range_request.py
--rw-rw-rw-   0        0        0     4506 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4105 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_clear_charts_request.py
--rw-rw-rw-   0        0        0     5285 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4093 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_comments_request.py
--rw-rw-rw-   0        0        0     5828 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py
--rw-rw-rw-   0        0        0     4507 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     4165 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py
--rw-rw-rw-   0        0        0     5804 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_date_filter_request.py
--rw-rw-rw-   0        0        0     4499 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_delete_chart_request.py
--rw-rw-rw-   0        0        0     4636 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_filter_request.py
--rw-rw-rw-   0        0        0     5624 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py
--rw-rw-rw-   0        0        0     4530 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     4103 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py
--rw-rw-rw-   0        0        0     4557 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4110 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_list_objects_request.py
--rw-rw-rw-   0        0        0     4541 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4105 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_ole_objects_request.py
--rw-rw-rw-   0        0        0     4498 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_picture_request.py
--rw-rw-rw-   0        0        0     4093 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pictures_request.py
--rw-rw-rw-   0        0        0     5207 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4812 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py
--rw-rw-rw-   0        0        0     4557 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     4110 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py
--rw-rw-rw-   0        0        0     4050 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_request.py
--rw-rw-rw-   0        0        0     4440 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4804 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     4083 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_shapes_request.py
--rw-rw-rw-   0        0        0     4563 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4130 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py
--rw-rw-rw-   0        0        0     4546 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4108 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_validations_request.py
--rw-rw-rw-   0        0        0     3849 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheets_request.py
--rw-rw-rw-   0        0        0     3678 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/download_file_request.py
--rw-rw-rw-   0        0        0     4426 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_cell_html_string_request.py
--rw-rw-rw-   0        0        0     3073 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_cells_cloud_service_status_request.py
--rw-rw-rw-   0        0        0     3072 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py
--rw-rw-rw-   0        0        0     4467 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_border_request.py
--rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_fill_format_request.py
--rw-rw-rw-   0        0        0     4432 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_request.py
--rw-rw-rw-   0        0        0     4473 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_category_axis_request.py
--rw-rw-rw-   0        0        0     4512 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_second_category_axis_request.py
--rw-rw-rw-   0        0        0     4494 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_second_value_axis_request.py
--rw-rw-rw-   0        0        0     4461 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_series_axis_request.py
--rw-rw-rw-   0        0        0     4455 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_value_axis_request.py
--rw-rw-rw-   0        0        0     3212 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_disc_usage_request.py
--rw-rw-rw-   0        0        0     3844 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_document_properties_request.py
--rw-rw-rw-   0        0        0     4114 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_document_property_request.py
--rw-rw-rw-   0        0        0     4486 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_extract_barcodes_request.py
--rw-rw-rw-   0        0        0     3536 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_file_versions_request.py
--rw-rw-rw-   0        0        0     3340 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_files_list_request.py
--rw-rw-rw-   0        0        0     4042 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_footer_request.py
--rw-rw-rw-   0        0        0     4042 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_header_request.py
--rw-rw-rw-   0        0        0     4441 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4114 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_horizontal_page_breaks_request.py
--rw-rw-rw-   0        0        0     4091 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_metadata_request.py
--rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_named_range_value_request.py
--rw-rw-rw-   0        0        0     3677 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_named_ranges_request.py
--rw-rw-rw-   0        0        0     3652 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_page_count_request.py
--rw-rw-rw-   0        0        0     4046 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_page_setup_request.py
--rw-rw-rw-   0        0        0     5403 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4427 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4102 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_vertical_page_breaks_request.py
--rw-rw-rw-   0        0        0     3699 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_default_style_request.py
--rw-rw-rw-   0        0        0     4028 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_name_request.py
--rw-rw-rw-   0        0        0     4062 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_name_value_request.py
--rw-rw-rw-   0        0        0     3670 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_names_request.py
--rw-rw-rw-   0        0        0     4880 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_request.py
--rw-rw-rw-   0        0        0     3693 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_settings_request.py
--rw-rw-rw-   0        0        0     3691 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_text_items_request.py
--rw-rw-rw-   0        0        0     4090 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_auto_filter_request.py
--rw-rw-rw-   0        0        0     4704 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py
--rw-rw-rw-   0        0        0     4088 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_autoshapes_request.py
--rw-rw-rw-   0        0        0     4481 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4503 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cell_request.py
--rw-rw-rw-   0        0        0     4451 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cell_style_request.py
--rw-rw-rw-   0        0        0     4936 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cells_range_value_request.py
--rw-rw-rw-   0        0        0     4332 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cells_request.py
--rw-rw-rw-   0        0        0     4484 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4584 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4477 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4064 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_charts_request.py
--rw-rw-rw-   0        0        0     4466 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_column_request.py
--rw-rw-rw-   0        0        0     3951 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4437 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4076 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_comments_request.py
--rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     4162 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py
--rw-rw-rw-   0        0        0     4511 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     4088 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_hyperlinks_request.py
--rw-rw-rw-   0        0        0     4649 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_list_objects_request.py
--rw-rw-rw-   0        0        0     4539 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_merged_cell_request.py
--rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_merged_cells_request.py
--rw-rw-rw-   0        0        0     4621 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4090 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_ole_objects_request.py
--rw-rw-rw-   0        0        0     4070 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_page_count_request.py
--rw-rw-rw-   0        0        0     4888 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_picture_with_format_request.py
--rw-rw-rw-   0        0        0     4076 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pictures_request.py
--rw-rw-rw-   0        0        0     4993 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4592 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py
--rw-rw-rw-   0        0        0     4531 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_tables_request.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4333 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     4435 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     4064 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_shapes_request.py
--rw-rw-rw-   0        0        0     4549 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4120 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py
--rw-rw-rw-   0        0        0     4084 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_text_items_request.py
--rw-rw-rw-   0        0        0     4528 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4094 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_validations_request.py
--rw-rw-rw-   0        0        0     4942 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_with_format_request.py
--rw-rw-rw-   0        0        0     3670 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheets_request.py
--rw-rw-rw-   0        0        0     4290 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/move_file_request.py
--rw-rw-rw-   0        0        0     4137 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/move_folder_request.py
--rw-rw-rw-   0        0        0     3686 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/object_exists_request.py
--rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_assemble_request.py
--rw-rw-rw-   0        0        0     4054 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_workbook_columns_request.py
--rw-rw-rw-   0        0        0     4163 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_workbook_rows_request.py
--rw-rw-rw-   0        0        0     4610 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5265 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4559 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3481 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_batch_convert_request.py
--rw-rw-rw-   0        0        0     4565 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_cell_calculate_request.py
--rw-rw-rw-   0        0        0     4571 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_cell_characters_request.py
--rw-rw-rw-   0        0        0     4798 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_category_axis_request.py
--rw-rw-rw-   0        0        0     4844 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_second_category_axis_request.py
--rw-rw-rw-   0        0        0     4823 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_second_value_axis_request.py
--rw-rw-rw-   0        0        0     4784 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_series_axis_request.py
--rw-rw-rw-   0        0        0     4777 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_value_axis_request.py
--rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_contents_request.py
--rw-rw-rw-   0        0        0     4847 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_formats_request.py
--rw-rw-rw-   0        0        0     4661 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_objects_request.py
--rw-rw-rw-   0        0        0     4776 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_column_style_request.py
--rw-rw-rw-   0        0        0     4133 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_compress_request.py
--rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_csv_request.py
--rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_docx_request.py
--rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_html_request.py
--rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_json_request.py
--rw-rw-rw-   0        0        0     4005 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py
--rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py
--rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_png_request.py
--rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py
--rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_sql_request.py
--rw-rw-rw-   0        0        0     5290 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_cell_into_cell_request.py
--rw-rw-rw-   0        0        0     5652 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5164 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_request.py
--rw-rw-rw-   0        0        0     5547 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     4533 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_digital_signature_request.py
--rw-rw-rw-   0        0        0     4048 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_encrypt_workbook_request.py
--rw-rw-rw-   0        0        0     4247 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_export_request.py
--rw-rw-rw-   0        0        0     5117 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_footer_request.py
--rw-rw-rw-   0        0        0     5021 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_group_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5000 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_group_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5117 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_header_request.py
--rw-rw-rw-   0        0        0     4922 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_hide_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4839 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_hide_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3832 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_import_data_request.py
--rw-rw-rw-   0        0        0     3544 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_import_request.py
--rw-rw-rw-   0        0        0     4280 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_merge_request.py
--rw-rw-rw-   0        0        0     4246 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_metadata_request.py
--rw-rw-rw-   0        0        0     4391 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_move_worksheet_request.py
--rw-rw-rw-   0        0        0     4404 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_page_setup_request.py
--rw-rw-rw-   0        0        0     5756 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_cell_style_request.py
--rw-rw-rw-   0        0        0     6386 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py
--rw-rw-rw-   0        0        0     5634 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_field_move_to_request.py
--rw-rw-rw-   0        0        0     5058 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_style_request.py
--rw-rw-rw-   0        0        0     6086 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py
--rw-rw-rw-   0        0        0     5635 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py
--rw-rw-rw-   0        0        0     3903 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_protect_request.py
--rw-rw-rw-   0        0        0     4048 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_protect_workbook_request.py
--rw-rw-rw-   0        0        0     4426 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_rename_worksheet_request.py
--rw-rw-rw-   0        0        0     4761 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_replace_request.py
--rw-rw-rw-   0        0        0     4461 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_reverse_request.py
--rw-rw-rw-   0        0        0     4456 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_rotate_request.py
--rw-rw-rw-   0        0        0     4725 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_row_style_request.py
--rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_run_task_request.py
--rw-rw-rw-   0        0        0     4415 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_search_request.py
--rw-rw-rw-   0        0        0     4465 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_set_cell_html_string_request.py
--rw-rw-rw-   0        0        0     5119 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_set_cell_range_value_request.py
--rw-rw-rw-   0        0        0     5001 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_set_worksheet_column_width_request.py
--rw-rw-rw-   0        0        0     4516 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_split_request.py
--rw-rw-rw-   0        0        0     4907 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5025 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5070 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_unhide_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4993 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_unhide_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3898 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_unlock_request.py
--rw-rw-rw-   0        0        0     4824 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_cell_style_request.py
--rw-rw-rw-   0        0        0     4875 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4427 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_property_request.py
--rw-rw-rw-   0        0        0     4799 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_range_style_request.py
--rw-rw-rw-   0        0        0     4735 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4429 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_zoom_request.py
--rw-rw-rw-   0        0        0     4597 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_watermark_request.py
--rw-rw-rw-   0        0        0     4026 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4423 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_export_xml_request.py
--rw-rw-rw-   0        0        0     4219 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py
--rw-rw-rw-   0        0        0     4848 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_import_xml_request.py
--rw-rw-rw-   0        0        0     4378 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_name_request.py
--rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_save_as_request.py
--rw-rw-rw-   0        0        0     4034 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_settings_request.py
--rw-rw-rw-   0        0        0     5068 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_split_request.py
--rw-rw-rw-   0        0        0     4459 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_text_replace_request.py
--rw-rw-rw-   0        0        0     4274 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbooks_merge_request.py
--rw-rw-rw-   0        0        0     4031 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_workbooks_text_search_request.py
--rw-rw-rw-   0        0        0     4133 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py
--rw-rw-rw-   0        0        0     4490 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4876 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cell_set_value_request.py
--rw-rw-rw-   0        0        0     4840 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py
--rw-rw-rw-   0        0        0     4448 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py
--rw-rw-rw-   0        0        0     5232 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py
--rw-rw-rw-   0        0        0     4563 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py
--rw-rw-rw-   0        0        0     4826 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py
--rw-rw-rw-   0        0        0     4512 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_style_request.py
--rw-rw-rw-   0        0        0     4463 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py
--rw-rw-rw-   0        0        0     5126 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_value_request.py
--rw-rw-rw-   0        0        0     4483 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_ranges_request.py
--rw-rw-rw-   0        0        0     4826 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4771 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4811 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4781 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4460 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_group_shape_request.py
--rw-rw-rw-   0        0        0     4871 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     5329 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_column_request.py
--rw-rw-rw-   0        0        0     5046 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_columns_total_request.py
--rw-rw-rw-   0        0        0     4639 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py
--rw-rw-rw-   0        0        0     4916 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4983 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py
--rw-rw-rw-   0        0        0     5661 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py
--rw-rw-rw-   0        0        0     4505 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_match_blanks_request.py
--rw-rw-rw-   0        0        0     4526 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py
--rw-rw-rw-   0        0        0     5622 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_merge_request.py
--rw-rw-rw-   0        0        0     4821 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_picture_request.py
--rw-rw-rw-   0        0        0     4603 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py
--rw-rw-rw-   0        0        0     5021 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py
--rw-rw-rw-   0        0        0     4829 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_range_sort_request.py
--rw-rw-rw-   0        0        0     4747 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     5016 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4423 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_text_search_request.py
--rw-rw-rw-   0        0        0     4492 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py
--rw-rw-rw-   0        0        0     5640 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_unmerge_request.py
--rw-rw-rw-   0        0        0     4896 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/post_worsheet_text_replace_request.py
--rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_active_worksheet_request.py
--rw-rw-rw-   0        0        0     4373 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_add_new_worksheet_request.py
--rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_change_visibility_worksheet_request.py
--rw-rw-rw-   0        0        0     4603 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_convert_workbook_request.py
--rw-rw-rw-   0        0        0     4062 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_document_property_request.py
--rw-rw-rw-   0        0        0     4080 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_document_protect_from_changes_request.py
--rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4973 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_new_worksheet_request.py
--rw-rw-rw-   0        0        0     5067 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4455 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4819 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5644 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4490 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_protect_worksheet_request.py
--rw-rw-rw-   0        0        0     4806 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4182 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_background_request.py
--rw-rw-rw-   0        0        0     4430 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_create_request.py
--rw-rw-rw-   0        0        0     4010 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_name_request.py
--rw-rw-rw-   0        0        0     4182 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_water_marker_request.py
--rw-rw-rw-   0        0        0     6894 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_add_chart_request.py
--rw-rw-rw-   0        0        0     5182 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_add_picture_request.py
--rw-rw-rw-   0        0        0     4575 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_background_request.py
--rw-rw-rw-   0        0        0     4764 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_cells_range_request.py
--rw-rw-rw-   0        0        0     4488 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4599 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     5539 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_color_filter_request.py
--rw-rw-rw-   0        0        0     4771 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4944 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     6443 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_custom_filter_request.py
--rw-rw-rw-   0        0        0     6443 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_date_filter_request.py
--rw-rw-rw-   0        0        0     5640 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py
--rw-rw-rw-   0        0        0     5482 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_filter_request.py
--rw-rw-rw-   0        0        0     6276 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_filter_top10_request.py
--rw-rw-rw-   0        0        0     4871 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_area_request.py
--rw-rw-rw-   0        0        0     6049 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py
--rw-rw-rw-   0        0        0     6330 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_request.py
--rw-rw-rw-   0        0        0     5597 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_freeze_panes_request.py
--rw-rw-rw-   0        0        0     5999 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     5918 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_icon_filter_request.py
--rw-rw-rw-   0        0        0     5244 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     5064 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     5126 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4801 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     5290 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     5651 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4223 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     3428 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/storage_exists_request.py
--rw-rw-rw-   0        0        0     4127 2023-04-21 23:29:09.000000 asposecellscloud-23.5.1/asposecellscloud/requests/upload_file_request.py
--rw-rw-rw-   0        0        0    14129 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/asposecellscloud/rest.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:37.751390 asposecellscloud-23.5.1/asposecellscloud.egg-info/
--rw-rw-rw-   0        0        0      900 2023-05-25 13:08:37.000000 asposecellscloud-23.5.1/asposecellscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    33054 2023-05-25 13:08:37.000000 asposecellscloud-23.5.1/asposecellscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:08:37.000000 asposecellscloud-23.5.1/asposecellscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-25 13:08:37.000000 asposecellscloud-23.5.1/asposecellscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-25 13:08:37.000000 asposecellscloud-23.5.1/asposecellscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:08:44.384696 asposecellscloud-23.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-05-25 13:06:11.000000 asposecellscloud-23.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:08:44.377694 asposecellscloud-23.5.1/test/
--rw-rw-rw-   0        0        0     7256 2022-12-08 07:15:43.000000 asposecellscloud-23.5.1/test/test_cells_chart_axis_api.py
--rw-rw-rw-   0        0        0     7996 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_auto_filter_controller.py
--rw-rw-rw-   0        0        0     1816 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_batch_controller.py
--rw-rw-rw-   0        0        0     1338 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_cells_barcodes_controller.py
--rw-rw-rw-   0        0        0    21475 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_cells_controller.py
--rw-rw-rw-   0        0        0     1774 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_cells_status_controller.py
--rw-rw-rw-   0        0        0     2297 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_chart_area_controller.py
--rw-rw-rw-   0        0        0     8079 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_charts_controller.py
--rw-rw-rw-   0        0        0     5842 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_conditional_formattings_controller.py
--rw-rw-rw-   0        0        0    70981 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_conversion.py
--rw-rw-rw-   0        0        0    18233 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_conversion_json.py
--rw-rw-rw-   0        0        0    17784 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_conversion_png.py
--rw-rw-rw-   0        0        0     3361 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_file_controller.py
--rw-rw-rw-   0        0        0     3093 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_folder_controller.py
--rw-rw-rw-   0        0        0     3932 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/test/tests_hypelinks_controller.py
--rw-rw-rw-   0        0        0   120147 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_light_cells.py
--rw-rw-rw-   0        0        0     7608 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_list_objects_controller.py
--rw-rw-rw-   0        0        0     4326 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_ole_objects_controller.py
--rw-rw-rw-   0        0        0     1333 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_one.py
--rw-rw-rw-   0        0        0     5884 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_page_breaks_controller.py
--rw-rw-rw-   0        0        0     4203 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_page_setup_controller.py
--rw-rw-rw-   0        0        0     4182 2023-05-25 12:57:31.000000 asposecellscloud-23.5.1/test/tests_pictures_controller.py
--rw-rw-rw-   0        0        0    12668 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_pivot_tables_controller.py
--rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_properties_controller.py
--rw-rw-rw-   0        0        0     8719 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_ranges_controller.py
--rw-rw-rw-   0        0        0     4970 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_shapes_controller.py
--rw-rw-rw-   0        0        0     4073 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_sparkline_groups_controller.py
--rw-rw-rw-   0        0        0     2573 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_storage_controller.py
--rw-rw-rw-   0        0        0    18939 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_workbook_controller.py
--rw-rw-rw-   0        0        0    21080 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_worksheet_controller.py
--rw-rw-rw-   0        0        0     3912 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_worksheet_validations_controller.py
--rw-rw-rw-   0        0        0     2422 2023-04-21 23:29:10.000000 asposecellscloud-23.5.1/test/tests_xml_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:06:04.268124 asposecellscloud-23.6/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 23:29:09.000000 asposecellscloud-23.6/LICENSE
+-rw-rw-rw-   0        0        0      898 2023-06-30 00:06:04.214111 asposecellscloud-23.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6973 2023-06-30 00:03:35.000000 asposecellscloud-23.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 00:05:39.732839 asposecellscloud-23.6/asposecellscloud/
+-rw-rw-rw-   0        0        0    43330 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/__init__.py
+-rw-rw-rw-   0        0        0    30489 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/api_client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:05:39.846236 asposecellscloud-23.6/asposecellscloud/apis/
+-rw-rw-rw-   0        0        0      128 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/apis/__init__.py
+-rw-rw-rw-   0        0        0  2601069 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/apis/cells_api.py
+-rw-rw-rw-   0        0        0    98544 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/apis/light_cells_api.py
+-rw-rw-rw-   0        0        0    86342 2022-01-24 09:49:53.000000 asposecellscloud-23.6/asposecellscloud/apis/lite_cells_api.py
+-rw-rw-rw-   0        0        0     8706 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:05:51.516913 asposecellscloud-23.6/asposecellscloud/models/
+-rw-rw-rw-   0        0        0    13788 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/__init__.py
+-rw-rw-rw-   0        0        0     7878 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/above_average.py
+-rw-rw-rw-   0        0        0    10430 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/access_token_response.py
+-rw-rw-rw-   0        0        0     8340 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/area.py
+-rw-rw-rw-   0        0        0     6499 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_filter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_filter_response.py
+-rw-rw-rw-   0        0        0     6636 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_fitter_options.py
+-rw-rw-rw-   0        0        0    30150 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_shape.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_shape_response.py
+-rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_shapes.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/auto_shapes_response.py
+-rw-rw-rw-   0        0        0    30674 2022-12-08 06:28:04.000000 asposecellscloud-23.6/asposecellscloud/models/axis.py
+-rw-rw-rw-   0        0        0     4464 2022-12-08 06:28:04.000000 asposecellscloud-23.6/asposecellscloud/models/axis_response.py
+-rw-rw-rw-   0        0        0     6075 2022-12-08 06:52:13.000000 asposecellscloud-23.6/asposecellscloud/models/barcode_response.py
+-rw-rw-rw-   0        0        0     4577 2022-05-26 05:48:42.000000 asposecellscloud-23.6/asposecellscloud/models/barcode_response_list.py
+-rw-rw-rw-   0        0        0     9409 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/batch_convert_request.py
+-rw-rw-rw-   0        0        0     7012 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/batch_lock_request.py
+-rw-rw-rw-   0        0        0     7596 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/batch_protect_request.py
+-rw-rw-rw-   0        0        0     8435 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/batch_split_request.py
+-rw-rw-rw-   0        0        0     5784 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/border.py
+-rw-rw-rw-   0        0        0     5119 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/border_response.py
+-rw-rw-rw-   0        0        0    22601 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/button.py
+-rw-rw-rw-   0        0        0     5102 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/button_response.py
+-rw-rw-rw-   0        0        0     5176 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/calculate_formula_response.py
+-rw-rw-rw-   0        0        0     7101 2022-01-09 23:56:52.000000 asposecellscloud-23.6/asposecellscloud/models/calculation_options.py
+-rw-rw-rw-   0        0        0    17986 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cell.py
+-rw-rw-rw-   0        0        0     6979 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cell_area.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cell_response.py
+-rw-rw-rw-   0        0        0     7712 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cell_value.py
+-rw-rw-rw-   0        0        0     8817 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells.py
+-rw-rw-rw-   0        0        0     6537 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_cloud_file_info.py
+-rw-rw-rw-   0        0        0     5253 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/cells_cloud_file_info_response.py
+-rw-rw-rw-   0        0        0     5207 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_cloud_response.py
+-rw-rw-rw-   0        0        0     7300 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_color.py
+-rw-rw-rw-   0        0        0     5567 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_document_properties.py
+-rw-rw-rw-   0        0        0     5010 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_document_properties_response.py
+-rw-rw-rw-   0        0        0     9807 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_document_property.py
+-rw-rw-rw-   0        0        0     4944 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_document_property_response.py
+-rw-rw-rw-   0        0        0    22637 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/cells_drawing.py
+-rw-rw-rw-   0        0        0     5144 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/cells_drawing_response.py
+-rw-rw-rw-   0        0        0     6787 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_error.py
+-rw-rw-rw-   0        0        0     6872 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_object_operate_task_parameter.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/cells_response.py
+-rw-rw-rw-   0        0        0    42900 2022-01-09 23:56:53.000000 asposecellscloud-23.6/asposecellscloud/models/chart.py
+-rw-rw-rw-   0        0        0    13338 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/chart_area.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/chart_area_response.py
+-rw-rw-rw-   0        0        0     8702 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_data_table.py
+-rw-rw-rw-   0        0        0     5343 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_data_table_response.py
+-rw-rw-rw-   0        0        0    13399 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/chart_frame.py
+-rw-rw-rw-   0        0        0    11252 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/chart_operate_parameter.py
+-rw-rw-rw-   0        0        0     7723 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_point.py
+-rw-rw-rw-   0        0        0     5231 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_point_response.py
+-rw-rw-rw-   0        0        0     4867 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_points.py
+-rw-rw-rw-   0        0        0     5255 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_points_response.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_response.py
+-rw-rw-rw-   0        0        0    22625 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/chart_shape.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/charts.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/charts_response.py
+-rw-rw-rw-   0        0        0    23958 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/check_box.py
+-rw-rw-rw-   0        0        0     5116 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/check_box_response.py
+-rw-rw-rw-   0        0        0     6206 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/color.py
+-rw-rw-rw-   0        0        0     7856 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/color_filter.py
+-rw-rw-rw-   0        0        0     6284 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/color_filter_request.py
+-rw-rw-rw-   0        0        0     9488 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/color_scale.py
+-rw-rw-rw-   0        0        0     7595 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/column.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/column_response.py
+-rw-rw-rw-   0        0        0     6821 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/columns.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:54.000000 asposecellscloud-23.6/asposecellscloud/models/columns_response.py
+-rw-rw-rw-   0        0        0    25729 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/combo_box.py
+-rw-rw-rw-   0        0        0     5116 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/combo_box_response.py
+-rw-rw-rw-   0        0        0    12495 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/comment.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/comment_response.py
+-rw-rw-rw-   0        0        0    23076 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/comment_shape.py
+-rw-rw-rw-   0        0        0     5178 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/comment_shape_response.py
+-rw-rw-rw-   0        0        0     5143 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/comments.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/comments_response.py
+-rw-rw-rw-   0        0        0     6091 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formatting.py
+-rw-rw-rw-   0        0        0     6615 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_icon.py
+-rw-rw-rw-   0        0        0     5044 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_response.py
+-rw-rw-rw-   0        0        0     7124 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_value.py
+-rw-rw-rw-   0        0        0     6424 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formattings.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/conditional_formattings_response.py
+-rw-rw-rw-   0        0        0     4697 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/convert_parameter.py
+-rw-rw-rw-   0        0        0     6330 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/convert_task_parameter.py
+-rw-rw-rw-   0        0        0    10343 2021-01-25 09:55:40.000000 asposecellscloud-23.6/asposecellscloud/models/convert_worksheet_task_parameter.py
+-rw-rw-rw-   0        0        0    10822 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/copy_options.py
+-rw-rw-rw-   0        0        0     9904 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/create_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4404 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/criteria_multiple_filter.py
+-rw-rw-rw-   0        0        0     5389 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/custom_filter.py
+-rw-rw-rw-   0        0        0     6181 2022-01-09 23:56:55.000000 asposecellscloud-23.6/asposecellscloud/models/custom_parser_config.py
+-rw-rw-rw-   0        0        0    14799 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/data_bar.py
+-rw-rw-rw-   0        0        0     5420 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/data_bar_border.py
+-rw-rw-rw-   0        0        0    20157 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/data_labels.py
+-rw-rw-rw-   0        0        0     5231 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/data_labels_response.py
+-rw-rw-rw-   0        0        0     6904 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/data_sorter.py
+-rw-rw-rw-   0        0        0     6974 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/date_time_group_item.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/dif_save_options.py
+-rw-rw-rw-   0        0        0     5507 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0    13288 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/display_unit_label.py
+-rw-rw-rw-   0        0        0     5391 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/display_unit_label_response.py
+-rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:18.000000 asposecellscloud-23.6/asposecellscloud/models/docx_save_options.py
+-rw-rw-rw-   0        0        0     5049 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/drop_bars.py
+-rw-rw-rw-   0        0        0     5183 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/drop_bars_response.py
+-rw-rw-rw-   0        0        0     6036 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/dynamic_filter.py
+-rw-rw-rw-   0        0        0     3856 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/error.py
+-rw-rw-rw-   0        0        0    16604 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/error_bar.py
+-rw-rw-rw-   0        0        0     5183 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/error_bar_response.py
+-rw-rw-rw-   0        0        0     5319 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/error_details.py
+-rw-rw-rw-   0        0        0     5975 2021-07-06 12:22:32.000000 asposecellscloud-23.6/asposecellscloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5302 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/file_source.py
+-rw-rw-rw-   0        0        0     5596 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4514 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4535 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4424 2021-07-06 12:22:32.000000 asposecellscloud-23.6/asposecellscloud/models/files_result.py
+-rw-rw-rw-   0        0        0     5357 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     8516 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/fill_format.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/fill_format_response.py
+-rw-rw-rw-   0        0        0    11145 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/filter_column.py
+-rw-rw-rw-   0        0        0     5574 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/find_response.py
+-rw-rw-rw-   0        0        0     7493 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/floor.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/floor_response.py
+-rw-rw-rw-   0        0        0    10480 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/font.py
+-rw-rw-rw-   0        0        0     7369 2022-01-09 23:56:56.000000 asposecellscloud-23.6/asposecellscloud/models/font_setting.py
+-rw-rw-rw-   0        0        0    31682 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/form.py
+-rw-rw-rw-   0        0        0     5071 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/form_response.py
+-rw-rw-rw-   0        0        0    15284 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/format_condition.py
+-rw-rw-rw-   0        0        0     4713 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/forms.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/forms_response.py
+-rw-rw-rw-   0        0        0     5300 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/formula_format_condition.py
+-rw-rw-rw-   0        0        0     6562 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/google_drive_storage_file.py
+-rw-rw-rw-   0        0        0     6793 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/gradient_fill.py
+-rw-rw-rw-   0        0        0     6156 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/gradient_fill_stop.py
+-rw-rw-rw-   0        0        0    23028 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/group_box.py
+-rw-rw-rw-   0        0        0     5116 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/group_box_response.py
+-rw-rw-rw-   0        0        0    22625 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/group_shape.py
+-rw-rw-rw-   0        0        0     6286 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/horizontal_page_break.py
+-rw-rw-rw-   0        0        0     4997 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/horizontal_page_break_response.py
+-rw-rw-rw-   0        0        0     5601 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/horizontal_page_breaks.py
+-rw-rw-rw-   0        0        0     5030 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/horizontal_page_breaks_response.py
+-rw-rw-rw-   0        0        0    35831 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/html_save_options.py
+-rw-rw-rw-   0        0        0     7164 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/hyperlink.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/hyperlink_response.py
+-rw-rw-rw-   0        0        0     5931 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/hyperlinks.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/hyperlinks_response.py
+-rw-rw-rw-   0        0        0     5303 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/icon_filter.py
+-rw-rw-rw-   0        0        0     9489 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/icon_set.py
+-rw-rw-rw-   0        0        0    14318 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/image_save_options.py
+-rw-rw-rw-   0        0        0     7525 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/import2_dimension_double_array_option.py
+-rw-rw-rw-   0        0        0     7505 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/import2_dimension_int_array_option.py
+-rw-rw-rw-   0        0        0     7523 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/import2_dimension_string_array_option.py
+-rw-rw-rw-   0        0        0     4682 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/import_batch_data_option.py
+-rw-rw-rw-   0        0        0     8921 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/import_csv_data_option.py
+-rw-rw-rw-   0        0        0     6508 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/import_data_task_parameter.py
+-rw-rw-rw-   0        0        0     6936 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/import_double_array_option.py
+-rw-rw-rw-   0        0        0     6864 2022-01-09 23:56:57.000000 asposecellscloud-23.6/asposecellscloud/models/import_int_array_option.py
+-rw-rw-rw-   0        0        0     6953 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/import_option.py
+-rw-rw-rw-   0        0        0     9052 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/import_picture_option.py
+-rw-rw-rw-   0        0        0     5368 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/models/import_position.py
+-rw-rw-rw-   0        0        0     6930 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/import_string_array_option.py
+-rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/models/import_xml_request.py
+-rw-rw-rw-   0        0        0     6968 2022-07-25 09:20:20.000000 asposecellscloud-23.6/asposecellscloud/models/json_save_options.py
+-rw-rw-rw-   0        0        0    22595 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/label.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/label_response.py
+-rw-rw-rw-   0        0        0    14632 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/legend.py
+-rw-rw-rw-   0        0        0     4896 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/legend_entries.py
+-rw-rw-rw-   0        0        0     5303 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/legend_entries_response.py
+-rw-rw-rw-   0        0        0     6264 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/legend_entry.py
+-rw-rw-rw-   0        0        0     5255 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/legend_entry_response.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/legend_response.py
+-rw-rw-rw-   0        0        0    17404 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/line.py
+-rw-rw-rw-   0        0        0    17619 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/line_format.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/line_response.py
+-rw-rw-rw-   0        0        0    26553 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/line_shape.py
+-rw-rw-rw-   0        0        0     5123 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/line_shape_response.py
+-rw-rw-rw-   0        0        0     6045 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/link.py
+-rw-rw-rw-   0        0        0     4374 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/link_element.py
+-rw-rw-rw-   0        0        0    26160 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/list_box.py
+-rw-rw-rw-   0        0        0     5109 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/list_box_response.py
+-rw-rw-rw-   0        0        0     7020 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_column.py
+-rw-rw-rw-   0        0        0    18926 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_object.py
+-rw-rw-rw-   0        0        0     4753 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_object_operate_parameter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_object_response.py
+-rw-rw-rw-   0        0        0     5261 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_objects.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/list_objects_response.py
+-rw-rw-rw-   0        0        0    10283 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/load_options.py
+-rw-rw-rw-   0        0        0    15529 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/m_html_save_options.py
+-rw-rw-rw-   0        0        0     6279 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/markdown_save_options.py
+-rw-rw-rw-   0        0        0     5669 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/marker.py
+-rw-rw-rw-   0        0        0     5643 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/match_condition_request.py
+-rw-rw-rw-   0        0        0     7627 2022-01-09 23:56:58.000000 asposecellscloud-23.6/asposecellscloud/models/merged_cell.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/merged_cell_response.py
+-rw-rw-rw-   0        0        0     5987 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/merged_cells.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/merged_cells_response.py
+-rw-rw-rw-   0        0        0     3801 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/multiple_filter.py
+-rw-rw-rw-   0        0        0     5541 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/multiple_filters.py
+-rw-rw-rw-   0        0        0     9541 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/name.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/name_response.py
+-rw-rw-rw-   0        0        0     5746 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/names.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/names_response.py
+-rw-rw-rw-   0        0        0     7728 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/negative_bar_format.py
+-rw-rw-rw-   0        0        0     5540 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3958 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/object_exists_extensions.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ods_save_options.py
+-rw-rw-rw-   0        0        0    35679 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ole_object.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ole_object_response.py
+-rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ole_objects.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ole_objects_response.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/ooxml_save_options.py
+-rw-rw-rw-   0        0        0     5436 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/operate_object.py
+-rw-rw-rw-   0        0        0     8551 2022-01-09 23:56:59.000000 asposecellscloud-23.6/asposecellscloud/models/operate_object_position.py
+-rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/operate_parameter.py
+-rw-rw-rw-   0        0        0    22589 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/oval.py
+-rw-rw-rw-   0        0        0     5088 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/oval_response.py
+-rw-rw-rw-   0        0        0     8394 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_break_operate_parameter.py
+-rw-rw-rw-   0        0        0     8214 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_section.py
+-rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_sections_response.py
+-rw-rw-rw-   0        0        0    36653 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_setup.py
+-rw-rw-rw-   0        0        0     4720 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_setup_operate_parameter.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/page_setup_response.py
+-rw-rw-rw-   0        0        0     4487 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/password_request.py
+-rw-rw-rw-   0        0        0     6858 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/paste_options.py
+-rw-rw-rw-   0        0        0     9851 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/pattern_fill.py
+-rw-rw-rw-   0        0        0    12225 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/pdf_save_options.py
+-rw-rw-rw-   0        0        0    14691 2022-01-09 23:57:00.000000 asposecellscloud-23.6/asposecellscloud/models/pdf_security_options.py
+-rw-rw-rw-   0        0        0     7612 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pic_format_option.py
+-rw-rw-rw-   0        0        0    34670 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/picture.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/picture_response.py
+-rw-rw-rw-   0        0        0     5143 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pictures.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pictures_response.py
+-rw-rw-rw-   0        0        0    35618 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_field.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_field_response.py
+-rw-rw-rw-   0        0        0    11803 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_filter.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_filter_response.py
+-rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_filters_response.py
+-rw-rw-rw-   0        0        0     6544 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_item.py
+-rw-rw-rw-   0        0        0    62471 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_table.py
+-rw-rw-rw-   0        0        0     4488 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_table_field_request.py
+-rw-rw-rw-   0        0        0    11025 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_table_operate_parameter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_table_response.py
+-rw-rw-rw-   0        0        0     5261 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_tables.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.6/asposecellscloud/models/pivot_tables_response.py
+-rw-rw-rw-   0        0        0    11667 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/plot_area.py
+-rw-rw-rw-   0        0        0     5183 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/plot_area_response.py
+-rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:24.000000 asposecellscloud-23.6/asposecellscloud/models/pptx_save_options.py
+-rw-rw-rw-   0        0        0    19154 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/protect_sheet_parameter.py
+-rw-rw-rw-   0        0        0    23997 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/radio_button.py
+-rw-rw-rw-   0        0        0     5137 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/radio_button_response.py
+-rw-rw-rw-   0        0        0    11570 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/range.py
+-rw-rw-rw-   0        0        0     6655 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/range_copy_request.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/range_response.py
+-rw-rw-rw-   0        0        0     7038 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/range_set_outline_border_request.py
+-rw-rw-rw-   0        0        0     5147 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/range_set_style_request.py
+-rw-rw-rw-   0        0        0     4661 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/range_value_response.py
+-rw-rw-rw-   0        0        0     4469 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/ranges.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/ranges_response.py
+-rw-rw-rw-   0        0        0    22649 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/rectangle_shape.py
+-rw-rw-rw-   0        0        0     5158 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/rectangle_shape_response.py
+-rw-rw-rw-   0        0        0     6184 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/result_destination.py
+-rw-rw-rw-   0        0        0     9021 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/row.py
+-rw-rw-rw-   0        0        0     4431 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/row_response.py
+-rw-rw-rw-   0        0        0     6572 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/rows.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/rows_response.py
+-rw-rw-rw-   0        0        0     5504 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/save_files_to_cloud_result.py
+-rw-rw-rw-   0        0        0     5567 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/save_files_to_cloud_result_response.py
+-rw-rw-rw-   0        0        0    11282 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/save_options.py
+-rw-rw-rw-   0        0        0     4621 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/save_response.py
+-rw-rw-rw-   0        0        0     4525 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/save_result.py
+-rw-rw-rw-   0        0        0     5706 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/save_result_task_parameter.py
+-rw-rw-rw-   0        0        0    25940 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/scroll_bar.py
+-rw-rw-rw-   0        0        0     5123 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/scroll_bar_response.py
+-rw-rw-rw-   0        0        0    28722 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/series.py
+-rw-rw-rw-   0        0        0     6548 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/series_items.py
+-rw-rw-rw-   0        0        0     5119 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/series_response.py
+-rw-rw-rw-   0        0        0     5170 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/serieses_response.py
+-rw-rw-rw-   0        0        0     8516 2022-01-09 23:57:02.000000 asposecellscloud-23.6/asposecellscloud/models/shadow_effect.py
+-rw-rw-rw-   0        0        0    29570 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/shape.py
+-rw-rw-rw-   0        0        0     4569 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/shape_operate_parameter.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/shape_response.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/shapes.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/shapes_response.py
+-rw-rw-rw-   0        0        0     5135 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/single_value.py
+-rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/single_value_response.py
+-rw-rw-rw-   0        0        0     6559 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/smart_marker_task_parameter.py
+-rw-rw-rw-   0        0        0     5903 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/solid_fill.py
+-rw-rw-rw-   0        0        0     7683 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sort_key.py
+-rw-rw-rw-   0        0        0     5887 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sparkline.py
+-rw-rw-rw-   0        0        0    27947 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sparkline_group.py
+-rw-rw-rw-   0        0        0     4813 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sparkline_group_response.py
+-rw-rw-rw-   0        0        0     4776 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sparkline_groups.py
+-rw-rw-rw-   0        0        0     4846 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/sparkline_groups_response.py
+-rw-rw-rw-   0        0        0    24897 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/spinner.py
+-rw-rw-rw-   0        0        0     5109 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/spinner_response.py
+-rw-rw-rw-   0        0        0     4534 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/split_result.py
+-rw-rw-rw-   0        0        0     5141 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/split_result_document.py
+-rw-rw-rw-   0        0        0     4683 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/split_result_response.py
+-rw-rw-rw-   0        0        0     9690 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/split_workbook_task_parameter.py
+-rw-rw-rw-   0        0        0     6924 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/spreadsheet_ml2003_save_options.py
+-rw-rw-rw-   0        0        0    14315 2022-07-25 09:20:26.000000 asposecellscloud-23.6/asposecellscloud/models/sql_script_save_options.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7638 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    21950 2022-01-09 23:57:03.000000 asposecellscloud-23.6/asposecellscloud/models/style.py
+-rw-rw-rw-   0        0        0    10636 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/style_format_condition.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/style_response.py
+-rw-rw-rw-   0        0        0     4736 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/styles.py
+-rw-rw-rw-   0        0        0     4592 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/svg_save_options.py
+-rw-rw-rw-   0        0        0     6423 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/table_total_request.py
+-rw-rw-rw-   0        0        0     4418 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/task_data.py
+-rw-rw-rw-   0        0        0     5358 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/task_description.py
+-rw-rw-rw-   0        0        0     3796 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/task_parameter.py
+-rw-rw-rw-   0        0        0     3940 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/task_result_parameter.py
+-rw-rw-rw-   0        0        0     4945 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/task_run_result.py
+-rw-rw-rw-   0        0        0     5319 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/task_run_result_response.py
+-rw-rw-rw-   0        0        0    22607 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/text_box.py
+-rw-rw-rw-   0        0        0     5109 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/text_box_response.py
+-rw-rw-rw-   0        0        0     5662 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/text_format_condition.py
+-rw-rw-rw-   0        0        0     4942 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/text_item.py
+-rw-rw-rw-   0        0        0     5183 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/text_item_response.py
+-rw-rw-rw-   0        0        0     5186 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/text_items.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/text_items_response.py
+-rw-rw-rw-   0        0        0    14978 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/text_options.py
+-rw-rw-rw-   0        0        0     7524 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/text_water_marker_request.py
+-rw-rw-rw-   0        0        0     8184 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/texture_fill.py
+-rw-rw-rw-   0        0        0     5090 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/theme_color.py
+-rw-rw-rw-   0        0        0    12409 2022-12-08 06:28:10.000000 asposecellscloud-23.6/asposecellscloud/models/tick_labels.py
+-rw-rw-rw-   0        0        0     5231 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/tick_labels_response.py
+-rw-rw-rw-   0        0        0     8508 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/tile_pic_option.py
+-rw-rw-rw-   0        0        0     4472 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/time_period_format_condition.py
+-rw-rw-rw-   0        0        0    18670 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/title.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/title_response.py
+-rw-rw-rw-   0        0        0     6735 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/top10.py
+-rw-rw-rw-   0        0        0     6759 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/top10_filter.py
+-rw-rw-rw-   0        0        0     3898 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/total_request.py
+-rw-rw-rw-   0        0        0    19370 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/trendline.py
+-rw-rw-rw-   0        0        0     5191 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/trendline_response.py
+-rw-rw-rw-   0        0        0     4828 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/trendlines.py
+-rw-rw-rw-   0        0        0     5215 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/trendlines_response.py
+-rw-rw-rw-   0        0        0     6950 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/txt_save_options.py
+-rw-rw-rw-   0        0        0    18950 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/validation.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/validation_response.py
+-rw-rw-rw-   0        0        0     5968 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/validations.py
+-rw-rw-rw-   0        0        0     4695 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/validations_response.py
+-rw-rw-rw-   0        0        0     3776 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/value_type.py
+-rw-rw-rw-   0        0        0     6189 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/vertical_page_break.py
+-rw-rw-rw-   0        0        0     4931 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/vertical_page_break_response.py
+-rw-rw-rw-   0        0        0     5529 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/vertical_page_breaks.py
+-rw-rw-rw-   0        0        0     4964 2022-01-09 23:57:04.000000 asposecellscloud-23.6/asposecellscloud/models/vertical_page_breaks_response.py
+-rw-rw-rw-   0        0        0     9595 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/walls.py
+-rw-rw-rw-   0        0        0     5095 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/walls_response.py
+-rw-rw-rw-   0        0        0    11948 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook.py
+-rw-rw-rw-   0        0        0     6539 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_encryption_request.py
+-rw-rw-rw-   0        0        0     3936 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_operate_parameter.py
+-rw-rw-rw-   0        0        0     5709 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_protection_request.py
+-rw-rw-rw-   0        0        0     5491 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_replace_response.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_response.py
+-rw-rw-rw-   0        0        0    52420 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_settings.py
+-rw-rw-rw-   0        0        0     4951 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_settings_operate_parameter.py
+-rw-rw-rw-   0        0        0     4700 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/workbook_settings_response.py
+-rw-rw-rw-   0        0        0     5199 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/models/workbooks_response.py
+-rw-rw-rw-   0        0        0    32067 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheet.py
+-rw-rw-rw-   0        0        0     5720 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheet_moving_request.py
+-rw-rw-rw-   0        0        0     7026 2021-05-13 06:59:25.000000 asposecellscloud-23.6/asposecellscloud/models/worksheet_operate_parameter.py
+-rw-rw-rw-   0        0        0     5525 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheet_replace_response.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheet_response.py
+-rw-rw-rw-   0        0        0     5209 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheets.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/worksheets_response.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/xls_save_options.py
+-rw-rw-rw-   0        0        0     3862 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/xlsb_save_options.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.6/asposecellscloud/models/xps_save_options.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:06:02.767530 asposecellscloud-23.6/asposecellscloud/requests/
+-rw-rw-rw-   0        0        0    33820 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/__init__.py
+-rw-rw-rw-   0        0        0     4290 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/copy_file_request.py
+-rw-rw-rw-   0        0        0     4137 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/copy_folder_request.py
+-rw-rw-rw-   0        0        0     3513 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/create_folder_request.py
+-rw-rw-rw-   0        0        0     4058 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_decrypt_workbook_request.py
+-rw-rw-rw-   0        0        0     3715 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_document_properties_request.py
+-rw-rw-rw-   0        0        0     4246 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_document_property_request.py
+-rw-rw-rw-   0        0        0     3745 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py
+-rw-rw-rw-   0        0        0     3671 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_file_request.py
+-rw-rw-rw-   0        0        0     3674 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_folder_request.py
+-rw-rw-rw-   0        0        0     4092 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_header_footer_request.py
+-rw-rw-rw-   0        0        0     4450 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4241 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_horizontal_page_breaks_request.py
+-rw-rw-rw-   0        0        0     4087 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_metadata_request.py
+-rw-rw-rw-   0        0        0     5464 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_un_protect_workbook_request.py
+-rw-rw-rw-   0        0        0     4518 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_unprotect_worksheet_request.py
+-rw-rw-rw-   0        0        0     4438 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4249 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_vertical_page_breaks_request.py
+-rw-rw-rw-   0        0        0     3707 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_background_request.py
+-rw-rw-rw-   0        0        0     4049 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_name_request.py
+-rw-rw-rw-   0        0        0     3687 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_names_request.py
+-rw-rw-rw-   0        0        0     4103 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_background_request.py
+-rw-rw-rw-   0        0        0     4785 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_cells_range_request.py
+-rw-rw-rw-   0        0        0     4506 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4105 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_clear_charts_request.py
+-rw-rw-rw-   0        0        0     5285 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4093 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_comments_request.py
+-rw-rw-rw-   0        0        0     5828 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py
+-rw-rw-rw-   0        0        0     4507 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     4165 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py
+-rw-rw-rw-   0        0        0     5804 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_date_filter_request.py
+-rw-rw-rw-   0        0        0     4499 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_delete_chart_request.py
+-rw-rw-rw-   0        0        0     4636 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_filter_request.py
+-rw-rw-rw-   0        0        0     5624 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py
+-rw-rw-rw-   0        0        0     4530 2023-05-25 12:57:31.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     4103 2023-05-25 12:57:31.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py
+-rw-rw-rw-   0        0        0     4557 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4110 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_list_objects_request.py
+-rw-rw-rw-   0        0        0     4541 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4105 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_ole_objects_request.py
+-rw-rw-rw-   0        0        0     4498 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_picture_request.py
+-rw-rw-rw-   0        0        0     4093 2023-05-25 12:57:31.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pictures_request.py
+-rw-rw-rw-   0        0        0     5207 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4812 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py
+-rw-rw-rw-   0        0        0     4557 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4110 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py
+-rw-rw-rw-   0        0        0     4050 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_request.py
+-rw-rw-rw-   0        0        0     4440 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4804 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     4083 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_shapes_request.py
+-rw-rw-rw-   0        0        0     4563 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4130 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py
+-rw-rw-rw-   0        0        0     4546 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4108 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_validations_request.py
+-rw-rw-rw-   0        0        0     3849 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/delete_worksheets_request.py
+-rw-rw-rw-   0        0        0     3678 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/download_file_request.py
+-rw-rw-rw-   0        0        0     4426 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_cell_html_string_request.py
+-rw-rw-rw-   0        0        0     3073 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_cells_cloud_service_status_request.py
+-rw-rw-rw-   0        0        0     3072 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py
+-rw-rw-rw-   0        0        0     4467 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_border_request.py
+-rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_fill_format_request.py
+-rw-rw-rw-   0        0        0     4432 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_request.py
+-rw-rw-rw-   0        0        0     4473 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_category_axis_request.py
+-rw-rw-rw-   0        0        0     4512 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_second_category_axis_request.py
+-rw-rw-rw-   0        0        0     4494 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_second_value_axis_request.py
+-rw-rw-rw-   0        0        0     4461 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_series_axis_request.py
+-rw-rw-rw-   0        0        0     4455 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_chart_value_axis_request.py
+-rw-rw-rw-   0        0        0     3212 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_disc_usage_request.py
+-rw-rw-rw-   0        0        0     3844 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_document_properties_request.py
+-rw-rw-rw-   0        0        0     4114 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_document_property_request.py
+-rw-rw-rw-   0        0        0     4486 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_extract_barcodes_request.py
+-rw-rw-rw-   0        0        0     3536 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_file_versions_request.py
+-rw-rw-rw-   0        0        0     3340 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_files_list_request.py
+-rw-rw-rw-   0        0        0     4042 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_footer_request.py
+-rw-rw-rw-   0        0        0     4042 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_header_request.py
+-rw-rw-rw-   0        0        0     4441 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4114 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_horizontal_page_breaks_request.py
+-rw-rw-rw-   0        0        0     4091 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_metadata_request.py
+-rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_named_range_value_request.py
+-rw-rw-rw-   0        0        0     3677 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_named_ranges_request.py
+-rw-rw-rw-   0        0        0     3652 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_page_count_request.py
+-rw-rw-rw-   0        0        0     4046 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_page_setup_request.py
+-rw-rw-rw-   0        0        0     5403 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4427 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4102 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_vertical_page_breaks_request.py
+-rw-rw-rw-   0        0        0     3699 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_default_style_request.py
+-rw-rw-rw-   0        0        0     4028 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_name_request.py
+-rw-rw-rw-   0        0        0     4062 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_name_value_request.py
+-rw-rw-rw-   0        0        0     3670 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_names_request.py
+-rw-rw-rw-   0        0        0     4880 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_request.py
+-rw-rw-rw-   0        0        0     3693 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_settings_request.py
+-rw-rw-rw-   0        0        0     3691 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_workbook_text_items_request.py
+-rw-rw-rw-   0        0        0     4090 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_auto_filter_request.py
+-rw-rw-rw-   0        0        0     4704 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py
+-rw-rw-rw-   0        0        0     4088 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_autoshapes_request.py
+-rw-rw-rw-   0        0        0     4481 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4503 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cell_request.py
+-rw-rw-rw-   0        0        0     4451 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cell_style_request.py
+-rw-rw-rw-   0        0        0     4936 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cells_range_value_request.py
+-rw-rw-rw-   0        0        0     4332 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cells_request.py
+-rw-rw-rw-   0        0        0     4484 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4584 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4477 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4064 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_charts_request.py
+-rw-rw-rw-   0        0        0     4466 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_column_request.py
+-rw-rw-rw-   0        0        0     3951 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4437 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4076 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_comments_request.py
+-rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     4162 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py
+-rw-rw-rw-   0        0        0     4511 2023-05-25 12:57:31.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     4088 2023-05-25 12:57:31.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_hyperlinks_request.py
+-rw-rw-rw-   0        0        0     4649 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_list_objects_request.py
+-rw-rw-rw-   0        0        0     4539 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_merged_cell_request.py
+-rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_merged_cells_request.py
+-rw-rw-rw-   0        0        0     4621 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4090 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_ole_objects_request.py
+-rw-rw-rw-   0        0        0     4070 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_page_count_request.py
+-rw-rw-rw-   0        0        0     4888 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_picture_with_format_request.py
+-rw-rw-rw-   0        0        0     4076 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pictures_request.py
+-rw-rw-rw-   0        0        0     4993 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4592 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py
+-rw-rw-rw-   0        0        0     4531 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4096 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_tables_request.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4333 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     4435 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     4064 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_shapes_request.py
+-rw-rw-rw-   0        0        0     4549 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4120 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py
+-rw-rw-rw-   0        0        0     4084 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_text_items_request.py
+-rw-rw-rw-   0        0        0     4528 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4094 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_validations_request.py
+-rw-rw-rw-   0        0        0     4942 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_with_format_request.py
+-rw-rw-rw-   0        0        0     3670 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/get_worksheets_request.py
+-rw-rw-rw-   0        0        0     4290 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/move_file_request.py
+-rw-rw-rw-   0        0        0     4137 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/move_folder_request.py
+-rw-rw-rw-   0        0        0     3686 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/object_exists_request.py
+-rw-rw-rw-   0        0        0     4458 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_assemble_request.py
+-rw-rw-rw-   0        0        0     4054 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_autofit_workbook_columns_request.py
+-rw-rw-rw-   0        0        0     4163 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_autofit_workbook_rows_request.py
+-rw-rw-rw-   0        0        0     4610 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5265 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4559 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3481 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_batch_convert_request.py
+-rw-rw-rw-   0        0        0     3445 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_batch_lock_request.py
+-rw-rw-rw-   0        0        0     3481 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_batch_protect_request.py
+-rw-rw-rw-   0        0        0     3457 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_batch_split_request.py
+-rw-rw-rw-   0        0        0     3453 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_batch_unlock_request.py
+-rw-rw-rw-   0        0        0     4565 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_cell_calculate_request.py
+-rw-rw-rw-   0        0        0     4571 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_cell_characters_request.py
+-rw-rw-rw-   0        0        0     4798 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_chart_category_axis_request.py
+-rw-rw-rw-   0        0        0     4844 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_chart_second_category_axis_request.py
+-rw-rw-rw-   0        0        0     4823 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_chart_second_value_axis_request.py
+-rw-rw-rw-   0        0        0     4784 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_chart_series_axis_request.py
+-rw-rw-rw-   0        0        0     4777 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_chart_value_axis_request.py
+-rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_clear_contents_request.py
+-rw-rw-rw-   0        0        0     4847 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_clear_formats_request.py
+-rw-rw-rw-   0        0        0     4661 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_clear_objects_request.py
+-rw-rw-rw-   0        0        0     4776 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_column_style_request.py
+-rw-rw-rw-   0        0        0     4133 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_compress_request.py
+-rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_csv_request.py
+-rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_docx_request.py
+-rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_html_request.py
+-rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_json_request.py
+-rw-rw-rw-   0        0        0     4005 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py
+-rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py
+-rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_png_request.py
+-rw-rw-rw-   0        0        0     3989 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py
+-rw-rw-rw-   0        0        0     3985 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_sql_request.py
+-rw-rw-rw-   0        0        0     5290 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_copy_cell_into_cell_request.py
+-rw-rw-rw-   0        0        0     5652 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5164 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_request.py
+-rw-rw-rw-   0        0        0     5547 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     4533 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_digital_signature_request.py
+-rw-rw-rw-   0        0        0     4048 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_encrypt_workbook_request.py
+-rw-rw-rw-   0        0        0     4247 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_export_request.py
+-rw-rw-rw-   0        0        0     5117 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_footer_request.py
+-rw-rw-rw-   0        0        0     5021 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_group_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5000 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_group_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5117 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_header_request.py
+-rw-rw-rw-   0        0        0     4922 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_hide_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4839 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_hide_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3832 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_import_data_request.py
+-rw-rw-rw-   0        0        0     3544 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_import_request.py
+-rw-rw-rw-   0        0        0     4280 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_merge_request.py
+-rw-rw-rw-   0        0        0     4246 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_metadata_request.py
+-rw-rw-rw-   0        0        0     4391 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_move_worksheet_request.py
+-rw-rw-rw-   0        0        0     4404 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_page_setup_request.py
+-rw-rw-rw-   0        0        0     5756 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_cell_style_request.py
+-rw-rw-rw-   0        0        0     6386 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py
+-rw-rw-rw-   0        0        0     5634 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_field_move_to_request.py
+-rw-rw-rw-   0        0        0     5058 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_style_request.py
+-rw-rw-rw-   0        0        0     6086 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py
+-rw-rw-rw-   0        0        0     5635 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py
+-rw-rw-rw-   0        0        0     3903 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_protect_request.py
+-rw-rw-rw-   0        0        0     4048 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_protect_workbook_request.py
+-rw-rw-rw-   0        0        0     4426 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_rename_worksheet_request.py
+-rw-rw-rw-   0        0        0     4761 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_replace_request.py
+-rw-rw-rw-   0        0        0     4461 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_reverse_request.py
+-rw-rw-rw-   0        0        0     4456 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_rotate_request.py
+-rw-rw-rw-   0        0        0     4725 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_row_style_request.py
+-rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_run_task_request.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_search_request.py
+-rw-rw-rw-   0        0        0     4465 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_set_cell_html_string_request.py
+-rw-rw-rw-   0        0        0     5119 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_set_cell_range_value_request.py
+-rw-rw-rw-   0        0        0     5001 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_set_worksheet_column_width_request.py
+-rw-rw-rw-   0        0        0     4516 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_split_request.py
+-rw-rw-rw-   0        0        0     4907 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5025 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5070 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_unhide_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4993 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_unhide_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3898 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_unlock_request.py
+-rw-rw-rw-   0        0        0     4824 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_cell_style_request.py
+-rw-rw-rw-   0        0        0     4875 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4427 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_property_request.py
+-rw-rw-rw-   0        0        0     4799 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_range_style_request.py
+-rw-rw-rw-   0        0        0     4735 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4429 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_zoom_request.py
+-rw-rw-rw-   0        0        0     4597 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_watermark_request.py
+-rw-rw-rw-   0        0        0     4026 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4423 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_export_xml_request.py
+-rw-rw-rw-   0        0        0     4219 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py
+-rw-rw-rw-   0        0        0     4848 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_import_xml_request.py
+-rw-rw-rw-   0        0        0     4378 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_name_request.py
+-rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_save_as_request.py
+-rw-rw-rw-   0        0        0     4034 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_settings_request.py
+-rw-rw-rw-   0        0        0     5068 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_split_request.py
+-rw-rw-rw-   0        0        0     4459 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbook_text_replace_request.py
+-rw-rw-rw-   0        0        0     4274 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbooks_merge_request.py
+-rw-rw-rw-   0        0        0     4031 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_workbooks_text_search_request.py
+-rw-rw-rw-   0        0        0     4133 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py
+-rw-rw-rw-   0        0        0     4490 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4876 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cell_set_value_request.py
+-rw-rw-rw-   0        0        0     4840 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py
+-rw-rw-rw-   0        0        0     4448 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py
+-rw-rw-rw-   0        0        0     5232 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py
+-rw-rw-rw-   0        0        0     4563 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py
+-rw-rw-rw-   0        0        0     4826 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py
+-rw-rw-rw-   0        0        0     4512 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_style_request.py
+-rw-rw-rw-   0        0        0     4463 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py
+-rw-rw-rw-   0        0        0     5126 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_value_request.py
+-rw-rw-rw-   0        0        0     4483 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_ranges_request.py
+-rw-rw-rw-   0        0        0     4826 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4771 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4811 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4781 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4460 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_group_shape_request.py
+-rw-rw-rw-   0        0        0     4871 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     5329 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_column_request.py
+-rw-rw-rw-   0        0        0     5046 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_columns_total_request.py
+-rw-rw-rw-   0        0        0     4639 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py
+-rw-rw-rw-   0        0        0     4916 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4983 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py
+-rw-rw-rw-   0        0        0     5661 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4505 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_match_blanks_request.py
+-rw-rw-rw-   0        0        0     4526 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py
+-rw-rw-rw-   0        0        0     5622 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_merge_request.py
+-rw-rw-rw-   0        0        0     4821 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_picture_request.py
+-rw-rw-rw-   0        0        0     4603 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py
+-rw-rw-rw-   0        0        0     5021 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py
+-rw-rw-rw-   0        0        0     4829 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_range_sort_request.py
+-rw-rw-rw-   0        0        0     4747 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     5016 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4423 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_text_search_request.py
+-rw-rw-rw-   0        0        0     4492 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py
+-rw-rw-rw-   0        0        0     5640 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_unmerge_request.py
+-rw-rw-rw-   0        0        0     4896 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/post_worsheet_text_replace_request.py
+-rw-rw-rw-   0        0        0     4068 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_active_worksheet_request.py
+-rw-rw-rw-   0        0        0     4373 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_add_new_worksheet_request.py
+-rw-rw-rw-   0        0        0     4500 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_change_visibility_worksheet_request.py
+-rw-rw-rw-   0        0        0     4603 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_convert_workbook_request.py
+-rw-rw-rw-   0        0        0     4047 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/put_document_property_request.py
+-rw-rw-rw-   0        0        0     4080 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_document_protect_from_changes_request.py
+-rw-rw-rw-   0        0        0     4852 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4973 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_insert_new_worksheet_request.py
+-rw-rw-rw-   0        0        0     5067 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4455 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4819 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5644 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4490 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_protect_worksheet_request.py
+-rw-rw-rw-   0        0        0     4806 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4182 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_workbook_background_request.py
+-rw-rw-rw-   0        0        0     4430 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_workbook_create_request.py
+-rw-rw-rw-   0        0        0     4010 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_workbook_name_request.py
+-rw-rw-rw-   0        0        0     4182 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_workbook_water_marker_request.py
+-rw-rw-rw-   0        0        0     6894 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_add_chart_request.py
+-rw-rw-rw-   0        0        0     5182 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_add_picture_request.py
+-rw-rw-rw-   0        0        0     4575 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_background_request.py
+-rw-rw-rw-   0        0        0     4764 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_cells_range_request.py
+-rw-rw-rw-   0        0        0     4488 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4599 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     5539 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_color_filter_request.py
+-rw-rw-rw-   0        0        0     4771 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4944 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     6443 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_custom_filter_request.py
+-rw-rw-rw-   0        0        0     6443 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_date_filter_request.py
+-rw-rw-rw-   0        0        0     5640 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py
+-rw-rw-rw-   0        0        0     5482 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_filter_request.py
+-rw-rw-rw-   0        0        0     6276 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_filter_top10_request.py
+-rw-rw-rw-   0        0        0     4871 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_area_request.py
+-rw-rw-rw-   0        0        0     6049 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py
+-rw-rw-rw-   0        0        0     6330 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_request.py
+-rw-rw-rw-   0        0        0     5597 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_freeze_panes_request.py
+-rw-rw-rw-   0        0        0     5999 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     5918 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_icon_filter_request.py
+-rw-rw-rw-   0        0        0     5244 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     5064 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     5126 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4801 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     5290 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     5651 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4223 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     3428 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/storage_exists_request.py
+-rw-rw-rw-   0        0        0     4127 2023-04-21 23:29:09.000000 asposecellscloud-23.6/asposecellscloud/requests/upload_file_request.py
+-rw-rw-rw-   0        0        0    14273 2023-06-30 00:03:35.000000 asposecellscloud-23.6/asposecellscloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:05:39.793170 asposecellscloud-23.6/asposecellscloud.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-06-30 00:05:38.000000 asposecellscloud-23.6/asposecellscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    37775 2023-06-30 00:05:39.000000 asposecellscloud-23.6/asposecellscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 00:05:38.000000 asposecellscloud-23.6/asposecellscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-30 00:05:38.000000 asposecellscloud-23.6/asposecellscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-30 00:05:38.000000 asposecellscloud-23.6/asposecellscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 00:06:04.317197 asposecellscloud-23.6/setup.cfg
+-rw-rw-rw-   0        0        0     1451 2023-06-30 00:05:28.000000 asposecellscloud-23.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:06:04.208106 asposecellscloud-23.6/test/
+-rw-rw-rw-   0        0        0     7256 2022-12-08 07:15:43.000000 asposecellscloud-23.6/test/test_cells_chart_axis_api.py
+-rw-rw-rw-   0        0        0     7996 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_auto_filter_controller.py
+-rw-rw-rw-   0        0        0     4639 2023-06-30 00:03:35.000000 asposecellscloud-23.6/test/tests_batch_controller.py
+-rw-rw-rw-   0        0        0     1338 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_cells_barcodes_controller.py
+-rw-rw-rw-   0        0        0    21475 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_cells_controller.py
+-rw-rw-rw-   0        0        0     1774 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_cells_status_controller.py
+-rw-rw-rw-   0        0        0     2297 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_chart_area_controller.py
+-rw-rw-rw-   0        0        0     8079 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_charts_controller.py
+-rw-rw-rw-   0        0        0     5842 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_conditional_formattings_controller.py
+-rw-rw-rw-   0        0        0    70981 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_conversion.py
+-rw-rw-rw-   0        0        0    18233 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_conversion_json.py
+-rw-rw-rw-   0        0        0    17784 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_conversion_png.py
+-rw-rw-rw-   0        0        0     3361 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_file_controller.py
+-rw-rw-rw-   0        0        0     3093 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_folder_controller.py
+-rw-rw-rw-   0        0        0     3932 2023-06-30 00:03:35.000000 asposecellscloud-23.6/test/tests_hypelinks_controller.py
+-rw-rw-rw-   0        0        0   120147 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_light_cells.py
+-rw-rw-rw-   0        0        0     7608 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_list_objects_controller.py
+-rw-rw-rw-   0        0        0     4326 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_ole_objects_controller.py
+-rw-rw-rw-   0        0        0     1333 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_one.py
+-rw-rw-rw-   0        0        0     5884 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_page_breaks_controller.py
+-rw-rw-rw-   0        0        0     4203 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_page_setup_controller.py
+-rw-rw-rw-   0        0        0     4182 2023-06-30 00:03:35.000000 asposecellscloud-23.6/test/tests_pictures_controller.py
+-rw-rw-rw-   0        0        0    12668 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_pivot_tables_controller.py
+-rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_properties_controller.py
+-rw-rw-rw-   0        0        0     8719 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_ranges_controller.py
+-rw-rw-rw-   0        0        0     4970 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_shapes_controller.py
+-rw-rw-rw-   0        0        0     4073 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_sparkline_groups_controller.py
+-rw-rw-rw-   0        0        0     2573 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_storage_controller.py
+-rw-rw-rw-   0        0        0    18939 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_workbook_controller.py
+-rw-rw-rw-   0        0        0    21080 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_worksheet_controller.py
+-rw-rw-rw-   0        0        0     3912 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_worksheet_validations_controller.py
+-rw-rw-rw-   0        0        0     2422 2023-04-21 23:29:10.000000 asposecellscloud-23.6/test/tests_xml_controller.py
```

### Comparing `asposecellscloud-23.5.1/LICENSE` & `asposecellscloud-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/PKG-INFO` & `asposecellscloud-23.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asposecellscloud
-Version: 23.5.1
+Version: 23.6
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: aspose.cloud@aspose.com
 License: UNKNOWN
 Description: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Keywords: aspose,cells,cloud
```

### Comparing `asposecellscloud-23.5.1/README.md` & `asposecellscloud-23.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/23.5)
+![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/23.6)
 
 
 # Python SDK for Spreadsheet Processing in Cloud
 
 Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications. 
 
 [Aspose.Cells Cloud SDK for Python](https://products.aspose.cloud/cells/python) offers Excel® file creation, editing, conversion, & rendering. Developers can format worksheets, rows, columns or cells to the most granular level, create & manipulate chart & pivot tables, render worksheets, charts and specific data ranges to PDF & images, add & calculate Excel's built-in and custom formulas and much more.
@@ -17,17 +17,21 @@
 - Set complex formulas & calculate results via API.
 - Set protection on workbook, worksheet, cell, column or row.
 - Create & manipulate named ranges.
 - Populate worksheets through Smart Markers.
 - Convert worksheets to PDF, XPS & SVG formats.
 - Inter-convert files to popular Excel formats.
 
-## Feature & Enhancements in Version 23.5
+## Feature & Enhancements in Version 23.6
 
-- Fix few method names for spelling error.
+- Support to batch lock multi-files.
+- Support to batch unlock multi-files.
+- Support to protect lock multi-files.
+- Support to split lock multi-files.
+- Fix put document property api.
 
  
 ## Read & Write Spreadsheet Formats
 
 **Microsoft Excel:** XLS, XLSX, XLSB, XLSM, XLT, XLTX, XLTM
 **OpenOffice:** ODS
 **SpreadsheetML:** XML
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/api_client.py` & `asposecellscloud-23.6/asposecellscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = Configuration().host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Aspose.Cells.Cloud/23.5.1/python'
+        self.user_agent = 'Aspose.Cells.Cloud/23.6/python'
 
     @property
     def user_agent(self):
         """
         Gets user agent.
         """
         return self.default_headers['User-Agent']
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/apis/cells_api.py` & `asposecellscloud-23.6/asposecellscloud/apis/cells_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,14 +825,199 @@
                                         auth_settings=http_params['auth_settings'],
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
+    # <summary>
+    # </summary>
+    # <param name="request">Request. <see cref="PostBatchProtectRequest" /></param>
+    def post_batch_protect(self, request, **kwargs):
+
+        kwargs['_return_http_data_only'] = True
+        self.check_access_token()
+        if kwargs.get('callback'):
+            return self.post_batch_protect_with_http_info(request,**kwargs)
+        else:
+            (data) = self.post_batch_protect_with_http_info(request,**kwargs)
+            return data
+
+    def post_batch_protect_with_http_info(self, request, **kwargs):
+        all_params = []
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_batch_protect" % key
+                )
+            params[key] = val
+        del params['kwargs'] 
+
+        http_params = request.create_http_request(self.api_client)
+        return self.api_client.call_api(http_params['path'], http_params['method'],
+                                        None,
+                                        http_params['query_params'],
+                                        http_params['header_params'],
+                                        body=http_params['body'],
+                                        post_params=http_params['form_params'],
+                                        files=http_params['files'],
+                                        response_type=http_params['response_type'],
+                                        auth_settings=http_params['auth_settings'],
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=http_params['collection_formats'])
+
+
+
+    # <summary>
+    # </summary>
+    # <param name="request">Request. <see cref="PostBatchLockRequest" /></param>
+    def post_batch_lock(self, request, **kwargs):
+
+        kwargs['_return_http_data_only'] = True
+        self.check_access_token()
+        if kwargs.get('callback'):
+            return self.post_batch_lock_with_http_info(request,**kwargs)
+        else:
+            (data) = self.post_batch_lock_with_http_info(request,**kwargs)
+            return data
+
+    def post_batch_lock_with_http_info(self, request, **kwargs):
+        all_params = []
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_batch_lock" % key
+                )
+            params[key] = val
+        del params['kwargs'] 
+
+        http_params = request.create_http_request(self.api_client)
+        return self.api_client.call_api(http_params['path'], http_params['method'],
+                                        None,
+                                        http_params['query_params'],
+                                        http_params['header_params'],
+                                        body=http_params['body'],
+                                        post_params=http_params['form_params'],
+                                        files=http_params['files'],
+                                        response_type=http_params['response_type'],
+                                        auth_settings=http_params['auth_settings'],
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=http_params['collection_formats'])
+
+
+
+    # <summary>
+    # </summary>
+    # <param name="request">Request. <see cref="PostBatchUnlockRequest" /></param>
+    def post_batch_unlock(self, request, **kwargs):
+
+        kwargs['_return_http_data_only'] = True
+        self.check_access_token()
+        if kwargs.get('callback'):
+            return self.post_batch_unlock_with_http_info(request,**kwargs)
+        else:
+            (data) = self.post_batch_unlock_with_http_info(request,**kwargs)
+            return data
+
+    def post_batch_unlock_with_http_info(self, request, **kwargs):
+        all_params = []
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_batch_unlock" % key
+                )
+            params[key] = val
+        del params['kwargs'] 
+
+        http_params = request.create_http_request(self.api_client)
+        return self.api_client.call_api(http_params['path'], http_params['method'],
+                                        None,
+                                        http_params['query_params'],
+                                        http_params['header_params'],
+                                        body=http_params['body'],
+                                        post_params=http_params['form_params'],
+                                        files=http_params['files'],
+                                        response_type=http_params['response_type'],
+                                        auth_settings=http_params['auth_settings'],
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=http_params['collection_formats'])
+
+
+
+    # <summary>
+    # </summary>
+    # <param name="request">Request. <see cref="PostBatchSplitRequest" /></param>
+    def post_batch_split(self, request, **kwargs):
+
+        kwargs['_return_http_data_only'] = True
+        self.check_access_token()
+        if kwargs.get('callback'):
+            return self.post_batch_split_with_http_info(request,**kwargs)
+        else:
+            (data) = self.post_batch_split_with_http_info(request,**kwargs)
+            return data
+
+    def post_batch_split_with_http_info(self, request, **kwargs):
+        all_params = []
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_batch_split" % key
+                )
+            params[key] = val
+        del params['kwargs'] 
+
+        http_params = request.create_http_request(self.api_client)
+        return self.api_client.call_api(http_params['path'], http_params['method'],
+                                        None,
+                                        http_params['query_params'],
+                                        http_params['header_params'],
+                                        body=http_params['body'],
+                                        post_params=http_params['form_params'],
+                                        files=http_params['files'],
+                                        response_type=http_params['response_type'],
+                                        auth_settings=http_params['auth_settings'],
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=http_params['collection_formats'])
 
 
     # <summary>
     # </summary>
     # <param name="request">Request. <see cref="GetExtractBarcodesRequest" /></param>
     def get_extract_barcodes(self, request, **kwargs):
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/apis/light_cells_api.py` & `asposecellscloud-23.6/asposecellscloud/apis/light_cells_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/apis/lite_cells_api.py` & `asposecellscloud-23.6/asposecellscloud/apis/lite_cells_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/configuration.py` & `asposecellscloud-23.6/asposecellscloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,9 +251,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3.0\n"\
-               "SDK Package Version: 23.4".\
+               "SDK Package Version: 23.6".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/__init__.py` & `asposecellscloud-23.6/asposecellscloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from .access_token_response import AccessTokenResponse
 from .area import Area
 from .auto_fitter_options import AutoFitterOptions
 from .axis import Axis
 from .barcode_response import BarcodeResponse
 from .barcode_response_list import BarcodeResponseList
 from .batch_convert_request import BatchConvertRequest
+from .batch_lock_request import BatchLockRequest
+from .batch_protect_request import BatchProtectRequest
+from .batch_split_request import BatchSplitRequest
 from .border import Border
 from .calculation_options import CalculationOptions
 from .cell_area import CellArea
 from .cell_value import CellValue
 from .cells_cloud_file_info import CellsCloudFileInfo
 from .cells_cloud_response import CellsCloudResponse
 from .cells_color import CellsColor
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/above_average.py` & `asposecellscloud-23.6/asposecellscloud/models/above_average.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/access_token_response.py` & `asposecellscloud-23.6/asposecellscloud/models/access_token_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/area.py` & `asposecellscloud-23.6/asposecellscloud/models/area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_filter_response.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_fitter_options.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_fitter_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_shape.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_shape_response.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_shapes.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/auto_shapes_response.py` & `asposecellscloud-23.6/asposecellscloud/models/auto_shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/axis.py` & `asposecellscloud-23.6/asposecellscloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/axis_response.py` & `asposecellscloud-23.6/asposecellscloud/models/axis_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/barcode_response.py` & `asposecellscloud-23.6/asposecellscloud/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/barcode_response_list.py` & `asposecellscloud-23.6/asposecellscloud/models/barcode_response_list.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/batch_convert_request.py` & `asposecellscloud-23.6/asposecellscloud/models/batch_convert_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/border.py` & `asposecellscloud-23.6/asposecellscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/calculation_options.py` & `asposecellscloud-23.6/asposecellscloud/models/calculation_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cell.py` & `asposecellscloud-23.6/asposecellscloud/models/cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cell_area.py` & `asposecellscloud-23.6/asposecellscloud/models/cell_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cell_response.py` & `asposecellscloud-23.6/asposecellscloud/models/cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cell_value.py` & `asposecellscloud-23.6/asposecellscloud/models/cell_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells.py` & `asposecellscloud-23.6/asposecellscloud/models/cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_cloud_file_info.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_cloud_file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_cloud_response.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_cloud_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_color.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_document_properties.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_document_properties.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_document_properties_response.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_document_properties_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_document_property.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_document_property.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_document_property_response.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_document_property_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_error.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_error.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_object_operate_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_object_operate_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/cells_response.py` & `asposecellscloud-23.6/asposecellscloud/models/cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/chart.py` & `asposecellscloud-23.6/asposecellscloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/chart_area.py` & `asposecellscloud-23.6/asposecellscloud/models/chart_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/chart_area_response.py` & `asposecellscloud-23.6/asposecellscloud/models/chart_area_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/chart_frame.py` & `asposecellscloud-23.6/asposecellscloud/models/chart_frame.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/chart_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/chart_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/charts.py` & `asposecellscloud-23.6/asposecellscloud/models/charts.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/charts_response.py` & `asposecellscloud-23.6/asposecellscloud/models/charts_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/color.py` & `asposecellscloud-23.6/asposecellscloud/models/color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/color_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/color_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/color_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/models/color_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/color_scale.py` & `asposecellscloud-23.6/asposecellscloud/models/color_scale.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/column.py` & `asposecellscloud-23.6/asposecellscloud/models/column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/column_response.py` & `asposecellscloud-23.6/asposecellscloud/models/column_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/columns.py` & `asposecellscloud-23.6/asposecellscloud/models/columns.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/columns_response.py` & `asposecellscloud-23.6/asposecellscloud/models/columns_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/comment.py` & `asposecellscloud-23.6/asposecellscloud/models/comment.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/comment_response.py` & `asposecellscloud-23.6/asposecellscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/comments.py` & `asposecellscloud-23.6/asposecellscloud/models/comments.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/comments_response.py` & `asposecellscloud-23.6/asposecellscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formatting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_icon.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_icon.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_response.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formatting_value.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formatting_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formattings.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formattings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/conditional_formattings_response.py` & `asposecellscloud-23.6/asposecellscloud/models/conditional_formattings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/convert_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/convert_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/convert_worksheet_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/convert_worksheet_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/copy_options.py` & `asposecellscloud-23.6/asposecellscloud/models/copy_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/create_pivot_table_request.py` & `asposecellscloud-23.6/asposecellscloud/models/create_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/custom_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/custom_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/custom_parser_config.py` & `asposecellscloud-23.6/asposecellscloud/models/custom_parser_config.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/data_bar.py` & `asposecellscloud-23.6/asposecellscloud/models/data_bar.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/data_bar_border.py` & `asposecellscloud-23.6/asposecellscloud/models/data_bar_border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/data_sorter.py` & `asposecellscloud-23.6/asposecellscloud/models/data_sorter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/dif_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/dif_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/disc_usage.py` & `asposecellscloud-23.6/asposecellscloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/docx_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/docx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/dynamic_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/dynamic_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/error_details.py` & `asposecellscloud-23.6/asposecellscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/file_info.py` & `asposecellscloud-23.6/asposecellscloud/models/file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/file_source.py` & `asposecellscloud-23.6/asposecellscloud/models/file_source.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/file_version.py` & `asposecellscloud-23.6/asposecellscloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/file_versions.py` & `asposecellscloud-23.6/asposecellscloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/files_list.py` & `asposecellscloud-23.6/asposecellscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/files_result.py` & `asposecellscloud-23.6/asposecellscloud/models/files_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/files_upload_result.py` & `asposecellscloud-23.6/asposecellscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/fill_format.py` & `asposecellscloud-23.6/asposecellscloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/fill_format_response.py` & `asposecellscloud-23.6/asposecellscloud/models/fill_format_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/filter_column.py` & `asposecellscloud-23.6/asposecellscloud/models/filter_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/font.py` & `asposecellscloud-23.6/asposecellscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/font_setting.py` & `asposecellscloud-23.6/asposecellscloud/models/font_setting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/format_condition.py` & `asposecellscloud-23.6/asposecellscloud/models/format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/gradient_fill.py` & `asposecellscloud-23.6/asposecellscloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/gradient_fill_stop.py` & `asposecellscloud-23.6/asposecellscloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_break.py` & `asposecellscloud-23.6/asposecellscloud/models/horizontal_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_break_response.py` & `asposecellscloud-23.6/asposecellscloud/models/horizontal_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_breaks.py` & `asposecellscloud-23.6/asposecellscloud/models/horizontal_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/horizontal_page_breaks_response.py` & `asposecellscloud-23.6/asposecellscloud/models/horizontal_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/html_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/hyperlink.py` & `asposecellscloud-23.6/asposecellscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/hyperlink_response.py` & `asposecellscloud-23.6/asposecellscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/hyperlinks.py` & `asposecellscloud-23.6/asposecellscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/hyperlinks_response.py` & `asposecellscloud-23.6/asposecellscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/icon_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/icon_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/icon_set.py` & `asposecellscloud-23.6/asposecellscloud/models/icon_set.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/image_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/image_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_batch_data_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_batch_data_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_csv_data_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_csv_data_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_data_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/import_data_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_double_array_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_double_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_int_array_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_int_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_picture_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_picture_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_position.py` & `asposecellscloud-23.6/asposecellscloud/models/import_position.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_string_array_option.py` & `asposecellscloud-23.6/asposecellscloud/models/import_string_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/import_xml_request.py` & `asposecellscloud-23.6/asposecellscloud/models/import_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/json_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/json_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/legend.py` & `asposecellscloud-23.6/asposecellscloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/legend_response.py` & `asposecellscloud-23.6/asposecellscloud/models/legend_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/line.py` & `asposecellscloud-23.6/asposecellscloud/models/line.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/line_format.py` & `asposecellscloud-23.6/asposecellscloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/line_response.py` & `asposecellscloud-23.6/asposecellscloud/models/line_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/link.py` & `asposecellscloud-23.6/asposecellscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/link_element.py` & `asposecellscloud-23.6/asposecellscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_column.py` & `asposecellscloud-23.6/asposecellscloud/models/list_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_object.py` & `asposecellscloud-23.6/asposecellscloud/models/list_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_object_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/list_object_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_object_response.py` & `asposecellscloud-23.6/asposecellscloud/models/list_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_objects.py` & `asposecellscloud-23.6/asposecellscloud/models/list_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/list_objects_response.py` & `asposecellscloud-23.6/asposecellscloud/models/list_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/m_html_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/m_html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/markdown_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/markdown_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/match_condition_request.py` & `asposecellscloud-23.6/asposecellscloud/models/match_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/merged_cell.py` & `asposecellscloud-23.6/asposecellscloud/models/merged_cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/merged_cell_response.py` & `asposecellscloud-23.6/asposecellscloud/models/merged_cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/merged_cells.py` & `asposecellscloud-23.6/asposecellscloud/models/merged_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/merged_cells_response.py` & `asposecellscloud-23.6/asposecellscloud/models/merged_cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/multiple_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/multiple_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/multiple_filters.py` & `asposecellscloud-23.6/asposecellscloud/models/multiple_filters.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/name.py` & `asposecellscloud-23.6/asposecellscloud/models/name.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/name_response.py` & `asposecellscloud-23.6/asposecellscloud/models/name_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/names.py` & `asposecellscloud-23.6/asposecellscloud/models/names.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/names_response.py` & `asposecellscloud-23.6/asposecellscloud/models/names_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/negative_bar_format.py` & `asposecellscloud-23.6/asposecellscloud/models/negative_bar_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/object_exist.py` & `asposecellscloud-23.6/asposecellscloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ods_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/ods_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ole_object.py` & `asposecellscloud-23.6/asposecellscloud/models/ole_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ole_object_response.py` & `asposecellscloud-23.6/asposecellscloud/models/ole_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ole_objects.py` & `asposecellscloud-23.6/asposecellscloud/models/ole_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ole_objects_response.py` & `asposecellscloud-23.6/asposecellscloud/models/ole_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ooxml_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/ooxml_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/operate_object.py` & `asposecellscloud-23.6/asposecellscloud/models/operate_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/operate_object_position.py` & `asposecellscloud-23.6/asposecellscloud/models/operate_object_position.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_break_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/page_break_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_section.py` & `asposecellscloud-23.6/asposecellscloud/models/page_section.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_sections_response.py` & `asposecellscloud-23.6/asposecellscloud/models/page_sections_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_setup.py` & `asposecellscloud-23.6/asposecellscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_setup_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/page_setup_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/page_setup_response.py` & `asposecellscloud-23.6/asposecellscloud/models/page_setup_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/password_request.py` & `asposecellscloud-23.6/asposecellscloud/models/password_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/paste_options.py` & `asposecellscloud-23.6/asposecellscloud/models/paste_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pattern_fill.py` & `asposecellscloud-23.6/asposecellscloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pdf_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/pdf_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pdf_security_options.py` & `asposecellscloud-23.6/asposecellscloud/models/pdf_security_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pic_format_option.py` & `asposecellscloud-23.6/asposecellscloud/models/pic_format_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/picture.py` & `asposecellscloud-23.6/asposecellscloud/models/picture.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/picture_response.py` & `asposecellscloud-23.6/asposecellscloud/models/picture_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pictures.py` & `asposecellscloud-23.6/asposecellscloud/models/pictures.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pictures_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pictures_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_field.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_field.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_field_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_field_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_filter_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_filters_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_filters_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_item.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_table.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_field_request.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_table_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_table_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_table_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_tables.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_tables.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pivot_tables_response.py` & `asposecellscloud-23.6/asposecellscloud/models/pivot_tables_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/pptx_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/pptx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/protect_sheet_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/protect_sheet_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/range.py` & `asposecellscloud-23.6/asposecellscloud/models/range.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/range_copy_request.py` & `asposecellscloud-23.6/asposecellscloud/models/range_copy_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/range_set_outline_border_request.py` & `asposecellscloud-23.6/asposecellscloud/models/range_set_outline_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/range_set_style_request.py` & `asposecellscloud-23.6/asposecellscloud/models/range_set_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/range_value_response.py` & `asposecellscloud-23.6/asposecellscloud/models/range_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ranges.py` & `asposecellscloud-23.6/asposecellscloud/models/ranges.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/ranges_response.py` & `asposecellscloud-23.6/asposecellscloud/models/ranges_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/result_destination.py` & `asposecellscloud-23.6/asposecellscloud/models/result_destination.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/row.py` & `asposecellscloud-23.6/asposecellscloud/models/row.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/row_response.py` & `asposecellscloud-23.6/asposecellscloud/models/row_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/rows.py` & `asposecellscloud-23.6/asposecellscloud/models/rows.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/rows_response.py` & `asposecellscloud-23.6/asposecellscloud/models/rows_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/save_response.py` & `asposecellscloud-23.6/asposecellscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/save_result.py` & `asposecellscloud-23.6/asposecellscloud/models/save_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/save_result_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/save_result_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shadow_effect.py` & `asposecellscloud-23.6/asposecellscloud/models/shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shape.py` & `asposecellscloud-23.6/asposecellscloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shape_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/shape_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shape_response.py` & `asposecellscloud-23.6/asposecellscloud/models/shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shapes.py` & `asposecellscloud-23.6/asposecellscloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/shapes_response.py` & `asposecellscloud-23.6/asposecellscloud/models/shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/single_value.py` & `asposecellscloud-23.6/asposecellscloud/models/single_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/single_value_response.py` & `asposecellscloud-23.6/asposecellscloud/models/single_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/smart_marker_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/smart_marker_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/solid_fill.py` & `asposecellscloud-23.6/asposecellscloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sort_key.py` & `asposecellscloud-23.6/asposecellscloud/models/sort_key.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sparkline.py` & `asposecellscloud-23.6/asposecellscloud/models/sparkline.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sparkline_group.py` & `asposecellscloud-23.6/asposecellscloud/models/sparkline_group.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sparkline_group_response.py` & `asposecellscloud-23.6/asposecellscloud/models/sparkline_group_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sparkline_groups.py` & `asposecellscloud-23.6/asposecellscloud/models/sparkline_groups.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sparkline_groups_response.py` & `asposecellscloud-23.6/asposecellscloud/models/sparkline_groups_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/split_result.py` & `asposecellscloud-23.6/asposecellscloud/models/split_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/split_result_document.py` & `asposecellscloud-23.6/asposecellscloud/models/split_result_document.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/split_result_response.py` & `asposecellscloud-23.6/asposecellscloud/models/split_result_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/split_workbook_task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/split_workbook_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/spreadsheet_ml2003_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/spreadsheet_ml2003_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/sql_script_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/sql_script_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/storage_exist.py` & `asposecellscloud-23.6/asposecellscloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/storage_file.py` & `asposecellscloud-23.6/asposecellscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/style.py` & `asposecellscloud-23.6/asposecellscloud/models/style.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/style_response.py` & `asposecellscloud-23.6/asposecellscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/svg_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/svg_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/table_total_request.py` & `asposecellscloud-23.6/asposecellscloud/models/table_total_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/task_data.py` & `asposecellscloud-23.6/asposecellscloud/models/task_data.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/task_description.py` & `asposecellscloud-23.6/asposecellscloud/models/task_description.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/task_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/text_item.py` & `asposecellscloud-23.6/asposecellscloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/text_items.py` & `asposecellscloud-23.6/asposecellscloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/text_items_response.py` & `asposecellscloud-23.6/asposecellscloud/models/text_items_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/text_options.py` & `asposecellscloud-23.6/asposecellscloud/models/text_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/text_water_marker_request.py` & `asposecellscloud-23.6/asposecellscloud/models/text_water_marker_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/texture_fill.py` & `asposecellscloud-23.6/asposecellscloud/models/texture_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/theme_color.py` & `asposecellscloud-23.6/asposecellscloud/models/theme_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/tick_labels.py` & `asposecellscloud-23.6/asposecellscloud/models/tick_labels.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/tile_pic_option.py` & `asposecellscloud-23.6/asposecellscloud/models/tile_pic_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/title.py` & `asposecellscloud-23.6/asposecellscloud/models/title.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/title_response.py` & `asposecellscloud-23.6/asposecellscloud/models/title_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/top10.py` & `asposecellscloud-23.6/asposecellscloud/models/top10.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/top10_filter.py` & `asposecellscloud-23.6/asposecellscloud/models/top10_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/txt_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/txt_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/validation.py` & `asposecellscloud-23.6/asposecellscloud/models/validation.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/validation_response.py` & `asposecellscloud-23.6/asposecellscloud/models/validation_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/validations.py` & `asposecellscloud-23.6/asposecellscloud/models/validations.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/validations_response.py` & `asposecellscloud-23.6/asposecellscloud/models/validations_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/value_type.py` & `asposecellscloud-23.6/asposecellscloud/models/value_type.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_break.py` & `asposecellscloud-23.6/asposecellscloud/models/vertical_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_break_response.py` & `asposecellscloud-23.6/asposecellscloud/models/vertical_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_breaks.py` & `asposecellscloud-23.6/asposecellscloud/models/vertical_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/vertical_page_breaks_response.py` & `asposecellscloud-23.6/asposecellscloud/models/vertical_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_encryption_request.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_encryption_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_protection_request.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_protection_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_replace_response.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_response.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_settings_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/workbook_settings_response.py` & `asposecellscloud-23.6/asposecellscloud/models/workbook_settings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheet.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheet.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheet_moving_request.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheet_moving_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheet_operate_parameter.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheet_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheet_replace_response.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheet_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheet_response.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheet_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheets.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheets.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/worksheets_response.py` & `asposecellscloud-23.6/asposecellscloud/models/worksheets_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/xls_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/xls_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/xlsb_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/xlsb_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/models/xps_save_options.py` & `asposecellscloud-23.6/asposecellscloud/models/xps_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/__init__.py` & `asposecellscloud-23.6/asposecellscloud/requests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 from asposecellscloud.requests.post_worksheet_match_non_blanks_request import PostWorksheetMatchNonBlanksRequest
 from asposecellscloud.requests.post_worksheet_auto_filter_refresh_request import PostWorksheetAutoFilterRefreshRequest
 from asposecellscloud.requests.delete_worksheet_date_filter_request import DeleteWorksheetDateFilterRequest
 from asposecellscloud.requests.delete_worksheet_filter_request import DeleteWorksheetFilterRequest
 from asposecellscloud.requests.get_worksheet_autoshapes_request import GetWorksheetAutoshapesRequest
 from asposecellscloud.requests.get_worksheet_autoshape_with_format_request import GetWorksheetAutoshapeWithFormatRequest
 from asposecellscloud.requests.post_batch_convert_request import PostBatchConvertRequest
+from asposecellscloud.requests.post_batch_lock_request import PostBatchLockRequest
+from asposecellscloud.requests.post_batch_protect_request import PostBatchProtectRequest
+from asposecellscloud.requests.post_batch_split_request import PostBatchSplitRequest
+from asposecellscloud.requests.post_batch_unlock_request import PostBatchUnlockRequest
 from asposecellscloud.requests.get_extract_barcodes_request import GetExtractBarcodesRequest
 from asposecellscloud.requests.post_clear_contents_request import PostClearContentsRequest
 from asposecellscloud.requests.post_clear_formats_request import PostClearFormatsRequest
 from asposecellscloud.requests.post_update_worksheet_range_style_request import PostUpdateWorksheetRangeStyleRequest
 from asposecellscloud.requests.post_worksheet_merge_request import PostWorksheetMergeRequest
 from asposecellscloud.requests.post_worksheet_unmerge_request import PostWorksheetUnmergeRequest
 from asposecellscloud.requests.get_worksheet_cells_request import GetWorksheetCellsRequest
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/copy_file_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/copy_folder_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/create_folder_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_decrypt_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_decrypt_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_properties_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_property_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_document_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_file_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_folder_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_header_footer_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_horizontal_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_horizontal_page_breaks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_horizontal_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_metadata_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_pivot_table_field_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_un_protect_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_un_protect_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_unprotect_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_unprotect_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_vertical_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_vertical_page_breaks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_vertical_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_background_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_name_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_workbook_names_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_workbook_names_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_background_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_cells_range_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_cells_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_chart_legend_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_chart_title_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_clear_charts_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_clear_charts_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_comment_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_comments_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_comments_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_date_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_date_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_delete_chart_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_delete_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_hyperlink_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_list_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_list_objects_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_list_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_ole_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_ole_objects_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_ole_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_picture_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_picture_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pictures_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pictures_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_table_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_row_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_shapes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_shapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_validation_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheet_validations_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheet_validations_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/delete_worksheets_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/delete_worksheets_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/download_file_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_cell_html_string_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_cell_html_string_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_cells_cloud_service_status_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_cells_cloud_service_status_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_border_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_fill_format_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_fill_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_area_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_category_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_second_category_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_second_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_second_value_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_second_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_series_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_series_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_chart_value_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_chart_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_disc_usage_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_disc_usage_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_document_properties_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_document_property_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_extract_barcodes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_extract_barcodes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_file_versions_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_file_versions_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_files_list_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_footer_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_header_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_header_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_horizontal_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_horizontal_page_breaks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_horizontal_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_metadata_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_named_range_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_named_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_named_ranges_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_named_ranges_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_page_count_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_page_count_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_page_setup_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_pivot_table_field_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_vertical_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_vertical_page_breaks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_vertical_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_default_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_default_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_name_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_name_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_name_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_names_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_names_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_settings_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_settings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_workbook_text_items_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_workbook_text_items_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_auto_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_auto_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_autoshapes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_autoshapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_calculate_formula_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cell_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cell_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cells_range_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cells_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_cells_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_cells_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_legend_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_chart_title_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_charts_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_charts_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_column_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_column_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_comment_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_comments_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_comments_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_hyperlink_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_hyperlinks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_list_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_list_objects_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_list_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_merged_cell_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_merged_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_merged_cells_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_merged_cells_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_ole_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_ole_objects_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_ole_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_page_count_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_page_count_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_picture_with_format_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_picture_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pictures_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pictures_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_table_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_pivot_tables_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_pivot_tables_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_row_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_shapes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_shapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_sparkline_group_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_text_items_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_text_items_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_validation_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_validations_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_validations_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheet_with_format_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheet_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/get_worksheets_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/get_worksheets_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/move_file_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/move_folder_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/object_exists_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/object_exists_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_assemble_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_assemble_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_workbook_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_autofit_workbook_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_workbook_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_autofit_workbook_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_row_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_autofit_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_autofit_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_batch_convert_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_batch_convert_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_cell_calculate_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_cell_calculate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_cell_characters_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_cell_characters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_category_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_chart_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_second_category_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_chart_second_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_second_value_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_chart_second_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_series_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_chart_series_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_chart_value_axis_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_chart_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_contents_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_clear_contents_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_formats_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_clear_formats_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_clear_objects_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_clear_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_column_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_column_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_compress_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_compress_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_csv_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_csv_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_docx_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_docx_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_html_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_html_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_json_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_json_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_png_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_png_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_convert_workbook_to_sql_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_convert_workbook_to_sql_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_cell_into_cell_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_copy_cell_into_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_copy_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_copy_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_digital_signature_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_digital_signature_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_encrypt_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_encrypt_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_export_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_export_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_footer_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_group_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_group_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_group_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_group_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_header_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_header_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_hide_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_hide_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_hide_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_hide_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_import_data_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_import_data_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_import_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_import_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_merge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_metadata_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_move_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_move_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_page_setup_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_cell_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_field_move_to_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_field_move_to_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_protect_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_protect_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_protect_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_protect_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_rename_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_rename_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_replace_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_reverse_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_reverse_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_rotate_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_rotate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_row_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_row_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_run_task_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_run_task_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_search_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_set_cell_html_string_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_set_cell_html_string_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_set_cell_range_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_set_cell_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_set_worksheet_column_width_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_set_worksheet_column_width_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_split_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_unhide_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_unhide_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_unhide_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_unhide_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_unlock_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_unlock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_cell_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_ole_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_property_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_range_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_range_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_row_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_update_worksheet_zoom_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_update_worksheet_zoom_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_watermark_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_watermark_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_calculate_formula_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_export_xml_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_export_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_import_xml_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_import_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_name_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_save_as_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_save_as_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_settings_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_settings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_split_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbook_text_replace_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbook_text_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbooks_merge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbooks_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_workbooks_text_search_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_workbooks_text_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_calculate_formula_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cell_set_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cell_set_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_style_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_range_value_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_cells_ranges_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_cells_ranges_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_legend_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_chart_title_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_comment_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_group_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_group_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_hyperlink_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_hyperlink_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="PostWorkSheetHyperlinkRequest.cs">
+<copyright company="Aspose" file="PostWorksheetHyperlinkRequest.cs">
   Copyright (c) 2023 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_column_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_column_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_columns_total_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_columns_total_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_match_blanks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_match_blanks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_merge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_picture_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_picture_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="PostWorkSheetPictureRequest.cs">
+<copyright company="Aspose" file="PostWorksheetPictureRequest.cs">
   Copyright (c) 2023 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_range_sort_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_range_sort_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_sparkline_group_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_text_search_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_text_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_unmerge_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_unmerge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worksheet_validation_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/post_worsheet_text_replace_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/post_worsheet_text_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_active_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_active_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_add_new_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_add_new_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_change_visibility_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_change_visibility_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_convert_workbook_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_convert_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_document_property_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_document_property_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             select_header_content_type(['application/json'])
 
         if self._property is not None:
              body_params =self._property 
 
         # Authentication setting
         auth_settings = []
-        resource_path = "/cells/{name}/documentproperties/{propertyName}"
+        resource_path = "/cells/{name}/documentproperties"
         # path parameters
         if path_params:
             path_params = api_client.sanitize_for_serialization(path_params)
             path_params = api_client.parameters_to_tuples(path_params, collection_formats)
             for k, v in path_params:
                 # specified safe chars, encode everything
                 resource_path = resource_path.replace('{%s}' % k, quote(str(v), safe='/'))
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_document_protect_from_changes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_document_protect_from_changes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_horizontal_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_new_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_insert_new_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_columns_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_row_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_insert_worksheet_rows_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_insert_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_pivot_table_field_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_protect_worksheet_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_protect_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_vertical_page_break_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_background_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_workbook_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_create_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_workbook_create_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_name_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_workbook_water_marker_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_workbook_water_marker_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_add_chart_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_add_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_add_picture_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_add_picture_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_background_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_cells_range_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_cells_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_chart_legend_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_chart_title_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_color_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_color_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_comment_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_custom_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_custom_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_date_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_date_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_filter_top10_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_filter_top10_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_area_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_format_condition_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_format_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_freeze_panes_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_freeze_panes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_hyperlink_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_hyperlink_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="PutWorkSheetHyperlinkRequest.cs">
+<copyright company="Aspose" file="PutWorksheetHyperlinkRequest.cs">
   Copyright (c) 2023 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_icon_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_icon_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_list_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_ole_object_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_pivot_table_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_shape_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_sparkline_group_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/put_worksheet_validation_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/put_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/storage_exists_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/storage_exists_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/requests/upload_file_request.py` & `asposecellscloud-23.6/asposecellscloud/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/asposecellscloud/rest.py` & `asposecellscloud-23.6/asposecellscloud/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all 
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+ THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+ IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+ FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+ AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+ LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+ OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+ SOFTWARE.
+</summary>
 """
 
-
 from __future__ import absolute_import
 
 import io
 import json
 import ssl
 import certifi
 import logging
@@ -53,23 +54,24 @@
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """
         Returns a dictionary of the response headers.
         """
+        # return self.urllib3_response.getheaders()
         return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """
         Returns a given response header.
         """
+        # return self.urllib3_response.getheader(name, default)
         return self.urllib3_response.headers.get(name, default)
 
-
 class RESTClientObject(object):
 
     def __init__(self, pools_size=4, maxsize=4):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680
         # maxsize is the number of requests to host that are allowed in parallel
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud.egg-info/PKG-INFO` & `asposecellscloud-23.6/asposecellscloud.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asposecellscloud
-Version: 23.5.1
+Version: 23.6
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: aspose.cloud@aspose.com
 License: UNKNOWN
 Description: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Keywords: aspose,cells,cloud
```

### Comparing `asposecellscloud-23.5.1/asposecellscloud.egg-info/SOURCES.txt` & `asposecellscloud-23.6/asposecellscloud.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -26,145 +26,211 @@
 asposecellscloud/models/auto_shapes.py
 asposecellscloud/models/auto_shapes_response.py
 asposecellscloud/models/axis.py
 asposecellscloud/models/axis_response.py
 asposecellscloud/models/barcode_response.py
 asposecellscloud/models/barcode_response_list.py
 asposecellscloud/models/batch_convert_request.py
+asposecellscloud/models/batch_lock_request.py
+asposecellscloud/models/batch_protect_request.py
+asposecellscloud/models/batch_split_request.py
 asposecellscloud/models/border.py
+asposecellscloud/models/border_response.py
+asposecellscloud/models/button.py
+asposecellscloud/models/button_response.py
+asposecellscloud/models/calculate_formula_response.py
 asposecellscloud/models/calculation_options.py
 asposecellscloud/models/cell.py
 asposecellscloud/models/cell_area.py
 asposecellscloud/models/cell_response.py
 asposecellscloud/models/cell_value.py
 asposecellscloud/models/cells.py
 asposecellscloud/models/cells_cloud_file_info.py
+asposecellscloud/models/cells_cloud_file_info_response.py
 asposecellscloud/models/cells_cloud_response.py
 asposecellscloud/models/cells_color.py
 asposecellscloud/models/cells_document_properties.py
 asposecellscloud/models/cells_document_properties_response.py
 asposecellscloud/models/cells_document_property.py
 asposecellscloud/models/cells_document_property_response.py
+asposecellscloud/models/cells_drawing.py
+asposecellscloud/models/cells_drawing_response.py
 asposecellscloud/models/cells_error.py
 asposecellscloud/models/cells_object_operate_task_parameter.py
 asposecellscloud/models/cells_response.py
 asposecellscloud/models/chart.py
 asposecellscloud/models/chart_area.py
 asposecellscloud/models/chart_area_response.py
+asposecellscloud/models/chart_data_table.py
+asposecellscloud/models/chart_data_table_response.py
 asposecellscloud/models/chart_frame.py
 asposecellscloud/models/chart_operate_parameter.py
+asposecellscloud/models/chart_point.py
+asposecellscloud/models/chart_point_response.py
+asposecellscloud/models/chart_points.py
+asposecellscloud/models/chart_points_response.py
+asposecellscloud/models/chart_response.py
+asposecellscloud/models/chart_shape.py
 asposecellscloud/models/charts.py
 asposecellscloud/models/charts_response.py
+asposecellscloud/models/check_box.py
+asposecellscloud/models/check_box_response.py
 asposecellscloud/models/color.py
 asposecellscloud/models/color_filter.py
 asposecellscloud/models/color_filter_request.py
 asposecellscloud/models/color_scale.py
 asposecellscloud/models/column.py
 asposecellscloud/models/column_response.py
 asposecellscloud/models/columns.py
 asposecellscloud/models/columns_response.py
+asposecellscloud/models/combo_box.py
+asposecellscloud/models/combo_box_response.py
 asposecellscloud/models/comment.py
 asposecellscloud/models/comment_response.py
+asposecellscloud/models/comment_shape.py
+asposecellscloud/models/comment_shape_response.py
 asposecellscloud/models/comments.py
 asposecellscloud/models/comments_response.py
 asposecellscloud/models/conditional_formatting.py
 asposecellscloud/models/conditional_formatting_icon.py
 asposecellscloud/models/conditional_formatting_response.py
 asposecellscloud/models/conditional_formatting_value.py
 asposecellscloud/models/conditional_formattings.py
 asposecellscloud/models/conditional_formattings_response.py
+asposecellscloud/models/convert_parameter.py
 asposecellscloud/models/convert_task_parameter.py
 asposecellscloud/models/convert_worksheet_task_parameter.py
 asposecellscloud/models/copy_options.py
 asposecellscloud/models/create_pivot_table_request.py
+asposecellscloud/models/criteria_multiple_filter.py
 asposecellscloud/models/custom_filter.py
 asposecellscloud/models/custom_parser_config.py
 asposecellscloud/models/data_bar.py
 asposecellscloud/models/data_bar_border.py
+asposecellscloud/models/data_labels.py
+asposecellscloud/models/data_labels_response.py
 asposecellscloud/models/data_sorter.py
+asposecellscloud/models/date_time_group_item.py
 asposecellscloud/models/dif_save_options.py
 asposecellscloud/models/disc_usage.py
+asposecellscloud/models/display_unit_label.py
+asposecellscloud/models/display_unit_label_response.py
 asposecellscloud/models/docx_save_options.py
+asposecellscloud/models/drop_bars.py
+asposecellscloud/models/drop_bars_response.py
 asposecellscloud/models/dynamic_filter.py
+asposecellscloud/models/error.py
+asposecellscloud/models/error_bar.py
+asposecellscloud/models/error_bar_response.py
 asposecellscloud/models/error_details.py
 asposecellscloud/models/file_info.py
 asposecellscloud/models/file_source.py
 asposecellscloud/models/file_version.py
 asposecellscloud/models/file_versions.py
 asposecellscloud/models/files_list.py
 asposecellscloud/models/files_result.py
 asposecellscloud/models/files_upload_result.py
 asposecellscloud/models/fill_format.py
 asposecellscloud/models/fill_format_response.py
 asposecellscloud/models/filter_column.py
+asposecellscloud/models/find_response.py
+asposecellscloud/models/floor.py
+asposecellscloud/models/floor_response.py
 asposecellscloud/models/font.py
 asposecellscloud/models/font_setting.py
+asposecellscloud/models/form.py
+asposecellscloud/models/form_response.py
 asposecellscloud/models/format_condition.py
+asposecellscloud/models/forms.py
+asposecellscloud/models/forms_response.py
+asposecellscloud/models/formula_format_condition.py
+asposecellscloud/models/google_drive_storage_file.py
 asposecellscloud/models/gradient_fill.py
 asposecellscloud/models/gradient_fill_stop.py
+asposecellscloud/models/group_box.py
+asposecellscloud/models/group_box_response.py
+asposecellscloud/models/group_shape.py
 asposecellscloud/models/horizontal_page_break.py
 asposecellscloud/models/horizontal_page_break_response.py
 asposecellscloud/models/horizontal_page_breaks.py
 asposecellscloud/models/horizontal_page_breaks_response.py
 asposecellscloud/models/html_save_options.py
 asposecellscloud/models/hyperlink.py
 asposecellscloud/models/hyperlink_response.py
 asposecellscloud/models/hyperlinks.py
 asposecellscloud/models/hyperlinks_response.py
 asposecellscloud/models/icon_filter.py
 asposecellscloud/models/icon_set.py
 asposecellscloud/models/image_save_options.py
+asposecellscloud/models/import2_dimension_double_array_option.py
+asposecellscloud/models/import2_dimension_int_array_option.py
+asposecellscloud/models/import2_dimension_string_array_option.py
 asposecellscloud/models/import_batch_data_option.py
 asposecellscloud/models/import_csv_data_option.py
 asposecellscloud/models/import_data_task_parameter.py
 asposecellscloud/models/import_double_array_option.py
 asposecellscloud/models/import_int_array_option.py
 asposecellscloud/models/import_option.py
 asposecellscloud/models/import_picture_option.py
 asposecellscloud/models/import_position.py
 asposecellscloud/models/import_string_array_option.py
 asposecellscloud/models/import_xml_request.py
 asposecellscloud/models/json_save_options.py
+asposecellscloud/models/label.py
+asposecellscloud/models/label_response.py
 asposecellscloud/models/legend.py
+asposecellscloud/models/legend_entries.py
+asposecellscloud/models/legend_entries_response.py
+asposecellscloud/models/legend_entry.py
+asposecellscloud/models/legend_entry_response.py
 asposecellscloud/models/legend_response.py
 asposecellscloud/models/line.py
 asposecellscloud/models/line_format.py
 asposecellscloud/models/line_response.py
+asposecellscloud/models/line_shape.py
+asposecellscloud/models/line_shape_response.py
 asposecellscloud/models/link.py
 asposecellscloud/models/link_element.py
+asposecellscloud/models/list_box.py
+asposecellscloud/models/list_box_response.py
 asposecellscloud/models/list_column.py
 asposecellscloud/models/list_object.py
 asposecellscloud/models/list_object_operate_parameter.py
 asposecellscloud/models/list_object_response.py
 asposecellscloud/models/list_objects.py
 asposecellscloud/models/list_objects_response.py
+asposecellscloud/models/load_options.py
 asposecellscloud/models/m_html_save_options.py
 asposecellscloud/models/markdown_save_options.py
+asposecellscloud/models/marker.py
 asposecellscloud/models/match_condition_request.py
 asposecellscloud/models/merged_cell.py
 asposecellscloud/models/merged_cell_response.py
 asposecellscloud/models/merged_cells.py
 asposecellscloud/models/merged_cells_response.py
 asposecellscloud/models/multiple_filter.py
 asposecellscloud/models/multiple_filters.py
 asposecellscloud/models/name.py
 asposecellscloud/models/name_response.py
 asposecellscloud/models/names.py
 asposecellscloud/models/names_response.py
 asposecellscloud/models/negative_bar_format.py
 asposecellscloud/models/object_exist.py
+asposecellscloud/models/object_exists_extensions.py
 asposecellscloud/models/ods_save_options.py
 asposecellscloud/models/ole_object.py
 asposecellscloud/models/ole_object_response.py
 asposecellscloud/models/ole_objects.py
 asposecellscloud/models/ole_objects_response.py
 asposecellscloud/models/ooxml_save_options.py
 asposecellscloud/models/operate_object.py
 asposecellscloud/models/operate_object_position.py
 asposecellscloud/models/operate_parameter.py
+asposecellscloud/models/oval.py
+asposecellscloud/models/oval_response.py
 asposecellscloud/models/page_break_operate_parameter.py
 asposecellscloud/models/page_section.py
 asposecellscloud/models/page_sections_response.py
 asposecellscloud/models/page_setup.py
 asposecellscloud/models/page_setup_operate_parameter.py
 asposecellscloud/models/page_setup_response.py
 asposecellscloud/models/password_request.py
@@ -185,32 +251,47 @@
 asposecellscloud/models/pivot_item.py
 asposecellscloud/models/pivot_table.py
 asposecellscloud/models/pivot_table_field_request.py
 asposecellscloud/models/pivot_table_operate_parameter.py
 asposecellscloud/models/pivot_table_response.py
 asposecellscloud/models/pivot_tables.py
 asposecellscloud/models/pivot_tables_response.py
+asposecellscloud/models/plot_area.py
+asposecellscloud/models/plot_area_response.py
 asposecellscloud/models/pptx_save_options.py
 asposecellscloud/models/protect_sheet_parameter.py
+asposecellscloud/models/radio_button.py
+asposecellscloud/models/radio_button_response.py
 asposecellscloud/models/range.py
 asposecellscloud/models/range_copy_request.py
+asposecellscloud/models/range_response.py
 asposecellscloud/models/range_set_outline_border_request.py
 asposecellscloud/models/range_set_style_request.py
 asposecellscloud/models/range_value_response.py
 asposecellscloud/models/ranges.py
 asposecellscloud/models/ranges_response.py
+asposecellscloud/models/rectangle_shape.py
+asposecellscloud/models/rectangle_shape_response.py
 asposecellscloud/models/result_destination.py
 asposecellscloud/models/row.py
 asposecellscloud/models/row_response.py
 asposecellscloud/models/rows.py
 asposecellscloud/models/rows_response.py
+asposecellscloud/models/save_files_to_cloud_result.py
+asposecellscloud/models/save_files_to_cloud_result_response.py
 asposecellscloud/models/save_options.py
 asposecellscloud/models/save_response.py
 asposecellscloud/models/save_result.py
 asposecellscloud/models/save_result_task_parameter.py
+asposecellscloud/models/scroll_bar.py
+asposecellscloud/models/scroll_bar_response.py
+asposecellscloud/models/series.py
+asposecellscloud/models/series_items.py
+asposecellscloud/models/series_response.py
+asposecellscloud/models/serieses_response.py
 asposecellscloud/models/shadow_effect.py
 asposecellscloud/models/shape.py
 asposecellscloud/models/shape_operate_parameter.py
 asposecellscloud/models/shape_response.py
 asposecellscloud/models/shapes.py
 asposecellscloud/models/shapes_response.py
 asposecellscloud/models/single_value.py
@@ -219,61 +300,82 @@
 asposecellscloud/models/solid_fill.py
 asposecellscloud/models/sort_key.py
 asposecellscloud/models/sparkline.py
 asposecellscloud/models/sparkline_group.py
 asposecellscloud/models/sparkline_group_response.py
 asposecellscloud/models/sparkline_groups.py
 asposecellscloud/models/sparkline_groups_response.py
+asposecellscloud/models/spinner.py
+asposecellscloud/models/spinner_response.py
 asposecellscloud/models/split_result.py
 asposecellscloud/models/split_result_document.py
 asposecellscloud/models/split_result_response.py
 asposecellscloud/models/split_workbook_task_parameter.py
 asposecellscloud/models/spreadsheet_ml2003_save_options.py
 asposecellscloud/models/sql_script_save_options.py
 asposecellscloud/models/storage_exist.py
 asposecellscloud/models/storage_file.py
 asposecellscloud/models/style.py
+asposecellscloud/models/style_format_condition.py
 asposecellscloud/models/style_response.py
+asposecellscloud/models/styles.py
 asposecellscloud/models/svg_save_options.py
 asposecellscloud/models/table_total_request.py
 asposecellscloud/models/task_data.py
 asposecellscloud/models/task_description.py
 asposecellscloud/models/task_parameter.py
+asposecellscloud/models/task_result_parameter.py
+asposecellscloud/models/task_run_result.py
+asposecellscloud/models/task_run_result_response.py
+asposecellscloud/models/text_box.py
+asposecellscloud/models/text_box_response.py
+asposecellscloud/models/text_format_condition.py
 asposecellscloud/models/text_item.py
+asposecellscloud/models/text_item_response.py
 asposecellscloud/models/text_items.py
 asposecellscloud/models/text_items_response.py
 asposecellscloud/models/text_options.py
 asposecellscloud/models/text_water_marker_request.py
 asposecellscloud/models/texture_fill.py
 asposecellscloud/models/theme_color.py
 asposecellscloud/models/tick_labels.py
+asposecellscloud/models/tick_labels_response.py
 asposecellscloud/models/tile_pic_option.py
+asposecellscloud/models/time_period_format_condition.py
 asposecellscloud/models/title.py
 asposecellscloud/models/title_response.py
 asposecellscloud/models/top10.py
 asposecellscloud/models/top10_filter.py
+asposecellscloud/models/total_request.py
+asposecellscloud/models/trendline.py
+asposecellscloud/models/trendline_response.py
+asposecellscloud/models/trendlines.py
+asposecellscloud/models/trendlines_response.py
 asposecellscloud/models/txt_save_options.py
 asposecellscloud/models/validation.py
 asposecellscloud/models/validation_response.py
 asposecellscloud/models/validations.py
 asposecellscloud/models/validations_response.py
 asposecellscloud/models/value_type.py
 asposecellscloud/models/vertical_page_break.py
 asposecellscloud/models/vertical_page_break_response.py
 asposecellscloud/models/vertical_page_breaks.py
 asposecellscloud/models/vertical_page_breaks_response.py
+asposecellscloud/models/walls.py
+asposecellscloud/models/walls_response.py
 asposecellscloud/models/workbook.py
 asposecellscloud/models/workbook_encryption_request.py
 asposecellscloud/models/workbook_operate_parameter.py
 asposecellscloud/models/workbook_protection_request.py
 asposecellscloud/models/workbook_replace_response.py
 asposecellscloud/models/workbook_response.py
 asposecellscloud/models/workbook_settings.py
 asposecellscloud/models/workbook_settings_operate_parameter.py
 asposecellscloud/models/workbook_settings_response.py
+asposecellscloud/models/workbooks_response.py
 asposecellscloud/models/worksheet.py
 asposecellscloud/models/worksheet_moving_request.py
 asposecellscloud/models/worksheet_operate_parameter.py
 asposecellscloud/models/worksheet_replace_response.py
 asposecellscloud/models/worksheet_response.py
 asposecellscloud/models/worksheets.py
 asposecellscloud/models/worksheets_response.py
@@ -426,14 +528,18 @@
 asposecellscloud/requests/post_assemble_request.py
 asposecellscloud/requests/post_autofit_workbook_columns_request.py
 asposecellscloud/requests/post_autofit_workbook_rows_request.py
 asposecellscloud/requests/post_autofit_worksheet_columns_request.py
 asposecellscloud/requests/post_autofit_worksheet_row_request.py
 asposecellscloud/requests/post_autofit_worksheet_rows_request.py
 asposecellscloud/requests/post_batch_convert_request.py
+asposecellscloud/requests/post_batch_lock_request.py
+asposecellscloud/requests/post_batch_protect_request.py
+asposecellscloud/requests/post_batch_split_request.py
+asposecellscloud/requests/post_batch_unlock_request.py
 asposecellscloud/requests/post_cell_calculate_request.py
 asposecellscloud/requests/post_cell_characters_request.py
 asposecellscloud/requests/post_chart_category_axis_request.py
 asposecellscloud/requests/post_chart_second_category_axis_request.py
 asposecellscloud/requests/post_chart_second_value_axis_request.py
 asposecellscloud/requests/post_chart_series_axis_request.py
 asposecellscloud/requests/post_chart_value_axis_request.py
```

### Comparing `asposecellscloud-23.5.1/setup.py` & `asposecellscloud-23.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "asposecellscloud"
-VERSION = "23.5.1"
+VERSION = "23.6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `asposecellscloud-23.5.1/test/test_cells_chart_axis_api.py` & `asposecellscloud-23.6/test/test_cells_chart_axis_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_auto_filter_controller.py` & `asposecellscloud-23.6/test/tests_auto_filter_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_batch_controller.py` & `asposecellscloud-23.6/test/tests_xml_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,39 +14,52 @@
 from asposecellscloud.apis.cells_api import CellsApi
 import AuthUtil
 from asposecellscloud.models import *
 from asposecellscloud.requests import *
 
 global_api = None
 
-class TestBatchControllerApi(unittest.TestCase):
+class TestXmlControllerApi(unittest.TestCase):
     def setUp(self):
         warnings.simplefilter('ignore', ResourceWarning)
         global global_api
         if global_api is None:
            global_api = CellsApi(AuthUtil.GetClientId(),AuthUtil.GetClientSecret(),"v3.0",AuthUtil.GetBaseUrl())
         self.api = global_api
 
     def tearDown(self):
         pass
 
-    def test_post_batch_convert(self):
+    def test_post_workbook_export_xml(self):
         remote_folder = 'TestData/In'
 
-        local_book1 = 'Book1.xlsx'
-        remote_book1 = 'Book1.xlsx'
-        local_my_doc = 'myDocument.xlsx'
-        remote_my_doc = 'myDocument.xlsx'
-
-        batchConvertRequestMatchCondition = MatchConditionRequest(regex_pattern= '(^Book)(.+)(xlsx$)' )
-        batchConvertRequest = BatchConvertRequest(source_folder= remote_folder ,format= 'pdf' ,out_folder= 'TestResult' ,match_condition= batchConvertRequestMatchCondition )
-        result = AuthUtil.Ready(self.api, local_book1, remote_folder + '/' + remote_book1 ,  '')
+        local_name = 'Template.xlsx'
+        remote_name = 'Template.xlsx'
+
+        result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
+        self.assertTrue(len(result.uploaded)>0) 
+     
+        request =  PostWorkbookExportXMLRequest( remote_name,folder= remote_folder,storage_name= '')
+        self.api.post_workbook_export_xml(request)
+
+
+    def test_post_workbook_import_xml(self):
+        remote_folder = 'TestData/In'
+
+        local_name = 'Template.xlsx'
+        data_xml = 'data.xml'
+        remote_name = 'Template.xlsx'
+
+        importXMLRequestXMLFileSource = FileSource(file_source_type= 'CloudFileSystem' ,file_path= remote_folder + '/data.xml' )
+        importXMLRequestImportPosition = ImportPosition(sheet_name= 'Sheet1' ,row_index= 3 ,column_index= 4 )
+        importXMLRequest = ImportXMLRequest(xml_file_source= importXMLRequestXMLFileSource ,import_position= importXMLRequestImportPosition )
+        result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
-        result = AuthUtil.Ready(self.api, local_my_doc, remote_folder + '/' + remote_my_doc ,  '')
+        result = AuthUtil.Ready(self.api, data_xml, remote_folder + '/data.xml' ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  PostBatchConvertRequest( batchConvertRequest)
-        self.api.post_batch_convert(request)
+        request =  PostWorkbookImportXMLRequest( remote_name, import_xml_request =   importXMLRequest , folder= remote_folder,storage_name= '')
+        self.api.post_workbook_import_xml(request)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `asposecellscloud-23.5.1/test/tests_cells_barcodes_controller.py` & `asposecellscloud-23.6/test/tests_cells_barcodes_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_cells_controller.py` & `asposecellscloud-23.6/test/tests_cells_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_cells_status_controller.py` & `asposecellscloud-23.6/test/tests_cells_status_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_chart_area_controller.py` & `asposecellscloud-23.6/test/tests_chart_area_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_charts_controller.py` & `asposecellscloud-23.6/test/tests_charts_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_conditional_formattings_controller.py` & `asposecellscloud-23.6/test/tests_conditional_formattings_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_conversion.py` & `asposecellscloud-23.6/test/tests_conversion.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_conversion_json.py` & `asposecellscloud-23.6/test/tests_conversion_json.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_conversion_png.py` & `asposecellscloud-23.6/test/tests_conversion_png.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_file_controller.py` & `asposecellscloud-23.6/test/tests_file_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_folder_controller.py` & `asposecellscloud-23.6/test/tests_folder_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_hypelinks_controller.py` & `asposecellscloud-23.6/test/tests_hypelinks_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,66 +47,66 @@
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  GetWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
+        request =  GetWorksheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
         self.api.get_worksheet_hyperlink(request)
 
 
     def test_delete_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  DeleteWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
+        request =  DeleteWorksheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
         self.api.delete_worksheet_hyperlink(request)
 
 
     def test_post_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         hyperlink = Hyperlink(address= 'https://products.aspose.cloud/cells/' )
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  PostWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0, hyperlink,folder= remote_folder,storage_name= '')
+        request =  PostWorksheetHyperlinkRequest( remote_name, 'Sheet1', 0, hyperlink,folder= remote_folder,storage_name= '')
         self.api.post_worksheet_hyperlink(request)
 
 
     def test_put_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  PutWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 1, 1, 2, 3, 'https://products.aspose.cloud/cells/',folder= remote_folder,storage_name= '')
+        request =  PutWorksheetHyperlinkRequest( remote_name, 'Sheet1', 1, 1, 2, 3, 'https://products.aspose.cloud/cells/',folder= remote_folder,storage_name= '')
         self.api.put_worksheet_hyperlink(request)
 
 
     def test_delete_worksheet_hyperlinks(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  DeleteWorkSheetHyperlinksRequest( remote_name, 'Sheet1',folder= remote_folder,storage_name= '')
+        request =  DeleteWorksheetHyperlinksRequest( remote_name, 'Sheet1',folder= remote_folder,storage_name= '')
         self.api.delete_worksheet_hyperlinks(request)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `asposecellscloud-23.5.1/test/tests_light_cells.py` & `asposecellscloud-23.6/test/tests_light_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_list_objects_controller.py` & `asposecellscloud-23.6/test/tests_list_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_ole_objects_controller.py` & `asposecellscloud-23.6/test/tests_ole_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_one.py` & `asposecellscloud-23.6/test/tests_one.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_page_breaks_controller.py` & `asposecellscloud-23.6/test/tests_page_breaks_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_page_setup_controller.py` & `asposecellscloud-23.6/test/tests_page_setup_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_pictures_controller.py` & `asposecellscloud-23.6/test/tests_pictures_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         picture = Picture(left= 10 ,bottom= 10 )
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  PostWorkSheetPictureRequest( remote_name, 'Sheet6', 0, picture,folder= remote_folder,storage_name= '')
+        request =  PostWorksheetPictureRequest( remote_name, 'Sheet6', 0, picture,folder= remote_folder,storage_name= '')
         self.api.post_worksheet_picture(request)
 
 
     def test_delete_worksheet_picture(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
@@ -103,13 +103,13 @@
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  DeleteWorkSheetPicturesRequest( remote_name, 'Sheet6',folder= remote_folder,storage_name= '')
+        request =  DeleteWorksheetPicturesRequest( remote_name, 'Sheet6',folder= remote_folder,storage_name= '')
         self.api.delete_worksheet_pictures(request)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `asposecellscloud-23.5.1/test/tests_pivot_tables_controller.py` & `asposecellscloud-23.6/test/tests_pivot_tables_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_properties_controller.py` & `asposecellscloud-23.6/test/tests_properties_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_ranges_controller.py` & `asposecellscloud-23.6/test/tests_ranges_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_shapes_controller.py` & `asposecellscloud-23.6/test/tests_shapes_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_sparkline_groups_controller.py` & `asposecellscloud-23.6/test/tests_sparkline_groups_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_storage_controller.py` & `asposecellscloud-23.6/test/tests_storage_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_workbook_controller.py` & `asposecellscloud-23.6/test/tests_workbook_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_worksheet_controller.py` & `asposecellscloud-23.6/test/tests_worksheet_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.5.1/test/tests_worksheet_validations_controller.py` & `asposecellscloud-23.6/test/tests_worksheet_validations_controller.py`

 * *Files identical despite different names*

