# Comparing `tmp/yyxx_game_pkg-2023.7.6.2.tar.gz` & `tmp/yyxx_game_pkg-2023.8.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.7.6.2.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.8.4.1.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.7.6.2.tar` & `yyxx_game_pkg-2023.8.4.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     4895 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/README.md
--rw-r--r--   0        0        0     1945 2023-07-06 07:53:26.321999 yyxx_game_pkg-2023.7.6.2/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-07-06 07:53:13.313860 yyxx_game_pkg-2023.7.6.2/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/__init__.py
--rw-r--r--   0        0        0     5166 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/Operator.py
--rw-r--r--   0        0        0     1505 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/OperatorServer.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/RechargeConfig.py
--rw-r--r--   0        0        0     2600 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/TableFieldConf.py
--rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/__init__.py
--rw-r--r--   0        0        0      124 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/__init__.py
--rw-r--r--   0        0        0     4353 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/check_token.py
--rw-r--r--   0        0        0     5805 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/map_core.py
--rw-r--r--   0        0        0     3506 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/recharge.py
--rw-r--r--   0        0        0     6894 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/__init__.py
--rw-r--r--   0        0        0     2053 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/global_settings.py
--rw-r--r--   0        0        0      128 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/aes.py
--rw-r--r--   0        0        0     1113 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/basic.py
--rw-r--r--   0        0        0     1351 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/make_sign.py
--rw-r--r--   0        0        0     2652 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/rsa.py
--rw-r--r--   0        0        0       83 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1304 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5596 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      149 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/__init__.py
--rw-r--r--   0        0        0     3443 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
--rw-r--r--   0        0        0      326 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
--rw-r--r--   0        0        0    10527 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
--rw-r--r--   0        0        0     7993 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
--rw-r--r--   0        0        0     3955 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2722 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     3215 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/op_helper.py
--rw-r--r--   0        0        0     1266 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2966 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-07-06 07:53:13.317860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0      666 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/formatters.py
--rw-r--r--   0        0        0     3467 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.385860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0      428 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/__init__.py
--rw-r--r--   0        0        0      132 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/cookiecutter.json
--rw-r--r--   0        0        0     4023 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
--rw-r--r--   0        0        0      624 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
--rw-r--r--   0        0        0     4077 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
--rw-r--r--   0        0        0       83 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5650 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     3135 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/error_code.py
--rw-r--r--   0        0        0     2845 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     9461 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     7441 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     2092 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xfutures.py
--rw-r--r--   0        0        0     3653 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0      573 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xstring.py
--rw-r--r--   0        0        0       69 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/__init__.py
--rw-r--r--   0        0        0     2852 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/middleware.py
--rw-r--r--   0        0        0       71 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/__init__.py
--rw-r--r--   0        0        0      564 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/common.py
--rw-r--r--   0        0        0      663 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/log_handlers.py
--rw-r--r--   0        0        0     1994 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/flask/__init__.py
--rw-r--r--   0        0        0     2969 2023-07-06 07:53:13.389860 yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     7116 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.7.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/README.md
+-rw-r--r--   0        0        0     1945 2023-08-04 08:07:43.088815 yyxx_game_pkg-2023.8.4.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-08-04 08:07:29.840517 yyxx_game_pkg-2023.8.4.1/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5805 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3506 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1351 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     6008 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      149 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/__init__.py
+-rw-r--r--   0        0        0     3443 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/mongo_op.py
+-rw-r--r--   0        0        0      326 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/__init__.py
+-rw-r--r--   0        0        0    10527 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py
+-rw-r--r--   0        0        0     7993 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py
+-rw-r--r--   0        0        0     3955 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2722 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-08-04 08:07:29.844517 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2482 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0      363 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/formatters.py
+-rw-r--r--   0        0        0     3467 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     5108 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-08-04 08:07:29.904521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      527 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      985 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2204 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0      988 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     4023 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4077 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     6247 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     9685 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7441 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     2092 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xfutures.py
+-rw-r--r--   0        0        0     3653 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     1570 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/middleware.py
+-rw-r--r--   0        0        0       71 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/util/__init__.py
+-rw-r--r--   0        0        0      564 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/util/common.py
+-rw-r--r--   0        0        0      663 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/util/log_handlers.py
+-rw-r--r--   0        0        0     1994 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/flask/__init__.py
+-rw-r--r--   0        0        0     2969 2023-08-04 08:07:29.908521 yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     7116 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.8.4.1/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.7.6.2/README.md` & `yyxx_game_pkg-2023.8.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/pyproject.toml` & `yyxx_game_pkg-2023.8.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.07.06.002"
+version = "v2023.08.04.001"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
```

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.8.4.1/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.8.4.1/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.8.4.1/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.8.4.1/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.8.4.1/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.8.4.1/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.8.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.8.4.1/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/test_logger.py` & `yyxx_game_pkg-2023.8.4.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/test_xtrace.py` & `yyxx_game_pkg-2023.8.4.1/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.8.4.1/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.8.4.1/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/Operator.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/Operator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/OperatorServer.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/OperatorServer.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/RechargeConfig.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/RechargeConfig.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/model/TableFieldConf.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/model/TableFieldConf.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/check_token.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/map_core.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/map_core.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/center_api/sdk/recharge.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/center_api/sdk/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/__init__.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/conf/global_settings.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/aes.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/basic.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/basic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/make_sign.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/make_sign.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/crypto/rsa.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/ch_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/das_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,38 @@
     elif isinstance(val, np.int64):
         val = int(val)
     elif isinstance(val, bytes):
         val = val.decode(encoding="utf8")
     return val
 
 
+class DasApiException(Exception):
+    pass
+
+
+class DasApiChQueryException(DasApiException):
+    pass
+
+
+class DasApiChExecuteException(DasApiException):
+    pass
+
+
+class DasApiMongoQueryException(DasApiException):
+    pass
+
+
+class DasApiEsQueryException(DasApiException):
+    pass
+
+
+class DasApiEsInsertException(DasApiException):
+    pass
+
+
 class DasApi:
     """
     DasApi py
     """
 
     @staticmethod
     def _post(das_url, post_type, post_data):
@@ -56,15 +80,15 @@
             'sql': sql,             # sql语句 支持sql 和 js_sql
             'server': mongo_url     # mongo链接
         }
         :return:
         """
         b_ok, res = DasApi._post(das_url, "das/mgo/query", post_data=post_data)
         if not b_ok:
-            raise Exception(res)
+            raise DasApiMongoQueryException(res)
         res = re.sub(
             r'{\\"\$numberLong\\": \\"\d+\\"}',
             lambda m: re.search(r"\d+", m.group()).group(),
             res.decode("utf-8"),
         )
         data = json.loads(res)
         data_list = data["data"]
@@ -86,15 +110,15 @@
             "search_from": search_from,     # 分页查询offset 最大5w
             "fetch_size": fetch_size        # 单次查询总行数
         }
         :return:
         """
         b_ok, res = DasApi._post(das_url, "das/es/query", post_data=post_data)
         if not b_ok:
-            raise Exception(res)
+            raise DasApiEsQueryException(res)
         engine = post_data.get("engine", 0)
         use_search = post_data.get("search_from", -1) >= 0
         data = json.loads(res)
 
         if engine == 0:
             # opendistro
             col_dict_lst = data["schema"]
@@ -126,30 +150,30 @@
             "topic": topic,             # kafka Topic
             "data_rows": data_rows      # 数据行
         }
         :return:
         """
         b_ok, res = DasApi._post(das_url, "das/es/insert", post_data=post_data)
         if not b_ok:
-            raise Exception(res)
+            raise DasApiEsInsertException(res)
         return res
 
     @staticmethod
     def ch_query(das_url, post_data):
         """
         sql语句 查询 clickhouse 库
         :param das_url: das_http_url
         :param post_data: {
             "sql": sql,                     # sql语句
         }
         :return:
         """
         b_ok, res = DasApi._post(das_url, "/das/ch/query", post_data=post_data)
         if not b_ok:
-            raise Exception(res)
+            raise DasApiChQueryException(res)
         data = json.loads(res)
 
         res_df = pd.DataFrame(data["datarows"], columns=data["columns"])
         return res_df
 
     @staticmethod
     def ch_execute(das_url, post_data):
@@ -159,15 +183,15 @@
         :param post_data: {
             "sql": sql,                     # sql语句
         }
         :return:
         """
         b_ok, res = DasApi._post(das_url, "/das/ch/exec", post_data=post_data)
         if not b_ok:
-            raise Exception(res)
+            raise DasApiChExecuteException(res)
         return b_ok
 
 
 # if __name__ == '__main__':
 # post_type = "das/mgo/query"
 # post_data_ = dict()
 # post_data_['js_sql'] = 'db.getSiblingDB("fumo_test").getCollection("player").find({})'
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/mongo_op.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/sql2mongo.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mongo_op/sql2mongo/test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/op_helper.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/op_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,19 @@
         """
         log_config = {
             "version": 1,
             "disable_existing_loggers": False,
             "formatters": {
                 "def_fmt": {
                     "datefmt": "%Y-%m-%d %H:%M:%S",
-                    "format": "[%(asctime)s,%(msecs)d: %(levelname)s/%(process)d] %(message)s",
-                    "class": "logging.Formatter",
+                    "class": "yyxx_game_pkg.logger.formatters.TraceFormatter",
+                    "format": (
+                        "[%(asctime)s,%(msecs)d: %(levelname)s/%(process)d][%(filename)s:%(funcName)s:%(lineno)d]"
+                        "[%(trace_id)s] %(message)s"
+                    ),
                 },
             },
             "handlers": {
                 "rotate_file_handler": {
                     "level": "INFO",
                     "formatter": "def_fmt",
                     "class": "yyxx_game_pkg.logger.handlers.MultiProcessTimedRotatingFileHandler",
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 # -*- coding: utf-8 -*-
 """
 @File: log
 @Author: ltw
 @Time: 2023/3/10
+@updateTime: 2023/07/24 by winslen
 """
-from yyxx_game_pkg.logger import log
-from yyxx_game_pkg.xtrace.helper import get_current_trace_id
+# 未使用的也不能删除
+from yyxx_game_pkg.logger.log import (
+    LogLevelTyping,
+    LogConfigTyping,
+    root_log,
+    Log,
+    logger,
+    local_logger,
+    local_log,
+    debug_logger,
+    debug_log,
+    LogConfig,
+)
 
 
-class StatLogConfig(log.LogConfig):
+class StatLogConfig(LogConfig):
     """
     logging 配置
     """
+
     LOCAL_LOG_FILE = "/data/logs/local.log"
     DEBUG_LOG_FILE = "/data/logs/debug.log"
 
 
-logger = log.Log(StatLogConfig)
-
-
-def local_log(msg):
-    """
-    local log rotate file
-    :param msg:
-    :return:
-    """
-    trace_id = get_current_trace_id()
-    msg = f"[{trace_id}] {msg}"
-    logger.local_log(msg)
-
-
-def debug_log(msg):
-    """
-    debug log file
-    :param msg:
-    :return:
-    """
-    logger.debug_log(msg)
+Log.init_config(StatLogConfig)
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/submit/submit.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from yyxx_game_pkg.stat.submit.logic.submit_logic import (
     to_protocol,
     process_proto,
     set_config,
     send,
 )
-from yyxx_game_pkg.logger.log import root_log
+from yyxx_game_pkg.stat.log import root_log
 
 
 def submit_schedule(schedule: str, file_path: str, api_addr: str, jaeger: dict):
     # 配置
     set_config(file_path, api_addr)
     if jaeger:
         from yyxx_game_pkg.xtrace.helper import register_to_jaeger
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 celery 实例入口
 """
 import argparse
 from celery import Celery
 
-from yyxx_game_pkg.logger.log import root_log
+from yyxx_game_pkg.stat.log import root_log
 
 
 class CeleryInstance:
     """
     celery 接口
     """
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -74,40 +74,53 @@
             res = func(*args, **kwargs)
         except Exception as e:
             _args = []
             for _arg in args:
                 _args.append(fix_str(_arg, 100))
             for k, _v in kwargs.items():
                 kwargs[k] = fix_str(_v, 100)
-            trace_id = get_current_trace_id()
             root_log(
-                f"<except_monitor> trace_id: {trace_id} "
+                "<except_monitor>"
                 f"func:{func.__module__}.{func.__name__}, args:{str(_args)}, kwargs:{str(kwargs)}, "
-                f"exc: {traceback.format_exc()} {e}"
+                f"exc: {traceback.format_exc()} {e}",
+                level="error",
             )
         return res
 
     return inner
 
 
-def except_return(default=None):
+def except_return(default=None, echo_raise=True):
     """
     # 异常后指定返回值
-    :param default: 返回值
+    :param default: 返回值(或者可执行函数)
+    :param echo_raise: 是否打印报错信息
     :return:
     """
 
     def decorator(func):
         @functools.wraps(func)
-        def wrapper(*args, **kw):
+        def wrapper(*args, **kwargs):
             try:
-                return func(*args, **kw)
+                return func(*args, **kwargs)
             except Exception as e:
-                root_log(f"{e}: exc:{traceback.format_exc()}")
-                return default
+                if echo_raise:
+                    _args = []
+                    for _arg in args:
+                        _args.append(fix_str(_arg, 100))
+                    for k, _v in kwargs.items():
+                        kwargs[k] = fix_str(_v, 100)
+                    root_log(
+                        "<except_return>"
+                        f"func:{func.__module__}.{func.__name__}, args:{str(_args)}, kwargs:{str(kwargs)}, "
+                        f"exc: {traceback.format_exc()} {e}",
+                        level="error",
+                    )
+
+                return default(e) if callable(default) else default
 
         return wrapper
 
     return decorator
 
 
 def singleton(cls):
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/error_code.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/error_code.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdataframe.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xdataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,79 +221,36 @@
 
 
 def fill_list(data):
     """填充[]到nan"""
     return [] if not isinstance(data, list) and pd.isna(data) else data
 
 
-def df_expand_labels(_df, key, bins, insert_zero=True):
-    """
-    # money_df ####
-    # player_id, money
-    # 19296,  8
-    # 21169,  8
-    # 24003,  98
-    # 25016,  2
-    # 25254,  2
-    money_df[["money_label", "label_rank"]] = df_expand_labels(
-        money_df, "money", bins=[0, 8, 41, 267, 500, 1000, 2000, 5000, 10000, 20000, 30000, 50000, 999999]
-    ) =>
-    # player_id, money, money_label, label_rank
-    # 19296,    8,  1-8,    8
-    # 21169,    8,  1-8,    8
-    # 24003,    98, 1-8,    8
-    # 25016,    2,  1-8,    8
-    # 25254,    2,  42-267, 267
-    insert_zero : 是否在bins最前面插入0
-    :return:
-    """
-
-    def prefix_bins(_bins):
-        _bins = sorted(map(int, _bins))
-        if insert_zero and _bins[0] != 0:
-            _bins.insert(0, 0)
-        return _bins
-
-    bins = prefix_bins(bins)
-    concat = "-"
-
-    def cut_bins(row):
-        val = row[key]
-        if not val:
-            return val
-
-        if val > bins[-1]:
-            val = bins[-1]
-
-        position = bisect_left(bins, val)
-        labels = f"{bins[position - 1] + 1}{concat}{bins[position]}"
-        return labels, bins[position]
-
-    return _df.apply(cut_bins, axis=1, result_type="expand")
-
-
 def div_rate(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
     """
     dataframe div函数计算百分比 top_key / bottom_key
     example:
         data_df["pay_rate"] = div_rate(data_df, "pid_cnt", "act_player_cnt")
     :return:
     """
+    fmt_show = f"%0.{precision}f"
     if isinstance(top_key, list):
         return (
             data_df[top_key]
             .div(data_df[bottom_key], axis=0)
             .round(precision + 2)
-            .applymap(lambda x: f"{round(x * 100, precision) }%")
+            .fillna(0)
+            .applymap(lambda x: f"{ fmt_show % round(x * 100, precision) }%")
         )
     return (
         data_df[top_key]
         .div(data_df[bottom_key], axis=0)
         .round(precision + 2)
-        .apply(lambda x: f"{round(x * 100, precision) }%")
+        .fillna(0)
+        .apply(lambda x: f"{fmt_show % round(x * 100, precision) }%")
     )
 
 
 def div_round(data_df: pd.DataFrame, top_key, bottom_key, precision=2) -> pd.Series:
     """
     dataframe div函数 top_key / bottom_key
     example:
@@ -331,7 +288,55 @@
     """
     if excludes:
         df_columns = _df.columns.tolist()
         columns = list(set(df_columns) - set(excludes))
     if columns:
         _df[columns] = _df[columns].astype(tpe)
     return _df
+
+
+def show_range_labels(_df, key, bins, insert_zero=True, max_label_fmt=None):
+    """
+    # money_df ####
+    # player_id, money
+    # 19296,  0
+    # 21169,  8
+    # 24003,  98
+    money_df[["money_label", "label_rank"]] = show_range_labels(
+        money_df, "money", bins=[0, 8, 41], max_label_fmt="{}+"
+    ) =>
+    # player_id, money, money_label, label_rank
+    # 19296,    0,  "",    -1
+    # 21169,    8,  "1-8",    8
+    # 24003,    98, "41+”,    41
+    insert_zero : 是否在bins最前面插入0
+    :return:
+    """
+
+    def prefix_bins(_bins):
+        _bins = sorted(map(int, _bins))
+        if insert_zero and _bins[0] != 0:
+            _bins.insert(0, 0)
+        return _bins
+
+    bins = prefix_bins(bins)
+    concat = "-"
+
+    def cut_bins(row):
+        val = row[key]
+        if not val:
+            return "", -1
+
+        if val > bins[-1]:
+            val = bins[-1]
+
+        position = bisect_left(bins, val)
+        if position <= 0:
+            return "", -1
+        left_val = bins[position - 1] + 1
+        right_val = bins[position]
+        labels = f"{left_val}{concat}{right_val}"
+        if position == len(bins) - 1 and max_label_fmt is not None:
+            labels = max_label_fmt.format(left_val)
+        return labels, bins[position]
+
+    return _df.apply(cut_bins, axis=1, result_type="expand")
```

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xdate.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xfutures.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xfutures.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xhttp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/utils/xstring.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/utils/xstring.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/__init__.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/middleware.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/middleware.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/common.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/util/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/django/util/log_handlers.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/django/util/log_handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/flask/__init__.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.8.4.1/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.7.6.2/PKG-INFO` & `yyxx_game_pkg-2023.8.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yyxx-game-pkg
-Version: 2023.7.6.2
+Version: 2023.8.4.1
 Summary: yyxx game custom module
 Home-page: https://github.com/yyxxgame/yyxxgame-pkg
 License: MIT
 Author: yyxx-game
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.7.6.2 Summary: yyxx
+Metadata-Version: 2.1 Name: yyxx-game-pkg Version: 2023.8.4.1 Summary: yyxx
 game custom module Home-page: https://github.com/yyxxgame/yyxxgame-pkg License:
 MIT Author: yyxx-game Requires-Python: >=3.8,<4 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: center-api Provides-Extra: server-
```

