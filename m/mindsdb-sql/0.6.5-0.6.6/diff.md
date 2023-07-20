# Comparing `tmp/mindsdb_sql-0.6.5.tar.gz` & `tmp/mindsdb_sql-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.5.tar", last modified: Thu Jun 15 18:36:41 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.6.tar", last modified: Thu Jul 20 12:23:05 2023, max compression
```

## Comparing `mindsdb_sql-0.6.5.tar` & `mindsdb_sql-0.6.6.tar`

### file list

```diff
@@ -1,143 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/
--rw-rw-rw-   0        0        0      535 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      567 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0     3196 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     2407 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      769 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1595 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8140 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    44911 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    52581 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21394 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8517 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    13228 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5282 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/test_parser/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/__init__.py
--rw-rw-rw-   0        0        0      776 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_ast.py
--rw-rw-rw-   0        0        0    11910 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_base_lexer.py
--rw-rw-rw-   0        0        0      223 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_base_sql.py
--rw-rw-rw-   0        0        0     1480 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_create.py
--rw-rw-rw-   0        0        0     2481 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_ddl.py
--rw-rw-rw-   0        0        0     1075 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_delete.py
--rw-rw-rw-   0        0        0     1094 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_describe.py
--rw-rw-rw-   0        0        0     2426 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_insert.py
--rw-rw-rw-   0        0        0     6945 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_misc_sql_queries.py
--rw-rw-rw-   0        0        0     3625 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_select_common_table_expression.py
--rw-rw-rw-   0        0        0    24799 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_select_operations.py
--rw-rw-rw-   0        0        0    45563 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_select_structure.py
--rw-rw-rw-   0        0        0    13620 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_show.py
--rw-rw-rw-   0        0        0     3114 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_union.py
--rw-rw-rw-   0        0        0     2462 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_update.py
--rw-rw-rw-   0        0        0      514 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_base_sql/test_use.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_chatbots.py
--rw-rw-rw-   0        0        0      605 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_create_file.py
--rw-rw-rw-   0        0        0     4203 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_create_integration.py
--rw-rw-rw-   0        0        0     6617 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_create_predictor.py
--rw-rw-rw-   0        0        0     2651 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_create_view.py
--rw-rw-rw-   0        0        0      520 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_drop_dataset.py
--rw-rw-rw-   0        0        0      861 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_drop_datasource.py
--rw-rw-rw-   0        0        0      866 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_drop_integration.py
--rw-rw-rw-   0        0        0     1708 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_drop_predictor.py
--rw-rw-rw-   0        0        0     1824 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_evaluate.py
--rw-rw-rw-   0        0        0     1339 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_finetune_predictor.py
--rw-rw-rw-   0        0        0     2056 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_jobs.py
--rw-rw-rw-   0        0        0     1587 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_ml_engine.py
--rw-rw-rw-   0        0        0     2242 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_retrain_predictor.py
--rw-rw-rw-   0        0        0     3572 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_selects.py
--rw-rw-rw-   0        0        0     1226 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_show_mindsdb.py
--rw-rw-rw-   0        0        0      959 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mindsdb/test_timeseries.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mysql/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mysql/__init__.py
--rw-rw-rw-   0        0        0      714 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mysql/test_mysql_lexer.py
--rw-rw-rw-   0        0        0     3050 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_parser/test_mysql/test_mysql_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:36:41.000000 mindsdb_sql-0.6.5/tests/test_render/
--rw-rw-rw-   0        0        0        0 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_render/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-06-15 18:36:18.000000 mindsdb_sql-0.6.5/tests/test_render/test_sqlalchemyrender.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/
+-rw-rw-rw-   0        0        0      535 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      591 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0      503 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/data.py
+-rw-rw-rw-   0        0        0     3196 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     3154 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      833 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     2569 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8179 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    46067 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+-rw-rw-rw-   0        0        0     1757 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/trigger.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    54044 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21394 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8739 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13228 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3380 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:23:05.000000 mindsdb_sql-0.6.6/sly/
+-rw-rw-rw-   0        0        0      109 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/ast.py
+-rw-rw-rw-   0        0        0    16707 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/lex.py
+-rw-rw-rw-   0        0        0    89289 2023-07-20 12:22:50.000000 mindsdb_sql-0.6.6/sly/yacc.py
```

### Comparing `mindsdb_sql-0.6.5/PKG-INFO` & `mindsdb_sql-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.6.5
+Version: 0.6.6
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.5/README.md` & `mindsdb_sql-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.6/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 from mindsdb_sql.parser.ast.base import ASTNode
 from mindsdb_sql.parser.utils import indent
 
 
 class Update(ASTNode):
     def __init__(self,
                  table,
-                 update_columns,
+                 update_columns=None,
+                 keys=None,
                  from_select=None,
                  from_select_alias=None,
                  where=None,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.table = table
+        # list[Identifier]
+        self.keys = keys
         # dict: {str: Identifier}
         self.update_columns = update_columns
         self.where = where
         self.from_select = from_select
         self.from_select_alias = from_select_alias
 
     def to_tree(self, *args, level=0, **kwargs):
         ind = indent(level)
         ind1 = indent(level + 1)
-        updated_ar = [
-            f'{k}={v.to_string()}'
-            for k, v in self.update_columns.items()
-        ]
-        updated_str = ', '.join(updated_ar)
+
+        updated_str = ''
+        if self.update_columns is not None:
+            updated_ar = [
+                f'{k}={v.to_string()}'
+                for k, v in self.update_columns.items()
+            ]
+            updated_str = ', '.join(updated_ar)
+            updated_str = f'{ind1}update_columns={updated_str}\n'
+
+        keys_str = ''
+        if self.keys is not None:
+            keys_ar = [k.to_string() for k in self.keys]
+            keys_str = ', '.join(keys_ar)
+            keys_str = f'{ind1}keys={keys_str}\n'
 
         where_str = ''
         if self.where is not None:
             where_str = ind1 + self.where.to_tree()
 
         if self.from_select is not None:
             from_select_str = f'{ind1}from_select=\n{self.from_select.to_tree(level=level+2)}\n'
             if self.from_select_alias is not None:
                 from_select_str += f'{ind1}from_select_alias=\n{self.from_select_alias.to_tree(level=level+2)}\n'
 
         else:
             from_select_str = ''
 
         out_str = f'{ind}Update(table={self.table.to_tree()}\n' \
-                  f'{ind1}update_columns={updated_str}\n' \
+                  f'{keys_str}' \
+                  f'{updated_str}' \
                   f'{where_str}' \
                   f'{from_select_str}' \
                   f'{ind})\n'
         return out_str
 
     def get_string(self, *args, **kwargs):
-        update_ar = [
-            f'{k}={v.to_string()}'
-            for k, v in self.update_columns.items()
-        ]
-        update_str = ', '.join(update_ar)
+        update_str = ''
+        if self.update_columns is not None:
+            update_ar = [
+                f'{k}={v.to_string()}'
+                for k, v in self.update_columns.items()
+            ]
+            update_str = ' set ' + ', '.join(update_ar)
+
+        keys_str = ''
+        if self.keys is not None:
+            keys_ar = [k.to_string() for k in self.keys]
+            keys_str = ' on ' + ', '.join(keys_ar)
 
         if self.from_select is not None:
             alias_str = ''
             if self.from_select_alias is not None:
                 alias_str = ' as ' + self.from_select_alias.to_string()
             from_select_str = f' from ({self.from_select.to_string()}){alias_str}'
         else:
             from_select_str = ''
 
         where_str = ''
         if self.where is not None:
             where_str = ' where ' + self.where.to_string()
 
-        return f'update {self.table.to_string()} set {update_str}{from_select_str}{where_str}'
+        return f'update {self.table.to_string()}{keys_str}{update_str}{from_select_str}{where_str}'
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 from .evaluate import Evaluate
 from .latest import Latest
 from .create_file import CreateFile
 from .create_ml_engine import CreateMLEngine
 from .drop_ml_engine import DropMLEngine
 from .create_job import CreateJob
 from .drop_job import DropJob
-from .chatbot import CreateChatBot, DropChatBot
+from .chatbot import CreateChatBot, UpdateChatBot, DropChatBot
+from .trigger import CreateTrigger, DropTrigger
 
 # remove it in next release
 CreateDatasource = CreateDatabase
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,37 @@
 
         using_str = ', '.join(using_ar)
 
         out_str = f'CREATE CHATBOT {self.name.to_string()} USING {using_str}'
         return out_str
 
 
+class UpdateChatBot(ASTNode):
+    def __init__(self, name, updated_params, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.name = name
+        self.params = updated_params
+
+    def to_tree(self, *args, level=0, **kwargs):
+        ind = indent(level)
+        out_str = f'{ind}UpdateChatBot(' \
+                  f'name={self.name.to_string()}, ' \
+                  f'updated_params={self.params})'
+        return out_str
+
+    def get_string(self, *args, **kwargs):
+        params = self.params.copy()
+
+        set_ar = [f'{k}={repr(v)}' for k, v in params.items()]
+        set_str = ', '.join(set_ar)
+
+        out_str = f'UPDATE CHATBOT {self.name.to_string()} USING {set_str}'
+        return out_str
+
+
 class DropChatBot(ASTNode):
     def __init__(self,
                  name,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = name
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         FINETUNE, EVALUATE,
         LATEST, HORIZON, USING,
         ENGINE, TRAIN, PREDICT, PARAMETERS, JOB, CHATBOT, EVERY,PROJECT,
 
         # SHOW/DDL Keywords
 
         SHOW, SCHEMAS, SCHEMA, DATABASES, DATABASE, TABLES, TABLE, FULL, EXTENDED, PROCESSLIST,
-        MUTEX, CODE, SLAVE, REPLICA, REPLICAS, CHANNEL, TRIGGERS, KEYS, STORAGE, LOGS, BINARY,
+        MUTEX, CODE, SLAVE, REPLICA, REPLICAS, CHANNEL, TRIGGERS, TRIGGER, KEYS, STORAGE, LOGS, BINARY,
         MASTER, PRIVILEGES, PROFILES, HOSTS, OPEN, INDEXES,
         VARIABLES, SESSION, STATUS,
         GLOBAL, PROCEDURE, FUNCTION, INDEX, WARNINGS,
         ENGINES, CHARSET, COLLATION, PLUGINS, CHARACTER,
         PERSIST, PERSIST_ONLY, DEFAULT,
         IF_EXISTS, COLUMNS, FIELDS, COLLATE,
         # SELECT Keywords
@@ -165,14 +165,15 @@
     MUTEX = r'\bMUTEX\b'
     CODE = r'\bCODE\b'
     SLAVE = r'\bSLAVE\b'
     REPLICA = r'\bREPLICA\b'
     REPLICAS = r'\bREPLICAS\b'
     CHANNEL = r'\bCHANNEL\b'
     TRIGGERS = r'\bTRIGGERS\b'
+    TRIGGER = r'\bTRIGGER\b'
     KEYS = r'\bKEYS\b'
     STORAGE = r'\bSTORAGE\b'
     LOGS = r'\bLOGS\b'
     BINARY = r'\bBINARY\b'
     MASTER = r'\bMASTER\b'
     PRIVILEGES = r'\bPRIVILEGES\b'
     PROFILES = r'\bPROFILES\b'
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from mindsdb_sql.parser.dialects.mindsdb.drop_dataset import DropDataset
 from mindsdb_sql.parser.dialects.mindsdb.drop_ml_engine import DropMLEngine
 from mindsdb_sql.parser.dialects.mindsdb.create_predictor import CreatePredictor
 from mindsdb_sql.parser.dialects.mindsdb.create_database import CreateDatabase
 from mindsdb_sql.parser.dialects.mindsdb.create_ml_engine import CreateMLEngine
 from mindsdb_sql.parser.dialects.mindsdb.create_view import CreateView
 from mindsdb_sql.parser.dialects.mindsdb.create_job import CreateJob
-from mindsdb_sql.parser.dialects.mindsdb.chatbot import CreateChatBot, DropChatBot
+from mindsdb_sql.parser.dialects.mindsdb.chatbot import CreateChatBot, UpdateChatBot, DropChatBot
 from mindsdb_sql.parser.dialects.mindsdb.drop_job import DropJob
+from mindsdb_sql.parser.dialects.mindsdb.trigger import CreateTrigger, DropTrigger
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
 from mindsdb_sql.parser.dialects.mindsdb.evaluate import Evaluate
 from mindsdb_sql.parser.dialects.mindsdb.create_file import CreateFile
 from mindsdb_sql.exceptions import ParsingException
 from mindsdb_sql.parser.dialects.mindsdb.lexer import MindsDBLexer
 from mindsdb_sql.parser.dialects.mindsdb.retrain_predictor import RetrainPredictor
 from mindsdb_sql.parser.dialects.mindsdb.finetune_predictor import FinetunePredictor
@@ -69,36 +70,62 @@
        'evaluate',
        'drop_database',
        'drop_view',
        'drop_table',
        'create_table',
        'create_job',
        'drop_job',
+       'create_chat_bot',
+       'drop_chat_bot',
+       'update_chat_bot',
+       'create_trigger',
+       'drop_trigger',
        )
     def query(self, p):
         return p[0]
 
     # -- ChatBot --
     @_('CREATE CHATBOT identifier USING kw_parameter_list')
-    def create_job(self, p):
+    def create_chat_bot(self, p):
         params = p.kw_parameter_list
 
         database = Identifier(params.pop('database'))
         model = Identifier(params.pop('model'))
         return CreateChatBot(
             name=p.identifier,
             database=database,
             model=model,
             params=params
         )
 
+    @_('UPDATE CHATBOT identifier SET kw_parameter_list')
+    def update_chat_bot(self, p):
+        return UpdateChatBot(name=p.identifier, updated_params=p.kw_parameter_list)
+
+
     @_('DROP CHATBOT identifier')
-    def drop_job(self, p):
+    def drop_chat_bot(self, p):
         return DropChatBot(name=p.identifier)
 
+    # -- triggers --
+    @_('CREATE TRIGGER identifier ON identifier LPAREN raw_query RPAREN')
+    def create_trigger(self, p):
+        query_str = tokens_to_string(p.raw_query)
+
+        return CreateTrigger(
+            name=p.identifier0,
+            table=p.identifier1,
+            query_str=query_str
+        )
+
+    @_('DROP TRIGGER identifier')
+    def drop_trigger(self, p):
+        return DropTrigger(name=p.identifier)
+
+
     # -- Jobs --
     @_('CREATE JOB identifier LPAREN raw_query RPAREN job_schedule',
        'CREATE JOB identifier AS LPAREN raw_query RPAREN job_schedule',
        'CREATE JOB identifier LPAREN raw_query RPAREN',
        'CREATE JOB identifier AS LPAREN raw_query RPAREN')
     def create_job(self, p):
         query_str = tokens_to_string(p.raw_query)
@@ -492,14 +519,22 @@
             from_select_alias = Identifier(from_select_alias)
         return Update(table=p.identifier,
                       update_columns=p.update_parameter_list,
                       from_select=from_select,
                       from_select_alias=from_select_alias,
                       where=where)
 
+    # UPDATE
+    @_('UPDATE identifier ON ordering_terms FROM LPAREN select RPAREN')
+    def update(self, p):
+        keys = [i.field for i in p.ordering_terms]
+        return Update(table=p.identifier,
+                      keys=keys,
+                      from_select=p.select)
+
     # INSERT
     @_('INSERT INTO identifier LPAREN result_columns RPAREN select',
        'INSERT INTO identifier select')
     def insert(self, p):
         columns = getattr(p, 'result_columns', None)
         return Insert(table=p.identifier, columns=columns, from_select=p.select)
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.6/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                                     Update, NativeQuery, Parameter, Delete)
 
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
 from mindsdb_sql.planner.steps import (FetchDataframeStep, ProjectStep, JoinStep, ApplyPredictorStep,
                                        ApplyPredictorRowStep, FilterStep, GroupByStep, LimitOffsetStep, OrderByStep,
                                        UnionStep, MapReduceStep, MultipleSteps, ApplyTimeseriesPredictorStep,
                                        GetPredictorColumns, SaveToTable, InsertToTable, UpdateToTable, SubSelectStep,
-                                       DeleteStep)
+                                       DeleteStep, DataStep)
 from mindsdb_sql.planner.ts_utils import (validate_ts_where_condition, find_time_filter, replace_time_filter,
                                           find_and_remove_time_filter)
 from mindsdb_sql.planner.utils import (disambiguate_predictor_column_identifier,
                                        get_deepest_select,
                                        recursively_extract_column_values,
                                        recursively_check_join_identifiers_for_ambiguity,
                                        query_traversal)
