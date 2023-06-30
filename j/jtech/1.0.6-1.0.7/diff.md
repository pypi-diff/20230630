# Comparing `tmp/jtech-1.0.6.tar.gz` & `tmp/jtech-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtech-1.0.6.tar", max compression
+gzip compressed data, was "jtech-1.0.7.tar", max compression
```

## Comparing `jtech-1.0.6.tar` & `jtech-1.0.7.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0        0 2023-06-19 12:53:20.183574 jtech-1.0.6/jtech/__init__.py
--rw-r--r--   0        0        0     3002 2023-06-29 16:57:55.303758 jtech-1.0.6/jtech/__main__.py
--rw-r--r--   0        0        0        0 2023-06-19 12:57:41.640049 jtech-1.0.6/jtech/architecture/__init__.py
--rw-r--r--   0        0        0     6415 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/architecture/clean_architecture_generator.py
--rw-r--r--   0        0        0     5740 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/architecture/cqrs_architecture_generator.py
--rw-r--r--   0        0        0        0 2023-06-19 12:58:05.011675 jtech-1.0.6/jtech/clean_generators/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-20 16:24:08.670365 jtech-1.0.6/jtech/clean_generators/clean_adapter_generator.py
--rw-r--r--   0        0        0      866 2023-06-20 17:33:31.654651 jtech-1.0.6/jtech/clean_generators/clean_api_error_generator.py
--rw-r--r--   0        0        0      879 2023-06-20 17:37:47.222366 jtech-1.0.6/jtech/clean_generators/clean_api_sub_error_generator.py
--rw-r--r--   0        0        0      907 2023-06-20 17:39:21.310839 jtech-1.0.6/jtech/clean_generators/clean_api_validation_error_generator.py
--rw-r--r--   0        0        0     1200 2023-06-20 16:24:08.713367 jtech-1.0.6/jtech/clean_generators/clean_config_generator.py
--rw-r--r--   0        0        0     1277 2023-06-20 16:24:08.730367 jtech-1.0.6/jtech/clean_generators/clean_controller_generator.py
--rw-r--r--   0        0        0     1158 2023-06-20 16:24:08.675366 jtech-1.0.6/jtech/clean_generators/clean_domain_generator.py
--rw-r--r--   0        0        0     1911 2023-06-23 18:48:38.519153 jtech-1.0.6/jtech/clean_generators/clean_entity_generator.py
--rw-r--r--   0        0        0      835 2023-06-20 17:41:06.462602 jtech-1.0.6/jtech/clean_generators/clean_gen_id_generator.py
--rw-r--r--   0        0        0     7961 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_generator.py
--rw-r--r--   0        0        0      916 2023-06-20 17:36:09.141789 jtech-1.0.6/jtech/clean_generators/clean_global_handler_generator.py
--rw-r--r--   0        0        0     1307 2023-06-20 16:24:08.736367 jtech-1.0.6/jtech/clean_generators/clean_input_gateway_generator.py
--rw-r--r--   0        0        0      834 2023-06-20 17:42:13.571365 jtech-1.0.6/jtech/clean_generators/clean_jsons_generator.py
--rw-r--r--   0        0        0      874 2023-06-20 17:30:35.029010 jtech-1.0.6/jtech/clean_generators/clean_kafka_generator.py
--rw-r--r--   0        0        0      905 2023-06-20 17:43:54.808025 jtech-1.0.6/jtech/clean_generators/clean_openapi_generator.py
--rw-r--r--   0        0        0     1314 2023-06-20 16:24:08.692366 jtech-1.0.6/jtech/clean_generators/clean_output_gateway_generator.py
--rw-r--r--   0        0        0      899 2023-06-20 17:46:21.255873 jtech-1.0.6/jtech/clean_generators/clean_ready_event_listener_generator.py
--rw-r--r--   0        0        0      873 2023-06-20 17:47:43.993047 jtech-1.0.6/jtech/clean_generators/clean_redis_generator.py
--rw-r--r--   0        0        0     1394 2023-06-20 16:25:42.838850 jtech-1.0.6/jtech/clean_generators/clean_repository_default_generator.py
--rw-r--r--   0        0        0     1296 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_repository_jpa_generator.py
--rw-r--r--   0        0        0     1263 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_repository_mongo_generator.py
--rw-r--r--   0        0        0     1112 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_request_generator.py
--rw-r--r--   0        0        0     1175 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_response_generator.py
--rw-r--r--   0        0        0     1176 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/clean_generators/clean_usecase_generator.py
--rw-r--r--   0        0        0        0 2023-06-19 12:58:17.065998 jtech-1.0.6/jtech/cqrs_generators/__init__.py
--rw-r--r--   0        0        0     1082 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_aggregator_generator.py
--rw-r--r--   0        0        0      740 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_error_generator.py
--rw-r--r--   0        0        0      750 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_sub_error_generator.py
--rw-r--r--   0        0        0      771 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_api_validation_error_generator.py
--rw-r--r--   0        0        0      991 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_command_generator.py
--rw-r--r--   0        0        0     1038 2023-06-29 16:34:03.313942 jtech-1.0.6/jtech/cqrs_generators/cqrs_controller_generator.py
--rw-r--r--   0        0        0     1460 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_entity_generator.py
--rw-r--r--   0        0        0     1016 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_find_by_id_query_generator.py
--rw-r--r--   0        0        0      793 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_gen_id_generator.py
--rw-r--r--   0        0        0     5741 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_generator.py
--rw-r--r--   0        0        0      762 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_global_handler_generator.py
--rw-r--r--   0        0        0      951 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_http_utils_generator.py
--rw-r--r--   0        0        0      782 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_jsons_generator.py
--rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_kafka_generator.py
--rw-r--r--   0        0        0      740 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_openapi_generator.py
--rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_redis_generator.py
--rw-r--r--   0        0        0     1026 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_default_generator.py
--rw-r--r--   0        0        0     1170 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_jpa_generator.py
--rw-r--r--   0        0        0     1164 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_mongo_generator.py
--rw-r--r--   0        0        0      999 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_request_generator.py
--rw-r--r--   0        0        0     1003 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_response_generator.py
--rw-r--r--   0        0        0     1576 2023-06-29 16:34:03.314942 jtech-1.0.6/jtech/cqrs_generators/cqrs_service_generator.py
--rw-r--r--   0        0        0        0 2023-06-19 15:34:07.706004 jtech-1.0.6/jtech/creators/__init__.py
--rw-r--r--   0        0        0      271 2023-06-14 15:39:52.623663 jtech-1.0.6/jtech/creators/gradle_properties_creator.py
--rw-r--r--   0        0        0      709 2023-06-14 15:43:22.480067 jtech-1.0.6/jtech/creators/readme_creator.py
--rw-r--r--   0        0        0        0 2023-06-23 19:00:13.758726 jtech-1.0.6/jtech/docker_compose/__init__.py
--rw-r--r--   0        0        0     8152 2023-06-26 13:29:59.849326 jtech-1.0.6/jtech/docker_compose/generate_docker_compose.py
--rw-r--r--   0        0        0        0 2023-06-19 16:37:48.899891 jtech-1.0.6/jtech/manipulate/__init__.py
--rw-r--r--   0        0        0     7631 2023-06-23 19:08:33.286070 jtech-1.0.6/jtech/manipulate/application_yml_manipulator.py
--rw-r--r--   0        0        0     4034 2023-06-20 17:15:07.065746 jtech-1.0.6/jtech/manipulate/build_gradle_manipulator.py
--rw-r--r--   0        0        0     2717 2023-06-20 19:28:16.842650 jtech-1.0.6/jtech/manipulate/java_class_manipulator.py
--rw-r--r--   0        0        0      976 2023-06-23 19:08:14.046556 jtech-1.0.6/jtech/manipulate/yaml_manipulator.py
--rw-r--r--   0        0        0        0 2023-06-27 17:26:58.305867 jtech-1.0.6/jtech/mockserver/__init__.py
--rw-r--r--   0        0        0      586 2023-06-27 17:26:58.305867 jtech-1.0.6/jtech/mockserver/mockserver.py
--rw-r--r--   0        0        0        0 2023-06-23 14:19:25.872787 jtech-1.0.6/jtech/project/__init__.py
--rw-r--r--   0        0        0     7241 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/project/create_project.py
--rw-r--r--   0        0        0      540 2023-06-23 16:17:26.834452 jtech-1.0.6/jtech/resources/banner/banner.txt
--rw-r--r--   0        0        0     1695 2023-06-20 18:41:45.182305 jtech-1.0.6/jtech/resources/dependencies/dependencies.json
--rw-r--r--   0        0        0     2170 2023-06-26 14:52:11.058124 jtech-1.0.6/jtech/resources/mock/http.tar.gz
--rw-r--r--   0        0        0     1699 2023-06-26 14:52:21.954146 jtech-1.0.6/jtech/resources/mock/mqtt.tar.gz
--rw-r--r--   0        0        0     1096 2023-06-15 15:47:48.302121 jtech-1.0.6/jtech/resources/tpl/clean_adapter.tpl
--rw-r--r--   0        0        0     2176 2023-06-20 16:45:02.296425 jtech-1.0.6/jtech/resources/tpl/clean_api_error.tpl
--rw-r--r--   0        0        0      585 2023-06-20 16:46:15.081344 jtech-1.0.6/jtech/resources/tpl/clean_api_sub_error.tpl
--rw-r--r--   0        0        0     1206 2023-06-20 16:47:28.810287 jtech-1.0.6/jtech/resources/tpl/clean_api_validation_error.tpl
--rw-r--r--   0        0        0     1042 2023-06-15 15:47:25.965530 jtech-1.0.6/jtech/resources/tpl/clean_config.tpl
--rw-r--r--   0        0        0     1517 2023-06-20 16:00:46.105564 jtech-1.0.6/jtech/resources/tpl/clean_controller.tpl
--rw-r--r--   0        0        0     1528 2023-06-23 12:50:38.457021 jtech-1.0.6/jtech/resources/tpl/clean_domain.tpl
--rw-r--r--   0        0        0      899 2023-06-23 13:22:13.689725 jtech-1.0.6/jtech/resources/tpl/clean_entity.tpl
--rw-r--r--   0        0        0      794 2023-06-20 17:40:23.718478 jtech-1.0.6/jtech/resources/tpl/clean_gen_id.tpl
--rw-r--r--   0        0        0     2375 2023-06-20 16:43:30.448004 jtech-1.0.6/jtech/resources/tpl/clean_global_handler.tpl
--rw-r--r--   0        0        0      697 2023-06-15 15:48:21.222993 jtech-1.0.6/jtech/resources/tpl/clean_input_gateway.tpl
--rw-r--r--   0        0        0     1020 2023-06-23 12:26:52.913732 jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity2.tpl
--rw-r--r--   0        0        0     1026 2023-06-22 17:05:47.475660 jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity3.tpl
--rw-r--r--   0        0        0     4654 2023-06-20 16:34:17.510426 jtech-1.0.6/jtech/resources/tpl/clean_jsons.tpl
--rw-r--r--   0        0        0     1171 2023-06-20 16:42:13.632980 jtech-1.0.6/jtech/resources/tpl/clean_kafka.tpl
--rw-r--r--   0        0        0     1107 2023-06-23 13:20:23.008763 jtech-1.0.6/jtech/resources/tpl/clean_mongo_entity.tpl
--rw-r--r--   0        0        0     2490 2023-06-20 17:43:39.504623 jtech-1.0.6/jtech/resources/tpl/clean_openapi.tpl
--rw-r--r--   0        0        0      701 2023-06-15 15:48:32.462291 jtech-1.0.6/jtech/resources/tpl/clean_output_gateway.tpl
--rw-r--r--   0        0        0     1542 2023-06-22 16:26:15.375485 jtech-1.0.6/jtech/resources/tpl/clean_ready_listener.tpl
--rw-r--r--   0        0        0     3582 2023-06-20 16:38:23.431913 jtech-1.0.6/jtech/resources/tpl/clean_redis.tpl
--rw-r--r--   0        0        0      758 2023-06-15 15:48:41.589532 jtech-1.0.6/jtech/resources/tpl/clean_repository_default.tpl
--rw-r--r--   0        0        0      856 2023-06-23 13:09:29.436274 jtech-1.0.6/jtech/resources/tpl/clean_repository_jpa.tpl
--rw-r--r--   0        0        0      860 2023-06-23 13:10:31.845943 jtech-1.0.6/jtech/resources/tpl/clean_repository_mongo.tpl
--rw-r--r--   0        0        0      974 2023-06-15 15:49:11.150315 jtech-1.0.6/jtech/resources/tpl/clean_request.tpl
--rw-r--r--   0        0        0     1952 2023-06-15 15:49:19.726542 jtech-1.0.6/jtech/resources/tpl/clean_response.tpl
--rw-r--r--   0        0        0     1276 2023-06-15 15:49:29.709807 jtech-1.0.6/jtech/resources/tpl/clean_usecase.tpl
--rw-r--r--   0        0        0      941 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate.tpl
--rw-r--r--   0        0        0     1616 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate_impl.tpl
--rw-r--r--   0        0        0     2169 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_error.tpl
--rw-r--r--   0        0        0      578 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_sub_error.tpl
--rw-r--r--   0        0        0     1199 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_api_validation_error.tpl
--rw-r--r--   0        0        0     1760 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_controller_command.tpl
--rw-r--r--   0        0        0     1536 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_controller_query.tpl
--rw-r--r--   0        0        0     1355 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_create_command.tpl
--rw-r--r--   0        0        0      795 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_default_entity.tpl
--rw-r--r--   0        0        0     1055 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_2.tpl
--rw-r--r--   0        0        0      997 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_3.tpl
--rw-r--r--   0        0        0     1060 2023-06-29 16:34:03.315942 jtech-1.0.6/jtech/resources/tpl/cqrs_entity_mongo.tpl
--rw-r--r--   0        0        0      598 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_find_by_id_query.tpl
--rw-r--r--   0        0        0      780 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_gen_id.tpl
--rw-r--r--   0        0        0     2352 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_global_handler.tpl
--rw-r--r--   0        0        0      884 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_http_utils.tpl
--rw-r--r--   0        0        0     4644 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_jsons.tpl
--rw-r--r--   0        0        0     1158 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_kafka.tpl
--rw-r--r--   0        0        0     2474 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_openapi.tpl
--rw-r--r--   0        0        0     3569 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_redis.tpl
--rw-r--r--   0        0        0      745 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_default.tpl
--rw-r--r--   0        0        0      811 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_jpa.tpl
--rw-r--r--   0        0        0      815 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_repository_mongo.tpl
--rw-r--r--   0        0        0     1019 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_request.tpl
--rw-r--r--   0        0        0     1323 2023-06-29 16:34:03.316942 jtech-1.0.6/jtech/resources/tpl/cqrs_response.tpl
--rw-r--r--   0        0        0      803 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_command.tpl
--rw-r--r--   0        0        0     1260 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_command_impl.tpl
--rw-r--r--   0        0        0      771 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_query.tpl
--rw-r--r--   0        0        0     1306 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/resources/tpl/cqrs_service_query_impl.tpl
--rw-r--r--   0        0        0        0 2023-06-19 13:04:59.491638 jtech-1.0.6/jtech/template_processor/__init__.py
--rw-r--r--   0        0        0      924 2023-06-28 14:38:39.932374 jtech-1.0.6/jtech/template_processor/template_processor.py
--rw-r--r--   0        0        0        0 2023-06-19 16:37:32.717465 jtech-1.0.6/jtech/utils/__init__.py
--rw-r--r--   0        0        0      449 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/convert.py
--rw-r--r--   0        0        0     1630 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/dir_constants.py
--rw-r--r--   0        0        0      287 2023-06-20 19:39:52.159935 jtech-1.0.6/jtech/utils/file_remove.py
--rw-r--r--   0        0        0      504 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/generator.py
--rw-r--r--   0        0        0      688 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/param_configuration.py
--rw-r--r--   0        0        0      521 2023-06-26 15:18:33.671487 jtech-1.0.6/jtech/utils/tar_gz_extractor.py
--rw-r--r--   0        0        0     2180 2023-06-29 16:34:03.317942 jtech-1.0.6/jtech/utils/tpl_constants.py
--rw-r--r--   0        0        0        0 2023-06-19 16:35:55.615903 jtech-1.0.6/jtech/webclient/__init__.py
--rw-r--r--   0        0        0     1119 2023-06-19 17:10:17.936011 jtech-1.0.6/jtech/webclient/spring_boot_client.py
--rw-r--r--   0        0        0        0 2023-06-19 12:59:40.314234 jtech-1.0.6/jtech/wizards/__init__.py
--rw-r--r--   0        0        0      575 2023-06-19 16:15:08.306931 jtech-1.0.6/jtech/wizards/architecture_choice_wizard.py
--rw-r--r--   0        0        0     1248 2023-06-19 16:29:10.214206 jtech-1.0.6/jtech/wizards/checkbox_wizard.py
--rw-r--r--   0        0        0     1825 2023-06-23 16:39:20.028880 jtech-1.0.6/jtech/wizards/metadata_wizard.py
--rw-r--r--   0        0        0      741 2023-06-19 16:32:07.309879 jtech-1.0.6/jtech/wizards/project.py
--rw-r--r--   0        0        0      570 2023-06-20 16:16:32.641378 jtech-1.0.6/jtech/wizards/samples_choice_wizard.py
--rw-r--r--   0        0        0      659 2023-06-29 16:34:03.317942 jtech-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 jtech-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-19 12:53:20.183574 jtech-1.0.7/jtech/__init__.py
+-rw-r--r--   0        0        0     3032 2023-06-30 13:32:04.629463 jtech-1.0.7/jtech/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:57:41.640049 jtech-1.0.7/jtech/architecture/__init__.py
+-rw-r--r--   0        0        0     5911 2023-06-30 13:32:04.629463 jtech-1.0.7/jtech/architecture/clean_architecture_generator.py
+-rw-r--r--   0        0        0     5740 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/architecture/cqrs_architecture_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:05.011675 jtech-1.0.7/jtech/clean_generators/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-20 16:24:08.670365 jtech-1.0.7/jtech/clean_generators/clean_adapter_generator.py
+-rw-r--r--   0        0        0      866 2023-06-20 17:33:31.654651 jtech-1.0.7/jtech/clean_generators/clean_api_error_generator.py
+-rw-r--r--   0        0        0      879 2023-06-20 17:37:47.222366 jtech-1.0.7/jtech/clean_generators/clean_api_sub_error_generator.py
+-rw-r--r--   0        0        0      907 2023-06-20 17:39:21.310839 jtech-1.0.7/jtech/clean_generators/clean_api_validation_error_generator.py
+-rw-r--r--   0        0        0     1200 2023-06-20 16:24:08.713367 jtech-1.0.7/jtech/clean_generators/clean_config_generator.py
+-rw-r--r--   0        0        0     1277 2023-06-20 16:24:08.730367 jtech-1.0.7/jtech/clean_generators/clean_controller_generator.py
+-rw-r--r--   0        0        0     1158 2023-06-20 16:24:08.675366 jtech-1.0.7/jtech/clean_generators/clean_domain_generator.py
+-rw-r--r--   0        0        0     1911 2023-06-23 18:48:38.519153 jtech-1.0.7/jtech/clean_generators/clean_entity_generator.py
+-rw-r--r--   0        0        0      835 2023-06-20 17:41:06.462602 jtech-1.0.7/jtech/clean_generators/clean_gen_id_generator.py
+-rw-r--r--   0        0        0     7955 2023-06-30 13:32:04.629463 jtech-1.0.7/jtech/clean_generators/clean_generator.py
+-rw-r--r--   0        0        0      916 2023-06-20 17:36:09.141789 jtech-1.0.7/jtech/clean_generators/clean_global_handler_generator.py
+-rw-r--r--   0        0        0     1307 2023-06-20 16:24:08.736367 jtech-1.0.7/jtech/clean_generators/clean_input_gateway_generator.py
+-rw-r--r--   0        0        0      834 2023-06-20 17:42:13.571365 jtech-1.0.7/jtech/clean_generators/clean_jsons_generator.py
+-rw-r--r--   0        0        0      874 2023-06-20 17:30:35.029010 jtech-1.0.7/jtech/clean_generators/clean_kafka_generator.py
+-rw-r--r--   0        0        0      905 2023-06-20 17:43:54.808025 jtech-1.0.7/jtech/clean_generators/clean_openapi_generator.py
+-rw-r--r--   0        0        0     1314 2023-06-20 16:24:08.692366 jtech-1.0.7/jtech/clean_generators/clean_output_gateway_generator.py
+-rw-r--r--   0        0        0      899 2023-06-20 17:46:21.255873 jtech-1.0.7/jtech/clean_generators/clean_ready_event_listener_generator.py
+-rw-r--r--   0        0        0      873 2023-06-20 17:47:43.993047 jtech-1.0.7/jtech/clean_generators/clean_redis_generator.py
+-rw-r--r--   0        0        0     1394 2023-06-20 16:25:42.838850 jtech-1.0.7/jtech/clean_generators/clean_repository_default_generator.py
+-rw-r--r--   0        0        0     1296 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/clean_generators/clean_repository_jpa_generator.py
+-rw-r--r--   0        0        0     1263 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/clean_generators/clean_repository_mongo_generator.py
+-rw-r--r--   0        0        0     1112 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/clean_generators/clean_request_generator.py
+-rw-r--r--   0        0        0     1175 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/clean_generators/clean_response_generator.py
+-rw-r--r--   0        0        0     1176 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/clean_generators/clean_usecase_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:17.065998 jtech-1.0.7/jtech/cqrs_generators/__init__.py
+-rw-r--r--   0        0        0     1082 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_aggregator_generator.py
+-rw-r--r--   0        0        0      740 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_api_error_generator.py
+-rw-r--r--   0        0        0      750 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_api_sub_error_generator.py
+-rw-r--r--   0        0        0      771 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_api_validation_error_generator.py
+-rw-r--r--   0        0        0      991 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_command_generator.py
+-rw-r--r--   0        0        0     1038 2023-06-29 16:34:03.313942 jtech-1.0.7/jtech/cqrs_generators/cqrs_controller_generator.py
+-rw-r--r--   0        0        0     1460 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_entity_generator.py
+-rw-r--r--   0        0        0     1016 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_find_by_id_query_generator.py
+-rw-r--r--   0        0        0      793 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_gen_id_generator.py
+-rw-r--r--   0        0        0     5741 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_generator.py
+-rw-r--r--   0        0        0      762 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_global_handler_generator.py
+-rw-r--r--   0        0        0      951 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_http_utils_generator.py
+-rw-r--r--   0        0        0      782 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_jsons_generator.py
+-rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_kafka_generator.py
+-rw-r--r--   0        0        0      740 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_openapi_generator.py
+-rw-r--r--   0        0        0      732 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_redis_generator.py
+-rw-r--r--   0        0        0     1026 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_default_generator.py
+-rw-r--r--   0        0        0     1170 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_jpa_generator.py
+-rw-r--r--   0        0        0     1164 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_mongo_generator.py
+-rw-r--r--   0        0        0      999 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_request_generator.py
+-rw-r--r--   0        0        0     1003 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_response_generator.py
+-rw-r--r--   0        0        0     1576 2023-06-29 16:34:03.314942 jtech-1.0.7/jtech/cqrs_generators/cqrs_service_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 15:34:07.706004 jtech-1.0.7/jtech/creators/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-14 15:39:52.623663 jtech-1.0.7/jtech/creators/gradle_properties_creator.py
+-rw-r--r--   0        0        0      709 2023-06-14 15:43:22.480067 jtech-1.0.7/jtech/creators/readme_creator.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:00:13.758726 jtech-1.0.7/jtech/docker_compose/__init__.py
+-rw-r--r--   0        0        0     8152 2023-06-26 13:29:59.849326 jtech-1.0.7/jtech/docker_compose/generate_docker_compose.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:48.899891 jtech-1.0.7/jtech/manipulate/__init__.py
+-rw-r--r--   0        0        0     7631 2023-06-23 19:08:33.286070 jtech-1.0.7/jtech/manipulate/application_yml_manipulator.py
+-rw-r--r--   0        0        0     4034 2023-06-20 17:15:07.065746 jtech-1.0.7/jtech/manipulate/build_gradle_manipulator.py
+-rw-r--r--   0        0        0     2717 2023-06-20 19:28:16.842650 jtech-1.0.7/jtech/manipulate/java_class_manipulator.py
+-rw-r--r--   0        0        0      976 2023-06-23 19:08:14.046556 jtech-1.0.7/jtech/manipulate/yaml_manipulator.py
+-rw-r--r--   0        0        0        0 2023-06-27 17:26:58.305867 jtech-1.0.7/jtech/mockserver/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-27 17:26:58.305867 jtech-1.0.7/jtech/mockserver/mockserver.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:19:25.872787 jtech-1.0.7/jtech/project/__init__.py
+-rw-r--r--   0        0        0     7241 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/project/create_project.py
+-rw-r--r--   0        0        0      540 2023-06-23 16:17:26.834452 jtech-1.0.7/jtech/resources/banner/banner.txt
+-rw-r--r--   0        0        0     1695 2023-06-20 18:41:45.182305 jtech-1.0.7/jtech/resources/dependencies/dependencies.json
+-rw-r--r--   0        0        0     2170 2023-06-26 14:52:11.058124 jtech-1.0.7/jtech/resources/mock/http.tar.gz
+-rw-r--r--   0        0        0     1699 2023-06-26 14:52:21.954146 jtech-1.0.7/jtech/resources/mock/mqtt.tar.gz
+-rw-r--r--   0        0        0     1096 2023-06-15 15:47:48.302121 jtech-1.0.7/jtech/resources/tpl/clean_adapter.tpl
+-rw-r--r--   0        0        0     2176 2023-06-20 16:45:02.296425 jtech-1.0.7/jtech/resources/tpl/clean_api_error.tpl
+-rw-r--r--   0        0        0      585 2023-06-20 16:46:15.081344 jtech-1.0.7/jtech/resources/tpl/clean_api_sub_error.tpl
+-rw-r--r--   0        0        0     1206 2023-06-20 16:47:28.810287 jtech-1.0.7/jtech/resources/tpl/clean_api_validation_error.tpl
+-rw-r--r--   0        0        0     1042 2023-06-15 15:47:25.965530 jtech-1.0.7/jtech/resources/tpl/clean_config.tpl
+-rw-r--r--   0        0        0     1517 2023-06-20 16:00:46.105564 jtech-1.0.7/jtech/resources/tpl/clean_controller.tpl
+-rw-r--r--   0        0        0     1528 2023-06-23 12:50:38.457021 jtech-1.0.7/jtech/resources/tpl/clean_domain.tpl
+-rw-r--r--   0        0        0      899 2023-06-23 13:22:13.689725 jtech-1.0.7/jtech/resources/tpl/clean_entity.tpl
+-rw-r--r--   0        0        0      794 2023-06-20 17:40:23.718478 jtech-1.0.7/jtech/resources/tpl/clean_gen_id.tpl
+-rw-r--r--   0        0        0     2375 2023-06-20 16:43:30.448004 jtech-1.0.7/jtech/resources/tpl/clean_global_handler.tpl
+-rw-r--r--   0        0        0      697 2023-06-15 15:48:21.222993 jtech-1.0.7/jtech/resources/tpl/clean_input_gateway.tpl
+-rw-r--r--   0        0        0     1020 2023-06-23 12:26:52.913732 jtech-1.0.7/jtech/resources/tpl/clean_jpa_entity2.tpl
+-rw-r--r--   0        0        0     1026 2023-06-22 17:05:47.475660 jtech-1.0.7/jtech/resources/tpl/clean_jpa_entity3.tpl
+-rw-r--r--   0        0        0     4654 2023-06-20 16:34:17.510426 jtech-1.0.7/jtech/resources/tpl/clean_jsons.tpl
+-rw-r--r--   0        0        0     1171 2023-06-20 16:42:13.632980 jtech-1.0.7/jtech/resources/tpl/clean_kafka.tpl
+-rw-r--r--   0        0        0     1107 2023-06-23 13:20:23.008763 jtech-1.0.7/jtech/resources/tpl/clean_mongo_entity.tpl
+-rw-r--r--   0        0        0     2490 2023-06-20 17:43:39.504623 jtech-1.0.7/jtech/resources/tpl/clean_openapi.tpl
+-rw-r--r--   0        0        0      701 2023-06-15 15:48:32.462291 jtech-1.0.7/jtech/resources/tpl/clean_output_gateway.tpl
+-rw-r--r--   0        0        0     1542 2023-06-22 16:26:15.375485 jtech-1.0.7/jtech/resources/tpl/clean_ready_listener.tpl
+-rw-r--r--   0        0        0     3582 2023-06-20 16:38:23.431913 jtech-1.0.7/jtech/resources/tpl/clean_redis.tpl
+-rw-r--r--   0        0        0      758 2023-06-15 15:48:41.589532 jtech-1.0.7/jtech/resources/tpl/clean_repository_default.tpl
+-rw-r--r--   0        0        0      856 2023-06-23 13:09:29.436274 jtech-1.0.7/jtech/resources/tpl/clean_repository_jpa.tpl
+-rw-r--r--   0        0        0      860 2023-06-23 13:10:31.845943 jtech-1.0.7/jtech/resources/tpl/clean_repository_mongo.tpl
+-rw-r--r--   0        0        0      974 2023-06-15 15:49:11.150315 jtech-1.0.7/jtech/resources/tpl/clean_request.tpl
+-rw-r--r--   0        0        0     1952 2023-06-15 15:49:19.726542 jtech-1.0.7/jtech/resources/tpl/clean_response.tpl
+-rw-r--r--   0        0        0     1276 2023-06-15 15:49:29.709807 jtech-1.0.7/jtech/resources/tpl/clean_usecase.tpl
+-rw-r--r--   0        0        0      941 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_aggregate.tpl
+-rw-r--r--   0        0        0     1616 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_aggregate_impl.tpl
+-rw-r--r--   0        0        0     2169 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_api_error.tpl
+-rw-r--r--   0        0        0      578 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_api_sub_error.tpl
+-rw-r--r--   0        0        0     1199 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_api_validation_error.tpl
+-rw-r--r--   0        0        0     1760 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_controller_command.tpl
+-rw-r--r--   0        0        0     1536 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_controller_query.tpl
+-rw-r--r--   0        0        0     1355 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_create_command.tpl
+-rw-r--r--   0        0        0      795 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_default_entity.tpl
+-rw-r--r--   0        0        0     1055 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_entity_jpa_2.tpl
+-rw-r--r--   0        0        0      997 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_entity_jpa_3.tpl
+-rw-r--r--   0        0        0     1060 2023-06-29 16:34:03.315942 jtech-1.0.7/jtech/resources/tpl/cqrs_entity_mongo.tpl
+-rw-r--r--   0        0        0      598 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_find_by_id_query.tpl
+-rw-r--r--   0        0        0      780 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_gen_id.tpl
+-rw-r--r--   0        0        0     2352 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_global_handler.tpl
+-rw-r--r--   0        0        0      884 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_http_utils.tpl
+-rw-r--r--   0        0        0     4644 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_jsons.tpl
+-rw-r--r--   0        0        0     1158 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_kafka.tpl
+-rw-r--r--   0        0        0     2474 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_openapi.tpl
+-rw-r--r--   0        0        0     3569 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_redis.tpl
+-rw-r--r--   0        0        0      745 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_repository_default.tpl
+-rw-r--r--   0        0        0      811 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_repository_jpa.tpl
+-rw-r--r--   0        0        0      815 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_repository_mongo.tpl
+-rw-r--r--   0        0        0     1019 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_request.tpl
+-rw-r--r--   0        0        0     1323 2023-06-29 16:34:03.316942 jtech-1.0.7/jtech/resources/tpl/cqrs_response.tpl
+-rw-r--r--   0        0        0      803 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/resources/tpl/cqrs_service_command.tpl
+-rw-r--r--   0        0        0     1260 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/resources/tpl/cqrs_service_command_impl.tpl
+-rw-r--r--   0        0        0      771 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/resources/tpl/cqrs_service_query.tpl
+-rw-r--r--   0        0        0     1306 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/resources/tpl/cqrs_service_query_impl.tpl
+-rw-r--r--   0        0        0        0 2023-06-19 13:04:59.491638 jtech-1.0.7/jtech/template_processor/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-28 14:38:39.932374 jtech-1.0.7/jtech/template_processor/template_processor.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:32.717465 jtech-1.0.7/jtech/utils/__init__.py
+-rw-r--r--   0        0        0      449 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/utils/convert.py
+-rw-r--r--   0        0        0     1630 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/utils/dir_constants.py
+-rw-r--r--   0        0        0      287 2023-06-20 19:39:52.159935 jtech-1.0.7/jtech/utils/file_remove.py
+-rw-r--r--   0        0        0      504 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/utils/generator.py
+-rw-r--r--   0        0        0      688 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/utils/param_configuration.py
+-rw-r--r--   0        0        0      521 2023-06-26 15:18:33.671487 jtech-1.0.7/jtech/utils/tar_gz_extractor.py
+-rw-r--r--   0        0        0     2180 2023-06-29 16:34:03.317942 jtech-1.0.7/jtech/utils/tpl_constants.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:35:55.615903 jtech-1.0.7/jtech/webclient/__init__.py
+-rw-r--r--   0        0        0     1119 2023-06-19 17:10:17.936011 jtech-1.0.7/jtech/webclient/spring_boot_client.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:59:40.314234 jtech-1.0.7/jtech/wizards/__init__.py
+-rw-r--r--   0        0        0      575 2023-06-19 16:15:08.306931 jtech-1.0.7/jtech/wizards/architecture_choice_wizard.py
+-rw-r--r--   0        0        0     1248 2023-06-19 16:29:10.214206 jtech-1.0.7/jtech/wizards/checkbox_wizard.py
+-rw-r--r--   0        0        0     1825 2023-06-23 16:39:20.028880 jtech-1.0.7/jtech/wizards/metadata_wizard.py
+-rw-r--r--   0        0        0      741 2023-06-19 16:32:07.309879 jtech-1.0.7/jtech/wizards/project.py
+-rw-r--r--   0        0        0      570 2023-06-20 16:16:32.641378 jtech-1.0.7/jtech/wizards/samples_choice_wizard.py
+-rw-r--r--   0        0        0      659 2023-06-30 13:32:04.629463 jtech-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 jtech-1.0.7/PKG-INFO
```

### Comparing `jtech-1.0.6/jtech/__main__.py` & `jtech-1.0.7/jtech/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     parser.add_argument("--create", action='store_true', help='Create a Spring Boot Project')
 
     parser.add_argument("project_name", nargs='?', help='Name of the project to be created. Ex: jtech --create sansys-sample')
 
     vargs = parser.parse_args()
 
     if vargs.create:
