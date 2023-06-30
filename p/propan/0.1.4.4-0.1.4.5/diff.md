# Comparing `tmp/propan-0.1.4.4.tar.gz` & `tmp/propan-0.1.4.5.tar.gz`

## Comparing `propan-0.1.4.4.tar` & `propan-0.1.4.5.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.4/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 propan-0.1.4.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.4/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/__about__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/_compat.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/__init__.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/nats.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.4/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.4/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.4/scripts/publish.sh
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 propan-0.1.4.4/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.4/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.4/LICENSE
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 propan-0.1.4.4/README.md
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.4.4/pyproject.toml
--rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 propan-0.1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.5/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__about__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/_compat.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/py.typed
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/nats.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/publish.sh
+-rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.5/LICENSE
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 propan-0.1.4.5/README.md
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.4.5/pyproject.toml
+-rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 propan-0.1.4.5/PKG-INFO
```

### Comparing `propan-0.1.4.4/CONTRIBUTING.md` & `propan-0.1.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/SECURITY.md` & `propan-0.1.4.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.4.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.4.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/workflows/documentation.yml` & `propan-0.1.4.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/workflows/publish_coverage.yml` & `propan-0.1.4.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/workflows/publish_pypi.yml` & `propan-0.1.4.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/.github/workflows/tests.yml` & `propan-0.1.4.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/3_lifespan_events.py` & `propan-0.1.4.5/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/4_cli_attributes_promotion.py` & `propan-0.1.4.5/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/5_publishing.py` & `propan-0.1.4.5/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/6_arguments_casting.py` & `propan-0.1.4.5/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/7_handler_errors_processing.py` & `propan-0.1.4.5/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/1_dependency_injection.py` & `propan-0.1.4.5/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.4.5/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.4.5/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.4.5/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.4.5/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/dependencies/7_annotated.py` & `propan-0.1.4.5/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/quart.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.4.5/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/rabbit/direct.py` & `propan-0.1.4.5/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/rabbit/fanout.py` & `propan-0.1.4.5/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/rabbit/header.py` & `propan-0.1.4.5/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/rabbit/topic.py` & `propan-0.1.4.5/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/redis/direct.py` & `propan-0.1.4.5/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/redis/pattern.py` & `propan-0.1.4.5/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/examples/serialization/protobuf.py` & `propan-0.1.4.5/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/__about__.py` & `propan-0.1.4.5/propan/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.4.4"
+__version__ = "0.1.4.5"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.4.4/propan/__init__.py` & `propan-0.1.4.5/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/_compat.py` & `propan-0.1.4.5/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/annotations.py` & `propan-0.1.4.5/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/types.py` & `propan-0.1.4.5/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/__init__.py` & `propan-0.1.4.5/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/channels.py` & `propan-0.1.4.5/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/info.py` & `propan-0.1.4.5/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/main.py` & `propan-0.1.4.5/propan/asyncapi/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/message.py` & `propan-0.1.4.5/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/security.py` & `propan-0.1.4.5/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/subscription.py` & `propan-0.1.4.5/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/bindings/amqp.py` & `propan-0.1.4.5/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/bindings/kafka.py` & `propan-0.1.4.5/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/bindings/main.py` & `propan-0.1.4.5/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/asyncapi/bindings/redis.py` & `propan-0.1.4.5/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/push_back_watcher.py` & `propan-0.1.4.5/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/_model/broker_usecase.py` & `propan-0.1.4.5/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/_model/routing.py` & `propan-0.1.4.5/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/_model/schemas.py` & `propan-0.1.4.5/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/_model/utils.py` & `propan-0.1.4.5/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.4.5/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.4.5/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/kafka/routing.pyi` & `propan-0.1.4.5/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/kafka/schemas.py` & `propan-0.1.4.5/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/nats/nats_broker.py` & `propan-0.1.4.5/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.4.5/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.4.5/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/nats/routing.pyi` & `propan-0.1.4.5/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/nats/schemas.py` & `propan-0.1.4.5/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/rabbit/routing.pyi` & `propan-0.1.4.5/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/rabbit/schemas.py` & `propan-0.1.4.5/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/redis/redis_broker.py` & `propan-0.1.4.5/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.4.5/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/redis/routing.pyi` & `propan-0.1.4.5/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/redis/schemas.py` & `propan-0.1.4.5/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/sqs/routing.pyi` & `propan-0.1.4.5/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/sqs/schema.py` & `propan-0.1.4.5/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.4.5/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.4.5/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/app.py` & `propan-0.1.4.5/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/main.py` & `propan-0.1.4.5/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/docs/app.py` & `propan-0.1.4.5/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/docs/gen.py` & `propan-0.1.4.5/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/docs/serving.py` & `propan-0.1.4.5/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/core.py` & `propan-0.1.4.5/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/app.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/core.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/nats.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/redis.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.4.5/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/supervisors/basereload.py` & `propan-0.1.4.5/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/supervisors/multiprocess.py` & `propan-0.1.4.5/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/supervisors/utils.py` & `propan-0.1.4.5/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/supervisors/watchfiles.py` & `propan-0.1.4.5/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/utils/imports.py` & `propan-0.1.4.5/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/utils/logs.py` & `propan-0.1.4.5/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/cli/utils/parser.py` & `propan-0.1.4.5/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/fastapi/__init__.py` & `propan-0.1.4.5/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/fastapi/core/route.py` & `propan-0.1.4.5/propan/fastapi/core/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,30 @@
     solve_dependencies,
 )
 from fastapi.routing import run_endpoint_function
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
 from propan._compat import raise_fastapi_validation_error
