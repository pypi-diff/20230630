# Comparing `tmp/semantha_sdk-5.4.1.tar.gz` & `tmp/semantha_sdk-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.4.1.tar", max compression
+gzip compressed data, was "semantha_sdk-5.5.0.tar", max compression
```

## Comparing `semantha_sdk-5.4.1.tar` & `semantha_sdk-5.5.0.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.4.1/LICENSE
--rw-r--r--   0        0        0     1618 2023-06-14 13:09:39.839325 semantha_sdk-5.4.1/pyproject.toml
--rw-r--r--   0        0        0    14233 2023-06-13 15:55:55.289520 semantha_sdk-5.4.1/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.4.1/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 09:26:15.293945 semantha_sdk-5.4.1/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-14 12:18:47.608000 semantha_sdk-5.4.1/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0      930 2023-06-14 12:18:47.195000 semantha_sdk-5.4.1/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      729 2023-06-14 12:18:47.208000 semantha_sdk-5.4.1/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      739 2023-06-14 12:18:47.375000 semantha_sdk-5.4.1/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1673 2023-06-14 12:18:47.266000 semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1493 2023-06-14 12:18:47.230000 semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3716 2023-06-14 12:18:47.333000 semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3423 2023-06-14 12:18:47.364000 semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1236 2023-06-14 12:18:47.422000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      832 2023-06-14 12:18:47.442000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1775 2023-06-14 12:18:47.431000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1622 2023-06-14 12:18:47.459000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2722 2023-06-14 12:18:47.413000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      726 2023-06-14 12:18:47.390000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1554 2023-06-14 12:18:47.471000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1553 2023-06-14 12:18:47.486000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1261 2023-06-14 12:18:47.500000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1156 2023-06-14 12:18:47.511000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1215 2023-06-14 12:18:47.523000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0      976 2023-06-14 12:18:47.451000 semantha_sdk-5.4.1/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     5667 2023-06-14 12:18:47.772000 semantha_sdk-5.4.1/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1050 2023-06-14 12:18:47.530000 semantha_sdk-5.4.1/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1369 2023-06-14 12:18:47.555000 semantha_sdk-5.4.1/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     2350 2023-06-14 12:18:47.626000 semantha_sdk-5.4.1/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1387 2023-06-14 12:18:47.650000 semantha_sdk-5.4.1/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1823 2023-06-14 12:18:47.636000 semantha_sdk-5.4.1/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3601 2023-06-14 12:18:47.669000 semantha_sdk-5.4.1/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     3497 2023-06-14 12:18:47.684000 semantha_sdk-5.4.1/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4424 2023-06-14 12:18:47.589000 semantha_sdk-5.4.1/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1013 2023-06-14 12:18:47.564000 semantha_sdk-5.4.1/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      791 2023-06-14 12:18:47.999000 semantha_sdk-5.4.1/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1648 2023-06-14 12:18:48.004000 semantha_sdk-5.4.1/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1529 2023-06-14 12:18:48.014000 semantha_sdk-5.4.1/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1278 2023-06-14 12:18:48.045000 semantha_sdk-5.4.1/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1754 2023-06-14 12:18:48.039000 semantha_sdk-5.4.1/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0      762 2023-06-14 12:18:48.018000 semantha_sdk-5.4.1/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     2070 2023-06-14 12:18:48.033000 semantha_sdk-5.4.1/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      706 2023-06-14 12:18:48.026000 semantha_sdk-5.4.1/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0      777 2023-06-14 12:18:48.100000 semantha_sdk-5.4.1/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      774 2023-06-14 12:18:48.106000 semantha_sdk-5.4.1/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1798 2023-06-14 12:18:48.053000 semantha_sdk-5.4.1/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1314 2023-06-14 12:18:48.063000 semantha_sdk-5.4.1/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0     1266 2023-06-14 12:18:48.077000 semantha_sdk-5.4.1/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1738 2023-06-14 12:18:48.069000 semantha_sdk-5.4.1/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1247 2023-06-14 12:18:48.094000 semantha_sdk-5.4.1/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1715 2023-06-14 12:18:48.085000 semantha_sdk-5.4.1/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1107 2023-06-14 12:18:47.694000 semantha_sdk-5.4.1/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     2315 2023-06-14 12:18:47.709000 semantha_sdk-5.4.1/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1546 2023-06-14 12:18:47.781000 semantha_sdk-5.4.1/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1494 2023-06-14 12:18:47.855000 semantha_sdk-5.4.1/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      682 2023-06-14 12:18:47.843000 semantha_sdk-5.4.1/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2074 2023-06-14 12:18:47.831000 semantha_sdk-5.4.1/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0     8930 2023-06-14 12:18:47.740000 semantha_sdk-5.4.1/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0     6565 2023-06-14 12:18:47.905000 semantha_sdk-5.4.1/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      789 2023-06-14 12:18:47.537000 semantha_sdk-5.4.1/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-06-14 09:26:15.420011 semantha_sdk-5.4.1/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-06-14 09:26:15.422010 semantha_sdk-5.4.1/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      836 2023-06-14 12:18:47.883000 semantha_sdk-5.4.1/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      676 2023-06-14 12:18:47.865000 semantha_sdk-5.4.1/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1379 2023-06-14 12:18:47.915000 semantha_sdk-5.4.1/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5389 2023-06-14 12:18:47.931000 semantha_sdk-5.4.1/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4015 2023-06-14 12:18:47.941000 semantha_sdk-5.4.1/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      844 2023-06-14 12:18:47.793000 semantha_sdk-5.4.1/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1217 2023-06-14 12:18:47.948000 semantha_sdk-5.4.1/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      840 2023-06-14 12:18:47.963000 semantha_sdk-5.4.1/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1115 2023-06-14 12:18:47.968000 semantha_sdk-5.4.1/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0      912 2023-06-14 12:18:47.955000 semantha_sdk-5.4.1/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1310 2023-06-14 12:18:47.994000 semantha_sdk-5.4.1/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     4351 2023-06-12 08:36:49.200000 semantha_sdk-5.4.1/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      607 2023-06-12 08:36:48.908000 semantha_sdk-5.4.1/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      654 2023-06-12 08:36:48.924000 semantha_sdk-5.4.1/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      556 2023-06-12 08:36:49.089000 semantha_sdk-5.4.1/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      535 2023-06-12 08:36:49.028000 semantha_sdk-5.4.1/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      546 2023-06-12 08:36:48.976000 semantha_sdk-5.4.1/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      930 2023-06-12 08:36:48.998000 semantha_sdk-5.4.1/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      508 2023-06-12 08:36:48.929000 semantha_sdk-5.4.1/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      672 2023-06-12 08:36:48.945000 semantha_sdk-5.4.1/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1139 2023-06-12 08:36:48.960000 semantha_sdk-5.4.1/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      516 2023-06-12 08:36:49.045000 semantha_sdk-5.4.1/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      604 2023-06-12 08:36:49.155000 semantha_sdk-5.4.1/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      476 2023-06-12 08:36:48.898000 semantha_sdk-5.4.1/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      519 2023-06-12 08:36:49.063000 semantha_sdk-5.4.1/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1213 2023-06-12 08:36:49.150000 semantha_sdk-5.4.1/semantha_sdk/model/document.py
--rw-r--r--   0        0        0      939 2023-06-12 08:36:48.878000 semantha_sdk-5.4.1/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      723 2023-06-12 08:36:49.110000 semantha_sdk-5.4.1/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      566 2023-06-12 08:36:49.130000 semantha_sdk-5.4.1/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      628 2023-06-12 08:36:48.972000 semantha_sdk-5.4.1/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1004 2023-06-12 08:36:48.940000 semantha_sdk-5.4.1/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      503 2023-06-12 08:36:48.835000 semantha_sdk-5.4.1/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      498 2023-06-12 08:36:48.903000 semantha_sdk-5.4.1/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      510 2023-06-12 08:36:48.926000 semantha_sdk-5.4.1/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      564 2023-06-12 08:36:48.989000 semantha_sdk-5.4.1/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      447 2023-06-12 08:36:49.116000 semantha_sdk-5.4.1/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      597 2023-06-12 08:36:48.943000 semantha_sdk-5.4.1/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      729 2023-06-12 08:36:49.053000 semantha_sdk-5.4.1/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      536 2023-06-12 08:36:49.081000 semantha_sdk-5.4.1/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      842 2023-06-12 08:36:49.041000 semantha_sdk-5.4.1/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      512 2023-06-12 08:36:49.059000 semantha_sdk-5.4.1/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      498 2023-06-12 08:36:49.031000 semantha_sdk-5.4.1/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      524 2023-06-12 08:36:49.068000 semantha_sdk-5.4.1/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      839 2023-06-12 08:36:49.103000 semantha_sdk-5.4.1/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      531 2023-06-12 08:36:48.852000 semantha_sdk-5.4.1/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      408 2023-06-12 08:36:48.984000 semantha_sdk-5.4.1/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      474 2023-06-12 08:36:48.896000 semantha_sdk-5.4.1/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      576 2023-06-12 08:36:48.953000 semantha_sdk-5.4.1/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      483 2023-06-12 08:36:48.932000 semantha_sdk-5.4.1/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      582 2023-06-12 08:36:48.841000 semantha_sdk-5.4.1/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      499 2023-06-12 08:36:49.056000 semantha_sdk-5.4.1/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      493 2023-06-12 08:36:48.892000 semantha_sdk-5.4.1/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      430 2023-06-12 08:36:48.888000 semantha_sdk-5.4.1/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      528 2023-06-12 08:36:49.077000 semantha_sdk-5.4.1/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1482 2023-06-12 08:36:48.919000 semantha_sdk-5.4.1/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      485 2023-06-12 08:36:49.025000 semantha_sdk-5.4.1/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      812 2023-06-12 08:36:48.865000 semantha_sdk-5.4.1/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      528 2023-06-12 08:36:49.083000 semantha_sdk-5.4.1/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0      948 2023-06-12 08:36:49.123000 semantha_sdk-5.4.1/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      486 2023-06-12 08:36:48.981000 semantha_sdk-5.4.1/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      493 2023-06-12 08:36:49.132000 semantha_sdk-5.4.1/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      577 2023-06-12 08:36:48.948000 semantha_sdk-5.4.1/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      445 2023-06-12 08:36:49.073000 semantha_sdk-5.4.1/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      775 2023-06-12 08:36:49.095000 semantha_sdk-5.4.1/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      728 2023-06-12 08:36:48.894000 semantha_sdk-5.4.1/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      646 2023-06-12 08:36:49.007000 semantha_sdk-5.4.1/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      500 2023-06-12 08:36:49.141000 semantha_sdk-5.4.1/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.4.1/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      873 2023-06-12 08:36:49.127000 semantha_sdk-5.4.1/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      518 2023-06-12 08:36:48.950000 semantha_sdk-5.4.1/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      792 2023-06-12 08:36:48.965000 semantha_sdk-5.4.1/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1669 2023-06-12 08:36:49.022000 semantha_sdk-5.4.1/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      454 2023-06-12 08:36:49.033000 semantha_sdk-5.4.1/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      695 2023-06-12 08:36:48.860000 semantha_sdk-5.4.1/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      851 2023-06-12 08:36:48.969000 semantha_sdk-5.4.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      608 2023-06-12 08:36:49.114000 semantha_sdk-5.4.1/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      480 2023-06-12 08:36:48.869000 semantha_sdk-5.4.1/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      542 2023-06-12 08:36:49.136000 semantha_sdk-5.4.1/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      446 2023-06-12 08:36:48.884000 semantha_sdk-5.4.1/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      565 2023-06-12 08:36:49.004000 semantha_sdk-5.4.1/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      462 2023-06-12 08:36:48.881000 semantha_sdk-5.4.1/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      464 2023-06-12 08:36:48.992000 semantha_sdk-5.4.1/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.4.1/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.4.1/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.4.1/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.4.1/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3607 2023-06-14 12:18:25.638176 semantha_sdk-5.4.1/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.4.1/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.4.1/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0    14791 1970-01-01 00:00:00.000000 semantha_sdk-5.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.5.0/LICENSE
+-rw-r--r--   0        0        0     1618 2023-06-30 08:53:09.443616 semantha_sdk-5.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14524 2023-06-30 08:52:57.695383 semantha_sdk-5.5.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.5.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 06:39:31.917641 semantha_sdk-5.5.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-30 06:26:01.750523 semantha_sdk-5.5.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0     1004 2023-06-30 06:26:01.700367 semantha_sdk-5.5.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      839 2023-06-30 06:26:01.701367 semantha_sdk-5.5.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      817 2023-06-30 06:26:01.724526 semantha_sdk-5.5.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1792 2023-06-30 06:26:01.717524 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1576 2023-06-30 06:26:01.706366 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3758 2023-06-30 06:26:01.721524 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3406 2023-06-30 06:26:01.723526 semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1346 2023-06-30 06:26:01.728526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      923 2023-06-30 06:26:01.732523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1913 2023-06-30 06:26:01.730523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1735 2023-06-30 06:26:01.734526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2785 2023-06-30 06:26:01.727526 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      836 2023-06-30 06:26:01.725524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1662 2023-06-30 06:26:01.736524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1661 2023-06-30 06:26:01.739524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1373 2023-06-30 06:26:01.741524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1261 2023-06-30 06:26:01.742523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1322 2023-06-30 06:26:01.743524 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1098 2023-06-30 06:26:01.733523 semantha_sdk-5.5.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     5664 2023-06-30 06:26:01.762533 semantha_sdk-5.5.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1168 2023-06-30 06:26:01.744523 semantha_sdk-5.5.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1425 2023-06-30 06:26:01.746524 semantha_sdk-5.5.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     2385 2023-06-30 06:26:01.751524 semantha_sdk-5.5.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1565 2023-06-30 06:26:01.753524 semantha_sdk-5.5.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1997 2023-06-30 06:26:01.752523 semantha_sdk-5.5.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3592 2023-06-30 06:26:01.754524 semantha_sdk-5.5.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     3521 2023-06-30 06:26:01.755523 semantha_sdk-5.5.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4497 2023-06-30 06:26:01.748524 semantha_sdk-5.5.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1157 2023-06-30 06:26:01.747523 semantha_sdk-5.5.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      905 2023-06-30 06:26:01.781038 semantha_sdk-5.5.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1757 2023-06-30 06:26:01.782036 semantha_sdk-5.5.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1595 2023-06-30 06:26:01.783035 semantha_sdk-5.5.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1460 2023-06-30 06:26:01.787039 semantha_sdk-5.5.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1924 2023-06-30 06:26:01.786035 semantha_sdk-5.5.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0      840 2023-06-30 06:26:01.783035 semantha_sdk-5.5.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     2186 2023-06-30 06:26:01.785036 semantha_sdk-5.5.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      816 2023-06-30 06:26:01.784036 semantha_sdk-5.5.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0      855 2023-06-30 06:26:01.793038 semantha_sdk-5.5.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      852 2023-06-30 06:26:01.793038 semantha_sdk-5.5.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1970 2023-06-30 06:26:01.788036 semantha_sdk-5.5.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1494 2023-06-30 06:26:01.789036 semantha_sdk-5.5.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0     1449 2023-06-30 06:26:01.790038 semantha_sdk-5.5.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1907 2023-06-30 06:26:01.790038 semantha_sdk-5.5.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1430 2023-06-30 06:26:01.792039 semantha_sdk-5.5.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1882 2023-06-30 06:26:01.791038 semantha_sdk-5.5.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1217 2023-06-30 06:26:01.756523 semantha_sdk-5.5.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     2361 2023-06-30 06:26:01.757528 semantha_sdk-5.5.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1663 2023-06-30 06:26:01.763535 semantha_sdk-5.5.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1711 2023-06-30 06:26:01.770527 semantha_sdk-5.5.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      792 2023-06-30 06:26:01.768528 semantha_sdk-5.5.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2267 2023-06-30 06:26:01.767527 semantha_sdk-5.5.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0     8885 2023-06-30 06:26:01.759528 semantha_sdk-5.5.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0     6394 2023-06-30 06:26:01.774030 semantha_sdk-5.5.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      867 2023-06-30 06:26:01.745528 semantha_sdk-5.5.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-06-29 06:39:31.918640 semantha_sdk-5.5.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-06-29 06:39:31.920640 semantha_sdk-5.5.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      967 2023-06-30 06:26:01.772524 semantha_sdk-5.5.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      786 2023-06-30 06:26:01.771524 semantha_sdk-5.5.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1497 2023-06-30 06:26:01.775039 semantha_sdk-5.5.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5217 2023-06-30 06:26:01.776039 semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4070 2023-06-30 06:26:01.777036 semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      963 2023-06-30 06:26:01.764535 semantha_sdk-5.5.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1207 2023-06-30 06:26:01.778036 semantha_sdk-5.5.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      931 2023-06-30 06:26:01.779036 semantha_sdk-5.5.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1285 2023-06-30 06:26:01.779036 semantha_sdk-5.5.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1018 2023-06-30 06:26:01.778036 semantha_sdk-5.5.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1383 2023-06-30 06:26:01.780037 semantha_sdk-5.5.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     4351 2023-06-30 06:26:01.959034 semantha_sdk-5.5.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-30 06:26:01.932037 semantha_sdk-5.5.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      689 2023-06-30 06:26:01.928039 semantha_sdk-5.5.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      582 2023-06-30 06:26:01.923037 semantha_sdk-5.5.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      546 2023-06-30 06:26:01.926041 semantha_sdk-5.5.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      579 2023-06-30 06:26:01.912036 semantha_sdk-5.5.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      991 2023-06-30 06:26:01.893036 semantha_sdk-5.5.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      513 2023-06-30 06:26:01.892037 semantha_sdk-5.5.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      719 2023-06-30 06:26:01.890038 semantha_sdk-5.5.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1209 2023-06-30 06:26:01.905040 semantha_sdk-5.5.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      543 2023-06-30 06:26:01.940037 semantha_sdk-5.5.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      639 2023-06-30 06:26:01.895035 semantha_sdk-5.5.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      481 2023-06-30 06:26:01.918040 semantha_sdk-5.5.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      530 2023-06-30 06:26:01.885036 semantha_sdk-5.5.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1306 2023-06-30 06:26:01.904036 semantha_sdk-5.5.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1004 2023-06-30 06:26:01.936036 semantha_sdk-5.5.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      771 2023-06-30 06:26:01.940037 semantha_sdk-5.5.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      580 2023-06-30 06:26:01.941037 semantha_sdk-5.5.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      660 2023-06-30 06:26:01.939037 semantha_sdk-5.5.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1078 2023-06-30 06:26:01.910038 semantha_sdk-5.5.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      508 2023-06-30 06:26:01.922037 semantha_sdk-5.5.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      503 2023-06-30 06:26:01.945037 semantha_sdk-5.5.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      533 2023-06-30 06:26:01.942037 semantha_sdk-5.5.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      577 2023-06-30 06:26:01.911036 semantha_sdk-5.5.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      452 2023-06-30 06:26:01.937036 semantha_sdk-5.5.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      606 2023-06-30 06:26:01.906036 semantha_sdk-5.5.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      757 2023-06-30 06:26:01.930035 semantha_sdk-5.5.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      544 2023-06-30 06:26:01.920037 semantha_sdk-5.5.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      882 2023-06-30 06:26:01.938036 semantha_sdk-5.5.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      520 2023-06-30 06:26:01.889038 semantha_sdk-5.5.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      506 2023-06-30 06:26:01.933037 semantha_sdk-5.5.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      538 2023-06-30 06:26:01.917037 semantha_sdk-5.5.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      891 2023-06-30 06:26:01.900035 semantha_sdk-5.5.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      545 2023-06-30 06:26:01.895035 semantha_sdk-5.5.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      413 2023-06-30 06:26:01.944037 semantha_sdk-5.5.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      476 2023-06-30 06:26:01.882036 semantha_sdk-5.5.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      602 2023-06-30 06:26:01.908037 semantha_sdk-5.5.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      488 2023-06-30 06:26:01.898038 semantha_sdk-5.5.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      611 2023-06-30 06:26:01.883037 semantha_sdk-5.5.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      507 2023-06-30 06:26:01.909037 semantha_sdk-5.5.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      504 2023-06-30 06:26:01.929036 semantha_sdk-5.5.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      435 2023-06-30 06:26:01.919036 semantha_sdk-5.5.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      555 2023-06-30 06:26:01.891036 semantha_sdk-5.5.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1577 2023-06-30 07:31:02.968921 semantha_sdk-5.5.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      493 2023-06-30 06:26:01.923037 semantha_sdk-5.5.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      850 2023-06-30 06:26:01.930035 semantha_sdk-5.5.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      551 2023-06-30 06:26:01.886036 semantha_sdk-5.5.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1027 2023-06-30 06:26:01.931037 semantha_sdk-5.5.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      491 2023-06-30 06:26:01.925036 semantha_sdk-5.5.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      536 2023-06-30 06:26:01.942037 semantha_sdk-5.5.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      587 2023-06-30 06:26:01.926041 semantha_sdk-5.5.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      459 2023-06-30 06:26:01.943035 semantha_sdk-5.5.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      829 2023-06-30 06:26:01.907036 semantha_sdk-5.5.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      756 2023-06-30 06:26:01.901036 semantha_sdk-5.5.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      716 2023-06-30 06:26:01.934036 semantha_sdk-5.5.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      523 2023-06-30 06:26:01.902036 semantha_sdk-5.5.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      650 2023-06-29 06:39:31.921661 semantha_sdk-5.5.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      911 2023-06-30 06:26:01.921036 semantha_sdk-5.5.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      523 2023-06-30 06:26:01.881034 semantha_sdk-5.5.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      834 2023-06-30 06:26:01.888035 semantha_sdk-5.5.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1755 2023-06-30 06:26:01.894036 semantha_sdk-5.5.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      462 2023-06-30 06:26:01.907036 semantha_sdk-5.5.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      704 2023-06-30 06:26:01.935037 semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      892 2023-06-30 06:26:01.914037 semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      640 2023-06-30 06:26:01.913036 semantha_sdk-5.5.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      488 2023-06-30 06:26:01.903038 semantha_sdk-5.5.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      575 2023-06-30 06:26:01.915037 semantha_sdk-5.5.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      448 2023-06-30 06:26:01.937036 semantha_sdk-5.5.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      572 2023-06-30 06:26:01.888035 semantha_sdk-5.5.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      467 2023-06-30 06:26:01.916036 semantha_sdk-5.5.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      469 2023-06-30 06:26:01.914037 semantha_sdk-5.5.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.5.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.5.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.5.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.5.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3712 2023-06-20 12:43:00.735650 semantha_sdk-5.5.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.5.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.5.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    15077 1970-01-01 00:00:00.000000 semantha_sdk-5.5.0/PKG-INFO
```

### Comparing `semantha_sdk-5.4.1/LICENSE` & `semantha_sdk-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/pyproject.toml` & `semantha_sdk-5.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.4.1"
+version = "5.5.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
@@ -27,15 +27,15 @@
 requests = "2.31.0"
 marshmallow = "3.19.0"
 marshmallow-dataclass = "8.5.14"
 pyhumps = "3.8.0"
 
 [tool.poetry.group.unittest.dependencies]
 coverage = "7.2.7"
-pytest = "7.3.1"
+pytest = "7.4.0"
 pytest-cov = "4.1.0"
 toml = "0.10.2"
 parameterized = "^0.9.0"
 
 [tool.poetry.group.build.dependencies]
 pip-licenses = "4.3.2"
```

### Comparing `semantha_sdk-5.4.1/README.md` & `semantha_sdk-5.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
+### Version 5.5.0
+Removed language parameter on **/api/domains/{domainname}/references**
+Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
+Fixed return of binary responses of bulk services.
+
 ### Version 5.4.0
 Added **new** service: 
 - **/api/domains/{domainname}/summarizations** which generations a summarization for a given list of texts and a given topic.
 
 Added support for **existing** services: 
 - /api/model/domains/{domainname}/boostwords/{id}
 - /api/model/domains/{domainname}/namedentities
@@ -122,15 +127,15 @@
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
     - [x] **POST** -> None
@@ -169,69 +174,69 @@
 - [x] **/domains/{domainname}/answers** -> AnswersEndpoint
     - [x] **POST** -> Answer
 - [x] **/domains/{domainname}/documentannotations** -> DocumentannotationsEndpoint
     - [x] **POST** -> IOBase
 - [x] **/domains/{domainname}/documentclasses** -> DocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> DocumentClass
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
     - [x] **POST** -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
     - [x] **POST** -> List[DocumentInformation]
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
 - [x] **/domains/{domainname}/referencedocuments/statistic** -> StatisticEndpoint
     - [x] **GET** -> Statistic
 - [x] **/domains/{domainname}/referencedocuments/{documentid}** -> ReferencedocumentEndpoint
     - [x] **GET** -> Document
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PATCH** -> Paragraph
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
-    - [x] **POST** -> Any
+    - [x] **POST** -> str
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/validation** -> ValidationEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/info** -> InfoEndpoint
     - [x] **GET** -> Info
 - [x] **/languages** -> LanguagesEndpoint
     - [x] **POST** -> LanguageDetection
 - [x] **/model** -> ModelEndpoint
@@ -242,18 +247,18 @@
     - [x] **GET** -> IOBase
     - [x] **PATCH** -> IOBase
 - [ ] **/model/domains/{domainname}/attributes** 
 - [ ] **/model/domains/{domainname}/backups** 
 - [x] **/model/domains/{domainname}/boostwords** -> ModelBoostwordsEndpoint
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> BoostWord
 - [ ] **/model/domains/{domainname}/classes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
 - [ ] **/model/domains/{domainname}/dataproperties** 
@@ -268,40 +273,40 @@
 - [ ] **/model/domains/{domainname}/instances** 
 - [ ] **/model/domains/{domainname}/instances/{id}** 
 - [ ] **/model/domains/{domainname}/metadata** 
 - [ ] **/model/domains/{domainname}/metadata/{id}** 
 - [x] **/model/domains/{domainname}/namedentities** -> ModelNamedentitiesEndpoint
     - [x] **GET** -> List[NamedEntity]
     - [x] **POST** -> NamedEntity
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/namedentities/{id}** -> ModelNamedentityEndpoint
     - [x] **GET** -> NamedEntity
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> NamedEntity
 - [ ] **/model/domains/{domainname}/objectproperties** 
 - [ ] **/model/domains/{domainname}/regexes** 
 - [ ] **/model/domains/{domainname}/regexes/{id}** 
 - [ ] **/model/domains/{domainname}/relations** 
 - [ ] **/model/domains/{domainname}/relations/{id}** 
 - [ ] **/model/domains/{domainname}/rulefunctions** 
 - [ ] **/model/domains/{domainname}/rules** 
 - [ ] **/model/domains/{domainname}/rules/{id}** 
 - [x] **/model/domains/{domainname}/stopwords** -> ModelStopwordsEndpoint
     - [x] **GET** -> List[StopWord]
     - [x] **POST** -> StopWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/stopwords/{id}** -> ModelStopwordEndpoint
     - [x] **GET** -> StopWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> StopWord
 - [x] **/model/domains/{domainname}/synonyms** -> ModelSynonymsEndpoint
     - [x] **GET** -> List[Synonym]
     - [x] **POST** -> Synonym
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/synonyms/{id}** -> ModelSynonymEndpoint
     - [x] **GET** -> Synonym
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> Synonym
 - [x] **/model/extractortypes** -> ModelExtractortypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/metadatatypes** -> ModelMetadatatypesEndpoint
     - [x] **GET** -> List[str]
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/__init__.py` & `semantha_sdk-5.5.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/answers.py` & `semantha_sdk-5.5.0/semantha_sdk/api/answers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.answer import Answer, AnswerSchema
+from semantha_sdk.model.answer import Answer
+from semantha_sdk.model.answer import AnswerSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class AnswersEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/answers"
 
-    def post(self
-        , question: str = None
-        , maxreferences: int = None
-        , similaritythreshold: float = None
-        ) -> Answer:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        question: str = None,
+        maxreferences: int = None,
+        similaritythreshold: float = None,
+    ) -> Answer:
         """
         
         Args:
-            question (str): 
-            maxreferences (int): Maximum number of returned results.
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            
+        question (str): 
+    maxreferences (int): Maximum number of returned results.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "question": question,
                 "maxreferences": maxreferences,
-                "similaritythreshold": similaritythreshold
+                "similaritythreshold": similaritythreshold,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(AnswerSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulk.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from semantha_sdk.api.bulk_domains import BulkDomainsEndpoint
 from semantha_sdk.api.bulk_model import BulkModelEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/bulk"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-
         self.__domains = BulkDomainsEndpoint(session, self._endpoint)
         self.__model = BulkModelEndpoint(session, self._endpoint)
 
-
     @property
     def domains(self) -> BulkDomainsEndpoint:
         return self.__domains
-
-
     @property
     def model(self) -> BulkModelEndpoint:
         return self.__model
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulk_domains.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from semantha_sdk.api.bulkdomains_domain import BulkdomainsDomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkDomainsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/domains"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
 
-
-
-    def __call__(self, domainname: str) -> BulkdomainsDomainEndpoint:
+    def __call__(
+            self,
+            domainname: str,
+    ) -> BulkdomainsDomainEndpoint:
         return BulkdomainsDomainEndpoint(self._session, self._endpoint, domainname)
 
-
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulk_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from semantha_sdk.api.bulkmodel_domains import BulkmodelDomainsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkModelEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/model"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-
         self.__domains = BulkmodelDomainsEndpoint(session, self._endpoint)
 
-
     @property
     def domains(self) -> BulkmodelDomainsEndpoint:
         return self.__domains
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_class_bulk import DocumentClassBulk, DocumentClassBulkSchema
+from semantha_sdk.model.document_class_bulk import DocumentClassBulk
+from semantha_sdk.model.document_class_bulk import DocumentClassBulkSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkdomainsDocumentclassesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/documentclasses"
 
-    def get(self
-        ) -> List[DocumentClassBulk]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[DocumentClassBulk]:
         """
         Get all document classes
-        This is the quiet version of  'get /api/domains/{domainname}/documentclasses' 
+            This is the quiet version of  'get /api/domains/{domainname}/documentclasses'
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassBulkSchema)
 
-    def post(self
-        , body: List[DocumentClassBulk] = None
-        ) -> None:
+    def post(
+        self,
+        body: List[DocumentClassBulk] = None,
+    ) -> None:
         """
         Create one or more document classes
-        This is the quiet version of  'post /api/domains/{domainname}/documentclasses'
+            This is the quiet version of  'post /api/domains/{domainname}/documentclasses'
         Args:
-            body (List[DocumentClassBulk]): 
-            
+        body (List[DocumentClassBulk]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=DocumentClassBulkSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from semantha_sdk.api.bulkdomains_documentclasses import BulkdomainsDocumentclassesEndpoint
 from semantha_sdk.api.bulkdomains_referencedocuments import BulkdomainsReferencedocumentsEndpoint
 from semantha_sdk.api.bulkdomains_references import BulkdomainsReferencesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkdomainsDomainEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._domainname}"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        domainname: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-        self._domainname=domainname
+        self._domainname = domainname
         self.__documentclasses = BulkdomainsDocumentclassesEndpoint(session, self._endpoint)
         self.__referencedocuments = BulkdomainsReferencedocumentsEndpoint(session, self._endpoint)
         self.__references = BulkdomainsReferencesEndpoint(session, self._endpoint)
 
-
     @property
     def documentclasses(self) -> BulkdomainsDocumentclassesEndpoint:
         return self.__documentclasses
-
-
     @property
     def referencedocuments(self) -> BulkdomainsReferencedocumentsEndpoint:
         return self.__referencedocuments
-
-
     @property
     def references(self) -> BulkdomainsReferencesEndpoint:
         return self.__references
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkdomainsReferencedocumentsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/referencedocuments"
 
-    def get(self
-        ) -> List[Document]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[Document]:
         """
         Get all reference documents
-        This is the quiet version of  'get /api/domains/{domainname}/referencedocuments' 
+            This is the quiet version of  'get /api/domains/{domainname}/referencedocuments'
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentSchema)
 
-    def post(self
-        , name: str = None
-        , tags: str = None
-        , metadata: str = None
-        , file: IOBase = None
-        , text: str = None
-        , documenttype: str = None
-        , color: str = None
-        , comment: str = None
-        , documentclass: str = None
-        , addparagraphsasdocuments: bool = None
-        , detectlanguage: bool = None
-        ) -> None:
+    def post(
+        self,
+        name: str = None,
+        tags: str = None,
+        metadata: str = None,
+        file: IOBase = None,
+        text: str = None,
+        documenttype: str = None,
+        color: str = None,
+        comment: str = None,
+        documentclass: str = None,
+        addparagraphsasdocuments: bool = None,
+        detectlanguage: bool = None,
+    ) -> None:
         """
         Upload reference document
-        This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
+            This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
         Args:
-            name (str): The document name in your library (in contrast to the file name being used during upload).
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            metadata (str): Filter by metadata
-            file (IOBase): Input document (left document).
-            text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
-            comment (str): Use this parameter to add a comment to your reference document.
-            documentclass (str): 
-            addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
-            
+        name (str): The document name in your library (in contrast to the file name being used during upload).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    metadata (str): Filter by metadata
+    file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
+    comment (str): Use this parameter to add a comment to your reference document.
+    documentclass (str): 
+    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
         """
         q_params = {}
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "name": name,
                 "tags": tags,
                 "metadata": metadata,
                 "file": file,
                 "text": text,
                 "documenttype": documenttype,
                 "color": color,
                 "comment": comment,
                 "documentclass": documentclass,
-                "addparagraphsasdocuments": addparagraphsasdocuments
+                "addparagraphsasdocuments": addparagraphsasdocuments,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def delete(self, body: List[str]) -> None:
+    
+    def delete(
+        self,
+        body: List[str],
+    ) -> None:
         """
         
         """