@@ -157,15 +157,17 @@
                                                 f' {table.to_string()}, but a different table name has been specified.')
                 else:
                     node.parts = prefix + node.parts
 
                 # keep column name for target
                 if is_target:
                     if node.alias is None:
-                        node.alias = Identifier(parts=[node.parts[-1]])
+                        last_part = node.parts[-1]
+                        if isinstance(last_part, str):
+                            node.alias = Identifier(parts=[node.parts[-1]])
 
         utils.query_traversal(query, _prepare_integration_select)
 
     def get_integration_select_step(self, select):
         integration_name, table = self.resolve_database_table(select.from_table)
 
         fetch_df_select = copy.deepcopy(select)
@@ -206,27 +208,30 @@
         mdb_entities = []
         predictors = []
         # projects = set()
         integrations = set()
 
         def find_predictors(node, is_table, **kwargs):
 
-            if is_table and isinstance(node, ast.Identifier):
-                integration, _ = self.resolve_database_table(node)
-
-                if self.is_predictor(node):
-                    predictors.append(node)
-
-                if integration in self.projects:
-                    # it is project
+            if is_table:
+                if isinstance(node, ast.Identifier):
+                    integration, _ = self.resolve_database_table(node)
+
+                    if self.is_predictor(node):
+                        predictors.append(node)
+
+                    if integration in self.projects:
+                        # it is project
+                        mdb_entities.append(node)
+
+                    elif integration is not None:
+                        integrations.add(integration)
+                if isinstance(node, ast.NativeQuery) or isinstance(node, ast.Data):
                     mdb_entities.append(node)
 