-from propan.brokers._model import BrokerAsyncUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerAsyncUsecase,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers._model.schemas import PropanMessage as NativeMessage
 from propan.brokers._model.schemas import Queue
 from propan.types import AnyDict
 
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
         path: Union[Queue, str],
         *extra: Union[Queue, str],
-        endpoint: Callable[..., Any],
+        endpoint: HandlerCallable[T_HandlerReturn],
         broker: BrokerAsyncUsecase[Any, Any],
         dependencies: Sequence[params.Depends] = (),
         dependency_overrides_provider: Optional[Any] = None,
         **handle_kwargs: AnyDict,
     ) -> None:
         self.path = path
         self.broker = broker
```

### Comparing `propan-0.1.4.4/propan/fastapi/core/router.py` & `propan-0.1.4.5/propan/fastapi/core/router.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,40 +15,44 @@
     Type,
     Union,
 )
 
 from fastapi import APIRouter, FastAPI, Request, params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
-from fastapi.types import DecoratedCallable
 from fastapi.utils import generate_unique_id
 from starlette import routing
 from starlette.responses import HTMLResponse, JSONResponse, Response
 from starlette.routing import _DefaultLifespan
 from starlette.types import AppType, ASGIApp, Lifespan
 from typing_extensions import AsyncIterator, TypeVar
 
-from propan.brokers._model import BrokerAsyncUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerAsyncUsecase,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers._model.schemas import Queue
 from propan.cli.docs.gen import (
     gen_app_schema_json,
     gen_app_schema_yaml,
     get_app_schema,
     json_schema_to_yaml,
     schema_to_json,
 )
 from propan.cli.docs.serving import get_asyncapi_html
 from propan.fastapi.core.route import PropanRoute
-from propan.types import AnyDict, HandlerCallable
+from propan.types import AnyDict
 from propan.utils.functions import to_async
 
 Broker = TypeVar("Broker", bound=BrokerAsyncUsecase[Any, Any])
+MsgType = TypeVar("MsgType")
 
 
-class PropanRouter(APIRouter, Generic[Broker]):
+class PropanRouter(APIRouter, Generic[Broker, MsgType]):
     broker_class: Type[Broker]
     broker: Broker
     docs_router: Optional[APIRouter]
     _after_startup_hooks: List[
         Callable[[AppType], Awaitable[Optional[Mapping[str, Any]]]]
     ]
 
@@ -124,18 +128,18 @@
 
         self._after_startup_hooks = []
 
     def add_api_mq_route(
         self,
         path: Union[Queue, str],
         *extra: Union[Queue, str],
-        endpoint: DecoratedCallable,
+        endpoint: HandlerCallable[T_HandlerReturn],
         dependencies: Sequence[params.Depends],
         **broker_kwargs: AnyDict,
-    ) -> HandlerCallable:
+    ) -> Callable[[Any, bool], Awaitable[T_HandlerReturn]]:
         route = PropanRoute(
             path,
             *extra,
             endpoint=endpoint,
             dependencies=dependencies,
             dependency_overrides_provider=self.dependency_overrides_provider,
             broker=self.broker,
@@ -146,20 +150,25 @@
 
     def event(
         self,
         path: Union[str, Queue],
         *extra: Union[Queue, str],
         dependencies: Optional[Sequence[params.Depends]] = None,
         **broker_kwargs: Dict[str, Any],
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[MsgType, bool], Awaitable[T_HandlerReturn]],
+    ]:
         current_dependencies = self.dependencies.copy()
         if dependencies:
             current_dependencies.extend(dependencies)
 
-        def decorator(func: DecoratedCallable) -> HandlerCallable:
+        def decorator(
+            func: HandlerCallable[T_HandlerReturn],
+        ) -> Callable[[MsgType, bool], Awaitable[T_HandlerReturn]]:
             return self.add_api_mq_route(
                 path,
                 *extra,
                 endpoint=func,
                 dependencies=current_dependencies,
                 **broker_kwargs,
             )