-        self._session.delete(url=self._endpoint, json=body).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
+        self._session.delete(
+            url=self._endpoint,
+            json=body
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkdomainsReferencesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/references"
 
-    def post(self
-        , body: List[Document] = None
-        , referencedocumentids: str = None
-        , tags: str = None
-        , documentclassids: str = None
-        , similaritythreshold: float = None
-        , synonymousthreshold: float = None
-        , marknomatch: bool = None
-        , withreferencetext: bool = None
-        , withareas: bool = None
-        , language: str = None
-        , mode: str = None
-        , detectlanguage: bool = None
-        , maxreferences: int = None
-        , withcontext: bool = None
-        , considertexttype: bool = None
-        , resizeparagraphs: bool = None
-        ) -> List[Document]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        body: List[Document] = None,
+        referencedocumentids: str = None,
+        tags: str = None,
+        documentclassids: str = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+        withareas: bool = None,
+        mode: str = None,
+        detectlanguage: bool = None,
+        maxreferences: int = None,
+        withcontext: bool = None,
+        considertexttype: bool = None,
+        resizeparagraphs: bool = None,
+    ) -> List[Document]:
         """
         Determine references with several input documents
-        Matches several input documents ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
+            Matches several input documents ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
         Args:
-            body (List[Document]): 
-            
+        body (List[Document]): 
         """
         q_params = {}
         if referencedocumentids is not None:
             q_params["referencedocumentids"] = referencedocumentids
         if tags is not None:
             q_params["tags"] = tags
         if documentclassids is not None:
@@ -50,16 +58,14 @@
             q_params["synonymousthreshold"] = synonymousthreshold
         if marknomatch is not None:
             q_params["marknomatch"] = marknomatch
         if withreferencetext is not None:
             q_params["withreferencetext"] = withreferencetext
         if withareas is not None:
             q_params["withareas"] = withareas
-        if language is not None:
-            q_params["language"] = language
         if mode is not None:
             q_params["mode"] = mode
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         if maxreferences is not None:
             q_params["maxreferences"] = maxreferences
         if withcontext is not None:
@@ -72,12 +78,10 @@
             url=self._endpoint,
             json=DocumentSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.boost_word import BoostWord, BoostWordSchema
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkmodelBoostwordsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/boostwords"
 
-    def post(self
-        , body: List[BoostWord] = None
-        ) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        body: List[BoostWord] = None,
+    ) -> None:
         """
         Create one or more boostwords
-        This is the quiet version of  'post /api/domains/{domainname}/boostwords'
+            This is the quiet version of  'post /api/domains/{domainname}/boostwords'
         Args:
-            body (List[BoostWord]): 
-            
+        body (List[BoostWord]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=BoostWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from semantha_sdk.api.bulkmodelclass_instances import BulkmodelclassInstancesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkmodelClassEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._classid}"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str, classid: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        classid: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-        self._classid=classid
+        self._classid = classid
         self.__instances = BulkmodelclassInstancesEndpoint(session, self._endpoint)
 
-
     @property
     def instances(self) -> BulkmodelclassInstancesEndpoint:
         return self.__instances
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.5.0/semantha_sdk/api/validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,47 @@
-from semantha_sdk.api.bulkmodel_class import BulkmodelClassEndpoint
+from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.class_bulk import ClassBulk, ClassBulkSchema
+from semantha_sdk.model.semantic_model import SemanticModel
+from semantha_sdk.model.semantic_model import SemanticModelSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
-from typing import List
 
-
-class BulkmodelClassesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ValidationEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/classes"
+        return self._parent_endpoint + "/validation"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> List[ClassBulk]:
-        """
-        Get all classes
-        This is the quiet version of  'get /api/domains/{domainname}/classes' 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(ClassBulkSchema)
 
-    def post(self
-        , body: List[ClassBulk] = None
-        ) -> None:
+    
+    def post(
+        self,
+        file: IOBase = None,
+    ) -> SemanticModel:
         """
-        Create one or more classes
-        This is the quiet version of  'post /api/domains/{domainname}/classes'
+        Validate existing data in a document
+            The coordinates come back, if data is found
         Args:
-            body (List[ClassBulk]): 
-            
+        file (IOBase): Input document (left document).
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=ClassBulkSchema().dump(body),
+            body={
+                "file": file,
+            },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.as_none()
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, classid: str) -> BulkmodelClassEndpoint:
-        return BulkmodelClassEndpoint(self._session, self._endpoint, classid)
-
+        return response.to(SemanticModelSchema)
 
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.data_property import DataProperty, DataPropertySchema
+from semantha_sdk.model.data_property import DataProperty
+from semantha_sdk.model.data_property import DataPropertySchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkmodelDatapropertiesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/dataproperties"
 
-    def get(self
-        ) -> List[DataProperty]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[DataProperty]:
         """
         Get all dataproperties
-        This is the quiet version of  'get /api/domains/{domainname}/dataproperties' 
+            This is the quiet version of  'get /api/domains/{domainname}/dataproperties'
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DataPropertySchema)
 
-    def post(self
-        , body: List[DataProperty] = None
-        ) -> None:
+    def post(
+        self,
+        body: List[DataProperty] = None,
+    ) -> None:
         """
         Create one or more dataproperties
-        This is the quiet version of  'post /api/domains/{domainname}/dataproperties'
+            This is the quiet version of  'post /api/domains/{domainname}/dataproperties'
         Args:
-            body (List[DataProperty]): 
-            
+        body (List[DataProperty]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=DataPropertySchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,68 +5,61 @@
 from semantha_sdk.api.bulkmodel_metadata import BulkmodelMetadataEndpoint
 from semantha_sdk.api.bulkmodel_namedentities import BulkmodelNamedentitiesEndpoint
 from semantha_sdk.api.bulkmodel_stopwords import BulkmodelStopwordsEndpoint
 from semantha_sdk.api.bulkmodel_synonyms import BulkmodelSynonymsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkmodelDomainEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._domainname}"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        domainname: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-        self._domainname=domainname
+        self._domainname = domainname
         self.__boostwords = BulkmodelBoostwordsEndpoint(session, self._endpoint)
         self.__classes = BulkmodelClassesEndpoint(session, self._endpoint)
         self.__dataproperties = BulkmodelDatapropertiesEndpoint(session, self._endpoint)
         self.__instances = BulkmodelInstancesEndpoint(session, self._endpoint)
         self.__metadata = BulkmodelMetadataEndpoint(session, self._endpoint)
         self.__namedentities = BulkmodelNamedentitiesEndpoint(session, self._endpoint)
         self.__stopwords = BulkmodelStopwordsEndpoint(session, self._endpoint)
         self.__synonyms = BulkmodelSynonymsEndpoint(session, self._endpoint)
 
-
     @property
     def boostwords(self) -> BulkmodelBoostwordsEndpoint:
         return self.__boostwords
-
-
     @property
     def classes(self) -> BulkmodelClassesEndpoint:
         return self.__classes
-
-
     @property
     def dataproperties(self) -> BulkmodelDatapropertiesEndpoint:
         return self.__dataproperties
-
-
     @property
     def instances(self) -> BulkmodelInstancesEndpoint:
         return self.__instances
-
-
     @property
     def metadata(self) -> BulkmodelMetadataEndpoint:
         return self.__metadata
-
-
     @property
     def namedentities(self) -> BulkmodelNamedentitiesEndpoint:
         return self.__namedentities
-
-
     @property
     def stopwords(self) -> BulkmodelStopwordsEndpoint:
         return self.__stopwords
-
-
     @property
     def synonyms(self) -> BulkmodelSynonymsEndpoint:
         return self.__synonyms
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from semantha_sdk.api.bulkmodel_domain import BulkmodelDomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class BulkmodelDomainsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/domains"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
 
-
-
-    def __call__(self, domainname: str) -> BulkmodelDomainEndpoint:
+    def __call__(
+            self,
+            domainname: str,
+    ) -> BulkmodelDomainEndpoint:
         return BulkmodelDomainEndpoint(self._session, self._endpoint, domainname)
 
-
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.instance import Instance, InstanceSchema
+from semantha_sdk.model.instance import Instance
+from semantha_sdk.model.instance import InstanceSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkmodelInstancesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/instances"
 
-    def get(self
-        ) -> List[Instance]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[Instance]:
         """
         Get all instances
-        This is the quiet version of  'get /api/domains/{domainname}/instances' 
+            This is the quiet version of  'get /api/domains/{domainname}/instances'
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(InstanceSchema)
 
-    def post(self
-        , body: List[Instance] = None
-        ) -> None:
+    def post(
+        self,
+        body: List[Instance] = None,
+    ) -> None:
         """
         Create an instance
-        This is the quiet version of 'post /api/model/domains/{domainname}/instances'
+            This is the quiet version of 'post /api/model/domains/{domainname}/instances'
         Args:
-            body (List[Instance]): 
-            
+        body (List[Instance]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=InstanceSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,62 @@
+from semantha_sdk.api.bulkmodel_class import BulkmodelClassEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.metadata import Metadata, MetadataSchema
+from semantha_sdk.model.class_bulk import ClassBulk
+from semantha_sdk.model.class_bulk import ClassBulkSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class BulkmodelMetadataEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class BulkmodelClassesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/metadata"
+        return self._parent_endpoint + "/classes"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> List[Metadata]:
+    def __call__(
+            self,
+            classid: str,
+    ) -> BulkmodelClassEndpoint:
+        return BulkmodelClassEndpoint(self._session, self._endpoint, classid)
+
+    def get(
+        self,
+    ) -> List[ClassBulk]:
         """
-        Get all metadata
-        This is the quiet version of  'get /api/domains/{domainname}/metadata' 
+        Get all classes
+            This is the quiet version of  'get /api/domains/{domainname}/classes'
         Args:
-            
-        """
+            """
         q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(MetadataSchema)
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ClassBulkSchema)
 
-    def post(self
-        , body: List[Metadata] = None
-        ) -> None:
+    def post(
+        self,
+        body: List[ClassBulk] = None,
+    ) -> None:
         """
-        Create one or more metadata
-        This is the quiet version of  'post /api/domains/{domainname}/metadata'
+        Create one or more classes
+            This is the quiet version of  'post /api/domains/{domainname}/classes'
         Args:
-            body (List[Metadata]): 
-            
+        body (List[ClassBulk]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=MetadataSchema().dump(body),
+            json=ClassBulkSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.5.0/semantha_sdk/api/roles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.named_entity import NamedEntity, NamedEntitySchema
-from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class BulkmodelNamedentitiesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class RolesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/namedentities"
+        return self._parent_endpoint + "/roles"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def post(self
-        , body: List[NamedEntity] = None
-        ) -> None:
+
+    def get(
+        self,
+    ) -> List[str]:
         """
-        Create one or more named entities
-        This is the quiet version of  'post /api/domains/{domainname}/namedentities'
+        Get the role/s of the current user/s of a specific domain
         Args:
-            body (List[NamedEntity]): 
-            
-        """
+            """
         q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=NamedEntitySchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.stop_word import StopWord, StopWordSchema
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkmodelStopwordsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/stopwords"
 
-    def post(self
-        , body: List[StopWord] = None
-        ) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        body: List[StopWord] = None,
+    ) -> None:
         """
         Add a list of stop words to your domain
         Args:
-            body (List[StopWord]): 
-            
+        body (List[StopWord]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=StopWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.synonym import Synonym, SynonymSchema
+from semantha_sdk.model.named_entity import NamedEntity
+from semantha_sdk.model.named_entity import NamedEntitySchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class BulkmodelSynonymsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class BulkmodelNamedentitiesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/synonyms"
+        return self._parent_endpoint + "/namedentities"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
 
-    def post(self
-        , body: List[Synonym] = None
-        ) -> None:
+    
+    def post(
+        self,
+        body: List[NamedEntity] = None,
+    ) -> None:
         """
-        Create one or more synonyms
-        This is the quiet version of  'post /api/domains/{domainname}/synonyms'
+        Create one or more named entities
+            This is the quiet version of  'post /api/domains/{domainname}/namedentities'
         Args:
-            body (List[Synonym]): 
-            
+        body (List[NamedEntity]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=SynonymSchema().dump(body),
+            json=NamedEntitySchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.instance import Instance, InstanceSchema
+from semantha_sdk.model.instance import Instance
+from semantha_sdk.model.instance import InstanceSchema
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class BulkmodelclassInstancesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/instances"
 
-    def get(self
-        ) -> List[Instance]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[Instance]:
         """
         Get all instances of the classes by class id
-        This is the quiet version of 'get /api/model/domains/{domainname}/classes/{id}/instances' 
+            This is the quiet version of 'get /api/model/domains/{domainname}/classes/{id}/instances'
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(InstanceSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/clusters.py` & `semantha_sdk-5.5.0/semantha_sdk/api/clusters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.smart_cluster_response_container import SmartClusterResponseContainer, SmartClusterResponseContainerSchema
-from semantha_sdk.model.smart_cluster_semi_supervised_request import SmartClusterSemiSupervisedRequest, SmartClusterSemiSupervisedRequestSchema
+from semantha_sdk.model.smart_cluster_response_container import SmartClusterResponseContainer
+from semantha_sdk.model.smart_cluster_response_container import SmartClusterResponseContainerSchema
+from semantha_sdk.model.smart_cluster_semi_supervised_request import SmartClusterSemiSupervisedRequest
+from semantha_sdk.model.smart_cluster_semi_supervised_request import SmartClusterSemiSupervisedRequestSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ClustersEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/clusters"
 
-    def get(self
-        , documentids: str = None
-        , name: str = None
-        , createdafter: int = None
-        , createdbefore: int = None
-        , updatedafter: int = None
-        , updatedbefore: int = None
-        , tags: str = None
-        , documentclassids: str = None
-        , withoutdocumentclass: bool = None
-        , mincharacters: int = None
-        , metadata: str = None
-        , comment: str = None
-        , minclustersize: str = None
-        , clusteringstructure: str = None
-        , reduceoutliers: bool = None
-        , range: str = None
-        , neighbors: int = None
-        ) -> SmartClusterResponseContainer:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+        documentids: str = None,
+        name: str = None,
+        createdafter: int = None,
+        createdbefore: int = None,
+        updatedafter: int = None,
+        updatedbefore: int = None,
+        tags: str = None,
+        documentclassids: str = None,
+        withoutdocumentclass: bool = None,
+        mincharacters: int = None,
+        metadata: str = None,
+        comment: str = None,
+        minclustersize: str = None,
+        clusteringstructure: str = None,
+        reduceoutliers: bool = None,
+        range: str = None,
+        neighbors: int = None,
+    ) -> SmartClusterResponseContainer:
         """
-        Clusters reference documents based on their semantic content and provides labels for each cluster 
+        Clusters reference documents based on their semantic content and provides labels for each cluster
         Args:
-            documentids (str): List of document Ids for target. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            name (str): The document name in your library (in contrast to the file name being used during upload).
-            createdafter (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
-            createdbefore (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
-            updatedafter (int): 
-            updatedbefore (int): 
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            documentclassids (str): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            withoutdocumentclass (bool): Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
-            mincharacters (int): 
-            metadata (str): Filter by metadata
-            comment (str): Use this parameter to add a comment to your reference document.
-            minclustersize (str): Determines the size of the cluster, values are LOW, MEDIUM, HIGH
-            clusteringstructure (str): Determines how clusters are created, values are LOCAL, BALANCED, GLOBAL
-            reduceoutliers (bool): Boolean to try to reduce outlier on clustering
-            range (str): Use for topic over time clustering, values are HOURS, DAYS, MONTHS, YEARS
-            neighbors (int): 
-            
+        documentids str: List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    name str: The document name in your library (in contrast to the file name being used during upload).
+    createdafter int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
+    createdbefore int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
+    updatedafter int: 
+    updatedbefore int: 
+    tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    withoutdocumentclass bool: Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
+    mincharacters int: 
+    metadata str: Filter by metadata
+    comment str: Use this parameter to add a comment to your reference document.
+    minclustersize str: Determines the size of the cluster, values are LOW, MEDIUM, HIGH
+    clusteringstructure str: Determines how clusters are created, values are LOCAL, BALANCED, GLOBAL
+    reduceoutliers bool: Boolean to try to reduce outlier on clustering
+    range str: Use for topic over time clustering, values are HOURS, DAYS, MONTHS, YEARS
+    neighbors int: 
         """
         q_params = {}
         if documentids is not None:
             q_params["documentids"] = documentids
         if name is not None:
             q_params["name"] = name
         if createdafter is not None:
@@ -86,23 +95,24 @@
             q_params["clusteringstructure"] = clusteringstructure
         if reduceoutliers is not None:
             q_params["reduceoutliers"] = reduceoutliers
         if range is not None:
             q_params["range"] = range
         if neighbors is not None:
             q_params["neighbors"] = neighbors
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(SmartClusterResponseContainerSchema)
 
-    def put(self, smartclustersemisupervisedrequest: SmartClusterSemiSupervisedRequest) -> SmartClusterResponseContainer:
+    
+    
+    
+    def put(
+        self,
+        body: SmartClusterSemiSupervisedRequest
+    ) -> SmartClusterResponseContainer:
         """
         
         """
         return self._session.put(
             url=self._endpoint,
-            json=SmartClusterSemiSupervisedRequestSchema().dump(smartclustersemisupervisedrequest)
+            json=SmartClusterSemiSupervisedRequestSchema().dump(body)
         ).execute().to(SmartClusterResponseContainerSchema)
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.5.0/semantha_sdk/api/currentuser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from semantha_sdk.api.roles import RolesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.current_user import CurrentUser, CurrentUserSchema
+from semantha_sdk.model.current_user import CurrentUser
+from semantha_sdk.model.current_user import CurrentUserSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class CurrentuserEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/currentuser"
 
-    def get(self
-        ) -> CurrentUser:
-        """
-        Get the current user of a specific domain 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(CurrentUserSchema)
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-
         self.__roles = RolesEndpoint(session, self._endpoint)
 
-
     @property
     def roles(self) -> RolesEndpoint:
         return self.__roles
 
+    def get(
+        self,
+    ) -> CurrentUser:
+        """
+        Get the current user of a specific domain
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(CurrentUserSchema)
+
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/diff.py` & `semantha_sdk-5.5.0/semantha_sdk/api/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.difference import Difference, DifferenceSchema
+from semantha_sdk.model.difference import Difference
+from semantha_sdk.model.difference import DifferenceSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class DiffEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/diff"
 
-    def post(self
-        , left: str = None
-        , right: str = None
-        ) -> List[Difference]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        left: str = None,
+        right: str = None,
+    ) -> List[Difference]:
         """
         Create diff on structural basis
         Args:
-            left (str): The base for creating a diff
-            right (str): The changed text which gets compared to „left“ text.
-            
+        left (str): The base for creating a diff
+    right (str): The changed text which gets compared to „left“ text.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "left": left,
-                "right": right
+                "right": right,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DifferenceSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.5.0/semantha_sdk/api/documentannotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class DocumentannotationsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/documentannotations"
 
-    def post(self
-        , file: IOBase = None
-        , document: Document = None
-        , similaritythreshold: float = None
-        , synonymousthreshold: float = None
-        , marknomatch: bool = None
-        , withreferencetext: bool = None
-        ) -> IOBase:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        document: Document = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+    ) -> IOBase:
         """
         Download the original input document with the referenced document/library matches as annotated comments
         Args:
-            file (IOBase): Input document (left document).
-            document (Document): 
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            synonymousthreshold (float): Threshold for good matches.
-            marknomatch (bool): Marks the paragraphs that have not matched
-            withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
-            
+        file (IOBase): Input document (left document).
+    document (Document): 
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "document": document,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
-                "withreferencetext": withreferencetext
+                "withreferencetext": withreferencetext,
             },
-            
             headers=RestClient.to_header(MediaType.XLSX),
             q_params=q_params
         ).execute()
-        return response
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
+        return response.as_bytesio()
 
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.5.0/semantha_sdk/api/documentclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_class import DocumentClass, DocumentClassSchema
+from semantha_sdk.model.document_class import DocumentClass
+from semantha_sdk.model.document_class import DocumentClassSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class DocumentclassEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
 
-    def get(self
-        ) -> DocumentClass:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id = id
+
+
+    def get(
+        self,
+    ) -> DocumentClass:
         """
-        Get a class identified by id and all its subclasses 
+        Get a class identified by id and all its subclasses
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassSchema)
 
-    def put(self, documentclass: DocumentClass) -> DocumentClass:
+    
+    
+    def delete(
+        self,
+    ) -> None:
         """
-        Rename a document class identified by its id
+        Delete a document class identified by id
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=DocumentClassSchema().dump(documentclass)
-        ).execute().to(DocumentClassSchema)
+        ).execute()
 
-
-    def delete(self) -> None:
+    def put(
+        self,
+        body: DocumentClass
+    ) -> DocumentClass:
         """
-        Delete a document class identified by id
+        Rename a document class identified by its id
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
-
+        return self._session.put(
+            url=self._endpoint,
+            json=DocumentClassSchema().dump(body)
+        ).execute().to(DocumentClassSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.5.0/semantha_sdk/api/documentclasses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 from semantha_sdk.api.documentclass import DocumentclassEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_class import DocumentClass, DocumentClassSchema
+from semantha_sdk.model.document_class import DocumentClass
+from semantha_sdk.model.document_class import DocumentClassSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class DocumentclassesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/documentclasses"
 
-    def get(self
-        ) -> List[DocumentClass]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def __call__(
+            self,
+            id: str,
+    ) -> DocumentclassEndpoint:
+        return DocumentclassEndpoint(self._session, self._endpoint, id)
+
+    def get(
+        self,
+    ) -> List[DocumentClass]:
         """
-        Get all document classes 
+        Get all document classes
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassSchema)
 
-    def post(self
-        , body: DocumentClass = None
-        ) -> DocumentClass:
+    def post(
+        self,
+        body: DocumentClass = None,
+    ) -> DocumentClass:
         """
         Create one or more document classes
         Args:
-            body (DocumentClass): 
-            
+        body (DocumentClass): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=DocumentClassSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentClassSchema)
 
-
-    def delete(self) -> None:
+    
+    def delete(
+        self,
+    ) -> None:
         """
         Delete all document classes
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, id: str) -> DocumentclassEndpoint:
-        return DocumentclassEndpoint(self._session, self._endpoint, id)
-
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.5.0/semantha_sdk/api/documentcomparisons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_meta_data import DocumentMetaData, DocumentMetaDataSchema
+from semantha_sdk.model.document_meta_data import DocumentMetaData
+from semantha_sdk.model.document_meta_data import DocumentMetaDataSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class DocumentcomparisonsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/documentcomparisons"
 
-    def post(self
-        , file: IOBase = None
-        , referencedocument: IOBase = None
-        , similaritythreshold: float = None
-        , synonymousthreshold: float = None
-        , marknomatch: bool = None
-        , withreferencetext: bool = None
-        , documenttype: str = None
-        , metadata: List[DocumentMetaData] = None
-        , withcontext: bool = None
-        , considertexttype: bool = None
-        , resizeparagraphs: bool = None
-        , xlsxlegalstandard: bool = None
-        ) -> IOBase:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        referencedocument: IOBase = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+        documenttype: str = None,
+        metadata: List[DocumentMetaData] = None,
+        withcontext: bool = None,
+        considertexttype: bool = None,
+        resizeparagraphs: bool = None,
+        xlsxlegalstandard: bool = None,
+    ) -> IOBase:
         """
         Determine references (for temporary data)
         Args:
-            file (IOBase): Input document (left document).
-            referencedocument (IOBase): Reference document(s) to be used instead of the documents in the domain's library.
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            synonymousthreshold (float): Threshold for good matches.
-            marknomatch (bool): Marks the paragraphs that have not matched
-            withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            metadata (List[DocumentMetaData]): Filter by metadata
-            withcontext (bool): Creates and saves the context.
-            considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-            resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
-            xlsxlegalstandard (bool): 
-            
+        file (IOBase): Input document (left document).
+    referencedocument (IOBase): Reference document(s) to be used instead of the documents in the domain's library.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    metadata (List[DocumentMetaData]): Filter by metadata
+    withcontext (bool): Creates and saves the context.
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+    resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
+    xlsxlegalstandard (bool): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "referencedocument": referencedocument,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
                 "withreferencetext": withreferencetext,
                 "documenttype": documenttype,
                 "metadata": metadata,
                 "withcontext": withcontext,
                 "considertexttype": considertexttype,
                 "resizeparagraphs": resizeparagraphs,
-                "xlsxlegalstandard": xlsxlegalstandard
+                "xlsxlegalstandard": xlsxlegalstandard,
             },
-            
             headers=RestClient.to_header(MediaType.XLSX),
             q_params=q_params
         ).execute()
-        return response
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
+        return response.as_bytesio()
 
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/documents.py` & `semantha_sdk-5.5.0/semantha_sdk/api/documents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class DocumentsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/documents"
 
-    def post(self
-        , file: IOBase = None
-        , text: str = None
-        , type: str = None
-        , documenttype: str = None
-        , withareas: bool = None
-        , withcontext: bool = None
-        , mode: str = None
-        , withparagraphtype: bool = None
-        ) -> List[Document]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        withcontext: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> List[Document]:
         """
         Create a document model
         Args:
-            file (IOBase): Input document (left document).
-            text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-            type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            withareas (bool): Gives back the coordinates of referenced area.
-            withcontext (bool): Creates and saves the context.
-            mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
-        fingerprint: semantic search based on sentences; 
-        keyword: keyword: search based on sentences; 
-        document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
-        document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
-        fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-        Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-            withparagraphtype (bool): The type of the paragraph, for example heading, text
-            
+        file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
+    withcontext (bool): Creates and saves the context.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "text": text,
                 "type": type,
                 "documenttype": documenttype,
                 "withareas": withareas,
                 "withcontext": withcontext,
                 "mode": mode,
-                "withparagraphtype": withparagraphtype
+                "withparagraphtype": withparagraphtype,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/domain.py` & `semantha_sdk-5.5.0/semantha_sdk/api/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,33 @@
 from semantha_sdk.api.references import ReferencesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.settings import SettingsEndpoint
 from semantha_sdk.api.similaritymatrix import SimilaritymatrixEndpoint
 from semantha_sdk.api.summarizations import SummarizationsEndpoint
 from semantha_sdk.api.tags import TagsEndpoint
 from semantha_sdk.api.validation import ValidationEndpoint
-from semantha_sdk.model.domain import Domain, DomainSchema
+from semantha_sdk.model.domain import Domain
+from semantha_sdk.model.domain import DomainSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class DomainEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._domainname}"
 
-    def get(self
-        ) -> Domain:
-        """
-        Get the configuration settings of a specific domain 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(DomainSchema)
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        domainname: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-        self._domainname=domainname
+        self._domainname = domainname
         self.__answers = AnswersEndpoint(session, self._endpoint)
         self.__documentannotations = DocumentannotationsEndpoint(session, self._endpoint)
         self.__documentclasses = DocumentclassesEndpoint(session, self._endpoint)
         self.__documentcomparisons = DocumentcomparisonsEndpoint(session, self._endpoint)
         self.__documents = DocumentsEndpoint(session, self._endpoint)
         self.__modelclasses = ModelclassesEndpoint(session, self._endpoint)
         self.__modelinstances = ModelinstancesEndpoint(session, self._endpoint)
@@ -49,77 +43,65 @@
         self.__references = ReferencesEndpoint(session, self._endpoint)
         self.__settings = SettingsEndpoint(session, self._endpoint)
         self.__similaritymatrix = SimilaritymatrixEndpoint(session, self._endpoint)
         self.__summarizations = SummarizationsEndpoint(session, self._endpoint)
         self.__tags = TagsEndpoint(session, self._endpoint)
         self.__validation = ValidationEndpoint(session, self._endpoint)
 
-
     @property
     def answers(self) -> AnswersEndpoint:
         return self.__answers
-
-
     @property
     def documentannotations(self) -> DocumentannotationsEndpoint:
         return self.__documentannotations
-
-
     @property
     def documentclasses(self) -> DocumentclassesEndpoint:
         return self.__documentclasses
-
-
     @property
     def documentcomparisons(self) -> DocumentcomparisonsEndpoint:
         return self.__documentcomparisons
-
-
     @property
     def documents(self) -> DocumentsEndpoint:
         return self.__documents
-
-
     @property
     def modelclasses(self) -> ModelclassesEndpoint:
         return self.__modelclasses
-
-
     @property
     def modelinstances(self) -> ModelinstancesEndpoint:
         return self.__modelinstances
-
-
     @property
     def referencedocuments(self) -> ReferencedocumentsEndpoint:
         return self.__referencedocuments
-
-
     @property
     def references(self) -> ReferencesEndpoint:
         return self.__references
-
-
     @property
     def settings(self) -> SettingsEndpoint:
         return self.__settings
-
-
     @property
     def similaritymatrix(self) -> SimilaritymatrixEndpoint:
         return self.__similaritymatrix
-
-
     @property
     def summarizations(self) -> SummarizationsEndpoint:
         return self.__summarizations
-
-
     @property
     def tags(self) -> TagsEndpoint:
         return self.__tags
-
-
     @property
     def validation(self) -> ValidationEndpoint:
         return self.__validation
 