+        check_update(version)
         project = CreateProject()
         if vargs.project_name:
             project.create(vargs.project_name)
         else:
             project.create()
 
     elif vargs.version:
```

### Comparing `jtech-1.0.6/jtech/architecture/clean_architecture_generator.py` & `jtech-1.0.7/jtech/architecture/cqrs_architecture_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,141 @@
 import os
-import yaml
-from jtech.clean_generators.clean_generator import CleanArchitectureGenerator
+
+from jtech.cqrs_generators.cqrs_generator import CqrsArchitectureGenerator
 from jtech.docker_compose.generate_docker_compose import GenerateDockerCompose
 from jtech.manipulate.application_yml_manipulator import ApplicationYmlManipulator
 from jtech.manipulate.java_class_manipulator import JavaFileManipulator
 from jtech.mockserver.mockserver import GenerateMockServer
 from jtech.utils.file_remove import RemoveFile
-
 import jtech.utils.dir_constants as const
 
 
-class CleanArchitectureStructureCreator:
+class CqrsArchitectureStructureCreator:
     """
-    Generate clean architecture structure and sample files.
+    Generate cqrs architecture structure and sample files.
 
     :param param: DTO with all parameters.
     """
 
     def __init__(self, param):
         self.param = param
 
     def create_structure(self):
         """Create folder structure."""
         composer_dir, mockserver_dir, project_dir, resources_dir = self.generate_base_folder()