```

### Comparing `propan-0.1.4.4/propan/fastapi/kafka/router.pyi` & `propan-0.1.4.5/propan/fastapi/kafka/router.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from asyncio import AbstractEventLoop
 from enum import Enum
 from ssl import SSLContext
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Sequence, Type, Union
 
 from aiokafka.abc import AbstractTokenProvider
 from aiokafka.producer.producer import _missing
 from aiokafka.structs import ConsumerRecord
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
@@ -17,18 +17,22 @@
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 from typing_extensions import Literal, TypeVar
 
 from propan import KafkaBroker
 from propan.__about__ import __version__
-from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.broker_usecase import (
+    AsyncDecoder,
+    AsyncParser,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 Partition = TypeVar("Partition")
 
 class KafkaRouter(PropanRouter[KafkaBroker]):
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
@@ -95,23 +99,23 @@
         loop: Optional[AbstractEventLoop] = None,
         # Broker kwargs
         schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        decode_message: CustomDecoder[ConsumerRecord] = None,
-        parse_message: CustomParser[ConsumerRecord] = None,
+        decode_message: AsyncDecoder[ConsumerRecord] = None,
+        parse_message: AsyncParser[ConsumerRecord] = None,
         protocol: str = "kafka",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         *topics: str,
-        endpoint: AnyCallable,
+        endpoint: HandlerCallable[T_HandlerReturn],
         group_id: Optional[str] = None,
         key_deserializer: Optional[Callable[[bytes], Any]] = None,
         value_deserializer: Optional[Callable[[bytes], Any]] = None,
         fetch_max_wait_ms: int = 500,
         fetch_max_bytes: int = 52428800,
         fetch_min_bytes: int = 1,
         max_partition_fetch_bytes: int = 1 * 1024 * 1024,
@@ -135,19 +139,19 @@
         exclude_internal_topics: bool = True,
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
         # broker kwargs
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[ConsumerRecord] = None,
-        parse_message: CustomParser[ConsumerRecord] = None,
+        decode_message: AsyncDecoder[ConsumerRecord] = None,
+        parse_message: AsyncParser[ConsumerRecord] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> HandlerCallable:
+    ) -> Callable[[ConsumerRecord, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         *topics: str,
         group_id: Optional[str] = None,
         key_deserializer: Optional[Callable[[bytes], Any]] = None,
         value_deserializer: Optional[Callable[[bytes], Any]] = None,
@@ -176,12 +180,14 @@
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
         # broker kwargs
         dependencies: Optional[Sequence[params.Depends]] = None,
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[ConsumerRecord] = None,
-        parse_message: CustomParser[ConsumerRecord] = None,
+        decode_message: AsyncDecoder[ConsumerRecord] = None,
+        parse_message: AsyncParser[ConsumerRecord] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
-        pass
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[ConsumerRecord, bool], Awaitable[T_HandlerReturn]],
+    ]: ...
```

### Comparing `propan-0.1.4.4/propan/fastapi/nats/router.pyi` & `propan-0.1.4.5/propan/fastapi/nats/router.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import ssl
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Sequence, Type, Union
 
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
@@ -25,18 +25,22 @@
 )
 from nats.aio.msg import Msg
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import NatsBroker
-from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.broker_usecase import (
+    AsyncDecoder,
+    AsyncParser,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 class NatsRouter(PropanRouter[NatsBroker]):
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
@@ -89,37 +93,40 @@
         ),
         # Broker kwargs
         schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        decode_message: CustomDecoder[Msg] = None,
-        parse_message: CustomParser[Msg] = None,
+        decode_message: AsyncDecoder[Msg] = None,
+        parse_message: AsyncParser[Msg] = None,
         protocol: str = "nats",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         subject: str,
         *,
         queue: str = "",
-        endpoint: AnyCallable,
+        endpoint: HandlerCallable[T_HandlerReturn],
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[Msg] = None,
-        parse_message: CustomParser[Msg] = None,
+        decode_message: AsyncDecoder[Msg] = None,
+        parse_message: AsyncParser[Msg] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> HandlerCallable:
+    ) -> Callable[[Msg, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         subject: str,
         *,
         queue: str = "",
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[Msg] = None,
-        parse_message: CustomParser[Msg] = None,
+        decode_message: AsyncDecoder[Msg] = None,
+        parse_message: AsyncParser[Msg] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[Msg, bool], Awaitable[T_HandlerReturn]],
+    ]:
         pass