-                elif integration is not None:
-                    integrations.add(integration)
-
         utils.query_traversal(query, find_predictors)
         return {'mdb_entities': mdb_entities, 'integrations': integrations, 'predictors': predictors}
 
     def get_nested_selects_plan_fnc(self, main_integration, force=False):
         # returns function for traversal over query and inject fetch data query instead of subselects
         def find_selects(node, **kwargs):
             if isinstance(node, Select):
@@ -653,20 +658,20 @@
         }
 
     def plan_join_tables(self, query):
         query = copy.deepcopy(query)
 
         # replace sub selects, with identifiers with links to original selects
         def replace_subselects(node, **args):
-            if isinstance(node, Select) or isinstance(node, NativeQuery):
+            if isinstance(node, Select) or isinstance(node, NativeQuery) or isinstance(node, ast.Data):
                 name = f't_{id(node)}'
                 node2 = Identifier(name, alias=node.alias)
 
                 # save in attribute
-                if isinstance(node, NativeQuery):
+                if isinstance(node, NativeQuery) or isinstance(node, ast.Data):
                     # wrap to select
                     node = Select(targets=[Star()], from_table=node)
                 node2.sub_select = node
                 return node2
 
         query_traversal(query.from_table, replace_subselects)
 
@@ -799,18 +804,31 @@
 
                 if item['sub_select'] is not None:
                     # is sub select
                     item['sub_select'].alias = None
                     item['sub_select'].parentheses = False
                     step = self.plan_select(item['sub_select'])
 
