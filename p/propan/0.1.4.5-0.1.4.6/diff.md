# Comparing `tmp/propan-0.1.4.5.tar.gz` & `tmp/propan-0.1.4.6.tar.gz`

## Comparing `propan-0.1.4.5.tar` & `propan-0.1.4.6.tar`

### file list

```diff
@@ -1,185 +1,188 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.5/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/dependantbot.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 propan-0.1.4.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/redis/pattern.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/scheduling/rocketry.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/gen_py_code.sh
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/message.proto
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/protobuf.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/serialization/requirements.txt
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.5/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__about__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/__main__.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/_compat.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/routing.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    13106 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/routing.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/routing.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/routing.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/routing.pyi
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    14740 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/routing.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/routing.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/routing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/routing.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/routing.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/routing.pyi
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/__init__.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/app.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/nats.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/rabbit.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/redis.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/sqs.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/main.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.5/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/publish.sh
--rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.5/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.5/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.5/LICENSE
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 propan-0.1.4.5/README.md
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.4.5/pyproject.toml
--rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 propan-0.1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.6/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 propan-0.1.4.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.6/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__about__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/__main__.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/_compat.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/py.typed
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/constants.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    19850 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/logging.py
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/rabbit/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/app.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/nats.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/sqs.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.6/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/publish.sh
+-rwxr-xr-x   0        0        0      487 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.6/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.6/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.6/LICENSE
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 propan-0.1.4.6/README.md
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 propan-0.1.4.6/pyproject.toml
+-rw-r--r--   0        0        0    18745 2020-02-02 00:00:00.000000 propan-0.1.4.6/PKG-INFO
```

### Comparing `propan-0.1.4.5/CONTRIBUTING.md` & `propan-0.1.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/SECURITY.md` & `propan-0.1.4.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.4.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.4.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/workflows/documentation.yml` & `propan-0.1.4.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/workflows/publish_coverage.yml` & `propan-0.1.4.6/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/workflows/publish_pypi.yml` & `propan-0.1.4.6/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/.github/workflows/tests.yml` & `propan-0.1.4.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/3_lifespan_events.py` & `propan-0.1.4.6/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/4_cli_attributes_promotion.py` & `propan-0.1.4.6/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/5_publishing.py` & `propan-0.1.4.6/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/6_arguments_casting.py` & `propan-0.1.4.6/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/7_handler_errors_processing.py` & `propan-0.1.4.6/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/1_dependency_injection.py` & `propan-0.1.4.6/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.4.6/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.4.6/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.4.6/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.4.6/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/dependencies/7_annotated.py` & `propan-0.1.4.6/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/quart.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.4.6/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/rabbit/direct.py` & `propan-0.1.4.6/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/rabbit/fanout.py` & `propan-0.1.4.6/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/rabbit/header.py` & `propan-0.1.4.6/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/rabbit/topic.py` & `propan-0.1.4.6/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/redis/direct.py` & `propan-0.1.4.6/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/redis/pattern.py` & `propan-0.1.4.6/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/examples/serialization/protobuf.py` & `propan-0.1.4.6/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/__about__.py` & `propan-0.1.4.6/propan/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.4.5"
+__version__ = "0.1.4.6"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.4.5/propan/__init__.py` & `propan-0.1.4.6/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/_compat.py` & `propan-0.1.4.6/propan/_compat.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/annotations.py` & `propan-0.1.4.6/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/__init__.py` & `propan-0.1.4.6/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/channels.py` & `propan-0.1.4.6/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/info.py` & `propan-0.1.4.6/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/main.py` & `propan-0.1.4.6/propan/asyncapi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseModel, Field
 
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.info import AsyncAPIInfo
 from propan.asyncapi.message import AsyncAPIMessage
 from propan.asyncapi.servers import AsyncAPIServer
 from propan.asyncapi.utils import AsyncAPIExternalDocs, AsyncAPITag
