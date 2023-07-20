# Comparing `tmp/h2o_engine_manager-0.4.0.tar.gz` & `tmp/h2o_engine_manager-0.5.0.tar.gz`

## Comparing `h2o_engine_manager-0.4.0.tar` & `h2o_engine_manager-0.5.0.tar`

### file list

```diff
@@ -1,272 +1,273 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/Makefile
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/requirements.txt
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/docs/templates/config.mako
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/docs/templates/text.mako
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/local/ambassador_host.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/local/example.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/.openapi-generator-ignore
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/__init__.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/connection_config.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/exception.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_cli_config.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/login.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/duration_convertor.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/client_info.py
--rw-r--r--   0        0        0    21286 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
--rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/expression.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/client.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/dai_version.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/mapper.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/__init__.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/client.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/engine.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/mapper.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/page.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/state.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/token_api_client.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine_id/__init__.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine_id/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/__init__.py
--rw-r--r--   0        0        0    18472 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py
--rw-r--r--   0        0        0    12575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/page.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/state.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/client.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/mapper.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/page.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
--rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
--rw-r--r--   0        0        0    65707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
--rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
--rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
--rw-r--r--   0        0        0    21803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
--rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
--rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
--rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
--rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py
--rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
--rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
--rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/__init__.py
--rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api_client.py
--rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/configuration.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/exceptions.py
--rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model_utils.py
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/rest.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api/__init__.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/__init__.py
--rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    20396 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
--rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
--rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
--rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
--rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
--rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
--rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
--rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
--rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
--rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
--rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
--rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
--rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
--rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
--rw-r--r--   0        0        0    20349 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
--rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
--rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
--rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
--rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
--rw-r--r--   0        0        0    13036 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/setup.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_admission_webhook.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/create_dai_request.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_create.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_delete.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_get.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list_versions.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai/test_upgrade_available.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/engine/test_list_engines.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_create_h2o_engine.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_delete_h2o_engine.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_get_h2o_engine.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_engines.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_versions.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_connect.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_current_idle_running_duration.py
--rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_resume.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_lifecycle.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_login_discovery.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migrate_creator.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migration.py
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_update.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_upgrade_version.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_logs.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-connect.yaml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-setup.yaml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/system.default.yaml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_4.yaml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_5_mock.yaml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6.yaml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6_1.yaml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/system.default.yaml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/0_0_0_0_latest.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_38_0_4.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_versions/3_40_0_4.yaml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/sw_pods_creation/no_labels.yaml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_dai_engine.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_duration_convertor.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_engine_id_generator.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_engine_state.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_filter.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_h2o_cli_config.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_quantity_convertor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/dai_version/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/dai_version/test_mapper.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/tests/unit/test_data/h2o-cli-config.toml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/README.md
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/Makefile
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/docs/templates/config.mako
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/docs/templates/text.mako
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/local/ambassador_host.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/local/example.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/.openapi-generator-ignore
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/__init__.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/connection_config.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/exception.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_cli_config.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/login.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/duration_convertor.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/client_info.py
+-rw-r--r--   0        0        0    21489 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py
+-rw-r--r--   0        0        0    19872 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/expression.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/client.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/dai_version.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/mapper.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/__init__.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/client.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/engine.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/mapper.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/page.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/state.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/token_api_client.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/__init__.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/__init__.py
+-rw-r--r--   0        0        0    18472 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py
+-rw-r--r--   0        0        0    12778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/page.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/state.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/client.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/h2o_version.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/mapper.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/page.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39546 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    13685 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py
+-rw-r--r--   0        0        0    39350 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    65707 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    21561 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py
+-rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py
+-rw-r--r--   0        0        0    11879 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py
+-rw-r--r--   0        0        0    21803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py
+-rw-r--r--   0        0        0    14589 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py
+-rw-r--r--   0        0        0    11802 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py
+-rw-r--r--   0        0        0    12669 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py
+-rw-r--r--   0        0        0    11808 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py
+-rw-r--r--   0        0        0    39360 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py
+-rw-r--r--   0        0        0    12692 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/__init__.py
+-rw-r--r--   0        0        0    39287 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api_client.py
+-rw-r--r--   0        0        0    16312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/configuration.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/exceptions.py
+-rw-r--r--   0        0        0    82571 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model_utils.py
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/rest.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/__init__.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/__init__.py
+-rw-r--r--   0        0        0    14174 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    20794 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py
+-rw-r--r--   0        0        0    12642 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py
+-rw-r--r--   0        0        0    39550 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py
+-rw-r--r--   0        0        0    16369 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py
+-rw-r--r--   0        0        0    82609 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/__init__.py
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/__init__.py
+-rw-r--r--   0        0        0    14231 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py
+-rw-r--r--   0        0        0    12365 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py
+-rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py
+-rw-r--r--   0        0        0    39354 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py
+-rw-r--r--   0        0        0    16324 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py
+-rw-r--r--   0        0        0    82579 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/__init__.py
+-rw-r--r--   0        0        0    34374 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11812 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py
+-rw-r--r--   0        0        0    20349 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py
+-rw-r--r--   0        0        0    39364 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py
+-rw-r--r--   0        0        0    82581 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/__init__.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/__init__.py
+-rw-r--r--   0        0        0    14189 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py
+-rw-r--r--   0        0        0    13373 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/setup.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_admission_webhook.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/create_dai_request.py
+-rw-r--r--   0        0        0     6903 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_create.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_delete.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_get.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list_versions.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai/test_upgrade_available.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/engine/test_list_engines.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_create_h2o_engine.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_delete_h2o_engine.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_get_h2o_engine.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_engines.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_versions.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_connect.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_current_idle_running_duration.py
+-rw-r--r--   0        0        0    11667 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_resume.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_lifecycle.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_login_discovery.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migrate_creator.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migration.py
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_update.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_upgrade_version.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_logs.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-connect.yaml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-setup.yaml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/system.default.yaml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_3.yaml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_4.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5_do_not_use_me.yaml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_5_mock.yaml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6.yaml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6_1.yaml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/dai_versions/1_10_6_1_aplha.yaml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/list-generic-engines.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/system.default.yaml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/0_0_0_0.yaml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/0_0_0_0_latest.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_36_1_5.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_38_0_4.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_versions/3_40_0_4.yaml
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-cpu-constraint.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-gpu-constraint.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_setups/invalid-max-idle-duration-constraint.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/alias_and_version_conflict.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/invalid_version_format.yaml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/repeated_alias.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/invalid_dai_versions/unsupported_version.yaml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/sw_pods_creation/no_labels.yaml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/integration/test_data/sw_pods_creation/unwanted_label.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_dai_engine.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_duration_convertor.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_engine_id_generator.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_engine_state.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_filter.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_h2o_cli_config.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_quantity_convertor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/dai_version/__init__.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/dai_version/test_mapper.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/tests/unit/test_data/h2o-cli-config.toml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/README.md
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 h2o_engine_manager-0.5.0/PKG-INFO
```