```

### Comparing `propan-0.1.4.4/propan/fastapi/rabbit/router.pyi` & `propan-0.1.4.5/propan/fastapi/rabbit/router.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import logging
 from enum import Enum
 from ssl import SSLContext
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Sequence, Type, Union
 
 import aio_pika
 from aio_pika.message import IncomingMessage
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from pamqp.common import FieldTable
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import RabbitBroker
-from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.broker_usecase import (
+    AsyncDecoder,
+    AsyncParser,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 class RabbitRouter(PropanRouter[RabbitBroker]):
     def __init__(
         self,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
@@ -55,39 +59,42 @@
         ),
         # Broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         consumers: Optional[int] = None,
-        decode_message: CustomDecoder[IncomingMessage] = None,
-        parse_message: CustomParser[IncomingMessage] = None,
+        decode_message: AsyncDecoder[IncomingMessage] = None,
+        parse_message: AsyncParser[IncomingMessage] = None,
         schema_url: str = "/asyncapi",
         protocol: str = "amqp",
         protocol_version: str = "0.9.1",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
-        endpoint: AnyCallable,
+        endpoint: HandlerCallable[T_HandlerReturn],
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[IncomingMessage] = None,
-        parse_message: CustomParser[IncomingMessage] = None,
+        decode_message: AsyncDecoder[IncomingMessage] = None,
+        parse_message: AsyncParser[IncomingMessage] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> HandlerCallable:
+    ) -> Callable[[IncomingMessage, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[IncomingMessage] = None,
-        parse_message: CustomParser[IncomingMessage] = None,
+        decode_message: AsyncDecoder[IncomingMessage] = None,
+        parse_message: AsyncParser[IncomingMessage] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[IncomingMessage, bool], Awaitable[T_HandlerReturn]],
+    ]:
         pass
```

### Comparing `propan-0.1.4.4/propan/fastapi/redis/router.pyi` & `propan-0.1.4.5/propan/fastapi/redis/router.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import logging
 from enum import Enum
-from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Type, Union
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+)
 
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from redis.asyncio.connection import BaseParser, DefaultParser, Encoder
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import RedisBroker
-from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.broker_usecase import (
+    AsyncDecoder,
+    AsyncParser,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, AnyDict, DecoratedCallable, HandlerCallable
+from propan.types import AnyDict
 
 class RedisRouter(PropanRouter[RedisBroker]):
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: float = 1.0,
         host: str = "localhost",
@@ -62,35 +78,38 @@
         ),
         # Broker kwargs
         schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         protocol: str = "redis",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         channel: str,
         *,
-        endpoint: AnyCallable,
+        endpoint: HandlerCallable[T_HandlerReturn],
         pattern: bool = False,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> HandlerCallable:
+    ) -> Callable[[AnyDict, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[AnyDict, bool], Awaitable[T_HandlerReturn]],
+    ]:
         pass
```

### Comparing `propan-0.1.4.4/propan/fastapi/sqs/router.pyi` & `propan-0.1.4.5/propan/fastapi/sqs/router.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import logging
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Sequence, Type, Union
 
 from aiobotocore.config import AioConfig
 from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import SQSBroker
-from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
+from propan.brokers._model.broker_usecase import (
+    AsyncDecoder,
+    AsyncParser,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers.sqs.schema import SQSQueue
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, AnyDict, DecoratedCallable, HandlerCallable
+from propan.types import AnyDict
 
 class SQSRouter(PropanRouter[SQSBroker]):
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
@@ -52,47 +57,50 @@
         ),
         # Broker kwargs
         schema_url: str = "/asyncapi",
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         protocol: str = "sqs",
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
-        endpoint: AnyCallable,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        endpoint: HandlerCallable[T_HandlerReturn],
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> HandlerCallable:
+    ) -> Callable[[AnyDict, bool], Awaitable[T_HandlerReturn]]:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
         attributes: Sequence[str] = (),
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
-        decode_message: CustomDecoder[AnyDict] = None,
-        parse_message: CustomParser[AnyDict] = None,
+        decode_message: AsyncDecoder[AnyDict] = None,
+        parse_message: AsyncParser[AnyDict] = None,
         description: str = "",
         dependencies: Optional[Sequence[params.Depends]] = None,
-    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[AnyDict, bool], Awaitable[T_HandlerReturn]],
+    ]:
         pass
```

### Comparing `propan-0.1.4.4/propan/log/formatter.py` & `propan-0.1.4.5/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/log/logging.py` & `propan-0.1.4.5/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/__init__.py` & `propan-0.1.4.5/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/kafka.py` & `propan-0.1.4.5/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/nats.py` & `propan-0.1.4.5/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/rabbit.py` & `propan-0.1.4.5/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/redis.py` & `propan-0.1.4.5/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/sqs.py` & `propan-0.1.4.5/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/test/utils.py` & `propan-0.1.4.5/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/utils/functions.py` & `propan-0.1.4.5/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/utils/context/main.py` & `propan-0.1.4.5/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/propan/utils/context/types.py` & `propan-0.1.4.5/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/LICENSE` & `propan-0.1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/README.md` & `propan-0.1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/pyproject.toml` & `propan-0.1.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.4/PKG-INFO` & `propan-0.1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