+                    where = None
+                    for cond in item['conditions']:
+                        if where is None:
+                            where = cond
+                        else:
+                            where = BinaryOperation(op='and', args=[where, cond])
+
                     # apply table alias
-                    query2 = Select(targets=[Star()])
+                    query2 = Select(targets=[Star()], where=where)
                     table_name = item['table'].alias.parts[-1]
-                    step2 = SubSelectStep(query2, step.result, table_name=table_name)
+
+                    add_absent_cols = False
+                    if hasattr (item['sub_select'], 'from_table') and\
+                         isinstance(item['sub_select'].from_table, ast.Data):
+                        add_absent_cols = True
+
+                    step2 = SubSelectStep(query2, step.result, table_name=table_name, add_absent_cols=add_absent_cols)
                     step2 = self.plan.add_step(step2)
                     step_stack.append(step2)
                 elif predictor_info is not None:
                     if len(step_stack) == 0:
                         raise NotImplementedError("Predictor can't be first element of join syntax")
                     if predictor_info.get('timeseries'):
                         raise NotImplementedError("TS predictor is not supported here yet")
@@ -981,32 +999,37 @@
         aliased_fields = self.get_aliased_fields(query.targets)
 
         recursively_check_join_identifiers_for_ambiguity(query.where)
         recursively_check_join_identifiers_for_ambiguity(query.group_by, aliased_fields=aliased_fields)
         recursively_check_join_identifiers_for_ambiguity(query.having)
         recursively_check_join_identifiers_for_ambiguity(query.order_by, aliased_fields=aliased_fields)
 