### Comparing `h2o_engine_manager-0.4.0/requirements.txt` & `h2o_engine_manager-0.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/docs/templates/config.mako` & `h2o_engine_manager-0.5.0/docs/templates/config.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/docs/templates/text.mako` & `h2o_engine_manager-0.5.0/docs/templates/text.mako`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/local/example.py` & `h2o_engine_manager-0.5.0/local/example.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/connection_config.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/connection_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/exception.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/exception.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_cli_config.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_cli_config.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/login.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/login.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/duration_convertor.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/duration_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/convert/quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/client_info.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,19 @@
                 https://requests.readthedocs.io/en/master/user/advanced/#ssl-cert-verification. Defaults to True.
             backend_version_override (Optional[str], optional): version of client backend to use, overrides
                 Driverless AI server version detection. Specify ``"latest"`` to get
                 the most recent backend supported. In most cases the user should
                 rely on Driverless AI server version detection and leave this as
                 the default. Defaults to None.
         """
+        if self.state is not DAIEngineState.STATE_RUNNING:
+            raise RuntimeError(
+                f"DAIEngine {self.name} in not in a running state. Current state: {self.state}."
+            )
+
         # In 1.10.3 version (and prior), the connect function called after the launch (or resume), might fail
         # due to a faulty health check on the DAI server. Client initialization is retried with a 1s delay if it fails.
         max_att = 5
         for i in range(max_att):
             try:
                 return driverlessai.Client(
                     address=self.api_url,
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/expression.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/expression.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/page.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/dai_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         update_time: datetime = None,
         delete_time: datetime = None,
         resume_time: datetime = None,
         login_url: str = "",
         annotations: Dict[str, str] = None,
         display_name: str = "",
         version: str = "",
+        deprecated_version: bool = False,
         cpu: int = 0,
         gpu: int = 0,
         memory_bytes: str = "",
         storage_bytes: str = "",
     ) -> None:
         self.name = name
         self.uid = uid
@@ -40,14 +41,15 @@
         self.update_time = update_time
         self.delete_time = delete_time
         self.resume_time = resume_time
         self.login_url = login_url
         self.annotations = annotations
         self.display_name = display_name
         self.version = version
+        self.deprecated_version = deprecated_version
         self.cpu = cpu
         self.gpu = gpu
         self.memory_bytes = memory_bytes
         self.storage_bytes = storage_bytes
 
     def __repr__(self) -> str:
         return pprint.pformat(self.__dict__)
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/mapper.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         update_time=api_engine.update_time,
         delete_time=api_engine.delete_time,
         resume_time=api_engine.resume_time,
         login_url=api_engine.login_url,
         annotations=api_engine.annotations,
         display_name=api_engine.display_name,
         version=api_engine.version,
+        deprecated_version=api_engine.deprecated_version,
         cpu=api_engine.cpu,
         gpu=api_engine.gpu,
         memory_bytes=quantity_convertor.number_str_to_quantity(api_engine.memory_bytes),
         storage_bytes=quantity_convertor.number_str_to_quantity(
             api_engine.storage_bytes
         ),
     )
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/page.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/engine_id/generator.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/engine_id/generator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/client_info.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/h2o_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,19 @@
             reconciling=self.reconciling,
             uid=self.uid,
         )
 
     def get_connection_config(self) -> H2OClusterConnectionConfig:
         """Returns configuration used for h2o.connect."""
 
+        if self.state is not H2OEngineState.STATE_RUNNING:
+            raise RuntimeError(
+                f"H2OEngine {self.name} in not in a running state. Current state: {self.state}."
+            )
+
         return H2OClusterConnectionConfig(
             https=True,
             verify_ssl_certificates=True,
             context_path=self.name,
             ip=urlparse(self.client_info.url).hostname,
             port=443,
         )
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/page.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_engine_constraint/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/mapper.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/mapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 
     Returns:
         mapped H2OVersion object
     """
     return H2OVersion(
         version=api_h2o_version.version,
         aliases=api_h2o_version.aliases,
+        deprecated=api_h2o_version.deprecated,
         annotations=api_h2o_version.annotations,
     )
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/page.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/page.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/clients/h2o_version/token_api_client.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/api/dai_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_dai_engine_constraint_set.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/model/v1_get_dai_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/api/dai_engine_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_resource.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_migrate_creator_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_pause_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_resume_dai_engine_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/dai_engine_service_upgrade_version_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_create_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_migrate_creator_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_service_upgrade_version_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_dai_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_delete_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_get_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_list_dai_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_pause_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_resume_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/model/v1_update_dai_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.dai_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.dai_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/api/dai_version_service_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             page_size (int): Maximum number of DAIVersions to return in a response. If unspecified (or set to 0), at most 50 DAIVersions will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListDAIVersionsResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, DAIVersions are ordered by their version name in descending order. This is equivalent to \"version desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: - version  The default sorting order is ascending. For example: \"version\" and \"version asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"version desc\".  Redundant space characters are insignificant.. [optional]
-            filter (str): Used to filter DAIVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases)  Examples: - `version > \"latest\" AND version >= \"1.10.3\"`. [optional]
+            filter (str): Used to filter DAIVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases) - deprecated  Examples: - `version > \"latest\" AND version >= \"1.10.3\"` - `deprecated = false`. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_dai_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,31 +79,34 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'version': (str,),  # noqa: E501
             'aliases': ([str],),  # noqa: E501