-from propan.brokers._model.utils import ContentTypes
+from propan.brokers.constants import ContentTypes
 from propan.types import AnyDict
 
 ASYNC_API_VERSION = "2.6.0"
 
 
 class AsyncAPIComponents(BaseModel):
     # TODO
```

### Comparing `propan-0.1.4.5/propan/asyncapi/message.py` & `propan-0.1.4.6/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/security.py` & `propan-0.1.4.6/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/subscription.py` & `propan-0.1.4.6/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/bindings/amqp.py` & `propan-0.1.4.6/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/bindings/kafka.py` & `propan-0.1.4.6/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/bindings/main.py` & `propan-0.1.4.6/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/asyncapi/bindings/redis.py` & `propan-0.1.4.6/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/_model/broker_usecase.py` & `propan-0.1.4.6/propan/brokers/_model/broker_usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,22 +25,21 @@
 from fast_depends.dependencies import Depends
 from fast_depends.utils import args_to_kwargs
 from typing_extensions import Self, TypeAlias, TypeVar
 
 from propan.brokers._model.routing import BrokerRouter
 from propan.brokers._model.schemas import BaseHandler, PropanMessage
 from propan.brokers._model.utils import (
-    ContentType,
-    ContentTypes,
     change_logger_handlers,
     get_watcher,
     set_message_context,
     suppress_decor,
     to_send,
 )
+from propan.brokers.constants import ContentType, ContentTypes
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import AnyDict, DecodedMessage, SendableMessage
 from propan.utils import apply_types, context
 from propan.utils.functions import get_function_positional_arguments, to_async
```

### Comparing `propan-0.1.4.5/propan/brokers/_model/routing.py` & `propan-0.1.4.6/propan/brokers/_model/routing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/_model/schemas.py` & `propan-0.1.4.6/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/_model/utils.py` & `propan-0.1.4.6/propan/brokers/_model/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 import logging
-from enum import Enum
 from functools import wraps
 from typing import Awaitable, Callable, Optional, Tuple, TypeVar, Union, cast
 
-from typing_extensions import TypeAlias
-
 from propan._compat import dump_json
+from propan.brokers.constants import ContentType, ContentTypes
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.types import SendableMessage
 from propan.utils import context
 
-ContentType: TypeAlias = str
-
-
-class ContentTypes(str, Enum):
-    text = "text/plain"
-    json = "application/json"
-
 
 def to_send(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
     if msg is None:
         return b"", None
 
     if isinstance(msg, bytes):
         return msg, None
```

### Comparing `propan-0.1.4.5/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.4.6/propan/brokers/kafka/kafka_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,24 @@
 from aiokafka.structs import ConsumerRecord
 from fast_depends.dependencies import Depends
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Literal, TypeAlias, TypeVar
 
 from propan.__about__ import __version__
-from propan.brokers._model.broker_usecase import BrokerAsyncUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerAsyncUsecase,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.kafka.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.types import (
-    AnyDict,
-    DecodedMessage,
-    HandlerCallable,
-    HandlerWrapper,
-    SendableMessage,
-)
+from propan.types import AnyDict, DecodedMessage, SendableMessage
 from propan.utils.context import context
 
 T = TypeVar("T")
 CorrelationId: TypeAlias = str
 KafkaMessage: TypeAlias = PropanMessage[ConsumerRecord]
 
 
@@ -169,18 +167,23 @@
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
         ## broker
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
-    ) -> HandlerWrapper:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[ConsumerRecord, bool], Awaitable[T_HandlerReturn]],
+    ]:
         super().handle()
 