-        self.generate_subfolders(project_dir)
-        self.generate_docker_and_mockserver(composer_dir, mockserver_dir)
-        project = self.generate_sample_files(project_dir)
+        self.create_subfolders(project_dir)
+        self.generate_docker_mockserver(composer_dir, mockserver_dir)
+        real_name = self.create_samples(project_dir)
         self.remove_application_properties(resources_dir)
-        self.create_yaml(resources_dir, project, self.param.package)
-        self.generate_docker_compose(composer_dir)
-        self.generate_mockserver(mockserver_dir)
+        self.create_yaml(os.path.join(resources_dir, "application.yml"), real_name, self.param.package)
+        self.create_docker_compose(composer_dir)
+        self.create_mockserver(mockserver_dir)
 
-    def generate_mockserver(self, mockserver_dir):
-        """Generate mockserver folder and add mockeserver"""
-        mockserver = GenerateMockServer(path=mockserver_dir, param=self.param)
-        mockserver.generate()
+    def generate_docker_mockserver(self, composer_dir, mockserver_dir):
+        os.makedirs(composer_dir, exist_ok=True)
+        os.makedirs(mockserver_dir, exist_ok=True)
 
-    def generate_docker_compose(self, composer_dir):
-        docker_compose = GenerateDockerCompose(path=os.path.join(composer_dir, 'docker-compose.yml'), param=self.param)
-        docker_compose.generate()
+    def generate_base_folder(self):
+        main_dir = os.path.join(self.param.base_dir, "src/main/java")
+        resources_dir = os.path.join(self.param.base_dir, "src/main/resources")
+        package_dir = self.param.package.replace(".", "/")
+        project_dir = os.path.join(main_dir, package_dir)
+        composer_dir = os.path.join(self.param.base_dir, "composer")
+        mockserver_dir = os.path.join(self.param.base_dir, "mockserver")
+        return composer_dir, mockserver_dir, project_dir, resources_dir
+
+    def create_samples(self, folder):
+        names = self.param.project.split("-")
+        project = names[-1]
+        capitalize = project[0].upper() + project[1:]
+        if self.param.samples:
+            self.generate_samples(project, capitalize, folder)
+        return project
 
     def remove_application_properties(self, resources_dir):
         application_properties = RemoveFile(os.path.join(resources_dir, "application.properties"))
         application_properties.remove()
 