+        # check predictor
         predictor = None
-        if isinstance(join_left, Identifier) and isinstance(join_right, Identifier):
-            if self.is_predictor(join_left) and self.is_predictor(join_right):
-                raise PlanningException(f'Can\'t join two predictors {str(join_left.parts[0])} and {str(join_left.parts[1])}')
+        table = None
+        predictor_namespace = None
+        predictor_is_left = False
+
+        if not (isinstance(join_right, Identifier) and self.is_predictor(join_right)):
+            # predictor not in the right, swap
+            join_left, join_right = join_right, join_left
+            predictor_is_left = True
 
-            predictor_namespace = None
-            table = None
-            predictor_is_left = False
-            if self.is_predictor(join_left):
-                predictor_namespace, predictor = self.get_predictor_namespace_and_name_from_identifier(join_left)
-                predictor_is_left = True
-            else:
-                table = join_left
+        if isinstance(join_right, Identifier) and self.is_predictor(join_right):
+            # predictor is in the right now
 
-            if self.is_predictor(join_right):
+            if isinstance(join_left, Identifier) and self.is_predictor(join_left):
+                # left is predictor too
+
+                raise PlanningException(f'Can\'t join two predictors {str(join_left.parts[0])} and {str(join_left.parts[1])}')
+            elif isinstance(join_left, Identifier):
+                # the left is table
                 predictor_namespace, predictor = self.get_predictor_namespace_and_name_from_identifier(join_right)