+    def get(
+        self,
+    ) -> Domain:
+        """
+        Get the configuration settings of a specific domain
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(DomainSchema)
+
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/domains.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_boostword.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,56 @@
-from semantha_sdk.api.domain import DomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.domain import Domain, DomainSchema
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import RestClient
-from typing import List
 
-
-class DomainsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelBoostwordEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/domains"
-
-    def get(self
-        ) -> List[Domain]:
-        """
-        Get all domains 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(DomainSchema)
+        return self._parent_endpoint + f"/{self._id}"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
+        self._id = id
 
 
+    def get(
+        self,
+    ) -> BoostWord:
+        """
+        Get a boostword by id
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(BoostWordSchema)
 
-    def __call__(self, domainname: str) -> DomainEndpoint:
-        return DomainEndpoint(self._session, self._endpoint, domainname)
-
-
+    
+    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete a boostword by id
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
+    def put(
+        self,
+        body: BoostWord
+    ) -> BoostWord:
+        """
+        Update a boostword by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=BoostWordSchema().dump(body)
+        ).execute().to(BoostWordSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/info.py` & `semantha_sdk-5.5.0/semantha_sdk/api/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.info import Info, InfoSchema
+from semantha_sdk.model.info import Info
+from semantha_sdk.model.info import InfoSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class InfoEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/info"
 
-    def get(self
-        ) -> Info:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> Info:
         """
-        Returns API version information. 
+        Returns API version information.
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(InfoSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/languages.py` & `semantha_sdk-5.5.0/semantha_sdk/api/languages.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.language_detection import LanguageDetection, LanguageDetectionSchema
+from semantha_sdk.model.language_detection import LanguageDetection
+from semantha_sdk.model.language_detection import LanguageDetectionSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class LanguagesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/languages"
 
-    def post(self
-        , file: IOBase = None
-        ) -> LanguageDetection:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+    ) -> LanguageDetection:
         """
         Identifies the language of the document and sends it back
-        Input: Support of all input formats (PDF, Docx, Text, JSON (DocumentModel)
-        
-        Output: Detected Language
-        
-        Supported Languages:
-        
-        "ar“, "cs", "da", "de", "en", "es", "el", "fr", "fi", "hu", "hr",
-        "it", "ja", "ko", "nl", "no", "pl", "pt", "ro", "ru", "sk", "sl",
-        "sv", "tr", "zh-CN"
+            Input: Support of all input formats (PDF, Docx, Text, JSON (DocumentModel)
+            
+            Output: Detected Language
+            
+            Supported Languages:
+            
+            "ar“, "cs", "da", "de", "en", "es", "el", "fr", "fi", "hu", "hr",
+            "it", "ja", "ko", "nl", "no", "pl", "pt", "ro", "ru", "sk", "sl",
+            "sv", "tr", "zh-CN"
         Args:
-            file (IOBase): Input document (left document).
-            
+        file (IOBase): Input document (left document).
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
-                "file": file
+                "file": file,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(LanguageDetectionSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from semantha_sdk.api.model_datatypes import ModelDatatypesEndpoint
 from semantha_sdk.api.model_domains import ModelDomainsEndpoint
 from semantha_sdk.api.model_extractortypes import ModelExtractortypesEndpoint
 from semantha_sdk.api.model_metadatatypes import ModelMetadatatypesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ModelEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/model"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-
         self.__datatypes = ModelDatatypesEndpoint(session, self._endpoint)
         self.__domains = ModelDomainsEndpoint(session, self._endpoint)
         self.__extractortypes = ModelExtractortypesEndpoint(session, self._endpoint)
         self.__metadatatypes = ModelMetadatatypesEndpoint(session, self._endpoint)
 
-
     @property
     def datatypes(self) -> ModelDatatypesEndpoint:
         return self.__datatypes
-
-
     @property
     def domains(self) -> ModelDomainsEndpoint:
         return self.__domains
-
-
     @property
     def extractortypes(self) -> ModelExtractortypesEndpoint:
         return self.__extractortypes
-
-
     @property
     def metadatatypes(self) -> ModelMetadatatypesEndpoint:
         return self.__metadatatypes
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_boostword.py` & `semantha_sdk-5.5.0/semantha_sdk/api/sentence.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.boost_word import BoostWord, BoostWordSchema
+from semantha_sdk.model.sentence import Sentence
+from semantha_sdk.model.sentence import SentenceSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
-class ModelBoostwordEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class SentenceEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
 
-    def get(self
-        ) -> BoostWord:
-        """
-        Get a boostword by id 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(BoostWordSchema)
-
-    def put(self, boostword: BoostWord) -> BoostWord:
-        """
-        Update a boostword by id
-        """
-        return self._session.put(
-            url=self._endpoint,
-            json=BoostWordSchema().dump(boostword)
-        ).execute().to(BoostWordSchema)
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id = id
 
 
-    def delete(self) -> None:
+    def get(
+        self,
+    ) -> Sentence:
         """
-        Delete a boostword by id
-        """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
+        Get sentence by ID
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(SentenceSchema)
 
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_boostwords.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 from semantha_sdk.api.model_boostword import ModelBoostwordEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.boost_word import BoostWord, BoostWordSchema
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ModelBoostwordsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/boostwords"
 
-    def get(self
-        ) -> List[BoostWord]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelBoostwordEndpoint:
+        return ModelBoostwordEndpoint(self._session, self._endpoint, id)
+
+    def get(
+        self,
+    ) -> List[BoostWord]:
         """
-        Get all boostwords 
+        Get all boostwords
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(BoostWordSchema)
 
-    def post(self
-        , body: BoostWord = None
-        ) -> BoostWord:
+    def post(
+        self,
+        body: BoostWord = None,
+    ) -> BoostWord:
         """
         Create a boostword
         Args:
-            body (BoostWord): 
-            
+        body (BoostWord): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=BoostWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(BoostWordSchema)
 
-
-    def delete(self) -> None:
+    
+    def delete(
+        self,
+    ) -> None:
         """
         Delete all boostwords
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, id: str) -> ModelBoostwordEndpoint:
-        return ModelBoostwordEndpoint(self._session, self._endpoint, id)
-
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.5.0/semantha_sdk/api/tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
+from semantha_sdk.api.tag import TagEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class ModelDatatypesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class TagsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/datatypes"
+        return self._parent_endpoint + "/tags"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> List[str]:
+    def __call__(
+            self,
+            tagname: str,
+    ) -> TagEndpoint:
+        return TagEndpoint(self._session, self._endpoint, tagname)
+
+    def get(
+        self,
+    ) -> List[str]:
         """
-        Get all datatypes 
+        Get tags
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,63 +2,66 @@
 from semantha_sdk.api.model_boostwords import ModelBoostwordsEndpoint
 from semantha_sdk.api.model_namedentities import ModelNamedentitiesEndpoint
 from semantha_sdk.api.model_stopwords import ModelStopwordsEndpoint
 from semantha_sdk.api.model_synonyms import ModelSynonymsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ModelDomainEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._domainname}"
 
-    def get(self
-        ) -> IOBase:
-        """
-        Get a domain by domainname 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute()
-
-    def patch(self, iobase: IOBase) -> IOBase:
-        """
-        Update a domain by domainname
-        """
-        return self._session.patch(
-            url=self._endpoint,
-            json=iobase
-        ).execute()
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        domainname: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
-        self._domainname=domainname
+        self._domainname = domainname
         self.__boostwords = ModelBoostwordsEndpoint(session, self._endpoint)
         self.__namedentities = ModelNamedentitiesEndpoint(session, self._endpoint)
         self.__stopwords = ModelStopwordsEndpoint(session, self._endpoint)
         self.__synonyms = ModelSynonymsEndpoint(session, self._endpoint)
 
-
     @property
     def boostwords(self) -> ModelBoostwordsEndpoint:
         return self.__boostwords
-
-
     @property
     def namedentities(self) -> ModelNamedentitiesEndpoint:
         return self.__namedentities
-
-
     @property
     def stopwords(self) -> ModelStopwordsEndpoint:
         return self.__stopwords
-
-
     @property
     def synonyms(self) -> ModelSynonymsEndpoint:
         return self.__synonyms
 
+    def get(
+        self,
+    ) -> IOBase:
+        """
+        Get a domain by domainname
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().as_bytesio()
+
+    
+    def patch(
+        self,
+        file: IOBase
+    ) -> IOBase:
+        """
+        Update a domain by domainname
+        """
+        return self._session.patch(
+            url=self._endpoint,
+            json=file
+        ).execute().as_bytesio()
+
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_domains.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from semantha_sdk.api.model_domain import ModelDomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ModelDomainsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/domains"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
 
-
-
-    def __call__(self, domainname: str) -> ModelDomainEndpoint:
+    def __call__(
+            self,
+            domainname: str,
+    ) -> ModelDomainEndpoint:
         return ModelDomainEndpoint(self._session, self._endpoint, domainname)
 
-
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_extractortypes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ModelExtractortypesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/extractortypes"
 
-    def get(self
-        ) -> List[str]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[str]:
         """
-        Get all extractortypes 
+        Get all extractortypes
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ModelMetadatatypesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/metadatatypes"
 
-    def get(self
-        ) -> List[str]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+    ) -> List[str]:
         """
-        Get all metadatatypes 
+        Get all metadatatypes
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_namedentities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 from semantha_sdk.api.model_namedentity import ModelNamedentityEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.named_entity import NamedEntity, NamedEntitySchema
+from semantha_sdk.model.named_entity import NamedEntity
+from semantha_sdk.model.named_entity import NamedEntitySchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ModelNamedentitiesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/namedentities"
 
-    def get(self
-        ) -> List[NamedEntity]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelNamedentityEndpoint:
+        return ModelNamedentityEndpoint(self._session, self._endpoint, id)
+
+    def get(
+        self,
+    ) -> List[NamedEntity]:
         """
-        Get custom entities 
+        Get custom entities
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(NamedEntitySchema)
 
-    def post(self
-        , body: NamedEntity = None
-        ) -> NamedEntity:
+    def post(
+        self,
+        body: NamedEntity = None,
+    ) -> NamedEntity:
         """
         Create a custom entity
         Args:
-            body (NamedEntity): 
-            
+        body (NamedEntity): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=NamedEntitySchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(NamedEntitySchema)
 
-
-    def delete(self) -> None:
+    
+    def delete(
+        self,
+    ) -> None:
         """
         Delete all custom entities
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, id: str) -> ModelNamedentityEndpoint:
-        return ModelNamedentityEndpoint(self._session, self._endpoint, id)
-
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_stopword.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.named_entity import NamedEntity, NamedEntitySchema
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
-class ModelNamedentityEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelStopwordEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
 
-    def get(self
-        ) -> NamedEntity:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id = id
+
+
+    def get(
+        self,
+    ) -> StopWord:
         """
-        Get a custom entity by id 
+        Get a stop word by id
         Args:
-            
-        """
+            """
         q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(NamedEntitySchema)
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(StopWordSchema)
 
-    def put(self, namedentity: NamedEntity) -> NamedEntity:
+    
+    
+    def delete(
+        self,
+    ) -> None:
         """
-        Update a custom entity by id
+        Delete a stop word by id
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=NamedEntitySchema().dump(namedentity)
-        ).execute().to(NamedEntitySchema)
+        ).execute()
 
-
-    def delete(self) -> None:
+    def put(
+        self,
+        body: StopWord
+    ) -> StopWord:
         """
-        Delete a custom entity by id
+        Update a stop word by id
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
-
+        return self._session.put(
+            url=self._endpoint,
+            json=StopWordSchema().dump(body)
+        ).execute().to(StopWordSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_stopword.py` & `semantha_sdk-5.5.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.stop_word import StopWord, StopWordSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-
-class ModelStopwordEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class TagReferencedocumentsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/referencedocuments"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> StopWord:
+
+    def get(
+        self,
+    ) -> List[DocumentInformation]:
         """
-        Get a stop word by id 
+        Get all reference documents with a specific tag
         Args:
-            
-        """
+            """
         q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(StopWordSchema)
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentInformationSchema)
 
-    def put(self, stopword: StopWord) -> StopWord:
+    
+    
+    def delete(
+        self,
+    ) -> None:
         """
-        Update a stop word by id
+        Delete reference documents with a specific tag
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=StopWordSchema().dump(stopword)
-        ).execute().to(StopWordSchema)
-
-
-    def delete(self) -> None:
-        """
-        Delete a stop word by id
-        """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_stopwords.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 from semantha_sdk.api.model_stopword import ModelStopwordEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.stop_word import StopWord, StopWordSchema
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ModelStopwordsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/stopwords"
 
-    def get(self
-        ) -> List[StopWord]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelStopwordEndpoint:
+        return ModelStopwordEndpoint(self._session, self._endpoint, id)
+
+    def get(
+        self,
+    ) -> List[StopWord]:
         """
-        Get all stop words 
+        Get all stop words
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(StopWordSchema)
 
-    def post(self
-        , body: StopWord = None
-        ) -> StopWord:
+    def post(
+        self,
+        body: StopWord = None,
+    ) -> StopWord:
         """
         Create a stop word
         Args:
-            body (StopWord): 
-            
+        body (StopWord): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             json=StopWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(StopWordSchema)
 
-
-    def delete(self) -> None:
+    
+    def delete(
+        self,
+    ) -> None:
         """
         Delete all stop words
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, id: str) -> ModelStopwordEndpoint:
-        return ModelStopwordEndpoint(self._session, self._endpoint, id)
-
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_synonym.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_synonyms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,69 @@
+from semantha_sdk.api.model_synonym import ModelSynonymEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.synonym import Synonym, SynonymSchema
+from semantha_sdk.model.synonym import Synonym
+from semantha_sdk.model.synonym import SynonymSchema
+from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-
-class ModelSynonymEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelSynonymsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/synonyms"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> Synonym:
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelSynonymEndpoint:
+        return ModelSynonymEndpoint(self._session, self._endpoint, id)
+
+    def get(
+        self,
+    ) -> List[Synonym]:
         """
-        Get a synonym by id 
+        Get all synonyms
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(SynonymSchema)
 
-    def put(self, synonym: Synonym) -> Synonym:
+    def post(
+        self,
+        body: Synonym = None,
+    ) -> Synonym:
         """
-        Update a synonym by id
+        Create a synonym
+        Args:
+        body (Synonym): 
         """
-        return self._session.put(
+        q_params = {}
+        response = self._session.post(
             url=self._endpoint,
-            json=SynonymSchema().dump(synonym)
-        ).execute().to(SynonymSchema)
-
-
-    def delete(self) -> None:
+            json=SynonymSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(SynonymSchema)
+
+    
+    def delete(
+        self,
+    ) -> None:
         """
-        Delete a synonym by id
+        Delete all synonyms
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.5.0/semantha_sdk/api/modelclasses.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,40 @@
-from semantha_sdk.api.model_synonym import ModelSynonymEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.synonym import Synonym, SynonymSchema
-from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.model.model_class import ModelClass
+from semantha_sdk.model.model_class import ModelClassSchema
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class ModelSynonymsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelclassesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/synonyms"
+        return self._parent_endpoint + "/modelclasses"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> List[Synonym]:
-        """
-        Get all synonyms 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(SynonymSchema)
 
-    def post(self
-        , body: Synonym = None
-        ) -> Synonym:
+    def get(
+        self,
+        uilanguage: str = None,
+    ) -> List[ModelClass]:
         """
-        Create a synonym
+        Get all model classes
         Args:
-            body (Synonym): 
-            
+        uilanguage str: Selects the language of the labels in the JSON response; useful with multi-language domain models.
         """
         q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=SynonymSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(SynonymSchema)
-
-
-    def delete(self) -> None:
-        """
-        Delete all synonyms
-        """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
-
-    def __call__(self, id: str) -> ModelSynonymEndpoint:
-        return ModelSynonymEndpoint(self._session, self._endpoint, id)
-
-
+        if uilanguage is not None:
+            q_params["uilanguage"] = uilanguage
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ModelClassSchema)
+
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.5.0/semantha_sdk/api/domains.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+from semantha_sdk.api.domain import DomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.model_class import ModelClass, ModelClassSchema
+from semantha_sdk.model.domain import Domain
+from semantha_sdk.model.domain import DomainSchema
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class ModelclassesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class DomainsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/modelclasses"
+        return self._parent_endpoint + "/domains"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        , uilanguage: str = None
-        ) -> List[ModelClass]:
+    def __call__(
+            self,
+            domainname: str,
+    ) -> DomainEndpoint:
+        return DomainEndpoint(self._session, self._endpoint, domainname)
+
+    def get(
+        self,
+    ) -> List[Domain]:
         """
-        Get all model classes 
+        Get all domains
         Args:
-            uilanguage (str): Selects the language of the labels in the JSON response; useful with multi-language domain models.
-            
-        """
+            """
         q_params = {}
-        if uilanguage is not None:
-            q_params["uilanguage"] = uilanguage
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(ModelClassSchema)
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(DomainSchema)
 
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.5.0/semantha_sdk/api/modelinstances.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.semantic_model import SemanticModel, SemanticModelSchema
+from semantha_sdk.model.semantic_model import SemanticModel
+from semantha_sdk.model.semantic_model import SemanticModelSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ModelinstancesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/modelinstances"
 
-    def post(self
-        , file: IOBase = None
-        , documentextractor: str = None
-        , applymatchersfordocumentextractor: bool = None
-        , withimages: bool = None
-        , withdocument: bool = None
-        , withadditionalroots: bool = None
-        , documenttype: str = None
-        , uilanguage: str = None
-        ) -> SemanticModel:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        documentextractor: str = None,
+        applymatchersfordocumentextractor: bool = None,
+        withimages: bool = None,
+        withdocument: bool = None,
+        withadditionalroots: bool = None,
+        documenttype: str = None,
+        uilanguage: str = None,
+    ) -> SemanticModel:
         """
         Extract semantic model for a list of documents
         Args:
-            file (IOBase): Input document (left document).
-            documentextractor (str): The document extractor you want to be considered.
-            applymatchersfordocumentextractor (bool): 
-            
+        file (IOBase): Input document (left document).
+    documentextractor (str): The document extractor you want to be considered.
+    applymatchersfordocumentextractor (bool): 
         """
         q_params = {}
         if withimages is not None:
             q_params["withimages"] = withimages
         if withdocument is not None:
             q_params["withdocument"] = withdocument
         if withadditionalroots is not None:
             q_params["withadditionalroots"] = withadditionalroots
         if documenttype is not None:
             q_params["documenttype"] = documenttype
         if uilanguage is not None:
             q_params["uilanguage"] = uilanguage
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "documentextractor": documentextractor,
-                "applymatchersfordocumentextractor": applymatchersfordocumentextractor
+                "applymatchersfordocumentextractor": applymatchersfordocumentextractor,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(SemanticModelSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.5.0/semantha_sdk/api/namedentities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_named_entity import DocumentNamedEntity, DocumentNamedEntitySchema
+from semantha_sdk.model.document_named_entity import DocumentNamedEntity
+from semantha_sdk.model.document_named_entity import DocumentNamedEntitySchema
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class NamedentitiesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/namedentities"
 
-    def get(self
-        , tags: str = None
-        , documentclassids: str = None
-        ) -> List[DocumentNamedEntity]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+        tags: str = None,
+        documentclassids: str = None,
+    ) -> List[DocumentNamedEntity]:
         """
-        Get all custom entities 
+        Get all custom entities
         Args:
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            documentclassids (str): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            
+        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
         """
         q_params = {}
         if tags is not None:
             q_params["tags"] = tags
         if documentclassids is not None:
             q_params["documentclassids"] = documentclassids
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentNamedEntitySchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.5.0/semantha_sdk/api/paragraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.paragraph import Paragraph, ParagraphSchema
-from semantha_sdk.model.paragraph_update import ParagraphUpdate, ParagraphUpdateSchema
+from semantha_sdk.model.paragraph import Paragraph
+from semantha_sdk.model.paragraph import ParagraphSchema
+from semantha_sdk.model.paragraph_update import ParagraphUpdate
+from semantha_sdk.model.paragraph_update import ParagraphUpdateSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ParagraphEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
 
-    def get(self
-        ) -> Paragraph:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id = id
+
+
+    def get(
+        self,
+    ) -> Paragraph:
         """
-        Get paragraph by ID 
+        Get paragraph by ID
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(ParagraphSchema)
 
-    def patch(self, paragraphupdate: ParagraphUpdate) -> ParagraphUpdate:
+    
+    def patch(
+        self,
+        body: ParagraphUpdate
+    ) -> ParagraphUpdate:
         """
         Update a specific paragraph of a specific reference document of the library
         """
         return self._session.patch(
             url=self._endpoint,
-            json=ParagraphUpdateSchema().dump(paragraphupdate)
+            json=ParagraphUpdateSchema().dump(body)
         ).execute().to(ParagraphSchema)
 
-
-    def delete(self) -> None:
+    def delete(
+        self,
+    ) -> None:
         """
         Delete a specific paragraph of a specific reference document of the library
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.5.0/semantha_sdk/api/statistic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
-from semantha_sdk.api.paragraph import ParagraphEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
+from semantha_sdk.model.statistic import Statistic
+from semantha_sdk.model.statistic import StatisticSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
-class ParagraphsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class StatisticEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/paragraphs"
-
+        return self._parent_endpoint + "/statistic"
 
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
 
 
-
-    def __call__(self, id: str) -> ParagraphEndpoint:
-        return ParagraphEndpoint(self._session, self._endpoint, id)
-
-
+    def get(
+        self,
+    ) -> Statistic:
+        """
+        Get statistical informations about library content
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(StatisticSchema)
+
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.5.0/semantha_sdk/api/referencedocument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 from semantha_sdk.api.paragraphs import ParagraphsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.sentences import SentencesEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
-from semantha_sdk.model.document_information import DocumentInformation, DocumentInformationSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class ReferencedocumentEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._documentid}"
 
-    def get(self
-        , querybyname: bool = None
-        ) -> Document:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        documentid: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._documentid = documentid
+        self.__paragraphs = ParagraphsEndpoint(session, self._endpoint)
+        self.__sentences = SentencesEndpoint(session, self._endpoint)
+
+    @property
+    def paragraphs(self) -> ParagraphsEndpoint:
+        return self.__paragraphs
+    @property
+    def sentences(self) -> SentencesEndpoint:
+        return self.__sentences
+
+    def get(
+        self,
+        querybyname: bool = None,
+    ) -> Document:
         """
-         
+        
         Args:
-            querybyname (bool): Select if you want forward a name instead of an ID.
-            
+        querybyname bool: Select if you want forward a name instead of an ID.
         """
         q_params = {}
         if querybyname is not None:
             q_params["querybyname"] = querybyname
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentSchema)
 
-    def patch(self, documentinformation: DocumentInformation) -> DocumentInformation:
+    
+    def patch(
+        self,
+        body: DocumentInformation
+    ) -> DocumentInformation:
         """
         
         """
         return self._session.patch(
             url=self._endpoint,
-            json=DocumentInformationSchema().dump(documentinformation)
+            json=DocumentInformationSchema().dump(body)
         ).execute().to(DocumentInformationSchema)
 
-
-    def delete(self) -> None:
+    def delete(
+        self,
+    ) -> None:
         """
         
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str, documentid: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._documentid=documentid
-        self.__paragraphs = ParagraphsEndpoint(session, self._endpoint)
-        self.__sentences = SentencesEndpoint(session, self._endpoint)
-
-
-    @property
-    def paragraphs(self) -> ParagraphsEndpoint:
-        return self.__paragraphs
-
-
-    @property
-    def sentences(self) -> SentencesEndpoint:
-        return self.__sentences
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.5.0/semantha_sdk/api/referencedocuments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,95 @@
 from io import IOBase
 from semantha_sdk.api.clusters import ClustersEndpoint
 from semantha_sdk.api.namedentities import NamedentitiesEndpoint
 from semantha_sdk.api.referencedocument import ReferencedocumentEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.statistic import StatisticEndpoint
-from semantha_sdk.model.document_information import DocumentInformation, DocumentInformationSchema
-from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainer, ReferenceDocumentsResponseContainerSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
+from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainer
+from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainerSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ReferencedocumentsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/referencedocuments"
 
-    def get(self
-        , tags: str = None
-        , documentids: str = None
-        , name: str = None
-        , createdafter: int = None
-        , createdbefore: int = None
-        , updatedafter: int = None
-        , updatedbefore: int = None
-        , documentclassids: str = None
-        , withoutdocumentclass: bool = None
-        , mincharacters: int = None
-        , metadata: str = None
-        , comment: str = None
-        , offset: int = None
-        , limit: int = None
-        , sort: str = None
-        , fields: str = None
-        ) -> ReferenceDocumentsResponseContainer:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self.__clusters = ClustersEndpoint(session, self._endpoint)
+        self.__namedentities = NamedentitiesEndpoint(session, self._endpoint)
+        self.__statistic = StatisticEndpoint(session, self._endpoint)
+
+    @property
+    def clusters(self) -> ClustersEndpoint:
+        return self.__clusters
+    @property
+    def namedentities(self) -> NamedentitiesEndpoint:
+        return self.__namedentities
+    @property
+    def statistic(self) -> StatisticEndpoint:
+        return self.__statistic
+    def __call__(
+            self,
+            documentid: str,
+    ) -> ReferencedocumentEndpoint:
+        return ReferencedocumentEndpoint(self._session, self._endpoint, documentid)
+
+    def get(
+        self,
+        tags: str = None,
+        documentids: str = None,
+        name: str = None,
+        createdafter: int = None,
+        createdbefore: int = None,
+        updatedafter: int = None,
+        updatedbefore: int = None,
+        documentclassids: str = None,
+        withoutdocumentclass: bool = None,
+        mincharacters: int = None,
+        metadata: str = None,
+        comment: str = None,
+        offset: int = None,
+        limit: int = None,
+        sort: str = None,
+        fields: str = None,
+    ) -> ReferenceDocumentsResponseContainer:
         """
         Get all reference documents
-        Please be aware that this service is limited: The query parameter ‚tags‘ can only be used in combination with an JSON export. 
+            Please be aware that this service is limited: The query parameter ‚tags‘ can only be used in combination with an JSON export.
         Args:
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            documentids (str): List of document Ids for target. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            name (str): The document name in your library (in contrast to the file name being used during upload).
-            createdafter (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
-            createdbefore (int): Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
-            updatedafter (int): 
-            updatedbefore (int): 
-            documentclassids (str): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            withoutdocumentclass (bool): Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
-            mincharacters (int): 
-            metadata (str): Filter by metadata
-            comment (str): Use this parameter to add a comment to your reference document.
-            offset (int): Specify from which number on reference documents should be returned.
-            limit (int): Specify the number of reference documents to be returned.
-            sort (str): Sort the returned reference documents by name, created, updated and/or metadata. Add a - before the field name to sort in descending order.
-            fields (str): Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: id, name, tags, metadata, filename, created, processed, lang, updated.
-            
+        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids str: List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    name str: The document name in your library (in contrast to the file name being used during upload).
+    createdafter int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
+    createdbefore int: Use this parameter to filter the returned reference documents by their date of creation using a UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
+    updatedafter int: 
+    updatedbefore int: 
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    withoutdocumentclass bool: Use this parameter to filter the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
+    mincharacters int: 
+    metadata str: Filter by metadata
+    comment str: Use this parameter to add a comment to your reference document.
+    offset int: Specify from which number on reference documents should be returned.
+    limit int: Specify the number of reference documents to be returned.
+    sort str: Sort the returned reference documents by name, created, updated and/or metadata. Add a - before the field name to sort in descending order.
+    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: id, name, tags, metadata, filename, created, processed, lang, updated.
         """
         q_params = {}
         if tags is not None:
             q_params["tags"] = tags
         if documentids is not None:
             q_params["documentids"] = documentids
         if name is not None:
@@ -90,96 +116,72 @@
             q_params["offset"] = offset
         if limit is not None:
             q_params["limit"] = limit
         if sort is not None:
             q_params["sort"] = sort
         if fields is not None:
             q_params["fields"] = fields
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(ReferenceDocumentsResponseContainerSchema)
 
-    def post(self
-        , name: str = None
-        , tags: str = None
-        , metadata: str = None
-        , file: IOBase = None
-        , text: str = None
-        , documenttype: str = None
-        , color: str = None
-        , comment: str = None
-        , documentclass: str = None
-        , addparagraphsasdocuments: bool = None
-        , detectlanguage: bool = None
-        ) -> List[DocumentInformation]:
+    def post(
+        self,
+        name: str = None,
+        tags: str = None,
+        metadata: str = None,
+        file: IOBase = None,
+        text: str = None,
+        documenttype: str = None,
+        color: str = None,
+        comment: str = None,
+        documentclass: str = None,
+        addparagraphsasdocuments: bool = None,
+        detectlanguage: bool = None,
+    ) -> List[DocumentInformation]:
         """
         Upload reference document
         Args:
-            name (str): The document name in your library (in contrast to the file name being used during upload).
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            metadata (str): Filter by metadata
-            file (IOBase): Input document (left document).
-            text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
-            comment (str): Use this parameter to add a comment to your reference document.
-            documentclass (str): 
-            addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
-            
+        name (str): The document name in your library (in contrast to the file name being used during upload).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    metadata (str): Filter by metadata
+    file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
+    comment (str): Use this parameter to add a comment to your reference document.
+    documentclass (str): 
+    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
         """
         q_params = {}
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "name": name,
                 "tags": tags,
                 "metadata": metadata,
                 "file": file,
                 "text": text,
                 "documenttype": documenttype,
                 "color": color,
                 "comment": comment,
                 "documentclass": documentclass,
-                "addparagraphsasdocuments": addparagraphsasdocuments
+                "addparagraphsasdocuments": addparagraphsasdocuments,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentInformationSchema)
 
-
-    def delete(self) -> None:
+    
+    def delete(
+        self,
+    ) -> None:
         """
         Delete all reference documents
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-        self.__clusters = ClustersEndpoint(session, self._endpoint)
-        self.__namedentities = NamedentitiesEndpoint(session, self._endpoint)
-        self.__statistic = StatisticEndpoint(session, self._endpoint)
-
-
-    @property
-    def clusters(self) -> ClustersEndpoint:
-        return self.__clusters
-
-
-    @property
-    def namedentities(self) -> NamedentitiesEndpoint:
-        return self.__namedentities
-
-
-    @property
-    def statistic(self) -> StatisticEndpoint:
-        return self.__statistic
-
-
-    def __call__(self, documentid: str) -> ReferencedocumentEndpoint:
-        return ReferencedocumentEndpoint(self._session, self._endpoint, documentid)
-
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
 
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/references.py` & `semantha_sdk-5.5.0/semantha_sdk/api/references.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,114 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import Document, DocumentSchema
-from semantha_sdk.model.document_meta_data import DocumentMetaData, DocumentMetaDataSchema
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.document_meta_data import DocumentMetaData
+from semantha_sdk.model.document_meta_data import DocumentMetaDataSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class ReferencesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/references"
 
-    def post(self
-        , file: IOBase = None
-        , referencedocument: IOBase = None
-        , referencedocumentids: List[str] = None
-        , tags: str = None
-        , documentclassids: List[str] = None
-        , similaritythreshold: float = None
-        , synonymousthreshold: float = None
-        , marknomatch: bool = None
-        , withreferencetext: bool = None
-        , language: str = None
-        , mode: str = None
-        , documenttype: str = None
-        , metadata: List[DocumentMetaData] = None
-        , withcontext: bool = None
-        , considertexttype: bool = None
-        , resizeparagraphs: bool = None
-        , text: str = None
-        , withareas: bool = None
-        , detectlanguage: bool = None
-        , maxreferences: int = None
-        ) -> Document:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        referencedocument: IOBase = None,
+        referencedocumentids: List[str] = None,
+        tags: str = None,
+        documentclassids: List[str] = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+        mode: str = None,
+        documenttype: str = None,
+        metadata: List[DocumentMetaData] = None,
+        withcontext: bool = None,
+        considertexttype: bool = None,
+        resizeparagraphs: bool = None,
+        text: str = None,
+        withareas: bool = None,
+        detectlanguage: bool = None,
+        maxreferences: int = None,
+    ) -> Document:
         """
         Determine references with one input document
-        Matches one input document ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
+            Matches one input document ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
         Args:
-            file (IOBase): Input document (left document).
-            referencedocument (IOBase): Reference document(s) to be used instead of the documents in the domain's library.
-            referencedocumentids (List[str]): To filter for document IDs. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            synonymousthreshold (float): Threshold for good matches.
-            marknomatch (bool): Marks the paragraphs that have not matched
-            withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
-            language (str): The language of the input document (only available if configured for the domain).
-            mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
-        fingerprint: semantic search based on sentences; 
-        keyword: keyword: search based on sentences; 
-        document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
-        document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
-        fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-        Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            metadata (List[DocumentMetaData]): Filter by metadata
-            withcontext (bool): Creates and saves the context.
-            considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-            resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
-            text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-            withareas (bool): Gives back the coordinates of referenced area.
-            
+        file (IOBase): Input document (left document).
+    referencedocument (IOBase): Reference document(s) to be used instead of the documents in the domain's library.
+    referencedocumentids (List[str]): To filter for document IDs. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    metadata (List[DocumentMetaData]): Filter by metadata
+    withcontext (bool): Creates and saves the context.
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+    resizeparagraphs (bool): Automatically resizes paragraphs based on their semantic meaning.
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    withareas (bool): Gives back the coordinates of referenced area.
         """
         q_params = {}
         if detectlanguage is not None:
             q_params["detectlanguage"] = detectlanguage
         if maxreferences is not None:
             q_params["maxreferences"] = maxreferences
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "referencedocument": referencedocument,
                 "referencedocumentids": referencedocumentids,
                 "tags": tags,
                 "documentclassids": documentclassids,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
                 "withreferencetext": withreferencetext,
-                "language": language,
                 "mode": mode,
                 "documenttype": documenttype,
                 "metadata": metadata,
                 "withcontext": withcontext,
                 "considertexttype": considertexttype,
                 "resizeparagraphs": resizeparagraphs,
                 "text": text,
-                "withareas": withareas
+                "withareas": withareas,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(DocumentSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/roles.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_datatypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class RolesEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelDatatypesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/roles"
+        return self._parent_endpoint + "/datatypes"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self
-        ) -> List[str]:
+
+    def get(
+        self,
+    ) -> List[str]:
         """
-        Get the role/s of the current user/s of a specific domain 
+        Get all datatypes
         Args:
-            
-        """
+            """
         q_params = {}
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.5.0/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/sentence.py` & `semantha_sdk-5.5.0/semantha_sdk/api/model_namedentity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,56 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.sentence import Sentence, SentenceSchema
+from semantha_sdk.model.named_entity import NamedEntity
+from semantha_sdk.model.named_entity import NamedEntitySchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
-class SentenceEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class ModelNamedentityEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
 