-    def generate_sample_files(self, project_dir):
-        names = self.param.project.split("-")
-        real_name = names[-1]
-        cap_name = real_name[0].upper() + real_name[1:]
-        if self.param.samples:
-            self.generate_samples(project_name=real_name, cap_name=cap_name, project_dir=project_dir)
-        return real_name
+    def create_docker_compose(self, composer_dir):
+        docker_compose = GenerateDockerCompose(path=os.path.join(composer_dir, 'docker-compose.yml'), param=self.param)
+        docker_compose.generate()
 
-    def generate_docker_and_mockserver(self, composer_dir, mockserver_dir):
-        os.makedirs(composer_dir, exist_ok=True)
-        os.makedirs(mockserver_dir, exist_ok=True)
+    def create_mockserver(self, mockserver_dir):
+        mockserver = GenerateMockServer(path=mockserver_dir, param=self.param)
+        mockserver.generate()
 
-    def generate_subfolders(self, project_dir):
-        """Create subfolders for project"""
-        os.makedirs(project_dir, exist_ok=True)
+    def create_subfolders(self, project_dir):
+        """Create subfolders in the project directory."""
         subfolders = [
-            const.CLEAN_DOMAINS,
-            const.CLEAN_USECASE,
-            const.CLEAN_PORT_INPUT,
-            const.CLEAN_PORT_OUTPUT,
-            const.CLEAN_ADAPTERS_INPUT_CONTROLLERS,
-            const.CLEAN_ADAPTERS_INPUT_HANDLERS,
-            const.CLEAN_ADAPTERS_INPUT_PROTOCOLS,
-            const.CLEAN_ADAPTERS_OUTPUT_ENTITIES,
-            const.CLEAN_CONFIG_INFRA_SWAGGER,
-            const.CLEAN_CONFIG_INFRA_UTILS,
-            const.CLEAN_CONFIG_INFRA_EXCEPTIONS,
-            const.CLEAN_CONFIG_INFRA_HANDLERS,
-            const.CLEAN_CONFIG_INFRA_LISTENERS,
-            const.CLEAN_CONFIG_USECASES,
+            const.CQRS_AGGREGATE_IMPL,
+            const.CQRS_CONTROLLERS_COMMANDS,
+            const.CQRS_CONTROLLERS_QUERIES,
+            const.CQRS_ENTITIES,
+            const.CQRS_INFRA,
+            const.CQRS_INFRA_EXCEPTIONS,
+            const.CQRS_PROTOCOLS,
+            const.CQRS_REPOSITORIES,
+            const.CQRS_COMMAND,
+            const.CQRS_SERVICES_COMMANDS_IMPL,
+            const.CQRS_QUERY,
+            const.CQRS_SERVICES_QUERIES_IMPL,
+            const.CQRS_UTILS,
+            const.CQRS_VALIDATOR
         ]
 
         for subfolder in subfolders:
-            os.makedirs(os.path.join(project_dir), subfolder)
-
-        if self.param.kafka:
-            os.makedirs(os.path.join(project_dir, const.CLEAN_CONFIG_INFRA_KAFKA), exist_ok=True)
-        if self.param.redis:
-            os.makedirs(os.path.join(project_dir, const.CLEAN_CONFIG_INFRA_REDIS), exist_ok=True)
-
-    def generate_base_folder(self):
-        main_dir = os.path.join(self.param.base_dir, "src/main/java")
-        resources_dir = os.path.join(self.param.base_dir, "src/main/resources")
-        package_dir = self.param.package.replace(".", "/")
-        project_dir = os.path.join(main_dir, package_dir)
-        composer_dir = os.path.join(self.param.base_dir, "composer")
-        mockserver_dir = os.path.join(self.param.base_dir, "mockserver")
-        return composer_dir, mockserver_dir, project_dir, resources_dir
+            os.makedirs(os.path.join(project_dir, subfolder), exist_ok=True)
 
-    def create_yaml(self, resources_dir, project, package):
-        file = os.path.join(resources_dir, "application.yml")
+    def create_yaml(self, file, project, package):
         application = ApplicationYmlManipulator(file)
         application.generate_header(project, package)
 
         if self.param.kafka:
             application.generate_kafka_configuration()
 
         if self.param.redis:
             application.generate_redis_configuration()
 