-            else:
-                table = join_right
+
+                table = join_left
 
             last_step = None
             if predictor:
                 # One argument is a table, another is a predictor
                 # Apply mindsdb model to result of last dataframe fetch
                 # Then join results of applying mindsdb with table
 
@@ -1173,18 +1196,25 @@
             integration = from_table.integration.parts[0].lower()
             step = FetchDataframeStep(integration=integration, raw_query=from_table.query)
             last_step = self.plan.add_step(step)
             sup_select = self.sub_select_step(query, step)
             if sup_select is not None:
                 last_step = self.plan.add_step(sup_select)
             return last_step
+        elif isinstance(from_table, ast.Data):
+            step = DataStep(from_table.data)
+            last_step = self.plan.add_step(step)
+            sup_select = self.sub_select_step(query, step, add_absent_cols=True)
+            if sup_select is not None:
+                last_step = self.plan.add_step(sup_select)
+            return last_step
         else:
             raise PlanningException(f'Unsupported from_table {type(from_table)}')
 
-    def sub_select_step(self, query, prev_step):
+    def sub_select_step(self, query, prev_step, add_absent_cols=False):
         if (
             query.group_by is not None
             or query.order_by is not None
             or query.having is not None
             or query.distinct is True
             or query.where is not None
             or query.limit is not None
@@ -1195,15 +1225,15 @@
             if query.from_table.alias is not None:
                 table_name = query.from_table.alias.parts[-1]
             else:
                 table_name = None
 
             query2 = copy.deepcopy(query)
             query2.from_table = None
-            return SubSelectStep(query2, prev_step.result, table_name=table_name)
+            return SubSelectStep(query2, prev_step.result, table_name=table_name, add_absent_cols=add_absent_cols)
 
     def plan_union(self, query):
         query1 = self.plan_select(query.left)
         query2 = self.plan_select(query.right)
 
         return self.plan.add_step(UnionStep(left=query1.result, right=query2.result, unique=query.unique))
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,13 +240,20 @@
         """Fills table with content of dataframe"""
         super().__init__(*args, **kwargs)
         self.table = table
         self.where = where
 
 
 class SubSelectStep(PlanStep):
-    def __init__(self, query, dataframe, table_name=None, *args, **kwargs):
+    def __init__(self, query, dataframe, table_name=None, add_absent_cols=False, *args, **kwargs):
         """Performs select from dataframe"""
         super().__init__(*args, **kwargs)
         self.query = query
         self.dataframe = dataframe
-        self.table_name = table_name
+        self.table_name = table_name
+        self.add_absent_cols = add_absent_cols
+
+
+class DataStep(PlanStep):
+    def __init__(self, data,  *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.data = data
```

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.6.6/mindsdb_sql/planner/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.6/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.5/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.6.6/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.6.5
+Version: 0.6.6
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.5/setup.py` & `mindsdb_sql-0.6.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     version=about['__version__'],
     url=about['__github__'],
     download_url=about['__pypi__'],
     license=about['__license__'],
     author=about['__author__'],
     author_email=about['__email__'],
     description=about['__description__'],
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=('tests*',)),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
```