-        def wrapper(func: HandlerCallable) -> HandlerCallable:
+        def wrapper(
+            func: HandlerCallable[T_HandlerReturn],
+        ) -> Callable[[ConsumerRecord, bool], Awaitable[T_HandlerReturn]]:
             for t in topics:
                 self.__max_topic_len = max((self.__max_topic_len, len(t)))
 
             func, dependant = self._wrap_handler(
                 func,
                 extra_dependencies=dependencies,
                 **original_kwargs,
```

### Comparing `propan-0.1.4.5/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.4.6/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/kafka/routing.pyi` & `propan-0.1.4.6/propan/brokers/kafka/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/kafka/schemas.py` & `propan-0.1.4.6/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/nats/nats_broker.py` & `propan-0.1.4.6/propan/brokers/nats/nats_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,24 @@
 from nats.aio.msg import Msg
 from nats.aio.subscription import (
     DEFAULT_SUB_PENDING_BYTES_LIMIT,
     DEFAULT_SUB_PENDING_MSGS_LIMIT,
 )
 from typing_extensions import TypeAlias
 
-from propan.brokers._model import BrokerAsyncUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerAsyncUsecase,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import WRONG_PUBLISH_ARGS
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.types import (
-    AnyDict,
-    DecodedMessage,
-    HandlerCallable,
-    HandlerWrapper,
-    SendableMessage,
-)
+from propan.types import AnyDict, DecodedMessage, SendableMessage
 from propan.utils import context
 
 T = TypeVar("T")
 NatsMessage: TypeAlias = PropanMessage[Msg]
 
 
 class NatsBroker(BrokerAsyncUsecase[Msg, Client]):
@@ -92,21 +90,26 @@
         queue: str = "",
         *,
         dependencies: Sequence[Depends] = (),
         pending_msgs_limit: int = DEFAULT_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_SUB_PENDING_BYTES_LIMIT,
         description: str = "",
         **original_kwargs: AnyDict,
-    ) -> HandlerWrapper:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[Msg, bool], Awaitable[T_HandlerReturn]],
+    ]:
         super().handle()
 
         self._max_subject_len = max((self._max_subject_len, len(subject)))
         self._max_queue_len = max((self._max_queue_len, len(queue)))
 
-        def wrapper(func: HandlerCallable) -> HandlerCallable:
+        def wrapper(
+            func: HandlerCallable[T_HandlerReturn],
+        ) -> Callable[[Msg, bool], Awaitable[T_HandlerReturn]]:
             func, dependant = self._wrap_handler(
                 func,
                 queue=queue,
                 subject=subject,
                 extra_dependencies=dependencies,
                 **original_kwargs,
             )
```

### Comparing `propan-0.1.4.5/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.4.6/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.4.6/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/nats/routing.pyi` & `propan-0.1.4.6/propan/brokers/nats/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/nats/schemas.py` & `propan-0.1.4.6/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,41 +22,45 @@
 from aio_pika.abc import DeliveryMode
 from anyio.streams.memory import MemoryObjectReceiveStream
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 from yarl import URL
 
 from propan._compat import model_to_dict
-from propan.brokers._model import BrokerAsyncUsecase
+from propan.brokers._model.broker_usecase import (
+    BrokerAsyncUsecase,
+    HandlerCallable,
+    T_HandlerReturn,
+)
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import WRONG_PUBLISH_ARGS
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
+from propan.brokers.rabbit.logging import RabbitLoggingMixin
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
-from propan.types import AnyDict, HandlerCallable, HandlerWrapper, SendableMessage
+from propan.brokers.rabbit.utils import validate_exchange, validate_queue
+from propan.types import AnyDict, SendableMessage
 from propan.utils import context
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage: TypeAlias = Union[aio_pika.message.Message, SendableMessage]
 RabbitMessage: TypeAlias = PropanMessage[aio_pika.message.IncomingMessage]
 T = TypeVar("T")
 
 RABBIT_REPLY = "amq.rabbitmq.reply-to"
 
 
 class RabbitBroker(
-    BrokerAsyncUsecase[aio_pika.message.IncomingMessage, aio_pika.RobustConnection]
+    RabbitLoggingMixin,
+    BrokerAsyncUsecase[aio_pika.message.IncomingMessage, aio_pika.RobustConnection],
 ):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
     _queues: Dict[RabbitQueue, aio_pika.RobustQueue]
     _exchanges: Dict[RabbitExchange, aio_pika.RobustExchange]