+            'deprecated': (bool,),  # noqa: E501
             'annotations': ({str: (str,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'version': 'version',  # noqa: E501
         'aliases': 'aliases',  # noqa: E501
+        'deprecated': 'deprecated',  # noqa: E501
         'annotations': 'annotations',  # noqa: E501
     }
 
     read_only_vars = {
         'version',  # noqa: E501
         'aliases',  # noqa: E501
+        'deprecated',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -138,14 +141,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             version (str): Unique identifier of Driverless AI version. For example \"1.10.1.2\".. [optional]  # noqa: E501
             aliases ([str]): Aliases for the specified Driverless AI version. For example {\"latest\", \"prerelease\"}.. [optional]  # noqa: E501
+            deprecated (bool): Indicates whether DAIVersion is deprecated.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the DAIVersion.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -226,14 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             version (str): Unique identifier of Driverless AI version. For example \"1.10.1.2\".. [optional]  # noqa: E501
             aliases ([str]): Aliases for the specified Driverless AI version. For example {\"latest\", \"prerelease\"}.. [optional]  # noqa: E501
+            deprecated (bool): Indicates whether DAIVersion is deprecated.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the DAIVersion.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/model/v1_list_dai_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/dai_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/api/engine_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         Args:
             parent (str): Workspace resource name. Format: workspaces/{workspace}
 
         Keyword Args:
             page_size (int): Maximum number of Engines to return in a response. If unspecified (or set to 0), at most 50 Engines will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListEnginesResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, Engines are ordered by their time of creation in descending order. This is equivalent to \"create_time desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: {name, version, cpu, gpu, memory_bytes, storage_bytes, creator, create_time, update_time, delete_time, resume_time, display_name, uid}  The default sorting order is ascending. For example: \"name\" and \"name asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"name desc\".  Redundant space characters are insignificant. For example these values are all equal: - \"  name, cpu     desc\" - \"name, cpu desc\" - \"name   , cpu desc   \". [optional]
-            filter (str): Used to filter Engines. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - name - engine_id - version (supporting version semantic comparison, does not support aliases) - state - cpu - gpu - memory_bytes - storage_bytes - creator - creator_display_name - create_time - update_time - delete_time - resume_time - reconciling - uid - display_name - max_idle_duration - max_running_duration - current_idle_duration - current_running_duration  Examples: - `cpu > 5` - `gpu < 3` - `cpu >= 5 AND gpu <= 3` - `cpu != 5 OR gpu == 3` - `NOT (cpu > 5 OR gpu < 3)` - `-(cpu > 5 OR gpu < 3)` - `NOT (cpu > 5 OR (gpu < 3))` - `(cpu > 5 OR gpu < 3) AND memory_bytes != 1000` - `(cpu > 5 OR gpu < 3) AND (NOT ((((memory_bytes = 1000)))))` - `state = STATE_RUNNING AND create_time > \"2012-04-21T11:30:00-04:00\"` - `version >= \"1.10.3\"` - `reconciling = true OR reconciling = false` - `engine_id = \"*e*\" OR display_name = \"*e*\"` (supporting prefix/suffix wildcard `*` for string fields equality comparison). [optional]
+            filter (str): Used to filter Engines. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - name - engine_id - version (supporting version semantic comparison, does not support aliases) - deprecated_version - state - cpu - gpu - memory_bytes - storage_bytes - creator - creator_display_name - create_time - update_time - delete_time - resume_time - reconciling - uid - display_name - max_idle_duration - max_running_duration - current_idle_duration - current_running_duration  Examples: - `cpu > 5` - `gpu < 3` - `cpu >= 5 AND gpu <= 3` - `cpu != 5 OR gpu == 3` - `NOT (cpu > 5 OR gpu < 3)` - `-(cpu > 5 OR gpu < 3)` - `NOT (cpu > 5 OR (gpu < 3))` - `(cpu > 5 OR gpu < 3) AND memory_bytes != 1000` - `(cpu > 5 OR gpu < 3) AND (NOT ((((memory_bytes = 1000)))))` - `state = STATE_RUNNING AND create_time > \"2012-04-21T11:30:00-04:00\"` - `version >= \"1.10.3\"` - `deprecated_version = false` - `reconciling = true OR reconciling = false` - `engine_id = \"*e*\" OR display_name = \"*e*\"` (supporting prefix/suffix wildcard `*` for string fields equality comparison). [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             'delete_time': (datetime, none_type,),  # noqa: E501
             'update_time': (datetime, none_type,),  # noqa: E501
             'resume_time': (datetime, none_type,),  # noqa: E501
             'login_url': (str,),  # noqa: E501
             'annotations': ({str: (str,)},),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'version': (str,),  # noqa: E501
+            'deprecated_version': (bool,),  # noqa: E501
             'cpu': (int,),  # noqa: E501
             'gpu': (int,),  # noqa: E501
             'memory_bytes': (str,),  # noqa: E501
             'storage_bytes': (str,),  # noqa: E501
             'upgrade_available': (bool,),  # noqa: E501
             'max_idle_duration': (str, none_type,),  # noqa: E501
             'max_running_duration': (str, none_type,),  # noqa: E501
@@ -132,14 +133,15 @@
         'delete_time': 'deleteTime',  # noqa: E501
         'update_time': 'updateTime',  # noqa: E501
         'resume_time': 'resumeTime',  # noqa: E501
         'login_url': 'loginUrl',  # noqa: E501
         'annotations': 'annotations',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'version': 'version',  # noqa: E501
+        'deprecated_version': 'deprecatedVersion',  # noqa: E501
         'cpu': 'cpu',  # noqa: E501
         'gpu': 'gpu',  # noqa: E501
         'memory_bytes': 'memoryBytes',  # noqa: E501
         'storage_bytes': 'storageBytes',  # noqa: E501
         'upgrade_available': 'upgradeAvailable',  # noqa: E501
         'max_idle_duration': 'maxIdleDuration',  # noqa: E501
         'max_running_duration': 'maxRunningDuration',  # noqa: E501
@@ -157,14 +159,15 @@
         'delete_time',  # noqa: E501
         'update_time',  # noqa: E501
         'resume_time',  # noqa: E501
         'login_url',  # noqa: E501
         'annotations',  # noqa: E501
         'display_name',  # noqa: E501
         'version',  # noqa: E501
+        'deprecated_version',  # noqa: E501
         'cpu',  # noqa: E501
         'gpu',  # noqa: E501
         'memory_bytes',  # noqa: E501
         'storage_bytes',  # noqa: E501
         'upgrade_available',  # noqa: E501
         'max_idle_duration',  # noqa: E501
         'max_running_duration',  # noqa: E501
@@ -221,14 +224,15 @@
             delete_time (datetime, none_type): Time when the Engine was deleted.. [optional]  # noqa: E501
             update_time (datetime, none_type): Time when the Engine was last updated.. [optional]  # noqa: E501
             resume_time (datetime, none_type): Time when the Engine was last resumed (or started for the first time).. [optional]  # noqa: E501
             login_url (str): The URL address to initiate login flow.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the Engine. Annotations are key/value pairs.. [optional]  # noqa: E501
             display_name (str): Human-readable name of the Engine. Contains at most 63 characters and is not unique.. [optional]  # noqa: E501
             version (str): Engine version identifier. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
+            deprecated_version (bool): Indicates, whether the used version is deprecated.. [optional]  # noqa: E501
             cpu (int): The amount of CPU units in total requested by this Engine.. [optional]  # noqa: E501
             gpu (int): The amount of GPU units in total requested by this Engine.. [optional]  # noqa: E501
             memory_bytes (str): The amount of memory in bytes requested by this Engine.. [optional]  # noqa: E501
             storage_bytes (str): The amount of storage in bytes requested by this Engine.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
             max_idle_duration (str, none_type): Maximum time the engine can be idle.. [optional]  # noqa: E501
             max_running_duration (str, none_type): Maximum time the engine can be running.. [optional]  # noqa: E501
@@ -330,14 +334,15 @@
             delete_time (datetime, none_type): Time when the Engine was deleted.. [optional]  # noqa: E501
             update_time (datetime, none_type): Time when the Engine was last updated.. [optional]  # noqa: E501
             resume_time (datetime, none_type): Time when the Engine was last resumed (or started for the first time).. [optional]  # noqa: E501
             login_url (str): The URL address to initiate login flow.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the Engine. Annotations are key/value pairs.. [optional]  # noqa: E501
             display_name (str): Human-readable name of the Engine. Contains at most 63 characters and is not unique.. [optional]  # noqa: E501
             version (str): Engine version identifier. For example: \"1.10.1\" or \"latest\".. [optional]  # noqa: E501
+            deprecated_version (bool): Indicates, whether the used version is deprecated.. [optional]  # noqa: E501
             cpu (int): The amount of CPU units in total requested by this Engine.. [optional]  # noqa: E501
             gpu (int): The amount of GPU units in total requested by this Engine.. [optional]  # noqa: E501
             memory_bytes (str): The amount of memory in bytes requested by this Engine.. [optional]  # noqa: E501
             storage_bytes (str): The amount of storage in bytes requested by this Engine.. [optional]  # noqa: E501
             upgrade_available (bool): Indicates, whether the used version can be upgraded to a later one.. [optional]  # noqa: E501
             max_idle_duration (str, none_type): Maximum time the engine can be idle.. [optional]  # noqa: E501
             max_running_duration (str, none_type): Maximum time the engine can be running.. [optional]  # noqa: E501
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_engine_type.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/model/v1_list_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_constraint_set_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/api/h2_o_engine_constraint_set_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_constraint_numeric.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_get_h2_o_engine_constraint_set_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/model/v1_h2_o_engine_constraint_set.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_constraint_set_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_engine_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_engine_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/api/h2_o_engine_service_api.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/api_http_body.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_create_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_delete_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_get_h2_o_engine_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_service_download_logs_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_h2_o_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/model/v1_list_h2_o_engines_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_engine_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: version not set
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # import ApiClient
 from h2o_engine_manager.gen.h2o_version_service.api_client import ApiClient
 
 # import Configuration
 from h2o_engine_manager.gen.h2o_version_service.configuration import Configuration
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.5.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: version not set\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model_utils.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/rest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/api/h2_o_version_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         >>> result = thread.get()
 
 
         Keyword Args:
             page_size (int): Maximum number of H2OVersions to return in a response. If unspecified (or set to 0), at most 50 H2OVersions will be returned. The maximum value is 1000; values above 1000 will be coerced to 1000.. [optional]
             page_token (str): Leave unset to receive the initial page. To list any subsequent pages use the value of 'next_page_token' returned from the ListH2OVersionsResponse.. [optional]
             order_by (str): Used to specify the sorting order.  When unset, H2OVersions are ordered by their version name in descending order. This is equivalent to \"version desc\".  When specified, the value must be a comma separated list of supported fields. The supported fields are: - version  The default sorting order is ascending. For example: \"version\" and \"version asc\" are equivalent values.  To specify descending order for a field, append a \" desc\" suffix. For example: \"version desc\".  Redundant space characters are insignificant.. [optional]
-            filter (str): Used to filter H2OVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases)  Examples: - `version > \"latest\" AND version >= \"3.38.0.1\"`. [optional]
+            filter (str): Used to filter H2OVersions. When unset, no filtering is applied.  Filtering implements specification https://google.aip.dev/160.  Supported filter fields: - version (supporting version semantic comparison and version aliases) - deprecated  Examples: - `version > \"latest\" AND version >= \"3.38.0.1\"` - `deprecated = false`. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_h2_o_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,31 +79,34 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'version': (str,),  # noqa: E501
             'aliases': ([str],),  # noqa: E501
+            'deprecated': (bool,),  # noqa: E501
             'annotations': ({str: (str,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'version': 'version',  # noqa: E501
         'aliases': 'aliases',  # noqa: E501
+        'deprecated': 'deprecated',  # noqa: E501
         'annotations': 'annotations',  # noqa: E501
     }
 
     read_only_vars = {
         'version',  # noqa: E501
         'aliases',  # noqa: E501
+        'deprecated',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
@@ -138,14 +141,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             version (str): Unique identifier of H2O version. For example \"3.38.0.1\".. [optional]  # noqa: E501
             aliases ([str]): Aliases for the specified H2O version. For example {\"latest\", \"prerelease\"}.. [optional]  # noqa: E501
+            deprecated (bool): Indicates whether H2OVersion is deprecated.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the H2OVersion.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -226,14 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             version (str): Unique identifier of H2O version. For example \"3.38.0.1\".. [optional]  # noqa: E501
             aliases ([str]): Aliases for the specified H2O version. For example {\"latest\", \"prerelease\"}.. [optional]  # noqa: E501
+            deprecated (bool): Indicates whether H2OVersion is deprecated.. [optional]  # noqa: E501
             annotations ({str: (str,)}): Additional arbitrary metadata associated with the H2OVersion.  Annotations are key/value pairs. The key must: - be 63 characters or less - begin and end with an alphanumeric character ([a-z0-9A-Z]) - with dashes (-), underscores (_), dots (.), and alphanumerics between - regex used for validation is: ^[A-Za-z0-9]([-A-Za-z0-9_.]{0,61}[A-Za-z0-9])?$. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/model/v1_list_h2_o_versions_response.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py` & `h2o_engine_manager-0.5.0/src/h2o_engine_manager/gen/h2o_version_service/models/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/conftest.py` & `h2o_engine_manager-0.5.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/setup.py` & `h2o_engine_manager-0.5.0/tests/integration/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,9 +140,9 @@
 system_namespace = os.getenv("TEST_K8S_SYSTEM_NAMESPACE")
 create_dai_versions(namespace=system_namespace)
 create_h2o_versions(namespace=system_namespace)
 create_dai_setups(namespace=system_namespace)
 create_h2o_setups(namespace=system_namespace)
 create_dai_license(namespace=system_namespace)
 
-if os.getenv("HAIC_CLUSTER") == "true":
+if os.getenv("MLOPS_CLUSTER") == "true":
     setup_mlops_secrets(namespace=system_namespace)
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_admission_webhook.py` & `h2o_engine_manager-0.5.0/tests/integration/test_admission_webhook.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/create_dai_request.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/create_dai_request.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_create.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,19 @@
 
 
 def incorrect_version(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
     req.version = "non-existing-version"
     return req
 
 
+def deprecated_version(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
+    req.version = "1.10.3"
+    return req
+
+
 def incorrect_config(req: CreateDAIEngineRequest) -> CreateDAIEngineRequest:
     req.config = {"base_url": "whatever"}
     return req
 
 
 def test_create_dai(dai_client):
     # When
@@ -123,14 +128,15 @@
         incorrect_workspace_id,
         incorrect_engine_id,
         cpu_below_min,
         gpu_below_min,
         memory_below_min,
         incorrect_display_name,
         incorrect_version,
+        deprecated_version,
         incorrect_config,
     ],
 )
 def test_create_dai_server_validation(dai_client, modify_func):
     # When
     req = modify_func(CreateDAIEngineRequest(workspace_id="create-dai-validation"))
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_delete.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_delete.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_get.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_get.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_list_versions.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_list_versions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from h2o_engine_manager.clients.dai_version.dai_version import DAIVersion
 from h2o_engine_manager.clients.exception import ApiException
 
 
 def test_list_all_dai_version(dai_client):
     # Arrange - DAIVersion CRDs are already present in the cluster.
     expected = [
-        DAIVersion(version="1.10.6.1", aliases=["latest"], annotations={}),
-        DAIVersion(version="1.10.6.1-alpha", aliases=[], annotations={}),
-        DAIVersion(version="1.10.6", aliases=[], annotations={}),
-        DAIVersion(version="1.10.5", aliases=[], annotations={}),
-        DAIVersion(version="1.10.5-mock", aliases=["mock", "alias-foo"], annotations={}),
-        DAIVersion(version="1.10.5-do-not-use-me", aliases=[], annotations={}),
-        DAIVersion(version="1.10.4", aliases=[], annotations={"foo": "foo"}),
+        DAIVersion(version="1.10.6.1", aliases=["latest"], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.6.1-alpha", aliases=[], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.6", aliases=[], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.5", aliases=[], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.5-mock", aliases=["mock", "alias-foo"], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.5-do-not-use-me", aliases=[], deprecated=False, annotations={}),
+        DAIVersion(version="1.10.4", aliases=[], deprecated=False, annotations={"foo": "foo"}),
+        DAIVersion(version="1.10.3", aliases=[], deprecated=True, annotations={}),
     ]
 
     # When
     dai_versions = dai_client.list_all_versions()
 
     # Then
     for i in range(0, len(expected)):
@@ -29,26 +30,26 @@
 def test_paging_dai_versions(dai_client):
     # Arrange - DAIVersion CRDs are already present in the cluster.
 
     # When - list first page.
     first_page = dai_client.list_versions(page_size=1)
 
     # Then
-    assert first_page.total_size == 7
+    assert first_page.total_size == 8
     assert len(first_page.dai_versions) == 1
     assert first_page.next_page_token != ""
 
     # When - list second (last) page.
     second_page = dai_client.list_versions(
-        page_size=6, page_token=first_page.next_page_token
+        page_size=7, page_token=first_page.next_page_token
     )
 
     # Then
-    assert second_page.total_size == 7
-    assert len(second_page.dai_versions) == 6
+    assert second_page.total_size == 8
+    assert len(second_page.dai_versions) == 7
     assert second_page.next_page_token == ""
     assert first_page.dai_versions[0].version != second_page.dai_versions[0].version
 
 
 def test_incorrect_page_token(dai_client):
     with pytest.raises(ApiException) as exc:
         dai_client.list_versions(page_token="non-existing-token")
@@ -63,15 +64,15 @@
 
 
 def test_page_size(dai_client):
     # When - request page size greater than total number of items.
     page = dai_client.list_versions(page_size=10000)
 
     # Then
-    assert page.total_size == 7
+    assert page.total_size == 8
 
 
 def test_filter(dai_client):
     # When supported filter expression (alias values are supported).
     vs = dai_client.list_versions(filter="version < \"latest\" AND version > \"1.10.6\"")
 
     # Then only one DAIVersion conforms to the filter expression
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai/test_upgrade_available.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai/test_upgrade_available.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py` & `h2o_engine_manager-0.5.0/tests/integration/api/dai_engine_constraint/test_get_dai_engine_constraint.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/engine/test_list_engines.py` & `h2o_engine_manager-0.5.0/tests/integration/api/engine/test_list_engines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import subprocess
 import time
 
 from h2o_engine_manager.clients.engine.state import EngineState
 from h2o_engine_manager.clients.engine.type import EngineType
 from tests.integration.api.dai.create_dai_request import CreateDAIEngineRequest
 from tests.integration.api.dai.create_dai_request import create_dai_from_request
 from tests.integration.conftest import CACHE_SYNC_SECONDS
@@ -40,14 +41,41 @@
         annotations={"e3": "v3"},
     )
     requests = [req1, req2, req3]
 
     for req in requests:
         create_dai_from_request(dai_client, req)
 
+    # We cannot create engine with deprecated version.
+    # Workaround: manually set daiEngine1's and daiEngine3's version 1.10.4 to a deprecated version 1.10.3.
+    # (overwriting annotation in the CRD object)
+    subprocess.run(
+        [
+            "kubectl",
+            "annotate",
+            "--overwrite",
+            f"--namespace={os.getenv('TEST_K8S_WORKLOADS_NAMESPACE')}",
+            "dai",
+            f"{workspace_id}.engine1",
+            "engine.h2o.ai/version=1.10.3"
+        ]
+    )
+    subprocess.run(
+        [
+            "kubectl",
+            "annotate",
+            "--overwrite",
+            f"--namespace={os.getenv('TEST_K8S_WORKLOADS_NAMESPACE')}",
+            "dai",
+            f"{workspace_id}.engine3",
+            "engine.h2o.ai/version=1.10.3"
+        ]
+    )
+
+
     h2o_engine_client.create_engine(
         workspace_id=workspace_id,
         engine_id="engine1",
         version="3.36.1.5",
         node_count=1,
         cpu=2,
         gpu=0,
@@ -157,27 +185,48 @@
     )
 
     # Then
     assert len(page.engines) == 0
     assert page.total_size == 0
     assert page.next_page_token == ""
 
+    # When filter engines with deprecated version
+    page = engine_client.list_engines(
+        workspace_id=workspace_id,
+        filter_expr="deprecated_version = true",
+    )
+
+    # Then
+    assert len(page.engines) == 2
+    assert page.total_size == 2
+    assert page.next_page_token == ""
+
+    # Newly created engine is listed first.
+    assert page.engines[0].name == f"workspaces/{workspace_id}/daiEngines/engine3"
+    assert page.engines[0].version == "1.10.3"
+    assert page.engines[0].deprecated_version is True
+
+    assert page.engines[1].name == f"workspaces/{workspace_id}/daiEngines/engine1"
+    assert page.engines[1].version == "1.10.3"
+    assert page.engines[1].deprecated_version is True
+
     # When filter
     expr = "type = TYPE_DRIVERLESS_AI AND version < \"1.10.5\" AND memory_bytes > 1024"
     page = engine_client.list_engines(workspace_id=workspace_id, filter_expr=expr)
 
     # Then
     assert len(page.engines) == 1
     assert page.total_size == 1
     assert page.next_page_token == ""
     assert page.engines[0].name == f"workspaces/{workspace_id}/daiEngines/engine1"
 
     # Extra check for correct mapping (Since we don't have GetEngine endpoint)
     eng = page.engines[0]
-    assert eng.version == "1.10.4"
+    assert eng.version == "1.10.3"
+    assert eng.deprecated_version is True
     assert eng.engine_type == EngineType.TYPE_DRIVERLESS_AI
     assert eng.cpu == 1
     assert eng.gpu == 0
     assert eng.create_time is not None
     assert eng.update_time is None
     assert eng.delete_time is None
     assert eng.annotations["e1"] == "v1"
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_create_h2o_engine.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_create_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_delete_h2o_engine.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_delete_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_get_h2o_engine.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_get_h2o_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_engines.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_engines.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o/test_list_h2o_versions.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o/test_list_h2o_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from h2o_engine_manager.clients.exception import ApiException
 from h2o_engine_manager.clients.h2o_version.h2o_version import H2OVersion
 
 
 def test_list_all_h2o_version(h2o_engine_client):
     expected = [
-        H2OVersion(version="3.40.0.3", aliases=["smoker"], annotations={}),
-        H2OVersion(version="3.38.0.4", aliases=[], annotations={}),
-        H2OVersion(version="3.36.1.5", aliases=[], annotations={"bar": "baz"}),
-        H2OVersion(version="0.0.0.0", aliases=["mock"], annotations={}),
-        H2OVersion(version="0.0.0.0-latest", aliases=["latest"], annotations={}),
+        H2OVersion(version="3.40.0.3", aliases=["smoker"], deprecated=False, annotations={}),
+        H2OVersion(version="3.38.0.4", aliases=[], deprecated=False, annotations={}),
+        H2OVersion(version="3.36.1.5", aliases=[], deprecated=False, annotations={"bar": "baz"}),
+        H2OVersion(version="0.0.0.0", aliases=["mock"], deprecated=False, annotations={}),
+        H2OVersion(version="0.0.0.0-latest", aliases=["latest"], deprecated=False, annotations={}),
     ]
 
     # When
     h2o_versions = h2o_engine_client.list_all_versions()
 
     # Then
     for i in range(0, len(expected)):
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py` & `h2o_engine_manager-0.5.0/tests/integration/api/h2o_engine_constraint/test_get_h2o_engine_constraint.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_connect.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import pytest
 import websocket
 
 from h2o_engine_manager.clients.dai_engine.dai_engine_state import DAIEngineState
 from tests.integration.conftest import DAI_CONNECT_WORKSPACE
 from tests.integration.conftest import NON_MOCKED_DAI_VERSION
 
@@ -27,29 +29,33 @@
         memory_bytes="8Gi",
         storage_bytes="16Gi",
         max_idle_duration="15m",
         max_running_duration="2d",
         display_name="My engine 1",
     )
     try:
+        #  Unable to connect before the engine is running.
+        with pytest.raises(RuntimeError):
+            engine.connect()
+
         # Wait for RUNNING
         engine.wait()
         assert engine.state.name == DAIEngineState.STATE_RUNNING.name
 
         # Test Connect to DAI.
         dai = engine.connect()
 
-        # Validate MLOps integration.
+        # Validate MLOps integration only if deployed with MLOps.
         # dai.projects.get() method itself does not verify existence,
         # we need to check another field for an existing record.
-        # TODO if it starts failing due to MLOps instance instability, remove the test
-        assert (
-            dai.projects.get("468557ab-bfab-4ac7-b409-046491965fde").name
-            == "aiem-mlops-test"
-        )
+        if os.getenv("MLOPS_CLUSTER") == "true":
+            assert (
+                dai.projects.get("468557ab-bfab-4ac7-b409-046491965fde").name
+                == "aiem-mlops-test"
+            )
     finally:
         dai_client.client_info.api_instance.d_ai_engine_service_delete_dai_engine(
             name=f"workspaces/{workspace_id}/daiEngines/{engine_id}", allow_missing=True
         )
 
 
 @pytest.mark.timeout(200)
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_current_idle_running_duration.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_current_idle_running_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_dai_resume.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_dai_resume.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_lifecycle.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_login_discovery.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_login_discovery.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migrate_creator.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migrate_creator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_migration.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_migration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_update.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_update.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/dai/test_upgrade_version.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/dai/test_upgrade_version.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_current_idle_running_duration.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_engine_lifecycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         annotations={"Lela": "Lulu"},
     )
     deleted = False
 
     try:
         assert e.state.name == H2OEngineState.STATE_STARTING.name
 
+        # Unable to get the connection config before the engine is running.
+        with pytest.raises(RuntimeError):
+            e.get_connection_config()
+
         e.wait()
         assert e.state.name == H2OEngineState.STATE_RUNNING.name
 
         h2o.connect(config=e.get_connection_config())
 
         df = h2o.import_file(path="https://s3.amazonaws.com/h2o-public-test-data/smalldata/gbm_test/ecology_model.csv")
```

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_logs.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_logs.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py` & `h2o_engine_manager-0.5.0/tests/integration/e2e/h2o/test_h2o_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-connect.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-connect.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-lifecycle.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-mocked-server-logs.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/dai-setup.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/dai-setup.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/existing-dai-engine-constraint-set.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/dai_setups/system.default.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/dai_setups/system.default.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/existing-h2o-engine-constraint-set.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/h2o-setup.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/integration/test_data/h2o_setups/system.default.yaml` & `h2o_engine_manager-0.5.0/tests/integration/test_data/h2o_setups/system.default.yaml`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_dai_engine.py` & `h2o_engine_manager-0.5.0/tests/unit/test_dai_engine.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_duration_convertor.py` & `h2o_engine_manager-0.5.0/tests/unit/test_duration_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_engine_id_generator.py` & `h2o_engine_manager-0.5.0/tests/unit/test_engine_id_generator.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_engine_state.py` & `h2o_engine_manager-0.5.0/tests/unit/test_engine_state.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_filter.py` & `h2o_engine_manager-0.5.0/tests/unit/test_filter.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/test_quantity_convertor.py` & `h2o_engine_manager-0.5.0/tests/unit/test_quantity_convertor.py`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/tests/unit/dai_version/test_mapper.py` & `h2o_engine_manager-0.5.0/tests/unit/dai_version/test_mapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from h2o_engine_manager.clients.dai_version.mapper import api_to_custom
 from h2o_engine_manager.gen.dai_version_service.model.v1_dai_version import V1DAIVersion
 
 
 def test_api_to_custom():
     # Arrange
     api_object = V1DAIVersion._from_openapi_data(
-        version="1.10.0", aliases=["latest", "prerelease"], annotations={"key1": "val1"}
+        version="1.10.0", aliases=["latest", "prerelease"], deprecated=False, annotations={"key1": "val1"}
     )
     expected_custom = DAIVersion(
-        version="1.10.0", aliases=["latest", "prerelease"], annotations={"key1": "val1"}
+        version="1.10.0", aliases=["latest", "prerelease"], deprecated=False, annotations={"key1": "val1"}
     )
 
     # When
     custom = api_to_custom(api_object)
 
     # Then
     assert expected_custom.__dict__ == custom.__dict__
```

### Comparing `h2o_engine_manager-0.4.0/README.md` & `h2o_engine_manager-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `h2o_engine_manager-0.4.0/pyproject.toml` & `h2o_engine_manager-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,17 @@
 admission-webhook = "python -m pytest -s tests/integration/test_admission_webhook.py --noconftest"
 
 [tool.pytest.ini_options]
 timeout = 10
 
 [tool.hatch.envs.lint]
 detached = true
+python = "3.10"
 dependencies = [
-    "black>=23.1.0",
+    "black==23.1.0",
     "isort==5.12.0",
 ]
 
 [tool.hatch.envs.lint.scripts]
 # TODO use flake8 and mypy
 check = [
     "black --check --diff .",
@@ -78,14 +79,17 @@
 [tool.isort]
 skip = ["src/h2o_engine_manager/gen"]
 force_single_line = true
 known_application = ["h2o_engine_manager"]
 profile = "black"
 
 [tool.hatch.envs.docs]
+# pdoc3 generates different results for different python versions
+# use fixed python version for stable docs output
+python = "3.10"
 dependencies = [
     "pdoc3==0.10.0",
 ]
 
 [tool.hatch.envs.docs.scripts]
 generate = [
     "pdoc3 --force --template-dir docs/templates --output-dir ../../docs/docs/py src/h2o_engine_manager/clients"
```

### Comparing `h2o_engine_manager-0.4.0/PKG-INFO` & `h2o_engine_manager-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-engine-manager
-Version: 0.4.0
+Version: 0.5.0
 Summary: H2O Engine Manager python client
 Project-URL: Documentation, https://github.com/h2oai/ai-engine-manager#readme
 Project-URL: Issues, https://github.com/h2oai/ai-engine-manager/issues
 Project-URL: Source, https://github.com/h2oai/ai-engine-manager/py/h2o-engine-manager
 Author-email: Jan Sykora <jan.sykora@h2o.ai>, Tomas Pastorek <tomas.pastorek@h2o.ai>, Ondrej Bilek <ondrej.bilek@h2o.ai>
 Requires-Python: >=3.7
 Requires-Dist: certifi>=2022.12.7
```