-        if self.param.is_jpa:
+        if self.param.jpa:
             application.generate_jpa_configuration()
 
         if self.param.mongo:
             application.generate_mongodb_configuration(project)
 
         if self.param.zipkin:
             application.generate_zipkin_configuration()
 
         if self.param.config_server:
             application.generate_config_server_configuration()
 
         if self.param.eureka_client:
             application.generate_eureka_client_configuration()
 
-    def generate_samples(self, project_name, cap_name, project_dir):
-        """Generate Clean Architecture sample files."""
-        generator = CleanArchitectureGenerator(project_name, cap_name, project_dir, self.param)
+    def generate_samples(self, project, capitalize, folder):
+        generator = CqrsArchitectureGenerator(project, capitalize, folder, self.param)
         generator.all()
 
-        manipulator = JavaFileManipulator(os.path.join(project_dir, "Start" + cap_name + ".java"))
+        file = os.path.join(folder, "Start" + capitalize + ".java")
+        manipulator = JavaFileManipulator(file)
 
         if self.param.redis & self.param.kafka:
             imports = [
-                self.param.package + ".config.infra.kafka.KafkaConfiguration",
-                self.param.package + ".config.infra.redis.RedisConfiguration",
+                self.param.package + ".infra.KafkaConfiguration",
+                self.param.package + ".infra.RedisConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class(["RedisConfiguration.class", "KafkaConfiguration.class"])
             manipulator.add_imports(imports)
         elif self.param.redis:
             imports = [
-                self.param.package + ".config.infra.redis.RedisConfiguration",
+                self.param.package + ".infra.RedisConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class("RedisConfiguration.class")
             manipulator.add_imports(imports)
         elif self.param.kafka:
             imports = [
-                self.param.package + ".config.infra.kafka.KafkaConfiguration",
+                self.param.package + ".infra.KafkaConfiguration",
                 "org.springframework.context.annotation.Import"
             ]
             manipulator.add_import_to_class("KafkaConfiguration.class")
             manipulator.add_imports(imports)
```

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_adapter_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_adapter_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_api_error_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_api_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_api_sub_error_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_api_sub_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_api_validation_error_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_api_validation_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_config_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_config_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_controller_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_controller_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_domain_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_domain_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_entity_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_entity_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_gen_id_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_gen_id_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,30 +58,30 @@
         """Generate Domain"""
         domain = CleanDomainGenerator(self.param.package, self.project, self.capitalize, self.path)
         domain.generate()
 
     def gen_entity(self):
         """Generate JPA or MongoDB Entity"""
         entity = CleanEntityGenerator(self.param.package, self.project, self.capitalize, self.path,
-                                      self.param.spring_version, self.param.is_jpa, self.param.mongo)
+                                      self.param.spring_version, self.param.jpa, self.param.mongo)
         entity.generate()
 
     def gen_input_gateway(self):
         """Generate Create Input Gateway Interface"""
         gateway = CleanInputGatewayGenerator(self.param.package, self.project, self.capitalize, self.path)
         gateway.generate()
 
     def gen_output_gateway(self):
         """Generate Create Output Gateway Interface"""
         gateway = CleanOutputGatewayGenerator(self.param.package, self.project, self.capitalize, self.path)
         gateway.generate()
 
     def gen_repository(self):
         """Generate JPA or MongoDB repository"""
-        if self.param.is_jpa:
+        if self.param.jpa:
             repository = CleanRepositoryJpaGenerator(self.param.package, self.project, self.capitalize, self.path)
             repository.generate()
         elif self.param.mongo:
             repository = CleanRepositoryMongoGenerator(self.param.package, self.project, self.capitalize,
                                                        self.path)
             repository.generate()
         else:
```

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_global_handler_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_global_handler_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_input_gateway_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_input_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_jsons_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_jsons_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_kafka_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_kafka_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_openapi_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_openapi_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_output_gateway_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_output_gateway_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_ready_event_listener_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_ready_event_listener_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_redis_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_redis_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_repository_default_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_repository_default_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_repository_jpa_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_repository_jpa_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_repository_mongo_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_repository_mongo_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_request_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_request_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_response_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_response_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/clean_generators/clean_usecase_generator.py` & `jtech-1.0.7/jtech/clean_generators/clean_usecase_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_aggregator_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_aggregator_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_api_error_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_api_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_api_sub_error_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_api_sub_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_api_validation_error_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_api_validation_error_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_command_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_command_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_controller_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_controller_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_entity_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_entity_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_find_by_id_query_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_find_by_id_query_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_gen_id_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_gen_id_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_global_handler_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_global_handler_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_http_utils_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_http_utils_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_jsons_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_jsons_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_kafka_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_kafka_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_openapi_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_openapi_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_redis_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_redis_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_default_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_default_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_jpa_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_jpa_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_repository_mongo_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_repository_mongo_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_request_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_request_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_response_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_response_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/cqrs_generators/cqrs_service_generator.py` & `jtech-1.0.7/jtech/cqrs_generators/cqrs_service_generator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/creators/readme_creator.py` & `jtech-1.0.7/jtech/creators/readme_creator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/docker_compose/generate_docker_compose.py` & `jtech-1.0.7/jtech/docker_compose/generate_docker_compose.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/manipulate/application_yml_manipulator.py` & `jtech-1.0.7/jtech/manipulate/application_yml_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/manipulate/build_gradle_manipulator.py` & `jtech-1.0.7/jtech/manipulate/build_gradle_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/manipulate/java_class_manipulator.py` & `jtech-1.0.7/jtech/manipulate/java_class_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/manipulate/yaml_manipulator.py` & `jtech-1.0.7/jtech/manipulate/yaml_manipulator.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/mockserver/mockserver.py` & `jtech-1.0.7/jtech/mockserver/mockserver.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/project/create_project.py` & `jtech-1.0.7/jtech/project/create_project.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/banner/banner.txt` & `jtech-1.0.7/jtech/resources/banner/banner.txt`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/dependencies/dependencies.json` & `jtech-1.0.7/jtech/resources/dependencies/dependencies.json`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/mock/http.tar.gz` & `jtech-1.0.7/jtech/resources/mock/http.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/mock/mqtt.tar.gz` & `jtech-1.0.7/jtech/resources/mock/mqtt.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_adapter.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_adapter.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_api_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_api_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_api_sub_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_api_sub_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_api_validation_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_api_validation_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_config.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_config.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_controller.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_controller.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_domain.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_domain.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_entity.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_gen_id.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_gen_id.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_global_handler.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_global_handler.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_input_gateway.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_input_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity2.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_jpa_entity2.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_jpa_entity3.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_jpa_entity3.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_jsons.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_jsons.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_kafka.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_kafka.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_mongo_entity.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_mongo_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_openapi.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_openapi.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_output_gateway.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_output_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_ready_listener.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_ready_listener.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_redis.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_redis.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_repository_default.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_repository_default.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_repository_jpa.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_repository_jpa.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_repository_mongo.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_repository_mongo.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_request.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_request.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_response.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_response.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/clean_usecase.tpl` & `jtech-1.0.7/jtech/resources/tpl/clean_usecase.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_aggregate.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_aggregate_impl.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_aggregate_impl.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_api_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_api_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_api_sub_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_api_sub_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_api_validation_error.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_api_validation_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_controller_command.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_controller_command.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_controller_query.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_controller_query.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_create_command.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_create_command.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_default_entity.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_default_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_2.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_entity_jpa_2.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_entity_jpa_3.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_entity_jpa_3.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_entity_mongo.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_entity_mongo.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_find_by_id_query.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_find_by_id_query.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_gen_id.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_gen_id.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_global_handler.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_global_handler.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_http_utils.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_http_utils.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_jsons.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_jsons.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_kafka.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_kafka.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_openapi.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_openapi.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_redis.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_redis.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_repository_default.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_repository_default.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_repository_jpa.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_repository_jpa.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_repository_mongo.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_repository_mongo.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_request.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_request.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_response.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_response.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_service_command.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_service_command.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_service_command_impl.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_service_command_impl.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_service_query.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_service_query.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/resources/tpl/cqrs_service_query_impl.tpl` & `jtech-1.0.7/jtech/resources/tpl/cqrs_service_query_impl.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/template_processor/template_processor.py` & `jtech-1.0.7/jtech/template_processor/template_processor.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/utils/dir_constants.py` & `jtech-1.0.7/jtech/utils/dir_constants.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/utils/param_configuration.py` & `jtech-1.0.7/jtech/utils/param_configuration.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/utils/tar_gz_extractor.py` & `jtech-1.0.7/jtech/utils/tar_gz_extractor.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/utils/tpl_constants.py` & `jtech-1.0.7/jtech/utils/tpl_constants.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/webclient/spring_boot_client.py` & `jtech-1.0.7/jtech/webclient/spring_boot_client.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/wizards/architecture_choice_wizard.py` & `jtech-1.0.7/jtech/wizards/architecture_choice_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/wizards/checkbox_wizard.py` & `jtech-1.0.7/jtech/wizards/checkbox_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/wizards/metadata_wizard.py` & `jtech-1.0.7/jtech/wizards/metadata_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/wizards/project.py` & `jtech-1.0.7/jtech/wizards/project.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/jtech/wizards/samples_choice_wizard.py` & `jtech-1.0.7/jtech/wizards/samples_choice_wizard.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.6/pyproject.toml` & `jtech-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "jtech"
-version = "1.0.6"
+version = "1.0.7"
 description = "Jtech Project CLI"
 authors = ["Angelo Vicente Filho <angelo.vicente@veolia.com>"]
 
 [tool.poetry.scripts]
 jtech = "jtech.__main__:main"
 
 [tool.poetry.dependencies]
```

### Comparing `jtech-1.0.6/PKG-INFO` & `jtech-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jtech
-Version: 1.0.6
+Version: 1.0.7
 Summary: Jtech Project CLI
 Author: Angelo Vicente Filho
 Author-email: angelo.vicente@veolia.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