-
-    __max_queue_len: int
-    __max_exchange_len: int
     _rpc_lock: anyio.Lock
 
     def __init__(
         self,
         url: Union[str, URL, None] = None,
         *,
         log_fmt: Optional[str] = None,
@@ -74,16 +78,16 @@
             **kwargs,
         )
         self._max_consumers = consumers
 
         self._channel = None
         self._rpc_lock = anyio.Lock()
 
-        self.__max_queue_len = 4
-        self.__max_exchange_len = 4
+        self._max_queue_len = 4
+        self._max_exchange_len = 4
         self._queues = {}
         self._exchanges = {}
 
     async def close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
@@ -122,22 +126,29 @@
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
-    ) -> HandlerWrapper:
+    ) -> Callable[
+        [HandlerCallable[T_HandlerReturn]],
+        Callable[[aio_pika.message.IncomingMessage, bool], Awaitable[T_HandlerReturn]],
+    ]:
         super().handle()
 
-        queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
+        queue, exchange = validate_queue(queue), validate_exchange(exchange)
 
-        self.__setup_log_context(queue, exchange)
+        self._setup_log_context(queue, exchange)
 
-        def wrapper(func: HandlerCallable) -> HandlerCallable:
+        def wrapper(
+            func: HandlerCallable[T_HandlerReturn],
+        ) -> Callable[
+            [aio_pika.message.IncomingMessage, bool], Awaitable[T_HandlerReturn]
+        ]:
             func, dependant = self._wrap_handler(
                 func,
                 queue=queue,
                 exchange=exchange,
                 extra_dependencies=dependencies,
                 **original_kwargs,
             )
@@ -188,15 +199,15 @@
         persist: bool = False,
         reply_to: Optional[str] = None,
         **message_kwargs,
     ) -> Union[aiormq.abc.ConfirmationFrameType, Dict, str, bytes, None]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
-        queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
+        queue, exchange = validate_queue(queue), validate_exchange(exchange)
 
         if callback is True:
             if reply_to is not None:
                 raise WRONG_PUBLISH_ARGS
             else:
                 context = RPCCallback(self._rpc_lock, self)
         else:
@@ -281,37 +292,14 @@
                     arguments=current.bind_arguments,
                 )
                 current = current.bind_to
                 current_exch = parent_exch
 
         return exch
 
-    def _get_log_context(
-        self,
-        message: Optional[RabbitMessage],
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange] = None,
-    ) -> Dict[str, Any]:
-        context = {
-            "queue": queue.name,
-            "exchange": exchange.name if exchange else "default",
-            **super()._get_log_context(message),
-        }
-        return context
-
-    @property
-    def fmt(self) -> str:
-        return super().fmt or (
-            "%(asctime)s %(levelname)s - "
-            f"%(exchange)-{self.__max_exchange_len}s | "
-            f"%(queue)-{self.__max_queue_len}s | "
-            f"%(message_id)-10s "
-            "- %(message)s"
-        )
-
     @staticmethod
     async def _parse_message(
         message: aio_pika.message.IncomingMessage,
     ) -> RabbitMessage:
         return PropanMessage(
             body=message.body,
             headers=message.headers,
@@ -330,18 +318,18 @@
         async def wrapper(message: RabbitMessage) -> T:
             pika_message = message.raw_message
             if watcher is None:
                 context = pika_message.process()
             else:
                 context = WatcherContext(
                     watcher,
-                    message.message_id,
-                    on_success=pika_message.ack,
-                    on_error=pika_message.nack,
-                    on_max=pika_message.reject,
+                    message,
+                    on_success=ack,
+                    on_error=nack,
+                    on_max=reject,
                 )
 
             async with context:
                 r = await func(message)
                 if message.reply_to:
                     await self.publish(
                         message=r,
@@ -378,56 +366,19 @@
                     "correlation_id": str(uuid4()),
                     **message_kwargs,
                 },
             )
 
         return message
 