-    def get(self
-        ) -> Sentence:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        id: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id = id
+
+
+    def get(
+        self,
+    ) -> NamedEntity:
         """
-        Get sentence by ID 
+        Get a custom entity by id
         Args:
-            
-        """
+            """
         q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(SentenceSchema)
-
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
-        super().__init__(session, parent_endpoint)
-        self._id=id
+    
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(NamedEntitySchema)
 
+    
+    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete a custom entity by id
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
+    def put(
+        self,
+        body: NamedEntity
+    ) -> NamedEntity:
+        """
+        Update a custom entity by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=NamedEntitySchema().dump(body)
+        ).execute().to(NamedEntitySchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/settings.py` & `semantha_sdk-5.5.0/semantha_sdk/api/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.settings import Settings, SettingsSchema
+from semantha_sdk.model.settings import Settings
+from semantha_sdk.model.settings import SettingsSchema
 from semantha_sdk.rest.rest_client import RestClient
 
-
 class SettingsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/settings"
 
-    def get(self
-        , withsimilaritymodelid: bool = None
-        ) -> Settings:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    def get(
+        self,
+        withsimilaritymodelid: bool = None,
+    ) -> Settings:
         """
-        Get the configuration settings of a specific domain 
+        Get the configuration settings of a specific domain
         Args:
-            withsimilaritymodelid (bool): 
-            
+        withsimilaritymodelid bool: 
         """
         q_params = {}
         if withsimilaritymodelid is not None:
             q_params["withsimilaritymodelid"] = withsimilaritymodelid
+    
         return self._session.get(self._endpoint, q_params=q_params).execute().to(SettingsSchema)
 
-    def patch(self, settings: Settings) -> Settings:
+    
+    def patch(
+        self,
+        body: Settings
+    ) -> Settings:
         """
         Update configuration settings for this domain, e.g. which similarity model to use
         """
         return self._session.patch(
             url=self._endpoint,
-            json=SettingsSchema().dump(settings)
+            json=SettingsSchema().dump(body)
         ).execute().to(SettingsSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 from io import IOBase
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.similaritymatrix_cluster import SimilaritymatrixClusterEndpoint
-from semantha_sdk.model.matrix_row import MatrixRow, MatrixRowSchema
+from semantha_sdk.model.matrix_row import MatrixRow
+from semantha_sdk.model.matrix_row import MatrixRowSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class SimilaritymatrixEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/similaritymatrix"
 
-    def post(self
-        , file: IOBase = None
-        , tags: str = None
-        , sourcetags: str = None
-        , documentids: List[str] = None
-        , sourcedocumentids: List[str] = None
-        , documentclassids: List[str] = None
-        , sourcedocumentclassids: List[str] = None
-        , similaritythreshold: float = None
-        , language: str = None
-        , mode: str = None
-        , documenttype: str = None
-        , considertexttype: bool = None
-        , withcontext: bool = None
-        ) -> List[MatrixRow]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self.__cluster = SimilaritymatrixClusterEndpoint(session, self._endpoint)
+
+    @property
+    def cluster(self) -> SimilaritymatrixClusterEndpoint:
+        return self.__cluster
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        tags: str = None,
+        sourcetags: str = None,
+        documentids: List[str] = None,
+        sourcedocumentids: List[str] = None,
+        documentclassids: List[str] = None,
+        sourcedocumentclassids: List[str] = None,
+        similaritythreshold: float = None,
+        mode: str = None,
+        documenttype: str = None,
+        considertexttype: bool = None,
+        withcontext: bool = None,
+    ) -> List[MatrixRow]:
         """
         Get a similarity matrix
         Args:
-            file (IOBase): Input document (left document).
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            sourcetags (str): Filters the input library by tags
-            documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            sourcedocumentids (List[str]): List of document IDs for source. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            sourcedocumentclassids (List[str]): List of documentclass IDs for the source. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            language (str): The language of the input document (only available if configured for the domain).
-            mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
-        fingerprint: semantic search based on sentences; 
-        keyword: keyword: search based on sentences; 
-        document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
-        document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
-        fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-        Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-            documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-            considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-            withcontext (bool): Creates and saves the context.
-            
+        file (IOBase): Input document (left document).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    sourcetags (str): Filters the input library by tags
+    documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    sourcedocumentids (List[str]): List of document IDs for source. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    sourcedocumentclassids (List[str]): List of documentclass IDs for the source. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+    withcontext (bool): Creates and saves the context.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "file": file,
                 "tags": tags,
                 "sourcetags": sourcetags,
                 "documentids": documentids,
                 "sourcedocumentids": sourcedocumentids,
                 "documentclassids": documentclassids,
                 "sourcedocumentclassids": sourcedocumentclassids,
                 "similaritythreshold": similaritythreshold,
-                "language": language,
                 "mode": mode,
                 "documenttype": documenttype,
                 "considertexttype": considertexttype,
-                "withcontext": withcontext
+                "withcontext": withcontext,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(MatrixRowSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-        self.__cluster = SimilaritymatrixClusterEndpoint(session, self._endpoint)
-
-
-    @property
-    def cluster(self) -> SimilaritymatrixClusterEndpoint:
-        return self.__cluster
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.5.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.matrix_row import MatrixRow, MatrixRowSchema
+from semantha_sdk.model.matrix_row import MatrixRow
+from semantha_sdk.model.matrix_row import MatrixRowSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
 class SimilaritymatrixClusterEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/cluster"
 
-    def post(self
-        , tags: str = None
-        , documentids: List[str] = None
-        , documentclassids: List[str] = None
-        , similaritythreshold: float = None
-        , mode: str = None
-        , considertexttype: bool = None
-        , withcontext: bool = None
-        ) -> List[MatrixRow]:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        tags: str = None,
+        documentids: List[str] = None,
+        documentclassids: List[str] = None,
+        similaritythreshold: float = None,
+        mode: str = None,
+        considertexttype: bool = None,
+        withcontext: bool = None,
+    ) -> List[MatrixRow]:
         """
         Get document clusters
-        Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
+            Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
         Args:
-            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-            documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
-        The IDs are passed as a JSON array.
-            documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
-        The IDs are passed as a JSON array.
-        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-        In general, the higher the threshold, the more precise the results.
-            mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
-        fingerprint: semantic search based on sentences; 
-        keyword: keyword: search based on sentences; 
-        document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
-        document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
-        fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-        Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-            considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-            withcontext (bool): Creates and saves the context.
-            
+        tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
+            The IDs are passed as a JSON array.
+    documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
+            The IDs are passed as a JSON array.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+    similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+            In general, the higher the threshold, the more precise the results.
+    mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
+            fingerprint: semantic search based on sentences; 
+            keyword: keyword: search based on sentences; 
+            document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
+            document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
+            fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+    withcontext (bool): Creates and saves the context.
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "tags": tags,
                 "documentids": documentids,
                 "documentclassids": documentclassids,
                 "similaritythreshold": similaritythreshold,
                 "mode": mode,
                 "considertexttype": considertexttype,
-                "withcontext": withcontext
+                "withcontext": withcontext,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(MatrixRowSchema)
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/statistic.py` & `semantha_sdk-5.5.0/semantha_sdk/api/tag.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.statistic import Statistic, StatisticSchema
+from semantha_sdk.api.tag_referencedocuments import TagReferencedocumentsEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-
-class StatisticEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class TagEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/statistic"
-
-    def get(self
-        ) -> Statistic:
-        """
-        Get statistical informations about library content 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(StatisticSchema)
+        return self._parent_endpoint + f"/{self._tagname}"
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+        tagname: str,
+    ) -> None:
         super().__init__(session, parent_endpoint)
+        self._tagname = tagname
+        self.__referencedocuments = TagReferencedocumentsEndpoint(session, self._endpoint)
 
+    @property
+    def referencedocuments(self) -> TagReferencedocumentsEndpoint:
+        return self.__referencedocuments
 
+    
+    
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/summarizations.py` & `semantha_sdk-5.5.0/semantha_sdk/api/summarizations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
-from typing import Any
 from typing import List
 
-
 class SummarizationsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + "/summarizations"
 
-    def post(self
-        , texts: List[str] = None
-        , topic: str = None
-        ) -> Any:
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+    
+    def post(
+        self,
+        texts: List[str] = None,
+        topic: str = None,
+    ) -> str:
         """
         
         Args:
-            texts (List[str]): 
-            topic (str): 
-            
+        texts (List[str]): 
+    topic (str): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            
             body={
-            
                 "texts": texts,
-                "topic": topic
+                "topic": topic,
             },
-            
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_str()
 
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.5.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document_information import DocumentInformation, DocumentInformationSchema
+from semantha_sdk.model.synonym import Synonym
+from semantha_sdk.model.synonym import SynonymSchema
+from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
-
-class TagReferencedocumentsEndpoint(SemanthaAPIEndpoint):
-    """ author semantha, this is a generated class do not change manually! """
+class BulkmodelSynonymsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! TODO: resource.comment?"""
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/referencedocuments"
+        return self._parent_endpoint + "/synonyms"
 
-    def get(self
-        ) -> List[DocumentInformation]:
-        """
-        Get all reference documents with a specific tag 
-        Args:
-            
-        """
-        q_params = {}
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentInformationSchema)
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
 
 
-    def delete(self) -> None:
+    
+    def post(
+        self,
+        body: List[Synonym] = None,
+    ) -> None:
         """
-        Delete reference documents with a specific tag
+        Create one or more synonyms
+            This is the quiet version of  'post /api/domains/{domainname}/synonyms'
+        Args:
+        body (List[Synonym]): 
         """
-        self._session.delete(self._endpoint).execute()
-
-    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
-        super().__init__(session, parent_endpoint)
-
-
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=SynonymSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+    
+
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/__init__.py` & `semantha_sdk-5.5.0/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.5.0/semantha_sdk/model/annotation_cell.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e66 6561 7475 7265 7320 696d  odel.features im
-000000d0: 706f 7274 2046 6561 7475 7265 730d 0a66  port Features..f
-000000e0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-000000f0: 2e6d 6f64 656c 2e72 6563 7420 696d 706f  .model.rect impo
-00000100: 7274 2052 6563 740d 0a66 726f 6d20 7479  rt Rect..from ty
-00000110: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
-00000120: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
-00000130: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
-00000140: 290d 0a63 6c61 7373 2041 6e6e 6f74 6174  )..class Annotat
-00000150: 696f 6e43 656c 6c28 5365 6d61 6e74 6861  ionCell(Semantha
-00000160: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a09  ModelEntity):...
-00000170: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-00000180: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-00000190: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-000001a0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001b0: 7561 6c6c 7921 2022 2222 0d0a 0962 626f  ually! """...bbo
-000001c0: 783a 204f 7074 696f 6e61 6c5b 5265 6374  x: Optional[Rect
-000001d0: 5d0d 0a09 7479 7065 3a20 4f70 7469 6f6e  ]...type: Option
-000001e0: 616c 5b73 7472 5d0d 0a09 6665 6174 7572  al[str]...featur
-000001f0: 6573 3a20 4f70 7469 6f6e 616c 5b46 6561  es: Optional[Fea
-00000200: 7475 7265 735d 0d0a 090d 0a09 0d0a 416e  tures]........An
-00000210: 6e6f 7461 7469 6f6e 4365 6c6c 5363 6865  notationCellSche
-00000220: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
-00000230: 6128 416e 6e6f 7461 7469 6f6e 4365 6c6c  a(AnnotationCell
-00000240: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
-00000250: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e66 6561 7475 7265 7320  .model.features 
+000000d0: 696d 706f 7274 2046 6561 7475 7265 730d  import Features.
+000000e0: 0a0d 0a66 726f 6d20 7365 6d61 6e74 6861  ...from semantha
+000000f0: 5f73 646b 2e6d 6f64 656c 2e72 6563 7420  _sdk.model.rect 
+00000100: 696d 706f 7274 2052 6563 740d 0a0d 0a66  import Rect....f
+00000110: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000120: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
+00000130: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+00000140: 5472 7565 290d 0a63 6c61 7373 2041 6e6e  True)..class Ann
+00000150: 6f74 6174 696f 6e43 656c 6c28 5365 6d61  otationCell(Sema
+00000160: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000170: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000180: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000190: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+000001a0: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+000001b0: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+000001c0: 220d 0a20 2020 2062 626f 783a 204f 7074  "..    bbox: Opt
+000001d0: 696f 6e61 6c5b 5265 6374 5d0d 0a20 2020  ional[Rect]..   
+000001e0: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+000001f0: 7374 725d 0d0a 2020 2020 6665 6174 7572  str]..    featur
+00000200: 6573 3a20 4f70 7469 6f6e 616c 5b46 6561  es: Optional[Fea
+00000210: 7475 7265 735d 0d0a 0d0a 416e 6e6f 7461  tures]....Annota
+00000220: 7469 6f6e 4365 6c6c 5363 6865 6d61 203d  tionCellSchema =
+00000230: 2063 6c61 7373 5f73 6368 656d 6128 416e   class_schema(An
+00000240: 6e6f 7461 7469 6f6e 4365 6c6c 2c20 6261  notationCell, ba
+00000250: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000260: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.5.0/semantha_sdk/model/annotation_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e61 6e6e 6f74 6174 696f 6e5f  odel.annotation_
-000000d0: 6365 6c6c 2069 6d70 6f72 7420 416e 6e6f  cell import Anno
-000000e0: 7461 7469 6f6e 4365 6c6c 0d0a 6672 6f6d  tationCell..from
-000000f0: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
-00000100: 6973 742c 204f 7074 696f 6e61 6c0d 0a0d  ist, Optional...
-00000110: 0a0d 0a40 6461 7461 636c 6173 7328 6672  ...@dataclass(fr
-00000120: 6f7a 656e 3d54 7275 6529 0d0a 636c 6173  ozen=True)..clas
-00000130: 7320 416e 6e6f 7461 7469 6f6e 5061 6765  s AnnotationPage
-00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000150: 7469 7479 293a 0d0a 0922 2222 2061 7574  tity):...""" aut
-00000160: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
-00000170: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
-00000180: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
-00000190: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
-000001a0: 2222 220d 0a09 6865 6967 6874 3a20 4f70  """...height: Op
-000001b0: 7469 6f6e 616c 5b69 6e74 5d0d 0a09 7769  tional[int]...wi
-000001c0: 6474 683a 204f 7074 696f 6e61 6c5b 696e  dth: Optional[in
-000001d0: 745d 0d0a 0970 6167 655f 6e75 6d62 6572  t]...page_number
-000001e0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0d  : Optional[int].
-000001f0: 0a09 6967 6e6f 7265 5f70 6167 653a 204f  ..ignore_page: O
-00000200: 7074 696f 6e61 6c5b 626f 6f6c 5d0d 0a09  ptional[bool]...
-00000210: 6365 6c6c 733a 204f 7074 696f 6e61 6c5b  cells: Optional[
-00000220: 4c69 7374 5b41 6e6e 6f74 6174 696f 6e43  List[AnnotationC
-00000230: 656c 6c5d 5d0d 0a09 0d0a 090d 0a41 6e6e  ell]]........Ann
-00000240: 6f74 6174 696f 6e50 6167 6553 6368 656d  otationPageSchem
-00000250: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-00000260: 2841 6e6e 6f74 6174 696f 6e50 6167 652c  (AnnotationPage,
-00000270: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
-00000280: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e61 6e6e 6f74 6174 696f  .model.annotatio
+000000d0: 6e5f 6365 6c6c 2069 6d70 6f72 7420 416e  n_cell import An
+000000e0: 6e6f 7461 7469 6f6e 4365 6c6c 0d0a 0d0a  notationCell....
+000000f0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000100: 7274 204c 6973 740d 0a66 726f 6d20 7479  rt List..from ty
+00000110: 7069 6e67 2069 6d70 6f72 7420 4f70 7469  ping import Opti
+00000120: 6f6e 616c 0d0a 0d0a 4064 6174 6163 6c61  onal....@datacla
+00000130: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
+00000140: 0a63 6c61 7373 2041 6e6e 6f74 6174 696f  .class Annotatio
+00000150: 6e50 6167 6528 5365 6d61 6e74 6861 4d6f  nPage(SemanthaMo
+00000160: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000170: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000180: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000190: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+000001a0: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+000001b0: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+000001c0: 2068 6569 6768 743a 204f 7074 696f 6e61   height: Optiona
+000001d0: 6c5b 696e 745d 0d0a 2020 2020 7769 6474  l[int]..    widt
+000001e0: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
+000001f0: 0d0a 2020 2020 7061 6765 5f6e 756d 6265  ..    page_numbe
+00000200: 723a 204f 7074 696f 6e61 6c5b 696e 745d  r: Optional[int]
+00000210: 0d0a 2020 2020 6967 6e6f 7265 5f70 6167  ..    ignore_pag
+00000220: 653a 204f 7074 696f 6e61 6c5b 626f 6f6c  e: Optional[bool
+00000230: 5d0d 0a20 2020 2063 656c 6c73 3a20 4f70  ]..    cells: Op
+00000240: 7469 6f6e 616c 5b4c 6973 745b 416e 6e6f  tional[List[Anno
+00000250: 7461 7469 6f6e 4365 6c6c 5d5d 0d0a 0d0a  tationCell]]....
+00000260: 416e 6e6f 7461 7469 6f6e 5061 6765 5363  AnnotationPageSc
+00000270: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000280: 656d 6128 416e 6e6f 7461 7469 6f6e 5061  ema(AnnotationPa
+00000290: 6765 2c20 6261 7365 5f73 6368 656d 613d  ge, base_schema=
+000002a0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+000002b0: 0a                                       .
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/answer.py` & `semantha_sdk-5.5.0/semantha_sdk/model/answer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.answer_reference import AnswerReference
-from typing import List, Optional
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class Answer(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	answer: Optional[str]
-	references: Optional[List[AnswerReference]]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    answer: Optional[str]
+    references: Optional[List[AnswerReference]]
+
 AnswerSchema = class_schema(Answer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.5.0/semantha_sdk/model/current_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2041 6e73  True)..class Ans
-000000f0: 7765 7252 6566 6572 656e 6365 2853 656d  werReference(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 0922 2222 2061 7574 686f 7220  ):...""" author 
-00000120: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000130: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000140: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-00000150: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000160: 0a09 6964 3a20 4f70 7469 6f6e 616c 5b73  ..id: Optional[s
-00000170: 7472 5d0d 0a09 6e61 6d65 3a20 4f70 7469  tr]...name: Opti
-00000180: 6f6e 616c 5b73 7472 5d0d 0a09 636f 6e74  onal[str]...cont
-00000190: 656e 743a 204f 7074 696f 6e61 6c5b 7374  ent: Optional[st
-000001a0: 725d 0d0a 096d 6574 6164 6174 613a 204f  r]...metadata: O
-000001b0: 7074 696f 6e61 6c5b 7374 725d 0d0a 090d  ptional[str]....
-000001c0: 0a09 0d0a 416e 7377 6572 5265 6665 7265  ....AnswerRefere
-000001d0: 6e63 6553 6368 656d 6120 3d20 636c 6173  nceSchema = clas
-000001e0: 735f 7363 6865 6d61 2841 6e73 7765 7252  s_schema(AnswerR
-000001f0: 6566 6572 656e 6365 2c20 6261 7365 5f73  eference, base_s
-00000200: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
-00000210: 6865 6d61 290d 0a                        hema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000100: 636c 6173 7320 4375 7272 656e 7455 7365  class CurrentUse
+00000110: 7228 5365 6d61 6e74 6861 4d6f 6465 6c45  r(SemanthaModelE
+00000120: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000130: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000140: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000150: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000160: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000170: 6c79 2120 2222 220d 0a20 2020 206e 616d  ly! """..    nam
+00000180: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00000190: 0d0a 2020 2020 7661 6c69 645f 756e 7469  ..    valid_unti
+000001a0: 6c3a 204f 7074 696f 6e61 6c5b 696e 745d  l: Optional[int]
+000001b0: 0d0a 2020 2020 726f 6c65 733a 204f 7074  ..    roles: Opt
+000001c0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+000001d0: 0d0a 0d0a 4375 7272 656e 7455 7365 7253  ....CurrentUserS
+000001e0: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+000001f0: 6865 6d61 2843 7572 7265 6e74 5573 6572  hema(CurrentUser
+00000200: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000210: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.5.0/semantha_sdk/model/extraction_reference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4c69 7374 2c20 4f70 7469 6f6e 616c 0d0a  List, Optional..
-000000d0: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
-000000e0: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
-000000f0: 7373 2042 6f6f 7374 576f 7264 2853 656d  ss BoostWord(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 0922 2222 2061 7574 686f 7220  ):...""" author 
-00000120: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000130: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000140: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-00000150: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000160: 0a09 6964 3a20 4f70 7469 6f6e 616c 5b73  ..id: Optional[s
-00000170: 7472 5d0d 0a09 776f 7264 3a20 4f70 7469  tr]...word: Opti
-00000180: 6f6e 616c 5b73 7472 5d0d 0a09 7265 6765  onal[str]...rege
-00000190: 783a 204f 7074 696f 6e61 6c5b 7374 725d  x: Optional[str]
-000001a0: 0d0a 0974 6167 733a 204f 7074 696f 6e61  ...tags: Optiona
-000001b0: 6c5b 4c69 7374 5b73 7472 5d5d 0d0a 096c  l[List[str]]...l
-000001c0: 6162 656c 3a20 4f70 7469 6f6e 616c 5b73  abel: Optional[s
-000001d0: 7472 5d0d 0a09 0d0a 090d 0a42 6f6f 7374  tr]........Boost
-000001e0: 576f 7264 5363 6865 6d61 203d 2063 6c61  WordSchema = cla
-000001f0: 7373 5f73 6368 656d 6128 426f 6f73 7457  ss_schema(BoostW
-00000200: 6f72 642c 2062 6173 655f 7363 6865 6d61  ord, base_schema
-00000210: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-00000220: 0d0a                                     ..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
+000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+000000e0: 5472 7565 290d 0a63 6c61 7373 2045 7874  True)..class Ext
+000000f0: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
+00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000110: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+00000160: 7921 2022 2222 0d0a 2020 2020 646f 6375  y! """..    docu
+00000170: 6d65 6e74 5f69 643a 204f 7074 696f 6e61  ment_id: Optiona
+00000180: 6c5b 7374 725d 0d0a 2020 2020 7369 6d69  l[str]..    simi
+00000190: 6c61 7269 7479 3a20 4f70 7469 6f6e 616c  larity: Optional
+000001a0: 5b66 6c6f 6174 5d0d 0a20 2020 2075 7365  [float]..    use
+000001b0: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
+000001c0: 5d0d 0a0d 0a45 7874 7261 6374 696f 6e52  ]....ExtractionR
+000001d0: 6566 6572 656e 6365 5363 6865 6d61 203d  eferenceSchema =
+000001e0: 2063 6c61 7373 5f73 6368 656d 6128 4578   class_schema(Ex
+000001f0: 7472 6163 7469 6f6e 5265 6665 7265 6e63  tractionReferenc
+00000200: 652c 2062 6173 655f 7363 6865 6d61 3d53  e, base_schema=S
+00000210: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.5.0/semantha_sdk/model/class_bulk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e6c 6162 656c 2069 6d70 6f72  odel.label impor
-000000d0: 7420 4c61 6265 6c0d 0a66 726f 6d20 7365  t Label..from se
-000000e0: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
-000000f0: 2e6d 6574 6164 6174 615f 7661 6c75 6520  .metadata_value 
-00000100: 696d 706f 7274 204d 6574 6164 6174 6156  import MetadataV
-00000110: 616c 7565 0d0a 6672 6f6d 2074 7970 696e  alue..from typin
-00000120: 6720 696d 706f 7274 204c 6973 742c 204f  g import List, O
-00000130: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
-00000140: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
-00000150: 7275 6529 0d0a 636c 6173 7320 436c 6173  rue)..class Clas
-00000160: 7342 756c 6b28 5365 6d61 6e74 6861 4d6f  sBulk(SemanthaMo
-00000170: 6465 6c45 6e74 6974 7929 3a0d 0a09 2222  delEntity):...""
-00000180: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000190: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-000001a0: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-000001b0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001c0: 6c6c 7921 2022 2222 0d0a 0969 643a 204f  lly! """...id: O
-000001d0: 7074 696f 6e61 6c5b 7374 725d 0d0a 096e  ptional[str]...n
-000001e0: 616d 653a 2073 7472 0d0a 0972 6561 645f  ame: str...read_
-000001f0: 6f6e 6c79 3a20 4f70 7469 6f6e 616c 5b62  only: Optional[b
-00000200: 6f6f 6c5d 0d0a 0966 756e 6374 696f 6e61  ool]...functiona
-00000210: 6c3a 204f 7074 696f 6e61 6c5b 626f 6f6c  l: Optional[bool
-00000220: 5d0d 0a09 6c61 6265 6c73 3a20 4f70 7469  ]...labels: Opti
-00000230: 6f6e 616c 5b4c 6973 745b 4c61 6265 6c5d  onal[List[Label]
-00000240: 5d0d 0a09 6d65 7461 6461 7461 3a20 4f70  ]...metadata: Op
-00000250: 7469 6f6e 616c 5b4c 6973 745b 4d65 7461  tional[List[Meta
-00000260: 6461 7461 5661 6c75 655d 5d0d 0a09 636f  dataValue]]...co
-00000270: 6d6d 656e 743a 204f 7074 696f 6e61 6c5b  mment: Optional[
-00000280: 7374 725d 0d0a 0964 6174 6174 7970 653a  str]...datatype:
-00000290: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000002a0: 0961 7474 7269 6275 7465 5f69 6473 3a20  .attribute_ids: 
-000002b0: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-000002c0: 725d 5d0d 0a09 7265 6c65 7661 6e74 5f66  r]]...relevant_f
-000002d0: 6f72 5f72 656c 6174 696f 6e3a 204f 7074  or_relation: Opt
-000002e0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a09 6f62  ional[bool]...ob
-000002f0: 6a65 6374 5f70 726f 7065 7274 795f 6964  ject_property_id
-00000300: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000310: 0a09 6f62 6a65 6374 5f70 726f 7065 7274  ..object_propert
-00000320: 795f 7479 7065 5f69 643a 204f 7074 696f  y_type_id: Optio
-00000330: 6e61 6c5b 7374 725d 0d0a 0970 6172 656e  nal[str]...paren
-00000340: 745f 6964 3a20 4f70 7469 6f6e 616c 5b73  t_id: Optional[s
-00000350: 7472 5d0d 0a09 0d0a 090d 0a43 6c61 7373  tr]........Class
-00000360: 4275 6c6b 5363 6865 6d61 203d 2063 6c61  BulkSchema = cla
-00000370: 7373 5f73 6368 656d 6128 436c 6173 7342  ss_schema(ClassB
-00000380: 756c 6b2c 2062 6173 655f 7363 6865 6d61  ulk, base_schema
-00000390: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
-000003a0: 0d0a                                     ..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
+000000d0: 6f72 7420 4c61 6265 6c0d 0a0d 0a66 726f  ort Label....fro
+000000e0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+000000f0: 6f64 656c 2e6d 6574 6164 6174 615f 7661  odel.metadata_va
+00000100: 6c75 6520 696d 706f 7274 204d 6574 6164  lue import Metad
+00000110: 6174 6156 616c 7565 0d0a 0d0a 6672 6f6d  ataValue....from
+00000120: 2074 7970 696e 6720 696d 706f 7274 204c   typing import L
+00000130: 6973 740d 0a66 726f 6d20 7479 7069 6e67  ist..from typing
+00000140: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
+00000150: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
+00000160: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
+00000170: 7373 2043 6c61 7373 4275 6c6b 2853 656d  ss ClassBulk(Sem
+00000180: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000190: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+000001a0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+000001b0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+000001c0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+000001d0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+000001e0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+000001f0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 206e  onal[str]..    n
+00000200: 616d 653a 2073 7472 0d0a 2020 2020 7265  ame: str..    re
+00000210: 6164 5f6f 6e6c 793a 204f 7074 696f 6e61  ad_only: Optiona
+00000220: 6c5b 626f 6f6c 5d0d 0a20 2020 2066 756e  l[bool]..    fun
+00000230: 6374 696f 6e61 6c3a 204f 7074 696f 6e61  ctional: Optiona
+00000240: 6c5b 626f 6f6c 5d0d 0a20 2020 206c 6162  l[bool]..    lab
+00000250: 656c 733a 204f 7074 696f 6e61 6c5b 4c69  els: Optional[Li
+00000260: 7374 5b4c 6162 656c 5d5d 0d0a 2020 2020  st[Label]]..    
+00000270: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
+00000280: 616c 5b4c 6973 745b 4d65 7461 6461 7461  al[List[Metadata
+00000290: 5661 6c75 655d 5d0d 0a20 2020 2063 6f6d  Value]]..    com
+000002a0: 6d65 6e74 3a20 4f70 7469 6f6e 616c 5b73  ment: Optional[s
+000002b0: 7472 5d0d 0a20 2020 2064 6174 6174 7970  tr]..    datatyp
+000002c0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+000002d0: 0d0a 2020 2020 6174 7472 6962 7574 655f  ..    attribute_
+000002e0: 6964 733a 204f 7074 696f 6e61 6c5b 4c69  ids: Optional[Li
+000002f0: 7374 5b73 7472 5d5d 0d0a 2020 2020 7265  st[str]]..    re
+00000300: 6c65 7661 6e74 5f66 6f72 5f72 656c 6174  levant_for_relat
+00000310: 696f 6e3a 204f 7074 696f 6e61 6c5b 626f  ion: Optional[bo
+00000320: 6f6c 5d0d 0a20 2020 206f 626a 6563 745f  ol]..    object_
+00000330: 7072 6f70 6572 7479 5f69 643a 204f 7074  property_id: Opt
+00000340: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000350: 6f62 6a65 6374 5f70 726f 7065 7274 795f  object_property_
+00000360: 7479 7065 5f69 643a 204f 7074 696f 6e61  type_id: Optiona
+00000370: 6c5b 7374 725d 0d0a 2020 2020 7061 7265  l[str]..    pare
+00000380: 6e74 5f69 643a 204f 7074 696f 6e61 6c5b  nt_id: Optional[
+00000390: 7374 725d 0d0a 0d0a 436c 6173 7342 756c  str]....ClassBul
+000003a0: 6b53 6368 656d 6120 3d20 636c 6173 735f  kSchema = class_
+000003b0: 7363 6865 6d61 2843 6c61 7373 4275 6c6b  schema(ClassBulk
+000003c0: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+000003d0: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.5.0/semantha_sdk/model/clustering_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.document_cluster import DocumentCluster
+
 from semantha_sdk.model.plotly_chart import PlotlyChart
-from typing import Dict, List, Optional
 
+from typing import Dict
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class ClusteringResponse(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	clusters: Optional[List[DocumentCluster]]
-	plotly: Optional[Dict[str, PlotlyChart]]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    clusters: Optional[List[DocumentCluster]]
+    plotly: Optional[Dict[str, PlotlyChart]]
+
 ClusteringResponseSchema = class_schema(ClusteringResponse, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.5.0/semantha_sdk/model/document_class_bulk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,25 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.extraction_area import ExtractionArea
-from semantha_sdk.model.extraction_reference import ExtractionReference
-from semantha_sdk.model.finding import Finding
-from semantha_sdk.model.label import Label
-from semantha_sdk.model.metadata import Metadata
-from typing import List, Optional
-
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
-class ComplexProperty(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	name: str
-	value: str
-	label: Optional[str]
-	id: Optional[str]
-	class_id: Optional[str]
-	relation_id: Optional[str]
-	original_value: Optional[str]
-	extracted_value: Optional[str]
-	datatype: Optional[str]
-	labels: Optional[List[Label]]
-	metadata: Optional[List[Metadata]]
-	extraction_area: Optional[ExtractionArea]
-	findings: Optional[List[Finding]]
-	references: Optional[List[ExtractionReference]]
-	
-	
-ComplexPropertySchema = class_schema(ComplexProperty, base_schema=SemanthaSchema)
+class DocumentClassBulk(SemanthaModelEntity):
+    """ author semantha, this is a generated class do not change manually! """
+    id: Optional[str]
+    name: str
+    document_ids: Optional[List[str]]
+    sub_classes: Optional[List["DocumentClassBulk"]]
+    tags: Optional[List[str]]
+    color: Optional[str]
+    comment: Optional[str]
+    created: Optional[int]
+    updated: Optional[int]
+    metata: Optional[str]
+
+DocumentClassBulkSchema = class_schema(DocumentClassBulk, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/current_user.py` & `semantha_sdk-5.5.0/semantha_sdk/model/row.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from typing import List, Optional
+from semantha_sdk.model.table_cell import TableCell
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
-class CurrentUser(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	name: Optional[str]
-	valid_until: Optional[int]
-	roles: Optional[List[str]]
-	
-	
-CurrentUserSchema = class_schema(CurrentUser, base_schema=SemanthaSchema)
+class Row(SemanthaModelEntity):
+    """ author semantha, this is a generated class do not change manually! """
+    cells: Optional[List[TableCell]]
+
+RowSchema = class_schema(Row, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/data_property.py` & `semantha_sdk-5.5.0/semantha_sdk/model/data_property.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e6c 6162 656c 2069 6d70 6f72  odel.label impor
-000000d0: 7420 4c61 6265 6c0d 0a66 726f 6d20 7479  t Label..from ty
-000000e0: 7069 6e67 2069 6d70 6f72 7420 4c69 7374  ping import List
-000000f0: 2c20 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  , Optional......
-00000100: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-00000110: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
-00000120: 6174 6150 726f 7065 7274 7928 5365 6d61  ataProperty(Sema
-00000130: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
-00000140: 3a0d 0a09 2222 2220 6175 7468 6f72 2073  :...""" author s
-00000150: 656d 616e 7468 612c 2074 6869 7320 6973  emantha, this is
-00000160: 2061 2067 656e 6572 6174 6564 2063 6c61   a generated cla
-00000170: 7373 2064 6f20 6e6f 7420 6368 616e 6765  ss do not change
-00000180: 206d 616e 7561 6c6c 7921 2022 2222 0d0a   manually! """..
-00000190: 0969 643a 204f 7074 696f 6e61 6c5b 7374  .id: Optional[st
-000001a0: 725d 0d0a 096e 616d 653a 2073 7472 0d0a  r]...name: str..
-000001b0: 0972 6561 645f 6f6e 6c79 3a20 4f70 7469  .read_only: Opti
-000001c0: 6f6e 616c 5b62 6f6f 6c5d 0d0a 0966 756e  onal[bool]...fun
-000001d0: 6374 696f 6e61 6c3a 204f 7074 696f 6e61  ctional: Optiona
-000001e0: 6c5b 626f 6f6c 5d0d 0a09 6c61 6265 6c73  l[bool]...labels
-000001f0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000200: 4c61 6265 6c5d 5d0d 0a09 0d0a 090d 0a44  Label]]........D
-00000210: 6174 6150 726f 7065 7274 7953 6368 656d  ataPropertySchem
-00000220: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-00000230: 2844 6174 6150 726f 7065 7274 792c 2062  (DataProperty, b
-00000240: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-00000250: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e6c 6162 656c 2069 6d70  .model.label imp
+000000d0: 6f72 7420 4c61 6265 6c0d 0a0d 0a66 726f  ort Label....fro
+000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+000000f0: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000100: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000110: 6c0d 0a0d 0a40 6461 7461 636c 6173 7328  l....@dataclass(
+00000120: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+00000130: 6173 7320 4461 7461 5072 6f70 6572 7479  ass DataProperty
+00000140: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000150: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000160: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000170: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000180: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000190: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+000001a0: 7921 2022 2222 0d0a 2020 2020 6964 3a20  y! """..    id: 
+000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001c0: 2020 206e 616d 653a 2073 7472 0d0a 2020     name: str..  
+000001d0: 2020 7265 6164 5f6f 6e6c 793a 204f 7074    read_only: Opt
+000001e0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
+000001f0: 2066 756e 6374 696f 6e61 6c3a 204f 7074   functional: Opt
+00000200: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
+00000210: 206c 6162 656c 733a 204f 7074 696f 6e61   labels: Optiona
+00000220: 6c5b 4c69 7374 5b4c 6162 656c 5d5d 0d0a  l[List[Label]]..
+00000230: 0d0a 4461 7461 5072 6f70 6572 7479 5363  ..DataPropertySc
+00000240: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000250: 656d 6128 4461 7461 5072 6f70 6572 7479  ema(DataProperty
+00000260: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000270: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/distance.py` & `semantha_sdk-5.5.0/semantha_sdk/model/distance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
 000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
 000000e0: 5472 7565 290d 0a63 6c61 7373 2044 6973  True)..class Dis
 000000f0: 7461 6e63 6528 5365 6d61 6e74 6861 4d6f  tance(SemanthaMo
-00000100: 6465 6c45 6e74 6974 7929 3a0d 0a09 2222  delEntity):...""
-00000110: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000120: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-00000130: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-00000140: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-00000150: 6c6c 7921 2022 2222 0d0a 0974 6f70 3a20  lly! """...top: 
-00000160: 4f70 7469 6f6e 616c 5b66 6c6f 6174 5d0d  Optional[float].
-00000170: 0a09 626f 7474 6f6d 3a20 4f70 7469 6f6e  ..bottom: Option
-00000180: 616c 5b66 6c6f 6174 5d0d 0a09 6c65 6674  al[float]...left
-00000190: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-000001a0: 5d0d 0a09 7269 6768 743a 204f 7074 696f  ]...right: Optio
-000001b0: 6e61 6c5b 666c 6f61 745d 0d0a 090d 0a09  nal[float]......
-000001c0: 0d0a 4469 7374 616e 6365 5363 6865 6d61  ..DistanceSchema
-000001d0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-000001e0: 4469 7374 616e 6365 2c20 6261 7365 5f73  Distance, base_s
-000001f0: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
-00000200: 6865 6d61 290d 0a                        hema)..
+00000100: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000110: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000120: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000130: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000140: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+00000150: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+00000160: 2074 6f70 3a20 4f70 7469 6f6e 616c 5b66   top: Optional[f
+00000170: 6c6f 6174 5d0d 0a20 2020 2062 6f74 746f  loat]..    botto
+00000180: 6d3a 204f 7074 696f 6e61 6c5b 666c 6f61  m: Optional[floa
+00000190: 745d 0d0a 2020 2020 6c65 6674 3a20 4f70  t]..    left: Op
+000001a0: 7469 6f6e 616c 5b66 6c6f 6174 5d0d 0a20  tional[float].. 
+000001b0: 2020 2072 6967 6874 3a20 4f70 7469 6f6e     right: Option
+000001c0: 616c 5b66 6c6f 6174 5d0d 0a0d 0a44 6973  al[float]....Dis
+000001d0: 7461 6e63 6553 6368 656d 6120 3d20 636c  tanceSchema = cl
+000001e0: 6173 735f 7363 6865 6d61 2844 6973 7461  ass_schema(Dista
+000001f0: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
+00000200: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000210: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document.py` & `semantha_sdk-5.5.0/semantha_sdk/model/model_instance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,99 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e65 6e74 6974 7920 696d 706f  odel.entity impo
-000000d0: 7274 2045 6e74 6974 790d 0a66 726f 6d20  rt Entity..from 
-000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-000000f0: 656c 2e70 6167 6520 696d 706f 7274 2050  el.page import P
-00000100: 6167 650d 0a66 726f 6d20 7365 6d61 6e74  age..from semant
-00000110: 6861 5f73 646b 2e6d 6f64 656c 2e72 6566  ha_sdk.model.ref
-00000120: 6572 656e 6365 2069 6d70 6f72 7420 5265  erence import Re
-00000130: 6665 7265 6e63 650d 0a66 726f 6d20 7479  ference..from ty
-00000140: 7069 6e67 2069 6d70 6f72 7420 4c69 7374  ping import List
-00000150: 2c20 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  , Optional......
-00000160: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-00000170: 6e3d 5472 7565 290d 0a63 6c61 7373 2044  n=True)..class D
-00000180: 6f63 756d 656e 7428 5365 6d61 6e74 6861  ocument(Semantha
-00000190: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a09  ModelEntity):...
-000001a0: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-000001b0: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-000001c0: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-000001d0: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001e0: 7561 6c6c 7921 2022 2222 0d0a 0969 643a  ually! """...id:
-000001f0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000200: 096e 616d 653a 204f 7074 696f 6e61 6c5b  .name: Optional[
-00000210: 7374 725d 0d0a 0974 6167 733a 204f 7074  str]...tags: Opt
-00000220: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-00000230: 0d0a 096d 6574 6164 6174 613a 204f 7074  ...metadata: Opt
-00000240: 696f 6e61 6c5b 7374 725d 0d0a 0966 696c  ional[str]...fil
-00000250: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
-00000260: 7374 725d 0d0a 0963 7265 6174 6564 3a20  str]...created: 
-00000270: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a09  Optional[int]...
-00000280: 7570 6461 7465 643a 204f 7074 696f 6e61  updated: Optiona
-00000290: 6c5b 696e 745d 0d0a 0970 726f 6365 7373  l[int]...process
-000002a0: 6564 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ed: Optional[boo
-000002b0: 6c5d 0d0a 096c 616e 673a 204f 7074 696f  l]...lang: Optio
-000002c0: 6e61 6c5b 7374 725d 0d0a 0963 6f6e 7465  nal[str]...conte
-000002d0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-000002e0: 5d0d 0a09 646f 6375 6d65 6e74 5f63 6c61  ]...document_cla
-000002f0: 7373 3a20 4f70 7469 6f6e 616c 5b45 6e74  ss: Optional[Ent
-00000300: 6974 795d 0d0a 0964 6572 6976 6564 5f74  ity]...derived_t
-00000310: 6167 733a 204f 7074 696f 6e61 6c5b 4c69  ags: Optional[Li
-00000320: 7374 5b73 7472 5d5d 0d0a 0963 6f6c 6f72  st[str]]...color
-00000330: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000340: 0a09 6465 7269 7665 645f 636f 6c6f 723a  ..derived_color:
-00000350: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000360: 0963 6f6d 6d65 6e74 3a20 4f70 7469 6f6e  .comment: Option
-00000370: 616c 5b73 7472 5d0d 0a09 6465 7269 7665  al[str]...derive
-00000380: 645f 636f 6d6d 656e 743a 204f 7074 696f  d_comment: Optio
-00000390: 6e61 6c5b 7374 725d 0d0a 0963 6f6e 7465  nal[str]...conte
-000003a0: 6e74 5f70 7265 7669 6577 3a20 4f70 7469  nt_preview: Opti
-000003b0: 6f6e 616c 5b73 7472 5d0d 0a09 7061 6765  onal[str]...page
-000003c0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-000003d0: 5b50 6167 655d 5d0d 0a09 7265 6665 7265  [Page]]...refere
-000003e0: 6e63 6573 3a20 4f70 7469 6f6e 616c 5b4c  nces: Optional[L
-000003f0: 6973 745b 5265 6665 7265 6e63 655d 5d0d  ist[Reference]].
-00000400: 0a09 696d 6167 655f 7061 6765 733a 204f  ..image_pages: O
-00000410: 7074 696f 6e61 6c5b 4c69 7374 5b73 7472  ptional[List[str
-00000420: 5d5d 0d0a 0964 6f63 756d 656e 745f 636c  ]]...document_cl
-00000430: 6173 735f 6964 3a20 4f70 7469 6f6e 616c  ass_id: Optional
-00000440: 5b73 7472 5d0d 0a09 0d0a 090d 0a09 6465  [str].........de
-00000450: 6620 5f5f 6861 7368 5f5f 2873 656c 6629  f __hash__(self)
-00000460: 3a0d 0a09 0972 6574 7572 6e20 7365 6c66  :....return self
-00000470: 2e69 640d 0a09 0d0a 446f 6375 6d65 6e74  .id.....Document
-00000480: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-00000490: 6368 656d 6128 446f 6375 6d65 6e74 2c20  chema(Document, 
-000004a0: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
-000004b0: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e63 6f6d 706c 6578 5f70  .model.complex_p
+000000d0: 726f 7065 7274 7920 696d 706f 7274 2043  roperty import C
+000000e0: 6f6d 706c 6578 5072 6f70 6572 7479 0d0a  omplexProperty..
+000000f0: 0d0a 6672 6f6d 2073 656d 616e 7468 615f  ..from semantha_
+00000100: 7364 6b2e 6d6f 6465 6c2e 6578 7472 6163  sdk.model.extrac
+00000110: 7469 6f6e 5f72 6566 6572 656e 6365 2069  tion_reference i
+00000120: 6d70 6f72 7420 4578 7472 6163 7469 6f6e  mport Extraction
+00000130: 5265 6665 7265 6e63 650d 0a0d 0a66 726f  Reference....fro
+00000140: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+00000150: 6f64 656c 2e66 696c 655f 7265 6665 7265  odel.file_refere
+00000160: 6e63 6520 696d 706f 7274 2046 696c 6552  nce import FileR
+00000170: 6566 6572 656e 6365 0d0a 0d0a 6672 6f6d  eference....from
+00000180: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
+00000190: 6465 6c2e 6669 6e64 696e 6720 696d 706f  del.finding impo
+000001a0: 7274 2046 696e 6469 6e67 0d0a 0d0a 6672  rt Finding....fr
+000001b0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
+000001c0: 6d6f 6465 6c2e 6c61 6265 6c20 696d 706f  model.label impo
+000001d0: 7274 204c 6162 656c 0d0a 0d0a 6672 6f6d  rt Label....from
+000001e0: 2073 656d 616e 7468 615f 7364 6b2e 6d6f   semantha_sdk.mo
+000001f0: 6465 6c2e 6c69 6e6b 6564 5f69 6e73 7461  del.linked_insta
+00000200: 6e63 6520 696d 706f 7274 204c 696e 6b65  nce import Linke
+00000210: 6449 6e73 7461 6e63 650d 0a0d 0a66 726f  dInstance....fro
+00000220: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+00000230: 6f64 656c 2e6d 6574 6164 6174 6120 696d  odel.metadata im
+00000240: 706f 7274 204d 6574 6164 6174 610d 0a0d  port Metadata...
+00000250: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
+00000260: 646b 2e6d 6f64 656c 2e73 696d 706c 655f  dk.model.simple_
+00000270: 7072 6f70 6572 7479 2069 6d70 6f72 7420  property import 
+00000280: 5369 6d70 6c65 5072 6f70 6572 7479 0d0a  SimpleProperty..
+00000290: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+000002a0: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
+000002b0: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+000002c0: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
+000002d0: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+000002e0: 290d 0a63 6c61 7373 204d 6f64 656c 496e  )..class ModelIn
+000002f0: 7374 616e 6365 2853 656d 616e 7468 614d  stance(SemanthaM
+00000300: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
+00000310: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
+00000320: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
+00000330: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
+00000340: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
+00000350: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
+00000360: 2020 6964 3a20 4f70 7469 6f6e 616c 5b73    id: Optional[s
+00000370: 7472 5d0d 0a20 2020 206e 616d 653a 204f  tr]..    name: O
+00000380: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000390: 2020 636c 6173 735f 6964 3a20 7374 720d    class_id: str.
+000003a0: 0a20 2020 2072 656c 6174 696f 6e5f 6964  .    relation_id
+000003b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000003c0: 0a20 2020 2074 7970 653a 204f 7074 696f  .    type: Optio
+000003d0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6967  nal[str]..    ig
+000003e0: 6e6f 7265 5f69 6d70 6f72 743a 204f 7074  nore_import: Opt
+000003f0: 696f 6e61 6c5b 626f 6f6c 5d0d 0a20 2020  ional[bool]..   
+00000400: 2073 696d 706c 655f 7072 6f70 6572 7469   simple_properti
+00000410: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
+00000420: 745b 5369 6d70 6c65 5072 6f70 6572 7479  t[SimpleProperty
+00000430: 5d5d 0d0a 2020 2020 6d65 7461 6461 7461  ]]..    metadata
+00000440: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+00000450: 4d65 7461 6461 7461 5d5d 0d0a 2020 2020  Metadata]]..    
+00000460: 7175 616c 6966 6965 645f 6e61 6d65 3a20  qualified_name: 
+00000470: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000480: 2020 2065 7874 7261 6374 6f72 5f63 6c61     extractor_cla
+00000490: 7373 5f69 6473 3a20 4f70 7469 6f6e 616c  ss_ids: Optional
+000004a0: 5b4c 6973 745b 7374 725d 5d0d 0a20 2020  [List[str]]..   
+000004b0: 206c 6162 656c 3a20 4f70 7469 6f6e 616c   label: Optional
+000004c0: 5b73 7472 5d0d 0a20 2020 206c 6162 656c  [str]..    label
+000004d0: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
+000004e0: 5b4c 6162 656c 5d5d 0d0a 2020 2020 6669  [Label]]..    fi
+000004f0: 6c65 3a20 4f70 7469 6f6e 616c 5b46 696c  le: Optional[Fil
+00000500: 6552 6566 6572 656e 6365 5d0d 0a20 2020  eReference]..   
+00000510: 2063 6f6d 706c 6578 5f70 726f 7065 7274   complex_propert
+00000520: 6965 733a 204f 7074 696f 6e61 6c5b 4c69  ies: Optional[Li
+00000530: 7374 5b43 6f6d 706c 6578 5072 6f70 6572  st[ComplexProper
+00000540: 7479 5d5d 0d0a 2020 2020 6669 6e64 696e  ty]]..    findin
+00000550: 6773 3a20 4f70 7469 6f6e 616c 5b4c 6973  gs: Optional[Lis
+00000560: 745b 4669 6e64 696e 675d 5d0d 0a20 2020  t[Finding]]..   
+00000570: 2072 6566 6572 656e 6365 733a 204f 7074   references: Opt
+00000580: 696f 6e61 6c5b 4c69 7374 5b45 7874 7261  ional[List[Extra
+00000590: 6374 696f 6e52 6566 6572 656e 6365 5d5d  ctionReference]]
+000005a0: 0d0a 2020 2020 6c69 6e6b 6564 5f69 6e73  ..    linked_ins
+000005b0: 7461 6e63 6573 3a20 4f70 7469 6f6e 616c  tances: Optional
+000005c0: 5b4c 6973 745b 4c69 6e6b 6564 496e 7374  [List[LinkedInst
+000005d0: 616e 6365 5d5d 0d0a 0d0a 4d6f 6465 6c49  ance]]....ModelI
+000005e0: 6e73 7461 6e63 6553 6368 656d 6120 3d20  nstanceSchema = 
+000005f0: 636c 6173 735f 7363 6865 6d61 284d 6f64  class_schema(Mod
+00000600: 656c 496e 7374 616e 6365 2c20 6261 7365  elInstance, base
+00000610: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+00000620: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document_class.py` & `semantha_sdk-5.5.0/semantha_sdk/model/document_information.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,68 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e64 6f63 756d 656e 745f 636c  odel.document_cl
-000000d0: 6173 735f 6e6f 6465 2069 6d70 6f72 7420  ass_node import 
-000000e0: 446f 6375 6d65 6e74 436c 6173 734e 6f64  DocumentClassNod
-000000f0: 650d 0a66 726f 6d20 7479 7069 6e67 2069  e..from typing i
-00000100: 6d70 6f72 7420 4c69 7374 2c20 4f70 7469  mport List, Opti
-00000110: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
-00000120: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
-00000130: 290d 0a63 6c61 7373 2044 6f63 756d 656e  )..class Documen
-00000140: 7443 6c61 7373 2853 656d 616e 7468 614d  tClass(SemanthaM
-00000150: 6f64 656c 456e 7469 7479 293a 0d0a 0922  odelEntity):..."
-00000160: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
-00000170: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
-00000180: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
-00000190: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
-000001a0: 616c 6c79 2120 2222 220d 0a09 6964 3a20  ally! """...id: 
-000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a09  Optional[str]...
-000001c0: 6e61 6d65 3a20 7374 720d 0a09 7061 7265  name: str...pare
-000001d0: 6e74 5f69 643a 204f 7074 696f 6e61 6c5b  nt_id: Optional[
-000001e0: 7374 725d 0d0a 096d 6574 6164 6174 613a  str]...metadata:
-000001f0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000200: 0964 6f63 756d 656e 7473 5f63 6f75 6e74  .documents_count
-00000210: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d0d  : Optional[int].
-00000220: 0a09 7375 625f 636c 6173 7365 733a 204f  ..sub_classes: O
-00000230: 7074 696f 6e61 6c5b 4c69 7374 5b44 6f63  ptional[List[Doc
-00000240: 756d 656e 7443 6c61 7373 4e6f 6465 5d5d  umentClassNode]]
-00000250: 0d0a 0974 6167 733a 204f 7074 696f 6e61  ...tags: Optiona
-00000260: 6c5b 4c69 7374 5b73 7472 5d5d 0d0a 0964  l[List[str]]...d
-00000270: 6572 6976 6564 5f74 6167 733a 204f 7074  erived_tags: Opt
-00000280: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-00000290: 0d0a 0963 6f6c 6f72 3a20 4f70 7469 6f6e  ...color: Option
-000002a0: 616c 5b73 7472 5d0d 0a09 6465 7269 7665  al[str]...derive
-000002b0: 645f 636f 6c6f 723a 204f 7074 696f 6e61  d_color: Optiona
-000002c0: 6c5b 7374 725d 0d0a 0963 6f6d 6d65 6e74  l[str]...comment
-000002d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000002e0: 0a09 6465 7269 7665 645f 636f 6d6d 656e  ..derived_commen
-000002f0: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-00000300: 0d0a 0963 7265 6174 6564 3a20 4f70 7469  ...created: Opti
-00000310: 6f6e 616c 5b69 6e74 5d0d 0a09 7570 6461  onal[int]...upda
-00000320: 7465 643a 204f 7074 696f 6e61 6c5b 696e  ted: Optional[in
-00000330: 745d 0d0a 0964 6572 6976 6564 5f6d 6574  t]...derived_met
-00000340: 6164 6174 613a 204f 7074 696f 6e61 6c5b  adata: Optional[
-00000350: 7374 725d 0d0a 090d 0a09 0d0a 446f 6375  str]........Docu
-00000360: 6d65 6e74 436c 6173 7353 6368 656d 6120  mentClassSchema 
-00000370: 3d20 636c 6173 735f 7363 6865 6d61 2844  = class_schema(D
-00000380: 6f63 756d 656e 7443 6c61 7373 2c20 6261  ocumentClass, ba
-00000390: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
-000003a0: 6861 5363 6865 6d61 290d 0a              haSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e65 6e74 6974 7920 696d  .model.entity im
+000000d0: 706f 7274 2045 6e74 6974 790d 0a0d 0a66  port Entity....f
+000000e0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000f0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+00000100: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+00000110: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+00000120: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000130: 636c 6173 7320 446f 6375 6d65 6e74 496e  class DocumentIn
+00000140: 666f 726d 6174 696f 6e28 5365 6d61 6e74  formation(Semant
+00000150: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
+00000160: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
+00000170: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
+00000180: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
+00000190: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
+000001a0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
+000001b0: 0a20 2020 2069 643a 204f 7074 696f 6e61  .    id: Optiona
+000001c0: 6c5b 7374 725d 0d0a 2020 2020 6e61 6d65  l[str]..    name
+000001d0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+000001e0: 0a20 2020 2074 6167 733a 204f 7074 696f  .    tags: Optio
+000001f0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 0d0a  nal[List[str]]..
+00000200: 2020 2020 6d65 7461 6461 7461 3a20 4f70      metadata: Op
+00000210: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000220: 2066 696c 656e 616d 653a 204f 7074 696f   filename: Optio
+00000230: 6e61 6c5b 7374 725d 0d0a 2020 2020 6372  nal[str]..    cr
+00000240: 6561 7465 643a 204f 7074 696f 6e61 6c5b  eated: Optional[
+00000250: 696e 745d 0d0a 2020 2020 7570 6461 7465  int]..    update
+00000260: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
+00000270: 0d0a 2020 2020 7072 6f63 6573 7365 643a  ..    processed:
+00000280: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
+00000290: 0a20 2020 206c 616e 673a 204f 7074 696f  .    lang: Optio
+000002a0: 6e61 6c5b 7374 725d 0d0a 2020 2020 636f  nal[str]..    co
+000002b0: 6e74 656e 743a 204f 7074 696f 6e61 6c5b  ntent: Optional[
+000002c0: 7374 725d 0d0a 2020 2020 646f 6375 6d65  str]..    docume
+000002d0: 6e74 5f63 6c61 7373 3a20 4f70 7469 6f6e  nt_class: Option
+000002e0: 616c 5b45 6e74 6974 795d 0d0a 2020 2020  al[Entity]..    
+000002f0: 6465 7269 7665 645f 7461 6773 3a20 4f70  derived_tags: Op
+00000300: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
+00000310: 5d0d 0a20 2020 2063 6f6c 6f72 3a20 4f70  ]..    color: Op
+00000320: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000330: 2064 6572 6976 6564 5f63 6f6c 6f72 3a20   derived_color: 
+00000340: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000350: 2020 2063 6f6d 6d65 6e74 3a20 4f70 7469     comment: Opti
+00000360: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2064  onal[str]..    d
+00000370: 6572 6976 6564 5f63 6f6d 6d65 6e74 3a20  erived_comment: 
+00000380: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000390: 2020 2063 6f6e 7465 6e74 5f70 7265 7669     content_previ
+000003a0: 6577 3a20 4f70 7469 6f6e 616c 5b73 7472  ew: Optional[str
+000003b0: 5d0d 0a20 2020 2064 6f63 756d 656e 745f  ]..    document_
+000003c0: 636c 6173 735f 6964 3a20 4f70 7469 6f6e  class_id: Option
+000003d0: 616c 5b73 7472 5d0d 0a0d 0a44 6f63 756d  al[str]....Docum
+000003e0: 656e 7449 6e66 6f72 6d61 7469 6f6e 5363  entInformationSc
+000003f0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000400: 656d 6128 446f 6375 6d65 6e74 496e 666f  ema(DocumentInfo
+00000410: 726d 6174 696f 6e2c 2062 6173 655f 7363  rmation, base_sc
+00000420: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
+00000430: 656d 6129 0d0a                           ema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.5.0/semantha_sdk/model/document_class.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,63 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4c69 7374 2c20 4f70 7469 6f6e 616c 0d0a  List, Optional..
-000000d0: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
-000000e0: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
-000000f0: 7373 2044 6f63 756d 656e 7443 6c61 7373  ss DocumentClass
-00000100: 4275 6c6b 2853 656d 616e 7468 614d 6f64  Bulk(SemanthaMod
-00000110: 656c 456e 7469 7479 293a 0d0a 0922 2222  elEntity):..."""
-00000120: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000130: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000140: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000150: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000160: 6c79 2120 2222 220d 0a09 6964 3a20 4f70  ly! """...id: Op
-00000170: 7469 6f6e 616c 5b73 7472 5d0d 0a09 6e61  tional[str]...na
-00000180: 6d65 3a20 7374 720d 0a09 646f 6375 6d65  me: str...docume
-00000190: 6e74 5f69 6473 3a20 4f70 7469 6f6e 616c  nt_ids: Optional
-000001a0: 5b4c 6973 745b 7374 725d 5d0d 0a09 7375  [List[str]]...su
-000001b0: 625f 636c 6173 7365 733a 204f 7074 696f  b_classes: Optio
-000001c0: 6e61 6c5b 4c69 7374 5b22 446f 6375 6d65  nal[List["Docume
-000001d0: 6e74 436c 6173 7342 756c 6b22 5d5d 0d0a  ntClassBulk"]]..
-000001e0: 0974 6167 733a 204f 7074 696f 6e61 6c5b  .tags: Optional[
-000001f0: 4c69 7374 5b73 7472 5d5d 0d0a 0963 6f6c  List[str]]...col
-00000200: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-00000210: 5d0d 0a09 636f 6d6d 656e 743a 204f 7074  ]...comment: Opt
-00000220: 696f 6e61 6c5b 7374 725d 0d0a 0963 7265  ional[str]...cre
-00000230: 6174 6564 3a20 4f70 7469 6f6e 616c 5b69  ated: Optional[i
-00000240: 6e74 5d0d 0a09 7570 6461 7465 643a 204f  nt]...updated: O
-00000250: 7074 696f 6e61 6c5b 696e 745d 0d0a 096d  ptional[int]...m
-00000260: 6574 6174 613a 204f 7074 696f 6e61 6c5b  etata: Optional[
-00000270: 7374 725d 0d0a 090d 0a09 0d0a 446f 6375  str]........Docu
-00000280: 6d65 6e74 436c 6173 7342 756c 6b53 6368  mentClassBulkSch
-00000290: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-000002a0: 6d61 2844 6f63 756d 656e 7443 6c61 7373  ma(DocumentClass
-000002b0: 4275 6c6b 2c20 6261 7365 5f73 6368 656d  Bulk, base_schem
-000002c0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-000002d0: 290d 0a                                  )..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
+000000d0: 636c 6173 735f 6e6f 6465 2069 6d70 6f72  class_node impor
+000000e0: 7420 446f 6375 6d65 6e74 436c 6173 734e  t DocumentClassN
+000000f0: 6f64 650d 0a0d 0a66 726f 6d20 7479 7069  ode....from typi
+00000100: 6e67 2069 6d70 6f72 7420 4c69 7374 0d0a  ng import List..
+00000110: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000120: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a40  rt Optional....@
+00000130: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000140: 3d54 7275 6529 0d0a 636c 6173 7320 446f  =True)..class Do
+00000150: 6375 6d65 6e74 436c 6173 7328 5365 6d61  cumentClass(Sema
+00000160: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000170: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000180: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000190: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+000001a0: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+000001b0: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+000001c0: 220d 0a20 2020 2069 643a 204f 7074 696f  "..    id: Optio
+000001d0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6e61  nal[str]..    na
+000001e0: 6d65 3a20 7374 720d 0a20 2020 2070 6172  me: str..    par
+000001f0: 656e 745f 6964 3a20 4f70 7469 6f6e 616c  ent_id: Optional
+00000200: 5b73 7472 5d0d 0a20 2020 206d 6574 6164  [str]..    metad
+00000210: 6174 613a 204f 7074 696f 6e61 6c5b 7374  ata: Optional[st
+00000220: 725d 0d0a 2020 2020 646f 6375 6d65 6e74  r]..    document
+00000230: 735f 636f 756e 743a 204f 7074 696f 6e61  s_count: Optiona
+00000240: 6c5b 696e 745d 0d0a 2020 2020 7375 625f  l[int]..    sub_
+00000250: 636c 6173 7365 733a 204f 7074 696f 6e61  classes: Optiona
+00000260: 6c5b 4c69 7374 5b44 6f63 756d 656e 7443  l[List[DocumentC
+00000270: 6c61 7373 4e6f 6465 5d5d 0d0a 2020 2020  lassNode]]..    
+00000280: 7461 6773 3a20 4f70 7469 6f6e 616c 5b4c  tags: Optional[L
+00000290: 6973 745b 7374 725d 5d0d 0a20 2020 2064  ist[str]]..    d
+000002a0: 6572 6976 6564 5f74 6167 733a 204f 7074  erived_tags: Opt
+000002b0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+000002c0: 0d0a 2020 2020 636f 6c6f 723a 204f 7074  ..    color: Opt
+000002d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000002e0: 6465 7269 7665 645f 636f 6c6f 723a 204f  derived_color: O
+000002f0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000300: 2020 636f 6d6d 656e 743a 204f 7074 696f    comment: Optio
+00000310: 6e61 6c5b 7374 725d 0d0a 2020 2020 6465  nal[str]..    de
+00000320: 7269 7665 645f 636f 6d6d 656e 743a 204f  rived_comment: O
+00000330: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000340: 2020 6372 6561 7465 643a 204f 7074 696f    created: Optio
+00000350: 6e61 6c5b 696e 745d 0d0a 2020 2020 7570  nal[int]..    up
+00000360: 6461 7465 643a 204f 7074 696f 6e61 6c5b  dated: Optional[
+00000370: 696e 745d 0d0a 2020 2020 6465 7269 7665  int]..    derive
+00000380: 645f 6d65 7461 6461 7461 3a20 4f70 7469  d_metadata: Opti
+00000390: 6f6e 616c 5b73 7472 5d0d 0a0d 0a44 6f63  onal[str]....Doc
+000003a0: 756d 656e 7443 6c61 7373 5363 6865 6d61  umentClassSchema
+000003b0: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+000003c0: 446f 6375 6d65 6e74 436c 6173 732c 2062  DocumentClass, b
+000003d0: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+000003e0: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.5.0/semantha_sdk/model/synonym.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2044 6f63  True)..class Doc
-000000f0: 756d 656e 7443 6c61 7373 4e6f 6465 2853  umentClassNode(S
-00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
-00000110: 7479 293a 0d0a 0922 2222 2061 7574 686f  ty):...""" autho
-00000120: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
-00000130: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
-00000140: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
-00000150: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
-00000160: 220d 0a09 6964 3a20 4f70 7469 6f6e 616c  "...id: Optional
-00000170: 5b73 7472 5d0d 0a09 6e61 6d65 3a20 7374  [str]...name: st
-00000180: 720d 0a09 7061 7265 6e74 5f69 643a 204f  r...parent_id: O
-00000190: 7074 696f 6e61 6c5b 7374 725d 0d0a 096d  ptional[str]...m
-000001a0: 6574 6164 6174 613a 204f 7074 696f 6e61  etadata: Optiona
-000001b0: 6c5b 7374 725d 0d0a 0964 6f63 756d 656e  l[str]...documen
-000001c0: 7473 5f63 6f75 6e74 3a20 4f70 7469 6f6e  ts_count: Option
-000001d0: 616c 5b69 6e74 5d0d 0a09 0d0a 090d 0a44  al[int]........D
-000001e0: 6f63 756d 656e 7443 6c61 7373 4e6f 6465  ocumentClassNode
-000001f0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-00000200: 6368 656d 6128 446f 6375 6d65 6e74 436c  chema(DocumentCl
-00000210: 6173 734e 6f64 652c 2062 6173 655f 7363  assNode, base_sc
-00000220: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000230: 656d 6129 0d0a                           ema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000100: 636c 6173 7320 5379 6e6f 6e79 6d28 5365  class Synonym(Se
+00000110: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
+00000120: 7929 3a0d 0a20 2020 2022 2222 2061 7574  y):..    """ aut
+00000130: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
+00000140: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
+00000150: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
+00000160: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
+00000170: 2222 220d 0a20 2020 2069 643a 204f 7074  """..    id: Opt
+00000180: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+00000190: 776f 7264 3a20 4f70 7469 6f6e 616c 5b73  word: Optional[s
+000001a0: 7472 5d0d 0a20 2020 2072 6567 6578 3a20  tr]..    regex: 
+000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001c0: 2020 2073 796e 6f6e 796d 3a20 4f70 7469     synonym: Opti
+000001d0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
+000001e0: 6167 733a 204f 7074 696f 6e61 6c5b 4c69  ags: Optional[Li
+000001f0: 7374 5b73 7472 5d5d 0d0a 0d0a 5379 6e6f  st[str]]....Syno
+00000200: 6e79 6d53 6368 656d 6120 3d20 636c 6173  nymSchema = clas
+00000210: 735f 7363 6865 6d61 2853 796e 6f6e 796d  s_schema(Synonym
+00000220: 2c20 6261 7365 5f73 6368 656d 613d 5365  , base_schema=Se
+00000230: 6d61 6e74 6861 5363 6865 6d61 290d 0a    manthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.5.0/semantha_sdk/model/document_cluster.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e63 6c75 7374 6572 6564 5f64  odel.clustered_d
-000000d0: 6f63 756d 656e 7420 696d 706f 7274 2043  ocument import C
-000000e0: 6c75 7374 6572 6564 446f 6375 6d65 6e74  lusteredDocument
-000000f0: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
-00000100: 706f 7274 204c 6973 742c 204f 7074 696f  port List, Optio
-00000110: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
-00000120: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000130: 0d0a 636c 6173 7320 446f 6375 6d65 6e74  ..class Document
-00000140: 436c 7573 7465 7228 5365 6d61 6e74 6861  Cluster(Semantha
-00000150: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a09  ModelEntity):...
-00000160: 2222 2220 6175 7468 6f72 2073 656d 616e  """ author seman
-00000170: 7468 612c 2074 6869 7320 6973 2061 2067  tha, this is a g
-00000180: 656e 6572 6174 6564 2063 6c61 7373 2064  enerated class d
-00000190: 6f20 6e6f 7420 6368 616e 6765 206d 616e  o not change man
-000001a0: 7561 6c6c 7921 2022 2222 0d0a 0969 643a  ually! """...id:
-000001b0: 204f 7074 696f 6e61 6c5b 696e 745d 0d0a   Optional[int]..
-000001c0: 0963 6f75 6e74 3a20 4f70 7469 6f6e 616c  .count: Optional
-000001d0: 5b69 6e74 5d0d 0a09 6c61 6265 6c3a 204f  [int]...label: O
-000001e0: 7074 696f 6e61 6c5b 7374 725d 0d0a 0963  ptional[str]...c
-000001f0: 6f6e 7465 6e74 3a20 4f70 7469 6f6e 616c  ontent: Optional
-00000200: 5b4c 6973 745b 436c 7573 7465 7265 6444  [List[ClusteredD
-00000210: 6f63 756d 656e 745d 5d0d 0a09 0d0a 090d  ocument]].......
-00000220: 0a44 6f63 756d 656e 7443 6c75 7374 6572  .DocumentCluster
-00000230: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-00000240: 6368 656d 6128 446f 6375 6d65 6e74 436c  chema(DocumentCl
-00000250: 7573 7465 722c 2062 6173 655f 7363 6865  uster, base_sche
-00000260: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-00000270: 6129 0d0a                                a)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e63 6c75 7374 6572 6564  .model.clustered
+000000d0: 5f64 6f63 756d 656e 7420 696d 706f 7274  _document import
+000000e0: 2043 6c75 7374 6572 6564 446f 6375 6d65   ClusteredDocume
+000000f0: 6e74 0d0a 0d0a 6672 6f6d 2074 7970 696e  nt....from typin
+00000100: 6720 696d 706f 7274 204c 6973 740d 0a66  g import List..f
+00000110: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00000120: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
+00000130: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+00000140: 5472 7565 290d 0a63 6c61 7373 2044 6f63  True)..class Doc
+00000150: 756d 656e 7443 6c75 7374 6572 2853 656d  umentCluster(Sem
+00000160: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+00000170: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+00000180: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+00000190: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+000001a0: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+000001b0: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+000001c0: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+000001d0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2063  onal[int]..    c
+000001e0: 6f75 6e74 3a20 4f70 7469 6f6e 616c 5b69  ount: Optional[i
+000001f0: 6e74 5d0d 0a20 2020 206c 6162 656c 3a20  nt]..    label: 
+00000200: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000210: 2020 2063 6f6e 7465 6e74 3a20 4f70 7469     content: Opti
+00000220: 6f6e 616c 5b4c 6973 745b 436c 7573 7465  onal[List[Cluste
+00000230: 7265 6444 6f63 756d 656e 745d 5d0d 0a0d  redDocument]]...
+00000240: 0a44 6f63 756d 656e 7443 6c75 7374 6572  .DocumentCluster
+00000250: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+00000260: 6368 656d 6128 446f 6375 6d65 6e74 436c  chema(DocumentCl
+00000270: 7573 7465 722c 2062 6173 655f 7363 6865  uster, base_sche
+00000280: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
+00000290: 6129 0d0a                                a)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/document_information.py` & `semantha_sdk-5.5.0/semantha_sdk/model/paragraph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e65 6e74 6974 7920 696d 706f  odel.entity impo
-000000d0: 7274 2045 6e74 6974 790d 0a66 726f 6d20  rt Entity..from 
-000000e0: 7479 7069 6e67 2069 6d70 6f72 7420 4c69  typing import Li
-000000f0: 7374 2c20 4f70 7469 6f6e 616c 0d0a 0d0a  st, Optional....
-00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
-00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
-00000120: 2044 6f63 756d 656e 7449 6e66 6f72 6d61   DocumentInforma
-00000130: 7469 6f6e 2853 656d 616e 7468 614d 6f64  tion(SemanthaMod
-00000140: 656c 456e 7469 7479 293a 0d0a 0922 2222  elEntity):..."""
-00000150: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
-00000160: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
-00000170: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
-00000180: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
-00000190: 6c79 2120 2222 220d 0a09 6964 3a20 4f70  ly! """...id: Op
-000001a0: 7469 6f6e 616c 5b73 7472 5d0d 0a09 6e61  tional[str]...na
-000001b0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-000001c0: 5d0d 0a09 7461 6773 3a20 4f70 7469 6f6e  ]...tags: Option
-000001d0: 616c 5b4c 6973 745b 7374 725d 5d0d 0a09  al[List[str]]...
-000001e0: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
-000001f0: 616c 5b73 7472 5d0d 0a09 6669 6c65 6e61  al[str]...filena
-00000200: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-00000210: 5d0d 0a09 6372 6561 7465 643a 204f 7074  ]...created: Opt
-00000220: 696f 6e61 6c5b 696e 745d 0d0a 0975 7064  ional[int]...upd
-00000230: 6174 6564 3a20 4f70 7469 6f6e 616c 5b69  ated: Optional[i
-00000240: 6e74 5d0d 0a09 7072 6f63 6573 7365 643a  nt]...processed:
-00000250: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d0d   Optional[bool].
-00000260: 0a09 6c61 6e67 3a20 4f70 7469 6f6e 616c  ..lang: Optional
-00000270: 5b73 7472 5d0d 0a09 636f 6e74 656e 743a  [str]...content:
-00000280: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000290: 0964 6f63 756d 656e 745f 636c 6173 733a  .document_class:
-000002a0: 204f 7074 696f 6e61 6c5b 456e 7469 7479   Optional[Entity
-000002b0: 5d0d 0a09 6465 7269 7665 645f 7461 6773  ]...derived_tags
-000002c0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-000002d0: 7374 725d 5d0d 0a09 636f 6c6f 723a 204f  str]]...color: O
-000002e0: 7074 696f 6e61 6c5b 7374 725d 0d0a 0964  ptional[str]...d
-000002f0: 6572 6976 6564 5f63 6f6c 6f72 3a20 4f70  erived_color: Op
-00000300: 7469 6f6e 616c 5b73 7472 5d0d 0a09 636f  tional[str]...co
-00000310: 6d6d 656e 743a 204f 7074 696f 6e61 6c5b  mment: Optional[
-00000320: 7374 725d 0d0a 0964 6572 6976 6564 5f63  str]...derived_c
-00000330: 6f6d 6d65 6e74 3a20 4f70 7469 6f6e 616c  omment: Optional
-00000340: 5b73 7472 5d0d 0a09 636f 6e74 656e 745f  [str]...content_
-00000350: 7072 6576 6965 773a 204f 7074 696f 6e61  preview: Optiona
-00000360: 6c5b 7374 725d 0d0a 0964 6f63 756d 656e  l[str]...documen
-00000370: 745f 636c 6173 735f 6964 3a20 4f70 7469  t_class_id: Opti
-00000380: 6f6e 616c 5b73 7472 5d0d 0a09 0d0a 090d  onal[str].......
-00000390: 0a44 6f63 756d 656e 7449 6e66 6f72 6d61  .DocumentInforma
-000003a0: 7469 6f6e 5363 6865 6d61 203d 2063 6c61  tionSchema = cla
-000003b0: 7373 5f73 6368 656d 6128 446f 6375 6d65  ss_schema(Docume
-000003c0: 6e74 496e 666f 726d 6174 696f 6e2c 2062  ntInformation, b
-000003d0: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
-000003e0: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e72 6563 7420 696d 706f  .model.rect impo
+000000d0: 7274 2052 6563 740d 0a0d 0a66 726f 6d20  rt Rect....from 
+000000e0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+000000f0: 656c 2e72 6566 6572 656e 6365 2069 6d70  el.reference imp
+00000100: 6f72 7420 5265 6665 7265 6e63 650d 0a0d  ort Reference...
+00000110: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
+00000120: 646b 2e6d 6f64 656c 2e73 656e 7465 6e63  dk.model.sentenc
+00000130: 6520 696d 706f 7274 2053 656e 7465 6e63  e import Sentenc
+00000140: 650d 0a0d 0a66 726f 6d20 7479 7069 6e67  e....from typing
+00000150: 2069 6d70 6f72 7420 4469 6374 0d0a 6672   import Dict..fr
+00000160: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000170: 204c 6973 740d 0a66 726f 6d20 7479 7069   List..from typi
+00000180: 6e67 2069 6d70 6f72 7420 4f70 7469 6f6e  ng import Option
+00000190: 616c 0d0a 0d0a 4064 6174 6163 6c61 7373  al....@dataclass
+000001a0: 2866 726f 7a65 6e3d 5472 7565 290d 0a63  (frozen=True)..c
+000001b0: 6c61 7373 2050 6172 6167 7261 7068 2853  lass Paragraph(S
+000001c0: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
+000001d0: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
+000001e0: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
+000001f0: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
+00000200: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
+00000210: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
+00000220: 2022 2222 0d0a 2020 2020 7465 7874 3a20   """..    text: 
+00000230: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000240: 2020 2074 7970 653a 204f 7074 696f 6e61     type: Optiona
+00000250: 6c5b 7374 725d 0d0a 2020 2020 6964 3a20  l[str]..    id: 
+00000260: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+00000270: 2020 2064 6f63 756d 656e 745f 6e61 6d65     document_name
+00000280: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+00000290: 0a20 2020 2073 656e 7465 6e63 6573 3a20  .    sentences: 
+000002a0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5365  Optional[List[Se
+000002b0: 6e74 656e 6365 5d5d 0d0a 2020 2020 7265  ntence]]..    re
+000002c0: 6665 7265 6e63 6573 3a20 4f70 7469 6f6e  ferences: Option
+000002d0: 616c 5b4c 6973 745b 5265 6665 7265 6e63  al[List[Referenc
+000002e0: 655d 5d0d 0a20 2020 2063 6f6e 7465 7874  e]]..    context
+000002f0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00000300: 7374 722c 2073 7472 5d5d 0d0a 2020 2020  str, str]]..    
+00000310: 6172 6561 733a 204f 7074 696f 6e61 6c5b  areas: Optional[
+00000320: 4c69 7374 5b52 6563 745d 5d0d 0a20 2020  List[Rect]]..   
+00000330: 2063 6f6d 6d65 6e74 3a20 4f70 7469 6f6e   comment: Option
+00000340: 616c 5b73 7472 5d0d 0a20 2020 2076 6572  al[str]..    ver
+00000350: 6966 6965 643a 204f 7074 696f 6e61 6c5b  ified: Optional[
+00000360: 626f 6f6c 5d0d 0a20 2020 2064 6174 615f  bool]..    data_
+00000370: 7572 6c5f 696d 6167 653a 204f 7074 696f  url_image: Optio
+00000380: 6e61 6c5b 7374 725d 0d0a 2020 2020 7265  nal[str]..    re
+00000390: 6665 7265 6e63 6573 5f73 6166 653a 204f  ferences_safe: O
+000003a0: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
+000003b0: 6572 656e 6365 5d5d 0d0a 0d0a 5061 7261  erence]]....Para
+000003c0: 6772 6170 6853 6368 656d 6120 3d20 636c  graphSchema = cl
+000003d0: 6173 735f 7363 6865 6d61 2850 6172 6167  ass_schema(Parag
+000003e0: 7261 7068 2c20 6261 7365 5f73 6368 656d  raph, base_schem
+000003f0: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000400: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/domain.py` & `semantha_sdk-5.5.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.settings import Settings
-from typing import Optional
+from semantha_sdk.model.document_information import DocumentInformation
 
+from semantha_sdk.model.response_meta_info import ResponseMetaInfo
+
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
-class Domain(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	id: Optional[str]
-	name: Optional[str]
-	base_url: Optional[str]
-	settings: Optional[Settings]
-	
-	
-DomainSchema = class_schema(Domain, base_schema=SemanthaSchema)
+class ReferenceDocumentsResponseContainer(SemanthaModelEntity):
+    """ author semantha, this is a generated class do not change manually! """
+    meta: Optional[ResponseMetaInfo]
+    data: Optional[List[DocumentInformation]]
+
+ReferenceDocumentsResponseContainerSchema = class_schema(ReferenceDocumentsResponseContainer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.5.0/semantha_sdk/model/response_meta_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from semantha_sdk.model.file_reference import FileReference
-from semantha_sdk.model.rect import Rect
-from typing import Optional
+from semantha_sdk.model.meta_info_page import MetaInfoPage
 
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
-class ExtractionArea(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	file: Optional[FileReference]
-	rect: Optional[Rect]
-	
-	
-ExtractionAreaSchema = class_schema(ExtractionArea, base_schema=SemanthaSchema)
+class ResponseMetaInfo(SemanthaModelEntity):
+    """ author semantha, this is a generated class do not change manually! """
+    info: Optional[str]
+    parameters: Optional[Dict[str, Any]]
+    warnings: Optional[List[str]]
+    page: Optional[MetaInfoPage]
+
+ResponseMetaInfoSchema = class_schema(ResponseMetaInfo, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.5.0/semantha_sdk/model/reference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e64 6f63 756d 656e 7420 696d  odel.document im
-000000d0: 706f 7274 2044 6f63 756d 656e 740d 0a66  port Document..f
-000000e0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-000000f0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a  t Optional......
-00000100: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-00000110: 6e3d 5472 7565 290d 0a63 6c61 7373 2045  n=True)..class E
-00000120: 7874 7261 6374 696f 6e46 696c 6528 5365  xtractionFile(Se
-00000130: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
-00000140: 7929 3a0d 0a09 2222 2220 6175 7468 6f72  y):...""" author
-00000150: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-00000160: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-00000170: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000180: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000190: 0d0a 0969 643a 204f 7074 696f 6e61 6c5b  ...id: Optional[
-000001a0: 7374 725d 0d0a 0965 7874 6572 6e61 6c5f  str]...external_
-000001b0: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-000001c0: 5d0d 0a09 6e61 6d65 3a20 4f70 7469 6f6e  ]...name: Option
-000001d0: 616c 5b73 7472 5d0d 0a09 7072 6f63 6573  al[str]...proces
-000001e0: 7365 643a 204f 7074 696f 6e61 6c5b 626f  sed: Optional[bo
-000001f0: 6f6c 5d0d 0a09 6269 6e61 7279 3a20 4f70  ol]...binary: Op
-00000200: 7469 6f6e 616c 5b73 7472 5d0d 0a09 646f  tional[str]...do
-00000210: 6375 6d65 6e74 6578 7472 6163 746f 723a  cumentextractor:
-00000220: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-00000230: 0964 6f63 756d 656e 743a 204f 7074 696f  .document: Optio
-00000240: 6e61 6c5b 446f 6375 6d65 6e74 5d0d 0a09  nal[Document]...
-00000250: 6669 6c65 6e61 6d65 3a20 4f70 7469 6f6e  filename: Option
-00000260: 616c 5b73 7472 5d0d 0a09 6372 6561 7465  al[str]...create
-00000270: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
-00000280: 0d0a 090d 0a09 0d0a 4578 7472 6163 7469  ........Extracti
-00000290: 6f6e 4669 6c65 5363 6865 6d61 203d 2063  onFileSchema = c
-000002a0: 6c61 7373 5f73 6368 656d 6128 4578 7472  lass_schema(Extr
-000002b0: 6163 7469 6f6e 4669 6c65 2c20 6261 7365  actionFile, base
-000002c0: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
-000002d0: 5363 6865 6d61 290d 0a                   Schema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4469 6374 0d0a 6672 6f6d 2074 7970  t Dict..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000100: 636c 6173 7320 5265 6665 7265 6e63 6528  class Reference(
+00000110: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000120: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000130: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000140: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000150: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000160: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000170: 2120 2222 220d 0a20 2020 2064 6f63 756d  ! """..    docum
+00000180: 656e 745f 6964 3a20 4f70 7469 6f6e 616c  ent_id: Optional
+00000190: 5b73 7472 5d0d 0a20 2020 2064 6f63 756d  [str]..    docum
+000001a0: 656e 745f 6e61 6d65 3a20 4f70 7469 6f6e  ent_name: Option
+000001b0: 616c 5b73 7472 5d0d 0a20 2020 2070 6167  al[str]..    pag
+000001c0: 655f 6e75 6d62 6572 3a20 4f70 7469 6f6e  e_number: Option
+000001d0: 616c 5b69 6e74 5d0d 0a20 2020 2070 6172  al[int]..    par
+000001e0: 6167 7261 7068 5f69 643a 204f 7074 696f  agraph_id: Optio
+000001f0: 6e61 6c5b 7374 725d 0d0a 2020 2020 7365  nal[str]..    se
+00000200: 6e74 656e 6365 5f69 643a 204f 7074 696f  ntence_id: Optio
+00000210: 6e61 6c5b 7374 725d 0d0a 2020 2020 7369  nal[str]..    si
+00000220: 6d69 6c61 7269 7479 3a20 4f70 7469 6f6e  milarity: Option
+00000230: 616c 5b66 6c6f 6174 5d0d 0a20 2020 2074  al[float]..    t
+00000240: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
+00000250: 725d 0d0a 2020 2020 636f 6e74 6578 743a  r]..    context:
+00000260: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
+00000270: 7472 2c20 7374 725d 5d0d 0a20 2020 2074  tr, str]]..    t
+00000280: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
+00000290: 725d 0d0a 2020 2020 636f 6c6f 723a 204f  r]..    color: O
+000002a0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000002b0: 2020 636f 6d6d 656e 743a 204f 7074 696f    comment: Optio
+000002c0: 6e61 6c5b 7374 725d 0d0a 2020 2020 6861  nal[str]..    ha
+000002d0: 735f 6f70 706f 7369 7465 5f6d 6561 6e69  s_opposite_meani
+000002e0: 6e67 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ng: Optional[boo
+000002f0: 6c5d 0d0a 0d0a 5265 6665 7265 6e63 6553  l]....ReferenceS
+00000300: 6368 656d 6120 3d20 636c 6173 735f 7363  chema = class_sc
+00000310: 6865 6d61 2852 6566 6572 656e 6365 2c20  hema(Reference, 
+00000320: 6261 7365 5f73 6368 656d 613d 5365 6d61  base_schema=Sema
+00000330: 6e74 6861 5363 6865 6d61 290d 0a         nthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.5.0/semantha_sdk/model/extraction_area.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2045 7874  True)..class Ext
-000000f0: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
-00000100: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000110: 7469 7479 293a 0d0a 0922 2222 2061 7574  tity):...""" aut
-00000120: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
-00000130: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
-00000140: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
-00000150: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
-00000160: 2222 220d 0a09 646f 6375 6d65 6e74 5f69  """...document_i
-00000170: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
-00000180: 0d0a 0973 696d 696c 6172 6974 793a 204f  ...similarity: O
-00000190: 7074 696f 6e61 6c5b 666c 6f61 745d 0d0a  ptional[float]..
-000001a0: 0975 7365 643a 204f 7074 696f 6e61 6c5b  .used: Optional[
-000001b0: 626f 6f6c 5d0d 0a09 0d0a 090d 0a45 7874  bool]........Ext
-000001c0: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
-000001d0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
-000001e0: 6368 656d 6128 4578 7472 6163 7469 6f6e  chema(Extraction
-000001f0: 5265 6665 7265 6e63 652c 2062 6173 655f  Reference, base_
-00000200: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
-00000210: 6368 656d 6129 0d0a                      chema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e66 696c 655f 7265 6665  .model.file_refe
+000000d0: 7265 6e63 6520 696d 706f 7274 2046 696c  rence import Fil
+000000e0: 6552 6566 6572 656e 6365 0d0a 0d0a 6672  eReference....fr
+000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
+00000100: 6d6f 6465 6c2e 7265 6374 2069 6d70 6f72  model.rect impor
+00000110: 7420 5265 6374 0d0a 0d0a 6672 6f6d 2074  t Rect....from t
+00000120: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
+00000130: 696f 6e61 6c0d 0a0d 0a40 6461 7461 636c  ional....@datacl
+00000140: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00000150: 0d0a 636c 6173 7320 4578 7472 6163 7469  ..class Extracti
+00000160: 6f6e 4172 6561 2853 656d 616e 7468 614d  onArea(SemanthaM
+00000170: 6f64 656c 456e 7469 7479 293a 0d0a 2020  odelEntity):..  
+00000180: 2020 2222 2220 6175 7468 6f72 2073 656d    """ author sem
+00000190: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
+000001a0: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
+000001b0: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
+000001c0: 616e 7561 6c6c 7921 2022 2222 0d0a 2020  anually! """..  
+000001d0: 2020 6669 6c65 3a20 4f70 7469 6f6e 616c    file: Optional
+000001e0: 5b46 696c 6552 6566 6572 656e 6365 5d0d  [FileReference].
+000001f0: 0a20 2020 2072 6563 743a 204f 7074 696f  .    rect: Optio
+00000200: 6e61 6c5b 5265 6374 5d0d 0a0d 0a45 7874  nal[Rect]....Ext
+00000210: 7261 6374 696f 6e41 7265 6153 6368 656d  ractionAreaSchem
+00000220: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
+00000230: 2845 7874 7261 6374 696f 6e41 7265 612c  (ExtractionArea,
+00000240: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
+00000250: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.5.0/semantha_sdk/model/semi_super_vised_document.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
 000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2046 696c  True)..class Fil
-000000f0: 6552 6566 6572 656e 6365 2853 656d 616e  eReference(Seman
-00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000110: 0d0a 0922 2222 2061 7574 686f 7220 7365  ...""" author se
-00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a09  manually! """...
-00000160: 6669 6c65 5f69 643a 204f 7074 696f 6e61  file_id: Optiona
-00000170: 6c5b 7374 725d 0d0a 096e 616d 653a 204f  l[str]...name: O
-00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 0970  ptional[str]...p
-00000190: 6167 655f 6e75 6d62 6572 3a20 4f70 7469  age_number: Opti
-000001a0: 6f6e 616c 5b69 6e74 5d0d 0a09 0d0a 090d  onal[int].......
-000001b0: 0a46 696c 6552 6566 6572 656e 6365 5363  .FileReferenceSc
-000001c0: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
-000001d0: 656d 6128 4669 6c65 5265 6665 7265 6e63  ema(FileReferenc
-000001e0: 652c 2062 6173 655f 7363 6865 6d61 3d53  e, base_schema=S
-000001f0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+000000e0: 5472 7565 290d 0a63 6c61 7373 2053 656d  True)..class Sem
+000000f0: 6953 7570 6572 5669 7365 6444 6f63 756d  iSuperVisedDocum
+00000100: 656e 7428 5365 6d61 6e74 6861 4d6f 6465  ent(SemanthaMode
+00000110: 6c45 6e74 6974 7929 3a0d 0a20 2020 2022  lEntity):..    "
+00000120: 2222 2061 7574 686f 7220 7365 6d61 6e74  "" author semant
+00000130: 6861 2c20 7468 6973 2069 7320 6120 6765  ha, this is a ge
+00000140: 6e65 7261 7465 6420 636c 6173 7320 646f  nerated class do
+00000150: 206e 6f74 2063 6861 6e67 6520 6d61 6e75   not change manu
+00000160: 616c 6c79 2120 2222 220d 0a20 2020 2064  ally! """..    d
+00000170: 6f63 756d 656e 745f 6964 3a20 4f70 7469  ocument_id: Opti
+00000180: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
+00000190: 6f70 6963 5f69 643a 204f 7074 696f 6e61  opic_id: Optiona
+000001a0: 6c5b 696e 745d 0d0a 0d0a 5365 6d69 5375  l[int]....SemiSu
+000001b0: 7065 7256 6973 6564 446f 6375 6d65 6e74  perVisedDocument
+000001c0: 5363 6865 6d61 203d 2063 6c61 7373 5f73  Schema = class_s
+000001d0: 6368 656d 6128 5365 6d69 5375 7065 7256  chema(SemiSuperV
+000001e0: 6973 6564 446f 6375 6d65 6e74 2c20 6261  isedDocument, ba
+000001f0: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000200: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.5.0/semantha_sdk/model/clustered_document.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
 000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2049 6e73  True)..class Ins
-000000f0: 7461 6e63 6543 6869 6c64 2853 656d 616e  tanceChild(Seman
-00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000110: 0d0a 0922 2222 2061 7574 686f 7220 7365  ...""" author se
-00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a09  manually! """...
-00000160: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-00000170: 5d0d 0a09 6e61 6d65 3a20 7374 720d 0a09  ]...name: str...
-00000180: 7265 6c61 7469 6f6e 5f69 643a 2073 7472  relation_id: str
-00000190: 0d0a 0963 6c61 7373 5f6e 616d 653a 204f  ...class_name: O
-000001a0: 7074 696f 6e61 6c5b 7374 725d 0d0a 0963  ptional[str]...c
-000001b0: 6c61 7373 5f69 643a 2073 7472 0d0a 090d  lass_id: str....
-000001c0: 0a09 0d0a 496e 7374 616e 6365 4368 696c  ....InstanceChil
-000001d0: 6453 6368 656d 6120 3d20 636c 6173 735f  dSchema = class_
-000001e0: 7363 6865 6d61 2849 6e73 7461 6e63 6543  schema(InstanceC
-000001f0: 6869 6c64 2c20 6261 7365 5f73 6368 656d  hild, base_schem
-00000200: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000210: 290d 0a                                  )..
+000000e0: 5472 7565 290d 0a63 6c61 7373 2043 6c75  True)..class Clu
+000000f0: 7374 6572 6564 446f 6375 6d65 6e74 2853  steredDocument(S
+00000100: 656d 616e 7468 614d 6f64 656c 456e 7469  emanthaModelEnti
+00000110: 7479 293a 0d0a 2020 2020 2222 2220 6175  ty):..    """ au
+00000120: 7468 6f72 2073 656d 616e 7468 612c 2074  thor semantha, t
+00000130: 6869 7320 6973 2061 2067 656e 6572 6174  his is a generat
+00000140: 6564 2063 6c61 7373 2064 6f20 6e6f 7420  ed class do not 
+00000150: 6368 616e 6765 206d 616e 7561 6c6c 7921  change manually!
+00000160: 2022 2222 0d0a 2020 2020 646f 6375 6d65   """..    docume
+00000170: 6e74 5f69 643a 204f 7074 696f 6e61 6c5b  nt_id: Optional[
+00000180: 7374 725d 0d0a 2020 2020 7072 6f62 6162  str]..    probab
+00000190: 696c 6974 793a 204f 7074 696f 6e61 6c5b  ility: Optional[
+000001a0: 666c 6f61 745d 0d0a 0d0a 436c 7573 7465  float]....Cluste
+000001b0: 7265 6444 6f63 756d 656e 7453 6368 656d  redDocumentSchem
+000001c0: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
+000001d0: 2843 6c75 7374 6572 6564 446f 6375 6d65  (ClusteredDocume
+000001e0: 6e74 2c20 6261 7365 5f73 6368 656d 613d  nt, base_schema=
+000001f0: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000200: 0a                                       .
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.5.0/semantha_sdk/model/linked_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.linked_value import LinkedValue
-from typing import List, Optional
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class LinkedInstance(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	instance_id: Optional[str]
-	linked_values: Optional[List[LinkedValue]]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    instance_id: Optional[str]
+    linked_values: Optional[List[LinkedValue]]
+
 LinkedInstanceSchema = class_schema(LinkedInstance, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.5.0/semantha_sdk/model/matrix_row.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e72 6566 6572 656e 6365 2069  odel.reference i
-000000d0: 6d70 6f72 7420 5265 6665 7265 6e63 650d  mport Reference.
-000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-000000f0: 6f72 7420 4c69 7374 2c20 4f70 7469 6f6e  ort List, Option
-00000100: 616c 0d0a 0d0a 0d0a 4064 6174 6163 6c61  al......@datacla
-00000110: 7373 2866 726f 7a65 6e3d 5472 7565 290d  ss(frozen=True).
-00000120: 0a63 6c61 7373 204d 6174 7269 7852 6f77  .class MatrixRow
-00000130: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
-00000140: 7469 7479 293a 0d0a 0922 2222 2061 7574  tity):...""" aut
-00000150: 686f 7220 7365 6d61 6e74 6861 2c20 7468  hor semantha, th
-00000160: 6973 2069 7320 6120 6765 6e65 7261 7465  is is a generate
-00000170: 6420 636c 6173 7320 646f 206e 6f74 2063  d class do not c
-00000180: 6861 6e67 6520 6d61 6e75 616c 6c79 2120  hange manually! 
-00000190: 2222 220d 0a09 646f 6375 6d65 6e74 5f69  """...document_i
-000001a0: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
-000001b0: 0d0a 0964 6f63 756d 656e 745f 6e61 6d65  ...document_name
-000001c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-000001d0: 0a09 7265 6665 7265 6e63 6573 3a20 4f70  ..references: Op
-000001e0: 7469 6f6e 616c 5b4c 6973 745b 5265 6665  tional[List[Refe
-000001f0: 7265 6e63 655d 5d0d 0a09 0d0a 090d 0a4d  rence]]........M
-00000200: 6174 7269 7852 6f77 5363 6865 6d61 203d  atrixRowSchema =
-00000210: 2063 6c61 7373 5f73 6368 656d 6128 4d61   class_schema(Ma
-00000220: 7472 6978 526f 772c 2062 6173 655f 7363  trixRow, base_sc
-00000230: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000240: 656d 6129 0d0a                           ema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e72 6566 6572 656e 6365  .model.reference
+000000d0: 2069 6d70 6f72 7420 5265 6665 7265 6e63   import Referenc
+000000e0: 650d 0a0d 0a66 726f 6d20 7479 7069 6e67  e....from typing
+000000f0: 2069 6d70 6f72 7420 4c69 7374 0d0a 6672   import List..fr
+00000100: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000110: 204f 7074 696f 6e61 6c0d 0a0d 0a40 6461   Optional....@da
+00000120: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
+00000130: 7275 6529 0d0a 636c 6173 7320 4d61 7472  rue)..class Matr
+00000140: 6978 526f 7728 5365 6d61 6e74 6861 4d6f  ixRow(SemanthaMo
+00000150: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000160: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000170: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000180: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000190: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+000001a0: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+000001b0: 2064 6f63 756d 656e 745f 6964 3a20 4f70   document_id: Op
+000001c0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000001d0: 2064 6f63 756d 656e 745f 6e61 6d65 3a20   document_name: 
+000001e0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001f0: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
+00000200: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
+00000210: 6572 656e 6365 5d5d 0d0a 0d0a 4d61 7472  erence]]....Matr
+00000220: 6978 526f 7753 6368 656d 6120 3d20 636c  ixRowSchema = cl
+00000230: 6173 735f 7363 6865 6d61 284d 6174 7269  ass_schema(Matri
+00000240: 7852 6f77 2c20 6261 7365 5f73 6368 656d  xRow, base_schem
+00000250: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
+00000260: 290d 0a                                  )..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/model_class.py` & `semantha_sdk-5.5.0/semantha_sdk/model/document_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-from typing import List, Optional
+from semantha_sdk.model.row import Row
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
-class ModelClass(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	name: Optional[str]
-	label: Optional[str]
-	sub_model_classes: Optional[List["ModelClass"]]
-	
-	
-ModelClassSchema = class_schema(ModelClass, base_schema=SemanthaSchema)
+class DocumentTable(SemanthaModelEntity):
+    """ author semantha, this is a generated class do not change manually! """
+    rows: Optional[List[Row]]
+
+DocumentTableSchema = class_schema(DocumentTable, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.5.0/semantha_sdk/model/complex_property.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,76 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e63 6f6d 706c 6578 5f70 726f  odel.complex_pro
-000000d0: 7065 7274 7920 696d 706f 7274 2043 6f6d  perty import Com
-000000e0: 706c 6578 5072 6f70 6572 7479 0d0a 6672  plexProperty..fr
-000000f0: 6f6d 2073 656d 616e 7468 615f 7364 6b2e  om semantha_sdk.
-00000100: 6d6f 6465 6c2e 6578 7472 6163 7469 6f6e  model.extraction
-00000110: 5f72 6566 6572 656e 6365 2069 6d70 6f72  _reference impor
-00000120: 7420 4578 7472 6163 7469 6f6e 5265 6665  t ExtractionRefe
-00000130: 7265 6e63 650d 0a66 726f 6d20 7365 6d61  rence..from sema
-00000140: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e66  ntha_sdk.model.f
-00000150: 696c 655f 7265 6665 7265 6e63 6520 696d  ile_reference im
-00000160: 706f 7274 2046 696c 6552 6566 6572 656e  port FileReferen
-00000170: 6365 0d0a 6672 6f6d 2073 656d 616e 7468  ce..from semanth
-00000180: 615f 7364 6b2e 6d6f 6465 6c2e 6669 6e64  a_sdk.model.find
-00000190: 696e 6720 696d 706f 7274 2046 696e 6469  ing import Findi
-000001a0: 6e67 0d0a 6672 6f6d 2073 656d 616e 7468  ng..from semanth
-000001b0: 615f 7364 6b2e 6d6f 6465 6c2e 6c61 6265  a_sdk.model.labe
-000001c0: 6c20 696d 706f 7274 204c 6162 656c 0d0a  l import Label..
-000001d0: 6672 6f6d 2073 656d 616e 7468 615f 7364  from semantha_sd
-000001e0: 6b2e 6d6f 6465 6c2e 6c69 6e6b 6564 5f69  k.model.linked_i
-000001f0: 6e73 7461 6e63 6520 696d 706f 7274 204c  nstance import L
-00000200: 696e 6b65 6449 6e73 7461 6e63 650d 0a66  inkedInstance..f
-00000210: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
-00000220: 2e6d 6f64 656c 2e6d 6574 6164 6174 6120  .model.metadata 
-00000230: 696d 706f 7274 204d 6574 6164 6174 610d  import Metadata.
-00000240: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
-00000250: 646b 2e6d 6f64 656c 2e73 696d 706c 655f  dk.model.simple_
-00000260: 7072 6f70 6572 7479 2069 6d70 6f72 7420  property import 
-00000270: 5369 6d70 6c65 5072 6f70 6572 7479 0d0a  SimpleProperty..
-00000280: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
-00000290: 7274 204c 6973 742c 204f 7074 696f 6e61  rt List, Optiona
-000002a0: 6c0d 0a0d 0a0d 0a40 6461 7461 636c 6173  l......@dataclas
-000002b0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
-000002c0: 636c 6173 7320 4d6f 6465 6c49 6e73 7461  class ModelInsta
-000002d0: 6e63 6528 5365 6d61 6e74 6861 4d6f 6465  nce(SemanthaMode
-000002e0: 6c45 6e74 6974 7929 3a0d 0a09 2222 2220  lEntity):...""" 
-000002f0: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000300: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000310: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000320: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000330: 7921 2022 2222 0d0a 0969 643a 204f 7074  y! """...id: Opt
-00000340: 696f 6e61 6c5b 7374 725d 0d0a 096e 616d  ional[str]...nam
-00000350: 653a 2073 7472 0d0a 0963 6c61 7373 5f69  e: str...class_i
-00000360: 643a 2073 7472 0d0a 0972 656c 6174 696f  d: str...relatio
-00000370: 6e5f 6964 3a20 4f70 7469 6f6e 616c 5b73  n_id: Optional[s
-00000380: 7472 5d0d 0a09 7479 7065 3a20 4f70 7469  tr]...type: Opti
-00000390: 6f6e 616c 5b73 7472 5d0d 0a09 6967 6e6f  onal[str]...igno
-000003a0: 7265 5f69 6d70 6f72 743a 204f 7074 696f  re_import: Optio
-000003b0: 6e61 6c5b 626f 6f6c 5d0d 0a09 7369 6d70  nal[bool]...simp
-000003c0: 6c65 5f70 726f 7065 7274 6965 733a 204f  le_properties: O
-000003d0: 7074 696f 6e61 6c5b 4c69 7374 5b53 696d  ptional[List[Sim
-000003e0: 706c 6550 726f 7065 7274 795d 5d0d 0a09  pleProperty]]...
-000003f0: 6d65 7461 6461 7461 3a20 4f70 7469 6f6e  metadata: Option
-00000400: 616c 5b4c 6973 745b 4d65 7461 6461 7461  al[List[Metadata
-00000410: 5d5d 0d0a 0971 7561 6c69 6669 6564 5f6e  ]]...qualified_n
-00000420: 616d 653a 204f 7074 696f 6e61 6c5b 7374  ame: Optional[st
-00000430: 725d 0d0a 0965 7874 7261 6374 6f72 5f63  r]...extractor_c
-00000440: 6c61 7373 5f69 6473 3a20 4f70 7469 6f6e  lass_ids: Option
-00000450: 616c 5b4c 6973 745b 7374 725d 5d0d 0a09  al[List[str]]...
-00000460: 6c61 6265 6c3a 204f 7074 696f 6e61 6c5b  label: Optional[
-00000470: 7374 725d 0d0a 096c 6162 656c 733a 204f  str]...labels: O
-00000480: 7074 696f 6e61 6c5b 4c69 7374 5b4c 6162  ptional[List[Lab
-00000490: 656c 5d5d 0d0a 0966 696c 653a 204f 7074  el]]...file: Opt
-000004a0: 696f 6e61 6c5b 4669 6c65 5265 6665 7265  ional[FileRefere
-000004b0: 6e63 655d 0d0a 0963 6f6d 706c 6578 5f70  nce]...complex_p
-000004c0: 726f 7065 7274 6965 733a 204f 7074 696f  roperties: Optio
-000004d0: 6e61 6c5b 4c69 7374 5b43 6f6d 706c 6578  nal[List[Complex
-000004e0: 5072 6f70 6572 7479 5d5d 0d0a 0966 696e  Property]]...fin
-000004f0: 6469 6e67 733a 204f 7074 696f 6e61 6c5b  dings: Optional[
-00000500: 4c69 7374 5b46 696e 6469 6e67 5d5d 0d0a  List[Finding]]..
-00000510: 0972 6566 6572 656e 6365 733a 204f 7074  .references: Opt
-00000520: 696f 6e61 6c5b 4c69 7374 5b45 7874 7261  ional[List[Extra
-00000530: 6374 696f 6e52 6566 6572 656e 6365 5d5d  ctionReference]]
-00000540: 0d0a 096c 696e 6b65 645f 696e 7374 616e  ...linked_instan
-00000550: 6365 733a 204f 7074 696f 6e61 6c5b 4c69  ces: Optional[Li
-00000560: 7374 5b4c 696e 6b65 6449 6e73 7461 6e63  st[LinkedInstanc
-00000570: 655d 5d0d 0a09 0d0a 090d 0a4d 6f64 656c  e]]........Model
-00000580: 496e 7374 616e 6365 5363 6865 6d61 203d  InstanceSchema =
-00000590: 2063 6c61 7373 5f73 6368 656d 6128 4d6f   class_schema(Mo
-000005a0: 6465 6c49 6e73 7461 6e63 652c 2062 6173  delInstance, bas
-000005b0: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
-000005c0: 6153 6368 656d 6129 0d0a                 aSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
+000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
+000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 0d0a  tractionArea....
+000000f0: 6672 6f6d 2073 656d 616e 7468 615f 7364  from semantha_sd
+00000100: 6b2e 6d6f 6465 6c2e 6578 7472 6163 7469  k.model.extracti
+00000110: 6f6e 5f72 6566 6572 656e 6365 2069 6d70  on_reference imp
+00000120: 6f72 7420 4578 7472 6163 7469 6f6e 5265  ort ExtractionRe
+00000130: 6665 7265 6e63 650d 0a0d 0a66 726f 6d20  ference....from 
+00000140: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+00000150: 656c 2e66 696e 6469 6e67 2069 6d70 6f72  el.finding impor
+00000160: 7420 4669 6e64 696e 670d 0a0d 0a66 726f  t Finding....fro
+00000170: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
+00000180: 6f64 656c 2e6c 6162 656c 2069 6d70 6f72  odel.label impor
+00000190: 7420 4c61 6265 6c0d 0a0d 0a66 726f 6d20  t Label....from 
+000001a0: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+000001b0: 656c 2e6d 6574 6164 6174 6120 696d 706f  el.metadata impo
+000001c0: 7274 204d 6574 6164 6174 610d 0a0d 0a66  rt Metadata....f
+000001d0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000001e0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000001f0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+00000200: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+00000210: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000220: 636c 6173 7320 436f 6d70 6c65 7850 726f  class ComplexPro
+00000230: 7065 7274 7928 5365 6d61 6e74 6861 4d6f  perty(SemanthaMo
+00000240: 6465 6c45 6e74 6974 7929 3a0d 0a20 2020  delEntity):..   
+00000250: 2022 2222 2061 7574 686f 7220 7365 6d61   """ author sema
+00000260: 6e74 6861 2c20 7468 6973 2069 7320 6120  ntha, this is a 
+00000270: 6765 6e65 7261 7465 6420 636c 6173 7320  generated class 
+00000280: 646f 206e 6f74 2063 6861 6e67 6520 6d61  do not change ma
+00000290: 6e75 616c 6c79 2120 2222 220d 0a20 2020  nually! """..   
+000002a0: 206e 616d 653a 2073 7472 0d0a 2020 2020   name: str..    
+000002b0: 7661 6c75 653a 2073 7472 0d0a 2020 2020  value: str..    
+000002c0: 6c61 6265 6c3a 204f 7074 696f 6e61 6c5b  label: Optional[
+000002d0: 7374 725d 0d0a 2020 2020 6964 3a20 4f70  str]..    id: Op
+000002e0: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+000002f0: 2063 6c61 7373 5f69 643a 204f 7074 696f   class_id: Optio
+00000300: 6e61 6c5b 7374 725d 0d0a 2020 2020 7265  nal[str]..    re
+00000310: 6c61 7469 6f6e 5f69 643a 204f 7074 696f  lation_id: Optio
+00000320: 6e61 6c5b 7374 725d 0d0a 2020 2020 6f72  nal[str]..    or
+00000330: 6967 696e 616c 5f76 616c 7565 3a20 4f70  iginal_value: Op
+00000340: 7469 6f6e 616c 5b73 7472 5d0d 0a20 2020  tional[str]..   
+00000350: 2065 7874 7261 6374 6564 5f76 616c 7565   extracted_value
+00000360: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+00000370: 0a20 2020 2064 6174 6174 7970 653a 204f  .    datatype: O
+00000380: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000390: 2020 6c61 6265 6c73 3a20 4f70 7469 6f6e    labels: Option
+000003a0: 616c 5b4c 6973 745b 4c61 6265 6c5d 5d0d  al[List[Label]].
+000003b0: 0a20 2020 206d 6574 6164 6174 613a 204f  .    metadata: O
+000003c0: 7074 696f 6e61 6c5b 4c69 7374 5b4d 6574  ptional[List[Met
+000003d0: 6164 6174 615d 5d0d 0a20 2020 2065 7874  adata]]..    ext
+000003e0: 7261 6374 696f 6e5f 6172 6561 3a20 4f70  raction_area: Op
+000003f0: 7469 6f6e 616c 5b45 7874 7261 6374 696f  tional[Extractio
+00000400: 6e41 7265 615d 0d0a 2020 2020 6669 6e64  nArea]..    find
+00000410: 696e 6773 3a20 4f70 7469 6f6e 616c 5b4c  ings: Optional[L
+00000420: 6973 745b 4669 6e64 696e 675d 5d0d 0a20  ist[Finding]].. 
+00000430: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
+00000440: 7074 696f 6e61 6c5b 4c69 7374 5b45 7874  ptional[List[Ext
+00000450: 7261 6374 696f 6e52 6566 6572 656e 6365  ractionReference
+00000460: 5d5d 0d0a 0d0a 436f 6d70 6c65 7850 726f  ]]....ComplexPro
+00000470: 7065 7274 7953 6368 656d 6120 3d20 636c  pertySchema = cl
+00000480: 6173 735f 7363 6865 6d61 2843 6f6d 706c  ass_schema(Compl
+00000490: 6578 5072 6f70 6572 7479 2c20 6261 7365  exProperty, base
+000004a0: 5f73 6368 656d 613d 5365 6d61 6e74 6861  _schema=Semantha
+000004b0: 5363 6865 6d61 290d 0a                   Schema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/page.py` & `semantha_sdk-5.5.0/semantha_sdk/model/page.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.annotation_page import AnnotationPage
+
 from semantha_sdk.model.document_table import DocumentTable
+
 from semantha_sdk.model.page_content import PageContent
+
 from semantha_sdk.model.paragraph import Paragraph
-from typing import List, Optional
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class Page(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	contents: Optional[List[PageContent]]
-	paragraphs: Optional[List[Paragraph]]
-	tables: Optional[List[DocumentTable]]
-	annotation_page: Optional[AnnotationPage]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    contents: Optional[List[PageContent]]
+    paragraphs: Optional[List[Paragraph]]
+    tables: Optional[List[DocumentTable]]
+    annotation_page: Optional[AnnotationPage]
+
 PageSchema = class_schema(Page, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/page_content.py` & `semantha_sdk-5.5.0/semantha_sdk/model/page_content.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.paragraph import Paragraph
-from typing import List, Optional
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class PageContent(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	paragraphs: Optional[List[Paragraph]]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    paragraphs: Optional[List[Paragraph]]
+
 PageContentSchema = class_schema(PageContent, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.5.0/semantha_sdk/model/extraction_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,48 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e72 6563 7420 696d 706f 7274  odel.rect import
-000000d0: 2052 6563 740d 0a66 726f 6d20 7365 6d61   Rect..from sema
-000000e0: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
-000000f0: 6566 6572 656e 6365 2069 6d70 6f72 7420  eference import 
-00000100: 5265 6665 7265 6e63 650d 0a66 726f 6d20  Reference..from 
-00000110: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
-00000120: 656c 2e73 656e 7465 6e63 6520 696d 706f  el.sentence impo
-00000130: 7274 2053 656e 7465 6e63 650d 0a66 726f  rt Sentence..fro
-00000140: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000150: 4469 6374 2c20 4c69 7374 2c20 4f70 7469  Dict, List, Opti
-00000160: 6f6e 616c 0d0a 0d0a 0d0a 4064 6174 6163  onal......@datac
-00000170: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
-00000180: 290d 0a63 6c61 7373 2050 6172 6167 7261  )..class Paragra
-00000190: 7068 2853 656d 616e 7468 614d 6f64 656c  ph(SemanthaModel
-000001a0: 456e 7469 7479 293a 0d0a 0922 2222 2061  Entity):...""" a
-000001b0: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
-000001c0: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
-000001d0: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
-000001e0: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
-000001f0: 2120 2222 220d 0a09 7465 7874 3a20 4f70  ! """...text: Op
-00000200: 7469 6f6e 616c 5b73 7472 5d0d 0a09 7479  tional[str]...ty
-00000210: 7065 3a20 4f70 7469 6f6e 616c 5b73 7472  pe: Optional[str
-00000220: 5d0d 0a09 6964 3a20 4f70 7469 6f6e 616c  ]...id: Optional
-00000230: 5b73 7472 5d0d 0a09 646f 6375 6d65 6e74  [str]...document
-00000240: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
-00000250: 7374 725d 0d0a 0973 656e 7465 6e63 6573  str]...sentences
-00000260: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000270: 5365 6e74 656e 6365 5d5d 0d0a 0972 6566  Sentence]]...ref
-00000280: 6572 656e 6365 733a 204f 7074 696f 6e61  erences: Optiona
-00000290: 6c5b 4c69 7374 5b52 6566 6572 656e 6365  l[List[Reference
-000002a0: 5d5d 0d0a 0963 6f6e 7465 7874 3a20 4f70  ]]...context: Op
-000002b0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-000002c0: 2073 7472 5d5d 0d0a 0961 7265 6173 3a20   str]]...areas: 
-000002d0: 4f70 7469 6f6e 616c 5b4c 6973 745b 5265  Optional[List[Re
-000002e0: 6374 5d5d 0d0a 0963 6f6d 6d65 6e74 3a20  ct]]...comment: 
-000002f0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a09  Optional[str]...
-00000300: 7665 7269 6669 6564 3a20 4f70 7469 6f6e  verified: Option
-00000310: 616c 5b62 6f6f 6c5d 0d0a 0964 6174 615f  al[bool]...data_
-00000320: 7572 6c5f 696d 6167 653a 204f 7074 696f  url_image: Optio
-00000330: 6e61 6c5b 7374 725d 0d0a 0972 6566 6572  nal[str]...refer
-00000340: 656e 6365 735f 7361 6665 3a20 4f70 7469  ences_safe: Opti
-00000350: 6f6e 616c 5b4c 6973 745b 5265 6665 7265  onal[List[Refere
-00000360: 6e63 655d 5d0d 0a09 0d0a 090d 0a50 6172  nce]]........Par
-00000370: 6167 7261 7068 5363 6865 6d61 203d 2063  agraphSchema = c
-00000380: 6c61 7373 5f73 6368 656d 6128 5061 7261  lass_schema(Para
-00000390: 6772 6170 682c 2062 6173 655f 7363 6865  graph, base_sche
-000003a0: 6d61 3d53 656d 616e 7468 6153 6368 656d  ma=SemanthaSchem
-000003b0: 6129 0d0a                                a)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 7420  .model.document 
+000000d0: 696d 706f 7274 2044 6f63 756d 656e 740d  import Document.
+000000e0: 0a0d 0a66 726f 6d20 7479 7069 6e67 2069  ...from typing i
+000000f0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
+00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000120: 2045 7874 7261 6374 696f 6e46 696c 6528   ExtractionFile(
+00000130: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
+00000140: 6974 7929 3a0d 0a20 2020 2022 2222 2061  ity):..    """ a
+00000150: 7574 686f 7220 7365 6d61 6e74 6861 2c20  uthor semantha, 
+00000160: 7468 6973 2069 7320 6120 6765 6e65 7261  this is a genera
+00000170: 7465 6420 636c 6173 7320 646f 206e 6f74  ted class do not
+00000180: 2063 6861 6e67 6520 6d61 6e75 616c 6c79   change manually
+00000190: 2120 2222 220d 0a20 2020 2069 643a 204f  ! """..    id: O
+000001a0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000001b0: 2020 6578 7465 726e 616c 5f69 643a 204f    external_id: O
+000001c0: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+000001d0: 2020 6e61 6d65 3a20 4f70 7469 6f6e 616c    name: Optional
+000001e0: 5b73 7472 5d0d 0a20 2020 2070 726f 6365  [str]..    proce
+000001f0: 7373 6564 3a20 4f70 7469 6f6e 616c 5b62  ssed: Optional[b
+00000200: 6f6f 6c5d 0d0a 2020 2020 6269 6e61 7279  ool]..    binary
+00000210: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+00000220: 0a20 2020 2064 6f63 756d 656e 7465 7874  .    documentext
+00000230: 7261 6374 6f72 3a20 4f70 7469 6f6e 616c  ractor: Optional
+00000240: 5b73 7472 5d0d 0a20 2020 2064 6f63 756d  [str]..    docum
+00000250: 656e 743a 204f 7074 696f 6e61 6c5b 446f  ent: Optional[Do
+00000260: 6375 6d65 6e74 5d0d 0a20 2020 2066 696c  cument]..    fil
+00000270: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
+00000280: 7374 725d 0d0a 2020 2020 6372 6561 7465  str]..    create
+00000290: 643a 204f 7074 696f 6e61 6c5b 696e 745d  d: Optional[int]
+000002a0: 0d0a 0d0a 4578 7472 6163 7469 6f6e 4669  ....ExtractionFi
+000002b0: 6c65 5363 6865 6d61 203d 2063 6c61 7373  leSchema = class
+000002c0: 5f73 6368 656d 6128 4578 7472 6163 7469  _schema(Extracti
+000002d0: 6f6e 4669 6c65 2c20 6261 7365 5f73 6368  onFile, base_sch
+000002e0: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
+000002f0: 6d61 290d 0a                             ma)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/process_information.py` & `semantha_sdk-5.5.0/semantha_sdk/model/process_information.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e76 6572 7369 6f6e 2069 6d70  odel.version imp
-000000d0: 6f72 7420 5665 7273 696f 6e0d 0a66 726f  ort Version..fro
-000000e0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000f0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-00000100: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-00000110: 5472 7565 290d 0a63 6c61 7373 2050 726f  True)..class Pro
-00000120: 6365 7373 496e 666f 726d 6174 696f 6e28  cessInformation(
-00000130: 5365 6d61 6e74 6861 4d6f 6465 6c45 6e74  SemanthaModelEnt
-00000140: 6974 7929 3a0d 0a09 2222 2220 6175 7468  ity):...""" auth
-00000150: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
-00000160: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
-00000170: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
-00000180: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
-00000190: 2222 0d0a 0963 7265 6174 6564 3a20 4f70  ""...created: Op
-000001a0: 7469 6f6e 616c 5b73 7472 5d0d 0a09 6564  tional[str]...ed
-000001b0: 6974 6564 3a20 4f70 7469 6f6e 616c 5b73  ited: Optional[s
-000001c0: 7472 5d0d 0a09 7665 7273 696f 6e3a 204f  tr]...version: O
-000001d0: 7074 696f 6e61 6c5b 5665 7273 696f 6e5d  ptional[Version]
-000001e0: 0d0a 090d 0a09 0d0a 5072 6f63 6573 7349  ........ProcessI
-000001f0: 6e66 6f72 6d61 7469 6f6e 5363 6865 6d61  nformationSchema
-00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
-00000210: 5072 6f63 6573 7349 6e66 6f72 6d61 7469  ProcessInformati
-00000220: 6f6e 2c20 6261 7365 5f73 6368 656d 613d  on, base_schema=
-00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
-00000240: 0a                                       .
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e76 6572 7369 6f6e 2069  .model.version i
+000000d0: 6d70 6f72 7420 5665 7273 696f 6e0d 0a0d  mport Version...
+000000e0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+000000f0: 6f72 7420 4f70 7469 6f6e 616c 0d0a 0d0a  ort Optional....
+00000100: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
+00000110: 6e3d 5472 7565 290d 0a63 6c61 7373 2050  n=True)..class P
+00000120: 726f 6365 7373 496e 666f 726d 6174 696f  rocessInformatio
+00000130: 6e28 5365 6d61 6e74 6861 4d6f 6465 6c45  n(SemanthaModelE
+00000140: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000150: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000160: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000170: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000180: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000190: 6c79 2120 2222 220d 0a20 2020 2063 7265  ly! """..    cre
+000001a0: 6174 6564 3a20 4f70 7469 6f6e 616c 5b73  ated: Optional[s
+000001b0: 7472 5d0d 0a20 2020 2065 6469 7465 643a  tr]..    edited:
+000001c0: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
+000001d0: 2020 2020 7665 7273 696f 6e3a 204f 7074      version: Opt
+000001e0: 696f 6e61 6c5b 5665 7273 696f 6e5d 0d0a  ional[Version]..
+000001f0: 0d0a 5072 6f63 6573 7349 6e66 6f72 6d61  ..ProcessInforma
+00000200: 7469 6f6e 5363 6865 6d61 203d 2063 6c61  tionSchema = cla
+00000210: 7373 5f73 6368 656d 6128 5072 6f63 6573  ss_schema(Proces
+00000220: 7349 6e66 6f72 6d61 7469 6f6e 2c20 6261  sInformation, ba
+00000230: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000240: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/reference.py` & `semantha_sdk-5.5.0/semantha_sdk/model/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4469 6374 2c20 4f70 7469 6f6e 616c 0d0a  Dict, Optional..
-000000d0: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
-000000e0: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
-000000f0: 7373 2052 6566 6572 656e 6365 2853 656d  ss Reference(Sem
-00000100: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
-00000110: 293a 0d0a 0922 2222 2061 7574 686f 7220  ):...""" author 
-00000120: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
-00000130: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
-00000140: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
-00000150: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
-00000160: 0a09 646f 6375 6d65 6e74 5f69 643a 204f  ..document_id: O
-00000170: 7074 696f 6e61 6c5b 7374 725d 0d0a 0964  ptional[str]...d
-00000180: 6f63 756d 656e 745f 6e61 6d65 3a20 4f70  ocument_name: Op
-00000190: 7469 6f6e 616c 5b73 7472 5d0d 0a09 7061  tional[str]...pa
-000001a0: 6765 5f6e 756d 6265 723a 204f 7074 696f  ge_number: Optio
-000001b0: 6e61 6c5b 696e 745d 0d0a 0970 6172 6167  nal[int]...parag
-000001c0: 7261 7068 5f69 643a 204f 7074 696f 6e61  raph_id: Optiona
-000001d0: 6c5b 7374 725d 0d0a 0973 656e 7465 6e63  l[str]...sentenc
-000001e0: 655f 6964 3a20 4f70 7469 6f6e 616c 5b73  e_id: Optional[s
-000001f0: 7472 5d0d 0a09 7369 6d69 6c61 7269 7479  tr]...similarity
-00000200: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00000210: 5d0d 0a09 7465 7874 3a20 4f70 7469 6f6e  ]...text: Option
-00000220: 616c 5b73 7472 5d0d 0a09 636f 6e74 6578  al[str]...contex
-00000230: 743a 204f 7074 696f 6e61 6c5b 4469 6374  t: Optional[Dict
-00000240: 5b73 7472 2c20 7374 725d 5d0d 0a09 7479  [str, str]]...ty
-00000250: 7065 3a20 4f70 7469 6f6e 616c 5b73 7472  pe: Optional[str
-00000260: 5d0d 0a09 636f 6c6f 723a 204f 7074 696f  ]...color: Optio
-00000270: 6e61 6c5b 7374 725d 0d0a 0963 6f6d 6d65  nal[str]...comme
-00000280: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-00000290: 5d0d 0a09 6861 735f 6f70 706f 7369 7465  ]...has_opposite
-000002a0: 5f6d 6561 6e69 6e67 3a20 4f70 7469 6f6e  _meaning: Option
-000002b0: 616c 5b62 6f6f 6c5d 0d0a 090d 0a09 0d0a  al[bool]........
-000002c0: 5265 6665 7265 6e63 6553 6368 656d 6120  ReferenceSchema 
-000002d0: 3d20 636c 6173 735f 7363 6865 6d61 2852  = class_schema(R
-000002e0: 6566 6572 656e 6365 2c20 6261 7365 5f73  eference, base_s
-000002f0: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
-00000300: 6865 6d61 290d 0a                        hema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4f70 7469 6f6e 616c 0d0a 0d0a 4064  t Optional....@d
+000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+000000e0: 5472 7565 290d 0a63 6c61 7373 2049 6e66  True)..class Inf
+000000f0: 6f28 5365 6d61 6e74 6861 4d6f 6465 6c45  o(SemanthaModelE
+00000100: 6e74 6974 7929 3a0d 0a20 2020 2022 2222  ntity):..    """
+00000110: 2061 7574 686f 7220 7365 6d61 6e74 6861   author semantha
+00000120: 2c20 7468 6973 2069 7320 6120 6765 6e65  , this is a gene
+00000130: 7261 7465 6420 636c 6173 7320 646f 206e  rated class do n
+00000140: 6f74 2063 6861 6e67 6520 6d61 6e75 616c  ot change manual
+00000150: 6c79 2120 2222 220d 0a20 2020 2074 6974  ly! """..    tit
+00000160: 6c65 3a20 4f70 7469 6f6e 616c 5b73 7472  le: Optional[str
+00000170: 5d0d 0a20 2020 2076 656e 646f 723a 204f  ]..    vendor: O
+00000180: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000190: 2020 7469 6d65 3a20 4f70 7469 6f6e 616c    time: Optional
+000001a0: 5b73 7472 5d0d 0a20 2020 2067 6974 3a20  [str]..    git: 
+000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001c0: 2020 2076 6572 7369 6f6e 3a20 4f70 7469     version: Opti
+000001d0: 6f6e 616c 5b73 7472 5d0d 0a0d 0a49 6e66  onal[str]....Inf
+000001e0: 6f53 6368 656d 6120 3d20 636c 6173 735f  oSchema = class_
+000001f0: 7363 6865 6d61 2849 6e66 6f2c 2062 6173  schema(Info, bas
+00000200: 655f 7363 6865 6d61 3d53 656d 616e 7468  e_schema=Semanth
+00000210: 6153 6368 656d 6129 0d0a                 aSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.5.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.5.0/semantha_sdk/model/semantic_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
 from semantha_sdk.model.extraction_file import ExtractionFile
+
 from semantha_sdk.model.model_instance import ModelInstance
+
 from semantha_sdk.model.process_information import ProcessInformation
+
 from semantha_sdk.model.table_instance import TableInstance
-from typing import List, Optional
 
+from typing import List
+from typing import Optional
 
 @dataclass(frozen=True)
 class SemanticModel(SemanthaModelEntity):
-	""" author semantha, this is a generated class do not change manually! """
-	files: Optional[List[ExtractionFile]]
-	instances: Optional[List[ModelInstance]]
-	tables: Optional[List[TableInstance]]
-	process_information: Optional[ProcessInformation]
-	
-	
+    """ author semantha, this is a generated class do not change manually! """
+    files: Optional[List[ExtractionFile]]
+    instances: Optional[List[ModelInstance]]
+    tables: Optional[List[TableInstance]]
+    process_information: Optional[ProcessInformation]
+
 SemanticModelSchema = class_schema(SemanticModel, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.5.0/semantha_sdk/model/domain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4f70 7469 6f6e 616c 0d0a 0d0a 0d0a 4064  Optional......@d
-000000d0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-000000e0: 5472 7565 290d 0a63 6c61 7373 2053 656d  True)..class Sem
-000000f0: 6953 7570 6572 5669 7365 6444 6f63 756d  iSuperVisedDocum
-00000100: 656e 7428 5365 6d61 6e74 6861 4d6f 6465  ent(SemanthaMode
-00000110: 6c45 6e74 6974 7929 3a0d 0a09 2222 2220  lEntity):...""" 
-00000120: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-00000130: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-00000140: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-00000150: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000160: 7921 2022 2222 0d0a 0964 6f63 756d 656e  y! """...documen
-00000170: 745f 6964 3a20 4f70 7469 6f6e 616c 5b73  t_id: Optional[s
-00000180: 7472 5d0d 0a09 746f 7069 635f 6964 3a20  tr]...topic_id: 
-00000190: 4f70 7469 6f6e 616c 5b69 6e74 5d0d 0a09  Optional[int]...
-000001a0: 0d0a 090d 0a53 656d 6953 7570 6572 5669  .....SemiSuperVi
-000001b0: 7365 6444 6f63 756d 656e 7453 6368 656d  sedDocumentSchem
-000001c0: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-000001d0: 2853 656d 6953 7570 6572 5669 7365 6444  (SemiSuperVisedD
-000001e0: 6f63 756d 656e 742c 2062 6173 655f 7363  ocument, base_sc
-000001f0: 6865 6d61 3d53 656d 616e 7468 6153 6368  hema=SemanthaSch
-00000200: 656d 6129 0d0a                           ema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e73 6574 7469 6e67 7320  .model.settings 
+000000d0: 696d 706f 7274 2053 6574 7469 6e67 730d  import Settings.
+000000e0: 0a0d 0a66 726f 6d20 7479 7069 6e67 2069  ...from typing i
+000000f0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
+00000100: 0d0a 4064 6174 6163 6c61 7373 2866 726f  ..@dataclass(fro
+00000110: 7a65 6e3d 5472 7565 290d 0a63 6c61 7373  zen=True)..class
+00000120: 2044 6f6d 6169 6e28 5365 6d61 6e74 6861   Domain(Semantha
+00000130: 4d6f 6465 6c45 6e74 6974 7929 3a0d 0a20  ModelEntity):.. 
+00000140: 2020 2022 2222 2061 7574 686f 7220 7365     """ author se
+00000150: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
+00000160: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
+00000170: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
+00000180: 6d61 6e75 616c 6c79 2120 2222 220d 0a20  manually! """.. 
+00000190: 2020 2069 643a 204f 7074 696f 6e61 6c5b     id: Optional[
+000001a0: 7374 725d 0d0a 2020 2020 6e61 6d65 3a20  str]..    name: 
+000001b0: 4f70 7469 6f6e 616c 5b73 7472 5d0d 0a20  Optional[str].. 
+000001c0: 2020 2062 6173 655f 7572 6c3a 204f 7074     base_url: Opt
+000001d0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000001e0: 7365 7474 696e 6773 3a20 4f70 7469 6f6e  settings: Option
+000001f0: 616c 5b53 6574 7469 6e67 735d 0d0a 0d0a  al[Settings]....
+00000200: 446f 6d61 696e 5363 6865 6d61 203d 2063  DomainSchema = c
+00000210: 6c61 7373 5f73 6368 656d 6128 446f 6d61  lass_schema(Doma
+00000220: 696e 2c20 6261 7365 5f73 6368 656d 613d  in, base_schema=
+00000230: 5365 6d61 6e74 6861 5363 6865 6d61 290d  SemanthaSchema).
+00000240: 0a                                       .
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/sentence.py` & `semantha_sdk-5.5.0/semantha_sdk/model/sentence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e64 6f63 756d 656e 745f 6e61  odel.document_na
-000000d0: 6d65 645f 656e 7469 7479 2069 6d70 6f72  med_entity impor
-000000e0: 7420 446f 6375 6d65 6e74 4e61 6d65 6445  t DocumentNamedE
-000000f0: 6e74 6974 790d 0a66 726f 6d20 7365 6d61  ntity..from sema
-00000100: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
-00000110: 6563 7420 696d 706f 7274 2052 6563 740d  ect import Rect.
-00000120: 0a66 726f 6d20 7365 6d61 6e74 6861 5f73  .from semantha_s
-00000130: 646b 2e6d 6f64 656c 2e72 6566 6572 656e  dk.model.referen
-00000140: 6365 2069 6d70 6f72 7420 5265 6665 7265  ce import Refere
-00000150: 6e63 650d 0a66 726f 6d20 7479 7069 6e67  nce..from typing
-00000160: 2069 6d70 6f72 7420 4c69 7374 2c20 4f70   import List, Op
-00000170: 7469 6f6e 616c 0d0a 0d0a 0d0a 4064 6174  tional......@dat
-00000180: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
-00000190: 7565 290d 0a63 6c61 7373 2053 656e 7465  ue)..class Sente
-000001a0: 6e63 6528 5365 6d61 6e74 6861 4d6f 6465  nce(SemanthaMode
-000001b0: 6c45 6e74 6974 7929 3a0d 0a09 2222 2220  lEntity):...""" 
-000001c0: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
-000001d0: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
-000001e0: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
-000001f0: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
-00000200: 7921 2022 2222 0d0a 0969 643a 204f 7074  y! """...id: Opt
-00000210: 696f 6e61 6c5b 7374 725d 0d0a 0974 6578  ional[str]...tex
-00000220: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
-00000230: 0d0a 0964 6f63 756d 656e 745f 6e61 6d65  ...document_name
-00000240: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
-00000250: 0a09 6e61 6d65 645f 656e 7469 7469 6573  ..named_entities
-00000260: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-00000270: 446f 6375 6d65 6e74 4e61 6d65 6445 6e74  DocumentNamedEnt
-00000280: 6974 795d 5d0d 0a09 7265 6665 7265 6e63  ity]]...referenc
-00000290: 6573 3a20 4f70 7469 6f6e 616c 5b4c 6973  es: Optional[Lis
-000002a0: 745b 5265 6665 7265 6e63 655d 5d0d 0a09  t[Reference]]...
-000002b0: 6172 6561 733a 204f 7074 696f 6e61 6c5b  areas: Optional[
-000002c0: 4c69 7374 5b52 6563 745d 5d0d 0a09 0d0a  List[Rect]].....
-000002d0: 090d 0a53 656e 7465 6e63 6553 6368 656d  ...SentenceSchem
-000002e0: 6120 3d20 636c 6173 735f 7363 6865 6d61  a = class_schema
-000002f0: 2853 656e 7465 6e63 652c 2062 6173 655f  (Sentence, base_
-00000300: 7363 6865 6d61 3d53 656d 616e 7468 6153  schema=SemanthaS
-00000310: 6368 656d 6129 0d0a                      chema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e64 6f63 756d 656e 745f  .model.document_
+000000d0: 6e61 6d65 645f 656e 7469 7479 2069 6d70  named_entity imp
+000000e0: 6f72 7420 446f 6375 6d65 6e74 4e61 6d65  ort DocumentName
+000000f0: 6445 6e74 6974 790d 0a0d 0a66 726f 6d20  dEntity....from 
+00000100: 7365 6d61 6e74 6861 5f73 646b 2e6d 6f64  semantha_sdk.mod
+00000110: 656c 2e72 6563 7420 696d 706f 7274 2052  el.rect import R
+00000120: 6563 740d 0a0d 0a66 726f 6d20 7365 6d61  ect....from sema
+00000130: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e72  ntha_sdk.model.r
+00000140: 6566 6572 656e 6365 2069 6d70 6f72 7420  eference import 
+00000150: 5265 6665 7265 6e63 650d 0a0d 0a66 726f  Reference....fro
+00000160: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00000170: 4c69 7374 0d0a 6672 6f6d 2074 7970 696e  List..from typin
+00000180: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
+00000190: 6c0d 0a0d 0a40 6461 7461 636c 6173 7328  l....@dataclass(
+000001a0: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
+000001b0: 6173 7320 5365 6e74 656e 6365 2853 656d  ass Sentence(Sem
+000001c0: 616e 7468 614d 6f64 656c 456e 7469 7479  anthaModelEntity
+000001d0: 293a 0d0a 2020 2020 2222 2220 6175 7468  ):..    """ auth
+000001e0: 6f72 2073 656d 616e 7468 612c 2074 6869  or semantha, thi
+000001f0: 7320 6973 2061 2067 656e 6572 6174 6564  s is a generated
+00000200: 2063 6c61 7373 2064 6f20 6e6f 7420 6368   class do not ch
+00000210: 616e 6765 206d 616e 7561 6c6c 7921 2022  ange manually! "
+00000220: 2222 0d0a 2020 2020 6964 3a20 4f70 7469  ""..    id: Opti
+00000230: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2074  onal[str]..    t
+00000240: 6578 743a 204f 7074 696f 6e61 6c5b 7374  ext: Optional[st
+00000250: 725d 0d0a 2020 2020 646f 6375 6d65 6e74  r]..    document
+00000260: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
+00000270: 7374 725d 0d0a 2020 2020 6e61 6d65 645f  str]..    named_
+00000280: 656e 7469 7469 6573 3a20 4f70 7469 6f6e  entities: Option
+00000290: 616c 5b4c 6973 745b 446f 6375 6d65 6e74  al[List[Document
+000002a0: 4e61 6d65 6445 6e74 6974 795d 5d0d 0a20  NamedEntity]].. 
+000002b0: 2020 2072 6566 6572 656e 6365 733a 204f     references: O
+000002c0: 7074 696f 6e61 6c5b 4c69 7374 5b52 6566  ptional[List[Ref
+000002d0: 6572 656e 6365 5d5d 0d0a 2020 2020 6172  erence]]..    ar
+000002e0: 6561 733a 204f 7074 696f 6e61 6c5b 4c69  eas: Optional[Li
+000002f0: 7374 5b52 6563 745d 5d0d 0a0d 0a53 656e  st[Rect]]....Sen
+00000300: 7465 6e63 6553 6368 656d 6120 3d20 636c  tenceSchema = cl
+00000310: 6173 735f 7363 6865 6d61 2853 656e 7465  ass_schema(Sente
+00000320: 6e63 652c 2062 6173 655f 7363 6865 6d61  nce, base_schema
+00000330: 3d53 656d 616e 7468 6153 6368 656d 6129  =SemanthaSchema)
+00000340: 0d0a                                     ..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e63 6c75 7374 6572 696e 675f  odel.clustering_
-000000d0: 7265 7370 6f6e 7365 2069 6d70 6f72 7420  response import 
-000000e0: 436c 7573 7465 7269 6e67 5265 7370 6f6e  ClusteringRespon
-000000f0: 7365 0d0a 6672 6f6d 2073 656d 616e 7468  se..from semanth
-00000100: 615f 7364 6b2e 6d6f 6465 6c2e 7265 7370  a_sdk.model.resp
-00000110: 6f6e 7365 5f6d 6574 615f 696e 666f 2069  onse_meta_info i
-00000120: 6d70 6f72 7420 5265 7370 6f6e 7365 4d65  mport ResponseMe
-00000130: 7461 496e 666f 0d0a 6672 6f6d 2074 7970  taInfo..from typ
-00000140: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
-00000150: 6e61 6c0d 0a0d 0a0d 0a40 6461 7461 636c  nal......@datacl
-00000160: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00000170: 0d0a 636c 6173 7320 536d 6172 7443 6c75  ..class SmartClu
-00000180: 7374 6572 5265 7370 6f6e 7365 436f 6e74  sterResponseCont
-00000190: 6169 6e65 7228 5365 6d61 6e74 6861 4d6f  ainer(SemanthaMo
-000001a0: 6465 6c45 6e74 6974 7929 3a0d 0a09 2222  delEntity):...""
-000001b0: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-000001c0: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-000001d0: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-000001e0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001f0: 6c6c 7921 2022 2222 0d0a 096d 6574 613a  lly! """...meta:
-00000200: 204f 7074 696f 6e61 6c5b 5265 7370 6f6e   Optional[Respon
-00000210: 7365 4d65 7461 496e 666f 5d0d 0a09 6461  seMetaInfo]...da
-00000220: 7461 3a20 4f70 7469 6f6e 616c 5b43 6c75  ta: Optional[Clu
-00000230: 7374 6572 696e 6752 6573 706f 6e73 655d  steringResponse]
-00000240: 0d0a 090d 0a09 0d0a 536d 6172 7443 6c75  ........SmartClu
-00000250: 7374 6572 5265 7370 6f6e 7365 436f 6e74  sterResponseCont
-00000260: 6169 6e65 7253 6368 656d 6120 3d20 636c  ainerSchema = cl
-00000270: 6173 735f 7363 6865 6d61 2853 6d61 7274  ass_schema(Smart
-00000280: 436c 7573 7465 7252 6573 706f 6e73 6543  ClusterResponseC
-00000290: 6f6e 7461 696e 6572 2c20 6261 7365 5f73  ontainer, base_s
-000002a0: 6368 656d 613d 5365 6d61 6e74 6861 5363  chema=SemanthaSc
-000002b0: 6865 6d61 290d 0a                        hema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e63 6c75 7374 6572 696e  .model.clusterin
+000000d0: 675f 7265 7370 6f6e 7365 2069 6d70 6f72  g_response impor
+000000e0: 7420 436c 7573 7465 7269 6e67 5265 7370  t ClusteringResp
+000000f0: 6f6e 7365 0d0a 0d0a 6672 6f6d 2073 656d  onse....from sem
+00000100: 616e 7468 615f 7364 6b2e 6d6f 6465 6c2e  antha_sdk.model.
+00000110: 7265 7370 6f6e 7365 5f6d 6574 615f 696e  response_meta_in
+00000120: 666f 2069 6d70 6f72 7420 5265 7370 6f6e  fo import Respon
+00000130: 7365 4d65 7461 496e 666f 0d0a 0d0a 6672  seMetaInfo....fr
+00000140: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000150: 204f 7074 696f 6e61 6c0d 0a0d 0a40 6461   Optional....@da
+00000160: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
+00000170: 7275 6529 0d0a 636c 6173 7320 536d 6172  rue)..class Smar
+00000180: 7443 6c75 7374 6572 5265 7370 6f6e 7365  tClusterResponse
+00000190: 436f 6e74 6169 6e65 7228 5365 6d61 6e74  Container(Semant
+000001a0: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
+000001b0: 0a20 2020 2022 2222 2061 7574 686f 7220  .    """ author 
+000001c0: 7365 6d61 6e74 6861 2c20 7468 6973 2069  semantha, this i
+000001d0: 7320 6120 6765 6e65 7261 7465 6420 636c  s a generated cl
+000001e0: 6173 7320 646f 206e 6f74 2063 6861 6e67  ass do not chang
+000001f0: 6520 6d61 6e75 616c 6c79 2120 2222 220d  e manually! """.
+00000200: 0a20 2020 206d 6574 613a 204f 7074 696f  .    meta: Optio
+00000210: 6e61 6c5b 5265 7370 6f6e 7365 4d65 7461  nal[ResponseMeta
+00000220: 496e 666f 5d0d 0a20 2020 2064 6174 613a  Info]..    data:
+00000230: 204f 7074 696f 6e61 6c5b 436c 7573 7465   Optional[Cluste
+00000240: 7269 6e67 5265 7370 6f6e 7365 5d0d 0a0d  ringResponse]...
+00000250: 0a53 6d61 7274 436c 7573 7465 7252 6573  .SmartClusterRes
+00000260: 706f 6e73 6543 6f6e 7461 696e 6572 5363  ponseContainerSc
+00000270: 6865 6d61 203d 2063 6c61 7373 5f73 6368  hema = class_sch
+00000280: 656d 6128 536d 6172 7443 6c75 7374 6572  ema(SmartCluster
+00000290: 5265 7370 6f6e 7365 436f 6e74 6169 6e65  ResponseContaine
+000002a0: 722c 2062 6173 655f 7363 6865 6d61 3d53  r, base_schema=S
+000002b0: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.5.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e73 656d 695f 7375 7065 725f  odel.semi_super_
-000000d0: 7669 7365 645f 646f 6375 6d65 6e74 2069  vised_document i
-000000e0: 6d70 6f72 7420 5365 6d69 5375 7065 7256  mport SemiSuperV
-000000f0: 6973 6564 446f 6375 6d65 6e74 0d0a 6672  isedDocument..fr
-00000100: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000110: 204c 6973 742c 204f 7074 696f 6e61 6c0d   List, Optional.
-00000120: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
-00000130: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-00000140: 6173 7320 536d 6172 7443 6c75 7374 6572  ass SmartCluster
-00000150: 5365 6d69 5375 7065 7276 6973 6564 5265  SemiSupervisedRe
-00000160: 7175 6573 7428 5365 6d61 6e74 6861 4d6f  quest(SemanthaMo
-00000170: 6465 6c45 6e74 6974 7929 3a0d 0a09 2222  delEntity):...""
-00000180: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
-00000190: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
-000001a0: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
-000001b0: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
-000001c0: 6c6c 7921 2022 2222 0d0a 0963 6c75 7374  lly! """...clust
-000001d0: 6572 696e 675f 6e61 6d65 3a20 4f70 7469  ering_name: Opti
-000001e0: 6f6e 616c 5b73 7472 5d0d 0a09 6d69 6e5f  onal[str]...min_
-000001f0: 636c 7573 7465 725f 7369 7a65 3a20 4f70  cluster_size: Op
-00000200: 7469 6f6e 616c 5b73 7472 5d0d 0a09 636c  tional[str]...cl
-00000210: 7573 7465 7269 6e67 5f73 7472 7563 7475  ustering_structu
-00000220: 7265 3a20 4f70 7469 6f6e 616c 5b73 7472  re: Optional[str
-00000230: 5d0d 0a09 746f 7069 635f 6f76 6572 5f74  ]...topic_over_t
-00000240: 696d 655f 7261 6e67 653a 204f 7074 696f  ime_range: Optio
-00000250: 6e61 6c5b 7374 725d 0d0a 0972 6564 7563  nal[str]...reduc
-00000260: 655f 6f75 746c 6965 7273 3a20 4f70 7469  e_outliers: Opti
-00000270: 6f6e 616c 5b62 6f6f 6c5d 0d0a 0975 6d61  onal[bool]...uma
-00000280: 705f 6e72 5f6f 665f 6e65 6967 6862 6f72  p_nr_of_neighbor
-00000290: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-000002a0: 0d0a 0964 6f63 756d 656e 7473 3a20 4f70  ...documents: Op
-000002b0: 7469 6f6e 616c 5b4c 6973 745b 5365 6d69  tional[List[Semi
-000002c0: 5375 7065 7256 6973 6564 446f 6375 6d65  SuperVisedDocume
-000002d0: 6e74 5d5d 0d0a 090d 0a09 0d0a 536d 6172  nt]]........Smar
-000002e0: 7443 6c75 7374 6572 5365 6d69 5375 7065  tClusterSemiSupe
-000002f0: 7276 6973 6564 5265 7175 6573 7453 6368  rvisedRequestSch
-00000300: 656d 6120 3d20 636c 6173 735f 7363 6865  ema = class_sche
-00000310: 6d61 2853 6d61 7274 436c 7573 7465 7253  ma(SmartClusterS
-00000320: 656d 6953 7570 6572 7669 7365 6452 6571  emiSupervisedReq
-00000330: 7565 7374 2c20 6261 7365 5f73 6368 656d  uest, base_schem
-00000340: 613d 5365 6d61 6e74 6861 5363 6865 6d61  a=SemanthaSchema
-00000350: 290d 0a                                  )..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e73 656d 695f 7375 7065  .model.semi_supe
+000000d0: 725f 7669 7365 645f 646f 6375 6d65 6e74  r_vised_document
+000000e0: 2069 6d70 6f72 7420 5365 6d69 5375 7065   import SemiSupe
+000000f0: 7256 6973 6564 446f 6375 6d65 6e74 0d0a  rVisedDocument..
+00000100: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+00000110: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
+00000120: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+00000130: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
+00000140: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00000150: 290d 0a63 6c61 7373 2053 6d61 7274 436c  )..class SmartCl
+00000160: 7573 7465 7253 656d 6953 7570 6572 7669  usterSemiSupervi
+00000170: 7365 6452 6571 7565 7374 2853 656d 616e  sedRequest(Seman
+00000180: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
+00000190: 0d0a 2020 2020 2222 2220 6175 7468 6f72  ..    """ author
+000001a0: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
+000001b0: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
+000001c0: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
+000001d0: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
+000001e0: 0d0a 2020 2020 636c 7573 7465 7269 6e67  ..    clustering
+000001f0: 5f6e 616d 653a 204f 7074 696f 6e61 6c5b  _name: Optional[
+00000200: 7374 725d 0d0a 2020 2020 6d69 6e5f 636c  str]..    min_cl
+00000210: 7573 7465 725f 7369 7a65 3a20 4f70 7469  uster_size: Opti
+00000220: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2063  onal[str]..    c
+00000230: 6c75 7374 6572 696e 675f 7374 7275 6374  lustering_struct
+00000240: 7572 653a 204f 7074 696f 6e61 6c5b 7374  ure: Optional[st
+00000250: 725d 0d0a 2020 2020 746f 7069 635f 6f76  r]..    topic_ov
+00000260: 6572 5f74 696d 655f 7261 6e67 653a 204f  er_time_range: O
+00000270: 7074 696f 6e61 6c5b 7374 725d 0d0a 2020  ptional[str]..  
+00000280: 2020 7265 6475 6365 5f6f 7574 6c69 6572    reduce_outlier
+00000290: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
+000002a0: 5d0d 0a20 2020 2075 6d61 705f 6e72 5f6f  ]..    umap_nr_o
+000002b0: 665f 6e65 6967 6862 6f72 733a 204f 7074  f_neighbors: Opt
+000002c0: 696f 6e61 6c5b 696e 745d 0d0a 2020 2020  ional[int]..    
+000002d0: 646f 6375 6d65 6e74 733a 204f 7074 696f  documents: Optio
+000002e0: 6e61 6c5b 4c69 7374 5b53 656d 6953 7570  nal[List[SemiSup
+000002f0: 6572 5669 7365 6444 6f63 756d 656e 745d  erVisedDocument]
+00000300: 5d0d 0a0d 0a53 6d61 7274 436c 7573 7465  ]....SmartCluste
+00000310: 7253 656d 6953 7570 6572 7669 7365 6452  rSemiSupervisedR
+00000320: 6571 7565 7374 5363 6865 6d61 203d 2063  equestSchema = c
+00000330: 6c61 7373 5f73 6368 656d 6128 536d 6172  lass_schema(Smar
+00000340: 7443 6c75 7374 6572 5365 6d69 5375 7065  tClusterSemiSupe
+00000350: 7276 6973 6564 5265 7175 6573 742c 2062  rvisedRequest, b
+00000360: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000370: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/statistic.py` & `semantha_sdk-5.5.0/semantha_sdk/model/statistic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e74 6167 5f64 6f63 7320 696d  odel.tag_docs im
-000000d0: 706f 7274 2054 6167 446f 6373 0d0a 6672  port TagDocs..fr
-000000e0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-000000f0: 204c 6973 742c 204f 7074 696f 6e61 6c0d   List, Optional.
-00000100: 0a0d 0a0d 0a40 6461 7461 636c 6173 7328  .....@dataclass(
-00000110: 6672 6f7a 656e 3d54 7275 6529 0d0a 636c  frozen=True)..cl
-00000120: 6173 7320 5374 6174 6973 7469 6328 5365  ass Statistic(Se
-00000130: 6d61 6e74 6861 4d6f 6465 6c45 6e74 6974  manthaModelEntit
-00000140: 7929 3a0d 0a09 2222 2220 6175 7468 6f72  y):...""" author
-00000150: 2073 656d 616e 7468 612c 2074 6869 7320   semantha, this 
-00000160: 6973 2061 2067 656e 6572 6174 6564 2063  is a generated c
-00000170: 6c61 7373 2064 6f20 6e6f 7420 6368 616e  lass do not chan
-00000180: 6765 206d 616e 7561 6c6c 7921 2022 2222  ge manually! """
-00000190: 0d0a 096c 6962 7261 7279 5f73 697a 653a  ...library_size:
-000001a0: 204f 7074 696f 6e61 6c5b 696e 745d 0d0a   Optional[int]..
-000001b0: 0973 697a 653a 204f 7074 696f 6e61 6c5b  .size: Optional[
-000001c0: 696e 745d 0d0a 096e 756d 6265 725f 6f66  int]...number_of
-000001d0: 5f73 656e 7465 6e63 6573 3a20 4f70 7469  _sentences: Opti
-000001e0: 6f6e 616c 5b69 6e74 5d0d 0a09 646f 6373  onal[int]...docs
-000001f0: 5f70 6572 5f74 6167 3a20 4f70 7469 6f6e  _per_tag: Option
-00000200: 616c 5b4c 6973 745b 5461 6744 6f63 735d  al[List[TagDocs]
-00000210: 5d0d 0a09 0d0a 090d 0a53 7461 7469 7374  ]........Statist
-00000220: 6963 5363 6865 6d61 203d 2063 6c61 7373  icSchema = class
-00000230: 5f73 6368 656d 6128 5374 6174 6973 7469  _schema(Statisti
-00000240: 632c 2062 6173 655f 7363 6865 6d61 3d53  c, base_schema=S
-00000250: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e74 6167 5f64 6f63 7320  .model.tag_docs 
+000000d0: 696d 706f 7274 2054 6167 446f 6373 0d0a  import TagDocs..
+000000e0: 0d0a 6672 6f6d 2074 7970 696e 6720 696d  ..from typing im
+000000f0: 706f 7274 204c 6973 740d 0a66 726f 6d20  port List..from 
+00000100: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+00000110: 7469 6f6e 616c 0d0a 0d0a 4064 6174 6163  tional....@datac
+00000120: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00000130: 290d 0a63 6c61 7373 2053 7461 7469 7374  )..class Statist
+00000140: 6963 2853 656d 616e 7468 614d 6f64 656c  ic(SemanthaModel
+00000150: 456e 7469 7479 293a 0d0a 2020 2020 2222  Entity):..    ""
+00000160: 2220 6175 7468 6f72 2073 656d 616e 7468  " author semanth
+00000170: 612c 2074 6869 7320 6973 2061 2067 656e  a, this is a gen
+00000180: 6572 6174 6564 2063 6c61 7373 2064 6f20  erated class do 
+00000190: 6e6f 7420 6368 616e 6765 206d 616e 7561  not change manua
+000001a0: 6c6c 7921 2022 2222 0d0a 2020 2020 6c69  lly! """..    li
+000001b0: 6272 6172 795f 7369 7a65 3a20 4f70 7469  brary_size: Opti
+000001c0: 6f6e 616c 5b69 6e74 5d0d 0a20 2020 2073  onal[int]..    s
+000001d0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+000001e0: 745d 0d0a 2020 2020 6e75 6d62 6572 5f6f  t]..    number_o
+000001f0: 665f 7365 6e74 656e 6365 733a 204f 7074  f_sentences: Opt
+00000200: 696f 6e61 6c5b 696e 745d 0d0a 2020 2020  ional[int]..    
+00000210: 646f 6373 5f70 6572 5f74 6167 3a20 4f70  docs_per_tag: Op
+00000220: 7469 6f6e 616c 5b4c 6973 745b 5461 6744  tional[List[TagD
+00000230: 6f63 735d 5d0d 0a0d 0a53 7461 7469 7374  ocs]]....Statist
+00000240: 6963 5363 6865 6d61 203d 2063 6c61 7373  icSchema = class
+00000250: 5f73 6368 656d 6128 5374 6174 6973 7469  _schema(Statisti
+00000260: 632c 2062 6173 655f 7363 6865 6d61 3d53  c, base_schema=S
+00000270: 656d 616e 7468 6153 6368 656d 6129 0d0a  emanthaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/synonym.py` & `semantha_sdk-5.5.0/semantha_sdk/model/model_class.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000c0: 4c69 7374 2c20 4f70 7469 6f6e 616c 0d0a  List, Optional..
-000000d0: 0d0a 0d0a 4064 6174 6163 6c61 7373 2866  ....@dataclass(f
-000000e0: 726f 7a65 6e3d 5472 7565 290d 0a63 6c61  rozen=True)..cla
-000000f0: 7373 2053 796e 6f6e 796d 2853 656d 616e  ss Synonym(Seman
-00000100: 7468 614d 6f64 656c 456e 7469 7479 293a  thaModelEntity):
-00000110: 0d0a 0922 2222 2061 7574 686f 7220 7365  ...""" author se
-00000120: 6d61 6e74 6861 2c20 7468 6973 2069 7320  mantha, this is 
-00000130: 6120 6765 6e65 7261 7465 6420 636c 6173  a generated clas
-00000140: 7320 646f 206e 6f74 2063 6861 6e67 6520  s do not change 
-00000150: 6d61 6e75 616c 6c79 2120 2222 220d 0a09  manually! """...
-00000160: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
-00000170: 5d0d 0a09 776f 7264 3a20 4f70 7469 6f6e  ]...word: Option
-00000180: 616c 5b73 7472 5d0d 0a09 7265 6765 783a  al[str]...regex:
-00000190: 204f 7074 696f 6e61 6c5b 7374 725d 0d0a   Optional[str]..
-000001a0: 0973 796e 6f6e 796d 3a20 4f70 7469 6f6e  .synonym: Option
-000001b0: 616c 5b73 7472 5d0d 0a09 7461 6773 3a20  al[str]...tags: 
-000001c0: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-000001d0: 725d 5d0d 0a09 0d0a 090d 0a53 796e 6f6e  r]]........Synon
-000001e0: 796d 5363 6865 6d61 203d 2063 6c61 7373  ymSchema = class
-000001f0: 5f73 6368 656d 6128 5379 6e6f 6e79 6d2c  _schema(Synonym,
-00000200: 2062 6173 655f 7363 6865 6d61 3d53 656d   base_schema=Sem
-00000210: 616e 7468 6153 6368 656d 6129 0d0a       anthaSchema)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+000000c0: 7420 4c69 7374 0d0a 6672 6f6d 2074 7970  t List..from typ
+000000d0: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+000000e0: 6e61 6c0d 0a0d 0a40 6461 7461 636c 6173  nal....@dataclas
+000000f0: 7328 6672 6f7a 656e 3d54 7275 6529 0d0a  s(frozen=True)..
+00000100: 636c 6173 7320 4d6f 6465 6c43 6c61 7373  class ModelClass
+00000110: 2853 656d 616e 7468 614d 6f64 656c 456e  (SemanthaModelEn
+00000120: 7469 7479 293a 0d0a 2020 2020 2222 2220  tity):..    """ 
+00000130: 6175 7468 6f72 2073 656d 616e 7468 612c  author semantha,
+00000140: 2074 6869 7320 6973 2061 2067 656e 6572   this is a gener
+00000150: 6174 6564 2063 6c61 7373 2064 6f20 6e6f  ated class do no
+00000160: 7420 6368 616e 6765 206d 616e 7561 6c6c  t change manuall
+00000170: 7921 2022 2222 0d0a 2020 2020 6e61 6d65  y! """..    name
+00000180: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d0d  : Optional[str].
+00000190: 0a20 2020 206c 6162 656c 3a20 4f70 7469  .    label: Opti
+000001a0: 6f6e 616c 5b73 7472 5d0d 0a20 2020 2073  onal[str]..    s
+000001b0: 7562 5f6d 6f64 656c 5f63 6c61 7373 6573  ub_model_classes
+000001c0: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+000001d0: 224d 6f64 656c 436c 6173 7322 5d5d 0d0a  "ModelClass"]]..
+000001e0: 0d0a 4d6f 6465 6c43 6c61 7373 5363 6865  ..ModelClassSche
+000001f0: 6d61 203d 2063 6c61 7373 5f73 6368 656d  ma = class_schem
+00000200: 6128 4d6f 6465 6c43 6c61 7373 2c20 6261  a(ModelClass, ba
+00000210: 7365 5f73 6368 656d 613d 5365 6d61 6e74  se_schema=Semant
+00000220: 6861 5363 6865 6d61 290d 0a              haSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.5.0/semantha_sdk/model/table_instance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00000010: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00000020: 730d 0a0d 0a66 726f 6d20 6d61 7273 686d  s....from marshm
-00000030: 616c 6c6f 775f 6461 7461 636c 6173 7320  allow_dataclass 
-00000040: 696d 706f 7274 2063 6c61 7373 5f73 6368  import class_sch
-00000050: 656d 610d 0a0d 0a66 726f 6d20 7365 6d61  ema....from sema
-00000060: 6e74 6861 5f73 646b 2e6d 6f64 656c 2e73  ntha_sdk.model.s
-00000070: 656d 616e 7468 615f 656e 7469 7479 2069  emantha_entity i
-00000080: 6d70 6f72 7420 5365 6d61 6e74 6861 4d6f  mport SemanthaMo
-00000090: 6465 6c45 6e74 6974 792c 2053 656d 616e  delEntity, Seman
-000000a0: 7468 6153 6368 656d 610d 0a0d 0a66 726f  thaSchema....fro
-000000b0: 6d20 7365 6d61 6e74 6861 5f73 646b 2e6d  m semantha_sdk.m
-000000c0: 6f64 656c 2e65 7874 7261 6374 696f 6e5f  odel.extraction_
-000000d0: 6172 6561 2069 6d70 6f72 7420 4578 7472  area import Extr
-000000e0: 6163 7469 6f6e 4172 6561 0d0a 6672 6f6d  actionArea..from
-000000f0: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
-00000100: 7074 696f 6e61 6c0d 0a0d 0a0d 0a40 6461  ptional......@da
-00000110: 7461 636c 6173 7328 6672 6f7a 656e 3d54  taclass(frozen=T
-00000120: 7275 6529 0d0a 636c 6173 7320 5461 626c  rue)..class Tabl
-00000130: 6549 6e73 7461 6e63 6528 5365 6d61 6e74  eInstance(Semant
-00000140: 6861 4d6f 6465 6c45 6e74 6974 7929 3a0d  haModelEntity):.
-00000150: 0a09 2222 2220 6175 7468 6f72 2073 656d  ..""" author sem
-00000160: 616e 7468 612c 2074 6869 7320 6973 2061  antha, this is a
-00000170: 2067 656e 6572 6174 6564 2063 6c61 7373   generated class
-00000180: 2064 6f20 6e6f 7420 6368 616e 6765 206d   do not change m
-00000190: 616e 7561 6c6c 7921 2022 2222 0d0a 0974  anually! """...t
-000001a0: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-000001b0: 725d 0d0a 0965 7874 7261 6374 696f 6e5f  r]...extraction_
-000001c0: 6172 6561 3a20 4f70 7469 6f6e 616c 5b45  area: Optional[E
-000001d0: 7874 7261 6374 696f 6e41 7265 615d 0d0a  xtractionArea]..
-000001e0: 090d 0a09 0d0a 5461 626c 6549 6e73 7461  ......TableInsta
-000001f0: 6e63 6553 6368 656d 6120 3d20 636c 6173  nceSchema = clas
-00000200: 735f 7363 6865 6d61 2854 6162 6c65 496e  s_schema(TableIn
-00000210: 7374 616e 6365 2c20 6261 7365 5f73 6368  stance, base_sch
-00000220: 656d 613d 5365 6d61 6e74 6861 5363 6865  ema=SemanthaSche
-00000230: 6d61 290d 0a                             ma)..
+00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
+00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
+00000020: 6173 730d 0a0d 0a66 726f 6d20 6d61 7273  ass....from mars
+00000030: 686d 616c 6c6f 775f 6461 7461 636c 6173  hmallow_dataclas
+00000040: 7320 696d 706f 7274 2063 6c61 7373 5f73  s import class_s
+00000050: 6368 656d 610d 0a0d 0a66 726f 6d20 7365  chema....from se
+00000060: 6d61 6e74 6861 5f73 646b 2e6d 6f64 656c  mantha_sdk.model
+00000070: 2e73 656d 616e 7468 615f 656e 7469 7479  .semantha_entity
+00000080: 2069 6d70 6f72 7420 5365 6d61 6e74 6861   import Semantha
+00000090: 4d6f 6465 6c45 6e74 6974 792c 2053 656d  ModelEntity, Sem
+000000a0: 616e 7468 6153 6368 656d 610d 0a0d 0a66  anthaSchema....f
+000000b0: 726f 6d20 7365 6d61 6e74 6861 5f73 646b  rom semantha_sdk
+000000c0: 2e6d 6f64 656c 2e65 7874 7261 6374 696f  .model.extractio
+000000d0: 6e5f 6172 6561 2069 6d70 6f72 7420 4578  n_area import Ex
+000000e0: 7472 6163 7469 6f6e 4172 6561 0d0a 0d0a  tractionArea....
+000000f0: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000100: 7274 204f 7074 696f 6e61 6c0d 0a0d 0a40  rt Optional....@
+00000110: 6461 7461 636c 6173 7328 6672 6f7a 656e  dataclass(frozen
+00000120: 3d54 7275 6529 0d0a 636c 6173 7320 5461  =True)..class Ta
+00000130: 626c 6549 6e73 7461 6e63 6528 5365 6d61  bleInstance(Sema
+00000140: 6e74 6861 4d6f 6465 6c45 6e74 6974 7929  nthaModelEntity)
+00000150: 3a0d 0a20 2020 2022 2222 2061 7574 686f  :..    """ autho
+00000160: 7220 7365 6d61 6e74 6861 2c20 7468 6973  r semantha, this
+00000170: 2069 7320 6120 6765 6e65 7261 7465 6420   is a generated 
+00000180: 636c 6173 7320 646f 206e 6f74 2063 6861  class do not cha
+00000190: 6e67 6520 6d61 6e75 616c 6c79 2120 2222  nge manually! ""
+000001a0: 220d 0a20 2020 2074 7970 653a 204f 7074  "..    type: Opt
+000001b0: 696f 6e61 6c5b 7374 725d 0d0a 2020 2020  ional[str]..    
+000001c0: 6578 7472 6163 7469 6f6e 5f61 7265 613a  extraction_area:
+000001d0: 204f 7074 696f 6e61 6c5b 4578 7472 6163   Optional[Extrac
+000001e0: 7469 6f6e 4172 6561 5d0d 0a0d 0a54 6162  tionArea]....Tab
+000001f0: 6c65 496e 7374 616e 6365 5363 6865 6d61  leInstanceSchema
+00000200: 203d 2063 6c61 7373 5f73 6368 656d 6128   = class_schema(
+00000210: 5461 626c 6549 6e73 7461 6e63 652c 2062  TableInstance, b
+00000220: 6173 655f 7363 6865 6d61 3d53 656d 616e  ase_schema=Seman
+00000230: 7468 6153 6368 656d 6129 0d0a            thaSchema)..
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.5.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.5.0/semantha_sdk/response/semantha_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+from io import BytesIO
 from typing import Dict, Type
 
 from marshmallow import EXCLUDE
 from requests import Response
 from requests.structures import CaseInsensitiveDict
 
 from semantha_sdk.model.semantha_entity import SemanthaSchema
@@ -69,14 +70,17 @@
     
     def as_str(self) -> str:
         return self.__content.decode()
     
     def as_none(self) -> None:
         return None
 
+    def as_bytesio(self) -> BytesIO:
+        return BytesIO(self.as_bytes())
+
     def __str__(self) -> str:
         return self.__raw_response.__str__()
 
 
 def _check_and_translate_errors(response: Response) -> Response:
     if response.status_code in [200, 201, 204]:
         return response
```

### Comparing `semantha_sdk-5.4.1/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.5.0/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.4.1/PKG-INFO` & `semantha_sdk-5.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 5.4.1
+Version: 5.5.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -39,14 +39,19 @@
 ### Disclaimer
 
 **IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
 ## Update Notes
 
+### Version 5.5.0
+Removed language parameter on **/api/domains/{domainname}/references**
+Fixed bug on serialization of **/api/domains/{domainname}/modelinstances** response.
+Fixed return of binary responses of bulk services.
+
 ### Version 5.4.0
 Added **new** service: 
 - **/api/domains/{domainname}/summarizations** which generations a summarization for a given list of texts and a given topic.
 
 Added support for **existing** services: 
 - /api/model/domains/{domainname}/boostwords/{id}
 - /api/model/domains/{domainname}/namedentities
@@ -145,15 +150,15 @@
 - [x] **/bulk/domains/{domainname}** -> BulkdomainsDomainEndpoint
 - [x] **/bulk/domains/{domainname}/documentclasses** -> BulkdomainsDocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClassBulk]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
     - [x] **POST** -> None
@@ -192,69 +197,69 @@
 - [x] **/domains/{domainname}/answers** -> AnswersEndpoint
     - [x] **POST** -> Answer
 - [x] **/domains/{domainname}/documentannotations** -> DocumentannotationsEndpoint
     - [x] **POST** -> IOBase
 - [x] **/domains/{domainname}/documentclasses** -> DocumentclassesEndpoint
     - [x] **GET** -> List[DocumentClass]
     - [x] **POST** -> DocumentClass
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/documentclasses/{id}** -> DocumentclassEndpoint
     - [x] **GET** -> DocumentClass
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> DocumentClass
 - [ ] **/domains/{domainname}/documentclasses/{id}/documentclasses** 
 - [ ] **/domains/{domainname}/documentclasses/{id}/referencedocuments** 
 - [x] **/domains/{domainname}/documentcomparisons** -> DocumentcomparisonsEndpoint
     - [x] **POST** -> IOBase
 - [x] **/domains/{domainname}/documents** -> DocumentsEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
     - [x] **POST** -> List[DocumentInformation]
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
 - [x] **/domains/{domainname}/referencedocuments/statistic** -> StatisticEndpoint
     - [x] **GET** -> Statistic
 - [x] **/domains/{domainname}/referencedocuments/{documentid}** -> ReferencedocumentEndpoint
     - [x] **GET** -> Document
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PATCH** -> DocumentInformation
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs** -> ParagraphsEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/paragraphs/{id}** -> ParagraphEndpoint
     - [x] **GET** -> Paragraph
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PATCH** -> Paragraph
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences** -> SentencesEndpoint
 - [x] **/domains/{domainname}/referencedocuments/{documentid}/sentences/{id}** -> SentenceEndpoint
     - [x] **GET** -> Sentence
 - [x] **/domains/{domainname}/references** -> ReferencesEndpoint
     - [x] **POST** -> Document
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
-    - [x] **POST** -> Any
+    - [x] **POST** -> str
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/domains/{domainname}/validation** -> ValidationEndpoint
     - [x] **POST** -> SemanticModel
 - [x] **/info** -> InfoEndpoint
     - [x] **GET** -> Info
 - [x] **/languages** -> LanguagesEndpoint
     - [x] **POST** -> LanguageDetection
 - [x] **/model** -> ModelEndpoint
@@ -265,18 +270,18 @@
     - [x] **GET** -> IOBase
     - [x] **PATCH** -> IOBase
 - [ ] **/model/domains/{domainname}/attributes** 
 - [ ] **/model/domains/{domainname}/backups** 
 - [x] **/model/domains/{domainname}/boostwords** -> ModelBoostwordsEndpoint
     - [x] **GET** -> List[BoostWord]
     - [x] **POST** -> BoostWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/boostwords/{id}** -> ModelBoostwordEndpoint
     - [x] **GET** -> BoostWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> BoostWord
 - [ ] **/model/domains/{domainname}/classes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/attributes/{id}** 
 - [ ] **/model/domains/{domainname}/classes/{classid}/instances** 
 - [ ] **/model/domains/{domainname}/dataproperties** 
@@ -291,41 +296,41 @@
 - [ ] **/model/domains/{domainname}/instances** 
 - [ ] **/model/domains/{domainname}/instances/{id}** 
 - [ ] **/model/domains/{domainname}/metadata** 
 - [ ] **/model/domains/{domainname}/metadata/{id}** 
 - [x] **/model/domains/{domainname}/namedentities** -> ModelNamedentitiesEndpoint
     - [x] **GET** -> List[NamedEntity]
     - [x] **POST** -> NamedEntity
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/namedentities/{id}** -> ModelNamedentityEndpoint
     - [x] **GET** -> NamedEntity
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> NamedEntity
 - [ ] **/model/domains/{domainname}/objectproperties** 
 - [ ] **/model/domains/{domainname}/regexes** 
 - [ ] **/model/domains/{domainname}/regexes/{id}** 
 - [ ] **/model/domains/{domainname}/relations** 
 - [ ] **/model/domains/{domainname}/relations/{id}** 
 - [ ] **/model/domains/{domainname}/rulefunctions** 
 - [ ] **/model/domains/{domainname}/rules** 
 - [ ] **/model/domains/{domainname}/rules/{id}** 
 - [x] **/model/domains/{domainname}/stopwords** -> ModelStopwordsEndpoint
     - [x] **GET** -> List[StopWord]
     - [x] **POST** -> StopWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/stopwords/{id}** -> ModelStopwordEndpoint
     - [x] **GET** -> StopWord
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> StopWord
 - [x] **/model/domains/{domainname}/synonyms** -> ModelSynonymsEndpoint
     - [x] **GET** -> List[Synonym]
     - [x] **POST** -> Synonym
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
 - [x] **/model/domains/{domainname}/synonyms/{id}** -> ModelSynonymEndpoint
     - [x] **GET** -> Synonym
-    - [x] **DELETE** -> 
+    - [x] **DELETE** -> void
     - [x] **PUT** -> Synonym
 - [x] **/model/extractortypes** -> ModelExtractortypesEndpoint
     - [x] **GET** -> List[str]
 - [x] **/model/metadatatypes** -> ModelMetadatatypesEndpoint
     - [x] **GET** -> List[str]
```