-    def __setup_log_context(
-        self,
-        queue: Optional[RabbitQueue] = None,
-        exchange: Optional[RabbitExchange] = None,
-    ) -> None:
-        if exchange is not None:
-            self.__max_exchange_len = max(self.__max_exchange_len, len(exchange.name))
-
-        if queue is not None:  # pragma: no branch
-            self.__max_queue_len = max(self.__max_queue_len, len(queue.name))
-
     @property
     def channel(self) -> aio_pika.RobustChannel:
         return self._channel
 
 
-def _validate_exchange(
-    exchange: Union[str, RabbitExchange, None] = None,
-) -> Optional[RabbitExchange]:
-    if exchange is not None:  # pragma: no branch
-        if isinstance(exchange, str):
-            exchange = RabbitExchange(name=exchange)
-        elif not isinstance(exchange, RabbitExchange):
-            raise ValueError(
-                f"Exchange '{exchange}' should be 'str' | 'RabbitExchange' instance"
-            )
-    return exchange
-
-
-def _validate_queue(
-    queue: Union[str, RabbitQueue, None] = None
-) -> Optional[RabbitQueue]:
-    if queue is not None:  # pragma: no branch
-        if isinstance(queue, str):
-            queue = RabbitQueue(name=queue)
-        elif not isinstance(queue, RabbitQueue):
-            raise ValueError(
-                f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
-            )
-    return queue
-
-
 class RPCCallback:
     def __init__(self, lock: anyio.Lock, broker: RabbitBroker):
         self.lock = lock
         self.broker = broker
 
     async def __aenter__(self) -> Tuple[str, MemoryObjectReceiveStream]:
         (
@@ -455,7 +406,37 @@
         self.lock.release()
         await self.queue.cancel(self.consumer_tag)
 
 
 @asynccontextmanager
 async def fake_context(reply_to: str) -> Tuple[str, None]:
     yield reply_to, None
+
+
+async def ack(message: RabbitMessage) -> None:
+    pika_message = message.raw_message
+    if (
+        pika_message._IncomingMessage__processed
+        or pika_message._IncomingMessage__no_ack
+    ):
+        return
+    await pika_message.ack()
+
+
+async def nack(message: RabbitMessage) -> None:
+    pika_message = message.raw_message
+    if (
+        pika_message._IncomingMessage__processed
+        or pika_message._IncomingMessage__no_ack
+    ):
+        return
+    await pika_message.nack()
+
+
+async def reject(message: RabbitMessage) -> None:
+    pika_message = message.raw_message
+    if (
+        pika_message._IncomingMessage__processed
+        or pika_message._IncomingMessage__no_ack
+    ):
+        return
+    await pika_message.reject()
```

### Comparing `propan-0.1.4.5/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.4.6/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/rabbit/routing.pyi` & `propan-0.1.4.6/propan/brokers/rabbit/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/rabbit/schemas.py` & `propan-0.1.4.6/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/redis/redis_broker.py` & `propan-0.1.4.6/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.4.6/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/redis/routing.pyi` & `propan-0.1.4.6/propan/brokers/redis/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/redis/schemas.py` & `propan-0.1.4.6/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/sqs/routing.pyi` & `propan-0.1.4.6/propan/brokers/sqs/routing.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/sqs/schema.py` & `propan-0.1.4.6/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.4.6/propan/brokers/sqs/sqs_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 T = TypeVar("T")
 QueueUrl: TypeAlias = str
 CorrelationId: TypeAlias = str
 SQSMessage: TypeAlias = PropanMessage[AnyDict]
 
 
-class SQSBroker(BrokerAsyncUsecase):
+class SQSBroker(BrokerAsyncUsecase[AnyDict, AioBaseClient]):
     _connection: AioBaseClient
     _queues: Dict[str, QueueUrl]
     __max_queue_len: int
     response_queue: str
     response_callbacks: Dict[CorrelationId, "asyncio.Future[DecodedMessage]"]
     handlers: List[Handler]
 
@@ -128,17 +128,18 @@
         if watcher is None:
             watcher = NotPushBackWatcher()
 
         @wraps(func)
         async def process_wrapper(message: SQSMessage) -> T:
             context = WatcherContext(
                 watcher,
-                message.message_id,
-                on_success=self.delete_message,
-                on_max=self.delete_message,
+                message,
+                on_success=delete_message,
+                on_max=delete_message,
+                connection=self._connection,
             )
 
             async with context:
                 r = await func(message)
 
                 if message.reply_to:
                     await self.publish(
@@ -330,21 +331,14 @@
         if url is None:
             url = (await self._connection.get_queue_url(QueueName=queue)).get(
                 "QueueUrl", ""
             )
             self._queues[queue] = url
         return url
 
-    async def delete_message(self) -> None:
-        message = context.get_local("message")
-        await self._connection.delete_message(
-            QueueUrl=context.get_local("queue_url"),
-            ReceiptHandle=message.get("ReceiptHandle", ""),
-        )
-
     async def _consume(self, queue_url: str, handler: Handler) -> NoReturn:
         c = self._get_log_context(None, handler.queue.name)
 
         connected = True
         with context.scope("queue_url", queue_url):
             while True:
                 try:
@@ -406,7 +400,17 @@
         self, message: Optional[SQSMessage], queue: str
     ) -> Dict[str, Any]:
         context = {
             "queue": queue,
             **super()._get_log_context(message),
         }
         return context
+
+
+async def delete_message(
+    message: SQSMessage, connection: Optional[AioBaseClient]
+) -> None:
+    if connection:
+        await connection.delete_message(
+            QueueUrl=context.get_local("queue_url"),
+            ReceiptHandle=message.raw_message.get("ReceiptHandle", ""),
+        )
```

### Comparing `propan-0.1.4.5/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.4.6/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/app.py` & `propan-0.1.4.6/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/main.py` & `propan-0.1.4.6/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/docs/app.py` & `propan-0.1.4.6/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/docs/gen.py` & `propan-0.1.4.6/propan/cli/docs/gen.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/docs/serving.py` & `propan-0.1.4.6/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/core.py` & `propan-0.1.4.6/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/app.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/core.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/nats.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/redis.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.4.6/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/supervisors/basereload.py` & `propan-0.1.4.6/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/supervisors/multiprocess.py` & `propan-0.1.4.6/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/supervisors/utils.py` & `propan-0.1.4.6/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/supervisors/watchfiles.py` & `propan-0.1.4.6/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/utils/imports.py` & `propan-0.1.4.6/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/utils/logs.py` & `propan-0.1.4.6/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/cli/utils/parser.py` & `propan-0.1.4.6/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/__init__.py` & `propan-0.1.4.6/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/core/route.py` & `propan-0.1.4.6/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/core/router.py` & `propan-0.1.4.6/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/kafka/router.pyi` & `propan-0.1.4.6/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/nats/router.pyi` & `propan-0.1.4.6/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/rabbit/router.pyi` & `propan-0.1.4.6/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/redis/router.pyi` & `propan-0.1.4.6/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/fastapi/sqs/router.pyi` & `propan-0.1.4.6/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/log/formatter.py` & `propan-0.1.4.6/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/log/logging.py` & `propan-0.1.4.6/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/__init__.py` & `propan-0.1.4.6/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/kafka.py` & `propan-0.1.4.6/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/nats.py` & `propan-0.1.4.6/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/rabbit.py` & `propan-0.1.4.6/propan/test/rabbit.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,16 @@
 
 from propan.brokers.rabbit import (
     ExchangeType,
     RabbitBroker,
     RabbitExchange,
     RabbitQueue,
 )
-from propan.brokers.rabbit.rabbit_broker import (  # type: ignore
-    PikaSendableMessage,
-    TimeoutType,
-    _validate_exchange,
-    _validate_queue,
-)
+from propan.brokers.rabbit.rabbit_broker import PikaSendableMessage, TimeoutType
+from propan.brokers.rabbit.utils import validate_exchange, validate_queue
 from propan.test.utils import call_handler
 
 __all__ = (
     "build_message",
     "TestRabbitBroker",
 )
 
@@ -47,15 +43,15 @@
     message: PikaSendableMessage = "",
     queue: Union[RabbitQueue, str] = "",
     exchange: Union[RabbitExchange, str, None] = None,
     *,
     routing_key: str = "",
     **message_kwargs: AnyDict,
 ) -> PatchedMessage:
-    que, exch = _validate_queue(queue), _validate_exchange(exchange)
+    que, exch = validate_queue(queue), validate_exchange(exchange)
     msg = RabbitBroker._validate_message(message, None, **message_kwargs)
 
     routing = routing_key or (que.name if que else "")
 
     return PatchedMessage(
         aiormq.abc.DeliveredMessage(
             delivery=spec.Basic.Deliver(
```

### Comparing `propan-0.1.4.5/propan/test/redis.py` & `propan-0.1.4.6/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/sqs.py` & `propan-0.1.4.6/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/test/utils.py` & `propan-0.1.4.6/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/utils/functions.py` & `propan-0.1.4.6/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/utils/context/main.py` & `propan-0.1.4.6/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/propan/utils/context/types.py` & `propan-0.1.4.6/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/LICENSE` & `propan-0.1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/README.md` & `propan-0.1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.4.5/pyproject.toml` & `propan-0.1.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 async-kafka = [
     "aiokafka>=0.8",
 ]
 
 doc = [
     "PyYAML",
     "email-validator>=2.0.0",
-    "polyfactory>=2.3.0; python_version > '3.7'",
+    "polyfactory>=2.5.0; python_version > '3.7'",
     "jsonref",
     "fastapi",
     "uvicorn",
 ]
 
 async-sqs = [
     "aiobotocore",
@@ -105,15 +105,15 @@
     "propan[async-rabbit]",
     "propan[async-nats]",
     "propan[async-redis]",
     "propan[async-kafka]",
     "propan[async-sqs]",
     "propan[testsuite]",
 
-    "fastapi==0.100.0b1",
+    "fastapi>=0.100.0b2",
     "httpx",
 ]
 
 dev-doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
```

### Comparing `propan-0.1.4.5/PKG-INFO` & `propan-0.1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.4.5
+Version: 0.1.4.6
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -66,19 +66,19 @@
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'dev-doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'dev-doc'
 Requires-Dist: typer[all]; extra == 'dev-doc'
 Provides-Extra: doc
 Requires-Dist: email-validator>=2.0.0; extra == 'doc'
 Requires-Dist: fastapi; extra == 'doc'
 Requires-Dist: jsonref; extra == 'doc'
-Requires-Dist: polyfactory>=2.3.0; python_version > '3.7' and extra == 'doc'
+Requires-Dist: polyfactory>=2.5.0; python_version > '3.7' and extra == 'doc'
 Requires-Dist: pyyaml; extra == 'doc'
 Requires-Dist: uvicorn; extra == 'doc'
 Provides-Extra: test
-Requires-Dist: fastapi==0.100.0b1; extra == 'test'
+Requires-Dist: fastapi>=0.100.0b2; extra == 'test'
 Requires-Dist: httpx; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: propan[async-sqs]; extra == 'test'
 Requires-Dist: propan[doc]; extra == 'test'
```

