# Comparing `tmp/wiliot-deployment-tools-4.0.8.tar.gz` & `tmp/wiliot-deployment-tools-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.8.tar", last modified: Tue Jun 13 09:01:38 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.1.0.tar", last modified: Thu Jul 20 11:44:22 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.8.tar` & `wiliot-deployment-tools-4.1.0.tar`

### file list

```diff
@@ -1,73 +1,143 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.942140 wiliot-deployment-tools-4.0.8/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.946140 wiliot-deployment-tools-4.0.8/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.946140 wiliot-deployment-tools-4.0.8/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     8103 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7612 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45893 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/gw_ssid.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/s3_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15516 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7926 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26356 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     8103 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2281 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.678200 wiliot-deployment-tools-4.1.0/.deploy/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.678200 wiliot-deployment-tools-4.1.0/.deploy/aws/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.686200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/common.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.686200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.686200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.686200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.678200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.678200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/terragrunt.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.678200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.deploy/aws/infrastructure/test/us-east-2/region.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.682200 wiliot-deployment-tools-4.1.0/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.gitignore
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    11235 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10717 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    11458 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.690200 wiliot-deployment-tools-4.1.0/ci/
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/ci/upload_to_s3.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/gw_certificate.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.694200 wiliot-deployment-tools-4.1.0/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.694200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.698200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/ut_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/wlt_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    78971 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/wlt_types_ag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/wlt_types_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/ag/wlt_types_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.702200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50389 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/gw_ssid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/s3_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.702200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15516 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.702200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/calibration_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/calibration_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.706200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.706200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/connectivity_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/connectivity_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13327 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.706200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.706200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/gw_certificate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.710200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     7803 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.710200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14788 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.710200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/interface/uart_ports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.714200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-20 11:44:04.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 11:44:22.698200 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11235 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-20 11:44:22.000000 wiliot-deployment-tools-4.1.0/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.8/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.1.0/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.1.0/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/LICENSE` & `wiliot-deployment-tools-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/PKG-INFO` & `wiliot-deployment-tools-4.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: wiliot-deployment-tools
-Version: 4.0.8
-Summary: A library for interacting with Wiliot's Deployment Tools
-Home-page: 
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-deployment-tools #
 
 wiliot-deployment-tools is a python library for accessing Wiliot's Deployment and Automation Tools.
 This python package includes the following CLI utilities:
  - Automatic Configuration Tool (`wlt-config`)
- - Power Management Tool (`wlt-power-mgmt`)
  - Calibration Management Tool (`wlt-clibration-mgmt`)
  - Firmware Update Tool (`wlt-firmware`)
+ - Power Management Tool (`wlt-power-mgmt`)
  - Log Viewer (`wlt-log`)
-
+ - Connectivity Analyzer (`wlt-connectivity-analyzer`)
+ - Gateway Certificate (`wlt-gw-certificate`)
 
 ## Installing wiliot-deployment-tools
 ````commandline
 pip install wiliot-deployment-tools
 ````
 
 ## Using wiliot-deployment-tools
@@ -51,62 +36,65 @@
                         bridges to ignore in the tool - their configuration won't be changed
   -expected_num_brgs EXPECTED_NUM_BRGS
                         Number of expected bridges in location. The tool will try to connect to all bridges (excluding those specified in ignore bridges) until reaching expected number.
 
 example usage: wlt-config --owner wiliot --location "My Deployment" --ota_upgrade --pacing_interval 10 --ignore_bridges 1234ABCD0123
 ```
 
-### Firmware Update
-Update Wiliot Gateways and Bridges firmware version OTA.
- #### Print Available Versions 
- Prints all avaliable Firmware versions for update for every GW Type
-```
-usage: wlt-firmware -owner OWNER [-beta] versions
-
-optional arguments:
-  -beta              show available beta versions / update to beta firmware
-
-example usage: wlt-firmware -o wiliot versions
-```
 ### Calibration Management
-Configure Wiliot Bridge calibration mode
+Configure Wiliot Bridge calibration mode, broadcast is optional
 ```
 usage: wlt-calibration-mgmt -owner OwnerID -brg BridgeID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
+usage (broadcast): wlt-calibration-mgmt -owner OwnerID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
-  -brg BRG      Bridge ID
-  -gw GW        GW ID to configure bridge
+  -brg BRG      Bridge ID (required only for non broadcast)
+  -gw GW        GW ID to configure bridge (required only for broadcast)
   -mode Mode    CalibrationMode on of 3 options: 0-regular, 1-no ch37, 2-ch37 on data only
 
 optional arguments:
-
   -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
 
   example usage: wlt-calibration-mgmt -owner wiliot -brg 0123ABCD -gw AB1234CD -mode 1
 ```
 
+### Firmware Update
+Update Wiliot Gateways and Bridges firmware version OTA.
+ #### Print Available Versions 
+ Prints all avaliable Firmware versions for update for every GW Type
+```
+usage: wlt-firmware -owner OWNER [-beta] versions
+
+optional arguments:
+  -beta              show available beta versions / update to beta firmware
+
+example usage: wlt-firmware -o wiliot versions
+```
+
  #### Firmware Update
  Run OTA Process, first updating specified GWs to latest / specified FW version. Afterwards seuqentially update each specified Bridges / all Bridges to the same Firmware version.
  ```
 usage: wlt-firmware update -owner OWNER [-beta] [-version VERSION] [-gw GW [GW ...]] [-brg BRG [BRG ...]] [-all_brgs] [-ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]] [-action]
 
+
 optional arguments:
   -beta              show available beta versions / update to beta firmware
   -version VERSION      Desired version. if not specified, will update to latest available version
   -gw GW [GW ...]       Gateways to update (multiple allowed)
   -brg BRG [BRG ...]    Bridges to update (multiple allowed)
   -all_brgs             update all bridges connected to Gateways
   -ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]
                         bridges to ignore
   -action               update using action API
   -force                update bridge even if its already in desired version (applicable only with -action)
 
   example usage: wlt-firmware -o wiliot update -gw GW0123 -all_brgs
   ```
+
 ### Power Management
 Use Wiliot Bridge power management functionality
 #### Enter Power Management
 Configure Specified Bridges to work in power management configuration.
 ```
 usage: wlt-power-mgmt -o OwnerID enter -brg BridgeID -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
 
@@ -140,33 +128,109 @@
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
 example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
+  
 
 ### Log Viewer
 View Wiliot Gateway logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
 Log Viewer - CLI Tool to view Wiliot Gateway logs
 
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
 ```
 
+
+
+### Connectivety Analyzer
+Check the rssi connection between gws and bridge (as received at the bridge)
+Can operate by: location, bridges or gateways
+Return the bridges with low connection
+```
+usage: wlt-connectivity-analyzer -owner OWNER -location Location
+
+required arguments:
+  -owner OWNER  Owner ID
+
+
+optional arguments:
+  -gws GwsList         List of gateways IDs to check connection to the bridges they see
+  -brgs BridgesList    List of bridges IDs to check connection 
+  -location Location   Location name (as written in platform) to check all bridges in
+```
+
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
+### Gateway Certificate
+Test Wiliot GWs capabilities.
+The GW Certificate includes different test that run sequentially to test each capability reported by the GW.
+
+#### Coupling Test
+The test switched the GW to an external MQTT Broker and uses a BLE Simulator (Wiliot WIFI GW connected using UART) to simulate bridges and test the coupling capability of the tested GW (Couple together Data and SideInfo packets)
+The test inclued the following stages:
+- STAGES = [InitStage, OneBrgStage, ThreeBrgInitStage, ThreeBrgStage]
+- Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
+- One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
+- Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
+- Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
+The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
+
+#### Release Notes:
+Version 4.1.0:
+* Coupling Test
+* Add CSV Output
+* Calculate test run
+
+Version 4.0.13:
+* Initial Release (Alpha)
+
+```
+usage: wlt-gw-certificate [-h] -owner OWNER -gw GW [-test] [-random] [-legacy]
+
+Gateway Certificate - CLI Tool to test Wiliot GWs
+
+optional arguments:
+  -h, --help    show this help message and exit
+  -test         If flag used, use test environment (prod is used by default)
+  -random       randomize packets (if not used same packets will be sent for each run)
+  -legacy       use legacy DevMode
+
+required arguments:
+  -owner OWNER  Owner ID
+  -gw GW        Gateway ID
+  ```
+
 
 ## Release Notes:
+Version 4.1.0:
+* Custom message support
+* GW Certificate - coupling test
+* Fixes for calibration management
+
+Version 4.0.13:
+* Add Gateway Certificate (Alpha)
+
+Version 4.0.12:
+* Add new Connectivity Analyzer
+
+Version 4.0.11:
+* Add broadcast to calibration management
+* Bugfixes for power management using android GW
+
+Version 4.0.10:
+* Internal fixes
 
 Version 4.0.8:
 * Support for python 3.11
 * Added new calibration mgmt tool
 
 Version 4.0.7:
 * Android power management support
```

### Comparing `wiliot-deployment-tools-4.0.8/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.1.0/bitbucket-pipelines.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 image: &wiliot-ci-image
-  name: 142654642153.dkr.ecr.us-east-1.amazonaws.com/aws-ci:latest
+  name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.3-alpine
   aws:
-    access-key: $AWS_ACCESS_KEY_ID
-    secret-key: $AWS_SECRET_ACCESS_KEY
-
+    access-key: $CLOUD_AWS_ACCESS_KEY_ID
+    secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
 
 definitions:
   services:
     docker:
       memory: 3072
   step:
     - step: &build_unittests_image
@@ -18,14 +17,36 @@
           - aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 142654642153.dkr.ecr.us-east-1.amazonaws.com
           - docker build -t 142654642153.dkr.ecr.us-east-1.amazonaws.com/pywiliot:unittests_$BITBUCKET_BUILD_NUMBER . -f unittests.dockerfile
           - docker push 142654642153.dkr.ecr.us-east-1.amazonaws.com/pywiliot:unittests_$BITBUCKET_BUILD_NUMBER
         services:
           - docker
 
 pipelines:
+  branches:
+    develop:
+      - step:
+          name: Build and publish internal version into codeartifact
+          image:
+            name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
+            aws:
+              access-key: $CLOUD_AWS_ACCESS_KEY_ID
+              secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
+          script:
+            - pip3 install setuptools_scm build wheel twine
+            - pip3 install gitpython
+            # get updated version number:
+            - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
+            # build python package:
+            - python3 setup.py sdist bdist_wheel
+            # update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
+            - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
+            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
+            - twine upload --repository codeartifact dist/*
 
   custom:
     update-major-version-number:
       - step:
           name: update major version number
           <<: *wiliot-ci-image
           script:
@@ -65,112 +86,163 @@
             #print current version:
             - python3 wiliot_deployment_tools/utils/get_version.py
             #Update patch version by git tag:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py next_patch`" && echo $version && git tag -a -m "[skip ci] build number $BITBUCKET_BUILD_NUMBER set the library patch version to $version." $version  && git push origin $version
             #print new version
             - python3 wiliot_deployment_tools/utils/get_version.py
     
-    publish-full-version-into-old-codeartifact:
-      - step:
-          name: Build and publish internal version into codeartifact
-          <<: *wiliot-ci-image
-          script:
-            - pip3 install setuptools_scm build wheel twine
-            - pip3 install gitpython
-            # get updated version number:
-            - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
-            # build python package:
-            - python3 -m build -C internal
-            # update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
-            - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
-            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
-            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
-            - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
-            - twine upload --repository codeartifact dist/*
-
     publish-full-version-into-new-codeartifact:
       - step:
           name: Build and publish internal version into codeartifact
           image:
             name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
             aws:
               access-key: $CLOUD_AWS_ACCESS_KEY_ID
               secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
           script:
             - pip3 install setuptools_scm build wheel twine
             - pip3 install gitpython
             # get updated version number:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
             # build python package:
-            - python3 -m build -C internal
+            - python3 setup.py sdist bdist_wheel
             # update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
             - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
             - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
             - twine upload --repository codeartifact dist/*
 
     publish-slim-version-into-pypi:
       - step:
           name: Build and publish slim version into pypi
           <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm build
+            - pip3 install setuptools_scm build wheel twine
             - pip3 install gitpython
             - apk add tree
             #Get current version (was already updated by prev steps) before cleaning internal files:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
             #update version.py with new patch version and build number:
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
             # configure testpypi and pypi access
             - echo "[pypi]" > ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $PYPI_KEY" >> ~/.pypirc && echo "[testpypi]" >> ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $TEST_PYPI_KEY" >> ~/.pypirc
             # cleanup all the "internal" folders
             - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
             - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
-            - python3 -m build
+            - python3 setup.py sdist bdist_wheel
             #Logging(?):
-            - ls -al dist/
+            - ls -al dist/ && ls -al build/
             # push into pypi
             - python3 -m twine upload --repository pypi dist/* #python3 -m twine upload --repository testpypi dist/*
 
     publish-slim-version-into-test-pypi:
       - step:
           name: Build and publish slim version into test-pypi
           <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm build twine
+            - pip3 install setuptools_scm build wheel twine
             - pip3 install gitpython
             - apk add tree
             # configure testpypi and pypi access
             - echo "[testpypi]" >> ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $TEST_PYPI_KEY" >> ~/.pypirc
             # get updated version- before cleaning internal trees:
             - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
             #update version.py with new patch version and build number:
             - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
             #Print version to log:
             - cat wiliot_deployment_tools/version.py
             # cleanup all the "internal" folders
             - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
             - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
-            - python3 -m build
-            - ls -al dist/
+            - python3 setup.py sdist bdist_wheel
+            - ls -al dist/ && ls -al build/
             # push into test-pypi
             - python3 -m twine upload --repository testpypi dist/*
 
     run-unit-tests:
       - step:
           name: Run unit tests
           <<: *wiliot-ci-image
           script:
             - apk add tree
             - pip3 install pytest
             - tree
             - cd wiliot_deployment_tools
             - pytest wiliot_deployment_tools/internal/tests
 
+    update-ag-files-from-nordic-firmware:
+      - step:
+          name: update ag files from nordic firmware
+          <<: *wiliot-ci-image
+          script:
+            - UT_PATH="wiliot-nordic-firmware/project/ut/"
+            - AG_PATH="wiliot_deployment_tools/ag/"
+            - git clone git@bitbucket.org:wiliot/wiliot-nordic-firmware.git -b develop
+            - cp "${UT_PATH}ag/wlt_types_ag.py" $AG_PATH
+            - cp "${UT_PATH}ut_defines.py" $AG_PATH
+            - cp "${AG_PATH}wlt_types_imports.py" "${AG_PATH}wlt_types.py" 
+            - sed '/^from/d' -i "${UT_PATH}wlt_types.py"
+            - cat "${UT_PATH}wlt_types.py" >> "${AG_PATH}wlt_types.py"
+            - COMMIT_HASH=$(git --git-dir=wiliot-nordic-firmware/.git rev-parse --short HEAD)
+            - git add $AG_PATH
+            - git commit -m "[skip ci] Updating AG files from nordic-firmware (develop) ${COMMIT_HASH}"
+            - git push
+
     Build unittests image:
       - step: *build_unittests_image
 
+    push-init-scripts-to-s3:
+      - variables:
+          - name: ENV
+            default: dev
+            allowed-values:
+              - dev
+              - test
+              - prod
+          - name: CLOUD
+            default: aws
+            allowed-values:
+              - aws
+              - gcp
+      - step:
+          name: Upload Databricks init scripts to S3 bucket
+          script:
+            - bash ci/upload_to_s3.sh
+    deploy-to-cloud-env-aws:
+      - variables:
+          - name: ENV
+            default: dev
+            allowed-values:
+              - dev
+              - test
+              - prod
+          - name: CLOUD
+            default: aws
+            allowed-values:
+              - aws
+              - gcp
+
+      - step:
+          name: Make plan on Cloud
+          <<: *wiliot-ci-image
+          script:
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID
+            - export AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - make aws.plan.$ENV
+      - step:
+          name: Upload Databricks init scripts to S3 bucket
+          script:
+            - bash ci/upload_to_s3.sh
+      - step:
+          name: Make apply on Cloud
+          <<: *wiliot-ci-image
+          trigger: manual
+          script:
+            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID
+            - export AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
+            - make aws.apply.$ENV
+
 options:
   docker: true
```

### Comparing `wiliot-deployment-tools-4.0.8/ci.py` & `wiliot-deployment-tools-4.1.0/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/setup.py` & `wiliot-deployment-tools-4.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import setuptools
 import sys
-# package internal only when running with --config-setting internal flag
-internal_flag = False
-# Check if the argument is present
-if "-C" in sys.argv:
-    arg_value = sys.argv[sys.argv.index("-C") + 1]
-    if arg_value == 'internal':
-        internal_flag = True
-packages = setuptools.find_packages() if internal_flag else setuptools.find_packages(exclude=['*.internal.*', 'internal.*', '*.internal'])
+packages = setuptools.find_packages()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='wiliot-deployment-tools',
                  use_scm_version={
                      'git_describe_command': "git describe --long --tags --match [0-9]*.[0-9]*.[0-9]*",
@@ -32,44 +25,48 @@
                  license='MIT',
                  classifiers=[
                      "Programming Language :: Python :: 3",
                      "License :: OSI Approved :: MIT License",
                      "Operating System :: OS Independent",
                  ],
                  packages=packages,
-                #  add all support files to the installation
-                #  package_data={"": ["*.*"]},
+                #  add all support files to the internal installation
+                 package_data={"": ["*.*"]},
                  install_requires=[
-                     'setuptools_scm==7.1.0',
-                     'wiliot-core==4.0.9',
-                     'wiliot-api==4.1.2',
+                     'setuptools_scm>=7.1.0',
+                     'wiliot-core>=4.0.9',
+                     'wiliot-api>=4.3.2',
                      'bitstruct==8.17.0',
                      'bokeh==2.4.1',
                      'boto3==1.26.77',
                      'colorama==0.4.6',
                      'jsonpickle==3.0.1',
-                     'numpy<=1.24.2',
+                     'numpy==1.22.4',
                      'pandas==1.5.3',
                      'plotly==5.13.0',
                      'pytz==2022.7.1',
-                     'requests==2.28.1',
-                     'setuptools==65.6.3',
-                     'setuptools_scm==7.1.0',
+                     'requests>=2.28.1',
+                     'setuptools>=65.6.3',
                      'tabulate==0.8.10',
                      'backports.zoneinfo==0.2.1; python_version < "3.9.0"',
-                     'tinytuya==1.10.2',
-                     'pyserial==3.5',
-                     'GitPython==3.1.31',
-                     'tzdata==2023.3'
+                     'tinytuya>=1.10.2',
+                     'pyserial>=3.5',
+                     'GitPython>=3.1.31',
+                     'tzdata>=2023.3',
+                     'confluent-kafka>=2.1.1',
+                     'paho-mqtt>=1.6.1'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                 #  include_package_data=False,
                 #  exclude_package_data={
                 #      "": ['*.internal.*', '*.internal', 'internal', 'internal.*']},
                  entry_points={'console_scripts': [
                      'wlt-firmware=wiliot_deployment_tools.firmware_update.firmware_update_cli:main_cli',
                      'wlt-power-mgmt=wiliot_deployment_tools.power_mgmt.power_mgmt_cli:main_cli',
                      'wlt-calibration-mgmt=wiliot_deployment_tools.calibration_mgmt.calibration_mgmt_cli:main_cli',
+                     'wlt-connectivity-analyzer=wiliot_deployment_tools.connectivity_analyzer.connectivity_analyzer_cli:main_cli',
                      'wlt-config=wiliot_deployment_tools.automatic_configuration_tool.configuration_tool_cli:main_cli',
-                     'wlt-log=wiliot_deployment_tools.log_viewer.log_viewer_cli:main_cli']},
+                     'wlt-log=wiliot_deployment_tools.log_viewer.log_viewer_cli:main_cli',
+                     'wlt-gw-certificate=wiliot_deployment_tools.gw_certificate.gw_certificate_cli:main_cli',
+                     'wlt-kafka=wiliot_deployment_tools.internal.kafka_consumer.kafka_consumer_cli:main_cli']},
                  )
```

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.1.0/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.1.0/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.1.0/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.1.0/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.1.0/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/unittests/test_utils.py` & `wiliot-deployment-tools-4.1.0/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/extended_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import urllib.parse
 
 # Internal Imports
 from wiliot_api.api_client import WiliotCloudError
 from wiliot_api.platform.platform import PlatformClient
 from wiliot_api.edge.edge import EdgeClient, BridgeAction
 from wiliot_deployment_tools.common.debug import debug_print
-from wiliot_deployment_tools.common.utils_defines import BO_DICT, SEP
+from wiliot_deployment_tools.common.utils_defines import BO_DICT, BROADCAST_DST_MAC, SEP
 
 EXCEPTIONS_TO_CATCH = (AttributeError, WiliotCloudError, JSONDecodeError)
 
 
 # Enum Classes
 class GatewayType(Enum):
     UNKNOWN = 'unknown'
@@ -30,14 +30,15 @@
 
 
 class GatewayAction(Enum):
     ADD_SSID = 'addSsid'
     TOGGLE_SSID = 'toggleDefaultSsid'
     REBOOT_GW = 'rebootGw'
     START_BRIDGE_OTA = '!send_msg_to_brg'
+    ENTER_DEV_MODE = 'DevModeEnable'
 
 class AndroidGatewayAction(Enum):
     DISABLE_UPLINK = -2
     ENABLE_UPLINK = -3
     DISABLE_BLE_LOGS = -4
     ENABLE_BLE_LOGS = -5
 
@@ -45,30 +46,41 @@
     REBOOT = '01'
     BLINK = '02'
     POWER_MGMT = '03'
     RESTORE_DEFAULTS = '04'
     SEND_HB = '05'
     PRODUCTION_MODE = '06'
     SPARSE_37 = '07'
+    GW_HB = '08'
 
 
 class BoardTypes(Enum):
+    FANSTEL_SINGLE = 'FanstelSingleBandV0'
+    FANSTEL_DUAL = 'FanstelDualBandV0'
+    MINEW_SINGLE = 'MinewSingleBandV0'
+    MINEW_DUAL = 'MinewDualBandV0'
+    ENERGOUS = 'EnergousV0'
+
+class BoardTypesActive(Enum):
     ENERGOUS = 'Energous Dual-Band (v0)'
     FANSTEL_SINGLE = 'Fanstel Single-Band (v0)'
     FANSTEL_DUAL = 'Fanstel Dual-Band (v0)'
     MINEW_SINGLE = 'Minew Single-Band (v0)'
     MINEW_DUAL = 'Minew Dual-Band (v0)'
     MOKO = 'Moko Dual-Band (v0)'
 
 
 # API Clients
 
 class ParamMissingError(Exception):
     pass
 
+class ExtendedEdgeClientError(Exception):
+    pass
+
 
 class ExtendedEdgeClient(EdgeClient):
     # Get Info
     def get_connected_brgs(self, gw, ignore_bridges=None):
         """
             returned all bridges connected to gateway and claimed by owner
             :type gw: string
@@ -151,15 +163,44 @@
                     if gw not in owners_gws:
                         continue
                     if gw not in gws_list.keys():
                         gws_list[gw] = [brg_id]
                     else:
                         gws_list[gw].append(brg_id)
         return gws_list
-            
+
+
+    def get_bridge_relevant_gw(self, bridge_id, get_gw_list = False):
+        """
+        Returns relevant GW for sending actions to bridge
+        :param bridge_id: Bridge ID
+        :rtype: str
+        :return: relevant Gateway ID
+        """
+
+        # TODO - return list of potential GWs
+        potential_gws = list()
+        owner_gws = self.get_gateways()
+        owner_gw_ids = []
+        owner_gw_ids.extend(g['gatewayId'] for g in owner_gws)
+        for gw in self.get_bridge(bridge_id)['connections']:
+            if gw['gatewayId'] not in owner_gw_ids:
+                continue
+            gw_id = gw['gatewayId']
+            gw_dict = self.get_gateway(gw_id)
+            if gw['connected'] and \
+                    bridge_id in self.get_seen_bridges(gw_id) and \
+                    self.check_gw_compatible_for_action(gw_id):
+                if bridge_id in self.get_seen_bridges(gw['gatewayId']):
+                    potential_gws.append(gw['gatewayId'])
+        if len(potential_gws) == 0:
+            raise ExtendedEdgeClientError(f'No relevant GW connected to bridge! Check deployment')
+        if get_gw_list:
+            return potential_gws
+        return potential_gws[0]        
             
     def get_seen_bridges(self, gw, ignore_bridges=None):
         """
         return all bridges 'seen' by GW
         :type gw: str
         :param gw: gateway ID
         :type ignore_bridges: list
@@ -239,15 +280,22 @@
         return False
 
     def get_bridge_board(self, brg_id):
         """
         :type brg_id: string
         :param brg_id: bridge id
         """
-        return self.get_bridge(brg_id)['boardType']
+        board_type = self.get_bridge(brg_id)['boardType']
+        if board_type in [member.value for member in BoardTypes.__members__.values()]:
+            return board_type
+        else:
+            try:
+                return (BoardTypes[BoardTypesActive(board_type).name]).value
+            except:
+                return None
 
     # Gateway & Bridge Actions
     def send_action_to_gateway(self, gateway_id, action, **kwargs):
         """
         Send an action to a gateway
         :param gateway_id: String - the ID of the gateway to send the action to
         :param action: GatewayAction - Required
@@ -277,54 +325,117 @@
             res = self._post(path, payload)
             return res['data'].lower().find("ok") != -1
         except WiliotCloudError as e:
             print("Failed to send action to gateway")
             raise WiliotCloudError(
                 "Failed to send action to gateway. Received the following error: {}".format(e.args[0]))
 
-    def send_bridge_action_through_gw(self, gateway_id, action_type, payload='0', bridge_id=None, broadcast=False, reps=8, ms_to_send=1200):
+    def enter_dev_mode(self, gateway_id, legacy=False):
         """
-        Send an action to a bridge through a gateway
-        :param broadcast: whether to broadcast
-        :param gateway_id: String - the ID of the gateway to send the action Through
-        :param bridge_id: String - the ID of the bridge to send the action to
-        :param action_type: BridgeThroughGatewayAction - Required
-        :param payload: 28 bytes (hex string)
-        :param reps: repetition (wifi gw only)
-        :param ms_to_send: milliseconds to send (android gw only)
-        :return: True if the cloud successfully sent the action to the gateway, False otherwise
+        enter GW Dev Mode
+        :type legacy: bool, optional
+        :param legacy: if True, sends legacy dev mode change, defaults to False
+        :return: True if sent successfully to GW
+        :rtype: bool
         """
+        if legacy:
+            return self.send_action_to_gateway(gateway_id, GatewayAction.ENTER_DEV_MODE)
+        dev_mode = {
+                    "custom-mqtt": True,
+                    "broker_url": "broker.hivemq.com",
+                    "port": 8883,
+                    "username": "",
+                    "password": "",
+                    "update-topic": f"update-test/{self.owner_id}/{gateway_id}",
+                    "status-topic": f"status-test/{self.owner_id}/{gateway_id}",
+                    "data-topic": f"data-test/{self.owner_id}/{gateway_id}"
+                    }
+        return self.send_custom_message_to_gateway(gateway_id, dev_mode)
+
+
+    
+    def send_packet_through_gw(self, gateway_id, raw_packet, is_ota=False, brg_id=None, repetitions=8, tx_rate=None):
+        """
+        send packet through GW
+        :param gateway_id: gateway ID
+        :type gateway_id: str
+
+        :param raw_packet: raw packet
+        :type raw_packet: str
+        :type is_ota: bool, optional
+        :param is_ota: start OTA with bridge, defaults to False
+        :type brg_id: bridge ID, optional
+        :param brg_id: str, defaults to None
+        :type repetitions: int, optional
+        :param repetitions: number of times to send the packet, defaults to 8
+        :type tx_rate: int, optional
+        :param tx_rate: tx rate to send the packet (used to calculate txMaxDurationMs):
+                        ANDROID GW - 140ms
+                        ERM GW - 50ms
+        :return: True if successful
+        :rtype: bool
+        """
+        
+        if len(raw_packet) < 62:
+            if len(raw_packet) == 54:
+                raw_packet = 'C6FC' + raw_packet
+            if len(raw_packet) == 58:
+                raw_packet = '1E16' + raw_packet
+        assert len(raw_packet) == 62, 'Raw Packet must be 62 chars long!'
+        # Android tx rate - 140ms
+        # ERM StarLink tx rate - 50ms
+        if tx_rate is None:
+            if self.get_gateway_type(gateway_id) == GatewayType.MOBILE:
+                tx_rate = 140
+            elif self.get_gateway_type(gateway_id) == GatewayType.LTE:
+                tx_rate = 50
+            else:
+                tx_rate = 140
+        payload = {'txPacket': raw_packet,
+                   # MOBILE GW looks at txMaxDurationMs (Android is sending advertisement packets at rate of 140ms)
+                   'txMaxDurationMs': tx_rate * repetitions,
+                   # All other GWs looks at txMaxRetries, 
+                   'txMaxRetries': repetitions,
+                   'action': 0}
+        if is_ota:
+            payload.update({'action': 1, 'bridgeId': brg_id})
+        return self.send_custom_message_to_gateway(gateway_id, payload)
+    
+    @staticmethod
+    def generate_bridge_action_packet(action_type, payload='0', bridge_id=None, broadcast=False):
         assert action_type in BridgeThroughGatewayAction, 'Not valid action type'
         assert (bridge_id is not None and broadcast is False) or (bridge_id is None and broadcast is True), \
             'Must supply bridgeId / set broadcast to True'
-        assert reps > 0, 'Repetitions must be a positive value!'
-        assert ms_to_send > 0, 'Milliseconds to send must be a positive value!'
         assert len(bridge_id) == 12
+        if broadcast:
+            bridge_id = BROADCAST_DST_MAC
         payload = str(payload).ljust(28, '0')
         # Packet Header: 0-5 ADVA, 6 Length, 7 AD Type, 8-9 UUID, 10-12 Group ID, 13 MSG type, 14 API Ver.
         header = '1E16C6FC0000ED0707'
         # Randomize Sequence ID
         seq_id = random.getrandbits(8).to_bytes(1, 'big').hex().upper()
-        gw_type = self.get_gateway_type(gateway_id)
-        if gw_type == GatewayType.MOBILE:
-            arg = ms_to_send
-        else:
-            arg = reps
-        payload = {
-            "action": f'!sp {header}{seq_id}{bridge_id}{action_type.value}{payload} {arg}'
-        }
-        path = "gateway/{}/action".format(gateway_id)
-        try:
-            res = self._post(path, payload)
-            return res['data'].lower().find("ok") != -1
-        except WiliotCloudError as e:
-            print("Failed to send action to gateway")
-            raise WiliotCloudError(
-                "Failed to send action to gateway. Received the following error: {}".format(e.args[0]))
-
+        # Assemble raw packet
+        return f'{header}{seq_id}{bridge_id}{action_type.value}{payload}'
+    
+    def send_bridge_action_through_gw(self, gateway_id, action_type, payload=None, bridge_id=None, broadcast=False, reps=8):
+        """
+        Send an action to a bridge through a gateway
+        :param broadcast: whether to broadcast
+        :param gateway_id: String - the ID of the gateway to send the action Through
+        :param bridge_id: String - the ID of the bridge to send the action to
+        :param action_type: BridgeThroughGatewayAction - Required
+        :param payload: 28 bytes (hex string)
+        :param reps: repetitions to send
+        :return: True if the cloud successfully sent the action to the gateway, False otherwise
+        """
+        if payload is None:
+            payload = '0'
+        raw_packet = self.generate_bridge_action_packet(action_type, payload, bridge_id, broadcast)
+        self.send_packet_through_gw(gateway_id, raw_packet, repetitions=reps)
+    
     def reboot_gateway(self, gateway_id):
         """
         Reboots specified GW
         :param gateway_id: Gateway ID
         :return: True if the cloud successfully sent the action to the gateway, False otherwise
         """
         return self.send_action_to_gateway(gateway_id, GatewayAction.REBOOT_GW)
@@ -789,17 +900,19 @@
             # Check if bridges updated
             for brg_id in set(brgs_list) - set(updated_brgs):
                 try:
                     brg_updated = check_updated(brg_id, config_dict)
                     if brg_updated:
                         updated_brgs.append(brg_id)
                     else:
-                        debug_print(f'Sending configuration again to bridge {brg_id}')
-                        sleep(3)
-                        update_bridge(brg_id, config_dict)
+                        pass
+                        ## TODO TEMP
+                        # debug_print(f'Sending configuration again to bridge {brg_id}')
+                        # sleep(3)
+                        # update_bridge(brg_id, config_dict)
                 except (EXCEPTIONS_TO_CATCH) as e:
                     debug_print(f'{brg_id}: {e}')
                     sleep_needed = True
                 except ParamMissingError as e:
                     params_missing.append((e, brg_id))
                     updated_brgs.append(brg_id)
         for error, brg in params_missing:
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/s3_client.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/api/s3_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 def main():
     # parser
     parser = ArgumentParser(prog='wlt-calibration-mgmt',
                             usage='%(prog)s -o OwnerID -brg BridgeID (-t) [mode]',
                             description='CLI Tool for using Wiliot Bridge calibration management functionality')
     parser.add_argument('-owner', type=str, help="Owner ID", required=True)
-    parser.add_argument('-brg', type=str, help="Bridge ID", required=False)
+    parser.add_argument('-brg', type=str, help="Bridge ID, For broadcast leave empty", required=False)
     parser.add_argument('-t', action='store_true',
                         help='if flag used, use test environment (prod is used by default)')
-    parser.add_argument('-gw', type=str, help="GW ID to configure bridge (required only for broadcast mode)", required=False)
+    parser.add_argument('-gw', type=str, help="GW ID to configure bridge (required only for non broadcast mode)", required=False)
     parser.add_argument('-m', type=int, help="Minutes timeout (not required, defaults to 5 minutes)", required=False, default=5)
     parser.add_argument('-mode', '--option', choices=[0,1,2], type=int, help="Calinration mode selection: 0 - regular 1 - 38,38,39 2 - 37 on data only", required=True)
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
@@ -36,14 +36,18 @@
     user_config_file_path, api_key, is_success = check_user_config_is_ok(owner_id, env, 'edge')
     if is_success:
         print('credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid credentials - please try again to login')
 
     client = CalibrationManagementClient(api_key, owner_id, env)
-    client.send_calibration_packet_until_ack(gateway_id = args.gw, bridge_id = args.brg, minutes_timeout=args.m,mode = args.option)
+    bridge_id = args.brg
+    if bridge_id is None:
+        client.broadcast_calibration_packet_until_ack(gateway_id = args.gw,minutes_timeout=args.m,mode = args.option)
+    else:
+        client.send_calibration_packet_until_ack(gateway_id = args.gw, bridge_id = bridge_id, minutes_timeout=args.m,mode = args.option)
 
 
 def main_cli():
     main()
 if __name__ == '__main__':
     main()
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from importlib import reload
 import os
 import shutil
 import subprocess
 import datetime
 from itertools import combinations, chain
 from time import sleep
 from pathlib import Path
@@ -1187,14 +1188,16 @@
     """
     initializes the logger to print to log and to logfile, which by default is named by the current timestamp (ms)
     when calling the function.
     :param working_directory: working directory to save logfile (in case running locally)
     :type working_directory: str
     :return: logger fileHandler filename
     """
+    logging.shutdown()
+    reload(logging)
     logger = logging.getLogger()
     for handler in logger.handlers:
         try:
             # extract current filename from log
             filename = handler.baseFilename.split('\\')[-1].split('.')[0]
             debug_print(f'Logger already initialized! passing logfile {filename}')
             return filename
@@ -1206,15 +1209,15 @@
         logging.getLogger("py4j.java_gateway").setLevel(logging.ERROR)
         logging.basicConfig(level=logging.DEBUG,
                             format='%(asctime)s | %(levelname)s | %(message)s',
                             handlers=[
                                 logging.FileHandler(f'{logger_filename}.log', 'a'),
                                 # logging.handlers.RotatingFileHandler
                                 logging.StreamHandler()
-                            ])
+                            ], force=True)
         logging.getLogger().handlers[0].setLevel(logging.DEBUG)
         logging.getLogger().handlers[1].setLevel(logging.INFO)
         debug_print(f'logger initialized at {logger_filename}', center=True)
         debug_print(f'logfile located at file:/databricks/driver/{logger_filename}.log')
     else:
         if working_directory is None:
             working_directory = os.path.join(user_data_dir(), 'wiliot', 'deployment_tools')
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,24 +382,22 @@
         if 'otaUpgradeEnabled' not in brg_keys:
             print(f'Cannot update OTA for bridge {brg_id}, otaUpgradeEnabled not in configuration parameters!')
             return None
         self.change_brg_config([brg_id], {"otaUpgradeEnabled": val}, minutes_timeout=30)
     
     def do_action_ota(self, gw_id, brg_id):
         """
-        does OTA using action API
+        does OTA using custom action API
         :param gw_id: GW id
         :param brg_id: BRG id
         """
-        assert self.get_gateway_type(gw_id) == GatewayType.WIFI
-        debug_print(f'Sending REBOOT to brg {brg_id}')
-        res = self.send_bridge_action_through_gw(gw_id, BridgeThroughGatewayAction.REBOOT, payload='000', bridge_id=brg_id)
-        time.sleep(3)
+        assert self.get_gateway_type(gw_id) in [GatewayType.WIFI, GatewayType.LTE]
         debug_print(f'Initializing DFU W/ GW {gw_id} to BRG {brg_id}')
-        res = self.send_action_to_gateway(gw_id, GatewayAction.START_BRIDGE_OTA, bridge_id=brg_id)
+        res = self.send_packet_through_gw(gw_id, self.generate_bridge_action_packet(BridgeThroughGatewayAction.REBOOT, bridge_id=brg_id), is_ota=True, brg_id=brg_id)
+        return res
 
     def wait_for_gw_firm_update(self, gw_id):
         gw = self.get_gateway(gw_id)
         while gw['online'] is False:
             debug_print('Waiting for GW to get back online...')
             sleep(10)
             gw = self.get_gateway(gw_id)
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from doctest import debug
+from struct import pack
 import sys
 import time
 import bitstruct
 from wiliot_deployment_tools.api.extended_api import EXCEPTIONS_TO_CATCH, AndroidGatewayAction, BridgeThroughGatewayAction, ExtendedEdgeClient, GatewayType
 from wiliot_deployment_tools.common.debug import debug_print
 from wiliot_deployment_tools.common.utils_defines import KEEP_ALIVE_PERIOD, KEEP_ALIVE_SCAN_DURATION, SEC_TO_SEND, BROADCAST_DST_MAC, EXIT_POWER_MGMT_GW_DICT
 
@@ -154,37 +155,15 @@
         keep_alive_period_secs = keep_alive_period * 5
         keep_alive_scan_ms = keep_alive_scan * 10
         return sleep_duration_mins, on_duration_secs, keep_alive_period_secs, keep_alive_scan_ms, leds_on
 
 
 class BridgePowerManagementClient(ExtendedEdgeClient):
 
-    def get_bridge_relevant_gw(self, bridge_id):
-        """
-        Returns relevant GW for sending actions to bridge
-        :param bridge_id: Bridge ID
-        :rtype: str
-        :return: relevant Gateway ID
-        """
-
-        # TODO - return list of potential GWs
-        owner_gws = self.get_gateways()
-        owner_gw_ids = []
-        owner_gw_ids.extend(g['gatewayId'] for g in owner_gws)
-        for gw in self.get_bridge(bridge_id)['connections']:
-            if gw['gatewayId'] not in owner_gw_ids:
-                continue
-            gw_id = gw['gatewayId']
-            if gw['connected'] and \
-                    bridge_id in self.get_seen_bridges(gw_id) and \
-                    self.check_gw_compatible_for_action(gw_id):
-                if bridge_id in self.get_seen_bridges(gw['gatewayId']):
-                            return gw['gatewayId']
-        raise PowerManagementError(f'No relevant GW connected to bridge! Check deployment')
-
+    
     def get_relevant_bridges(self, gateway_id):
         """
         Returns seen bridges by gateway that are associated to owner and have ble version with power management support
         :type gateway_id: str
         :param gateway_id: gateway ID
         :rtype: list
         :return: list of relevant bridge IDs
@@ -232,41 +211,37 @@
         :rtype: bool
         :return: True if sent, False otherwise
         """
         if gateway_id is None:
             via_gw = self.get_bridge_relevant_gw(bridge_id)
         else:
             via_gw = gateway_id
-        reps = 8
-        ms_to_send = 1200
         seconds_to_send = datetime.timedelta(seconds=seconds_to_send)
         # Check BRG Compatability
         brg_version = None
         if bridge_id is not BROADCAST_DST_MAC:
             brg_version = self.get_brg_ble_version(bridge_id)
         # Check GW Compatability
         gw_type = self.get_gateway_type(via_gw)
         if gw_type == GatewayType.WIFI:
             gw_version = self.get_gw_ble_version(via_gw)
             for version in filter(None, [brg_version, gw_version]):
                 if not self.check_ble_power_mgmt_support(version):
                     return False
             rxtx = datetime.timedelta(milliseconds=
                                     self.get_gateway(via_gw)['reportedConf']['additional']['rxTxPeriodMs'])
-            reps = seconds_to_send // rxtx + 1
-            if not silent:
-                debug_print(f'Sending packet through WIFI GW {via_gw} for {seconds_to_send.total_seconds()} seconds, rxTx = {int(rxtx.total_seconds()*1000)} ms, reps = {reps}')
         if gw_type == GatewayType.MOBILE:
-            if not silent:
-                debug_print(f'Sending packet through ANDROID GW {via_gw} for {seconds_to_send.total_seconds()} seconds')
-            ms_to_send = int(seconds_to_send.total_seconds()*1000)
+            rxtx = datetime.timedelta(milliseconds=140)
+        reps = seconds_to_send // rxtx + 1
+        if not silent:
+            debug_print(f'Sending packet through GW {via_gw} for {seconds_to_send.total_seconds()} seconds, rxTx = {int(rxtx.total_seconds()*1000)} ms, reps = {reps}')
         try:
             res = self.send_bridge_action_through_gw(gateway_id,
                                                  BridgeThroughGatewayAction.POWER_MGMT,
-                                                 packet.payload, bridge_id, reps=reps, ms_to_send=ms_to_send)
+                                                 packet.payload, bridge_id, reps=reps)
         except EXCEPTIONS_TO_CATCH as e:
             debug_print('Exception caught when sending power mgmt packet!')
             debug_print(e)
             return False
         return res
 
     def broadcast_pwr_mgmt_packet(self, packet, gateway_id, silent=False, seconds_to_send=1):
@@ -473,15 +448,27 @@
         if broadcast:
             if gateway_id is None:
                 raise PowerManagementError('Must specify GW ID to broadcast')
             return self.broadcast_packet_until_ack(gateway_id, packet, minutes_timeout)
         via_gw = self.get_bridge_relevant_gw(bridge_id) if gateway_id is None else gateway_id
         if not self.check_gw_compatible_for_action(via_gw):
             raise PowerManagementError(f'GW {via_gw} Not compatible for power management!')
-        return self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
+        res = self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
+        if False in res.values():
+            ###HOTFIX
+            if self.get_gateway_type(via_gw) == GatewayType.MOBILE:
+                self.send_packet_until_ack(via_gw, bridge_id, PowerManagementPacket.exit_packet(), minutes_timeout)
+                res = self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
+                if False in res.values():
+                    raise PowerManagementError(f'Failed to exit power management! {res}')
+                else:
+                    return res
+            else:
+                raise PowerManagementError(f'Failed to exit power management! {res}')
+        return res
 
     def exit_power_mgmt(self, gateway_id=None, update_gw=False, bridge_id=None, broadcast=False, minutes_timeout=3):
         """
         Exit power management mode (to normal bridge behavior).
         Function will search for the relevant gateway ID (if not specified) to send the configuration packet through.
         :type bridge_id: str
         :param bridge_id: Bridge ID
@@ -518,15 +505,17 @@
         if broadcast:
             res = self.broadcast_packet_until_ack(gateway_id, packet, minutes_timeout)
         else:
             res = self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
         if need_to_update and update_gw:
             debug_print('Finished sending exit packets, returning GW to old state')
             self.change_gw_config([via_gw], gw_dict)
-        return res
+        if False in res.values():
+                raise PowerManagementError(f'Failed to exit power management! {res}')
+        return res            
 
 
 class AndroidPowerManagementClient(ExtendedEdgeClient):
     def set_uplink_mode(self, gateway_id, uplink_mode):
         """
         set uplink mode (on/off) for android GW
         :param gateway_id: gateway ID
@@ -534,14 +523,24 @@
         :param uplink_mode: uplink mode
         :type uplink_mode: bool
         """
         payload = {True: AndroidGatewayAction.ENABLE_UPLINK,
                    False: AndroidGatewayAction.DISABLE_UPLINK}
         gw_type = self.get_gateway_type(gateway_id)
         assert gw_type == GatewayType.MOBILE, f'GW {gateway_id} not an android GW!'
-        debug_print(f'Setting GW {gateway_id} uplink to {uplink_mode}')
-        return self.send_action_to_gateway(gateway_id, payload[uplink_mode])
+        def send_uplink_mode_and_sleep(gateway_id, uplink_mode):
+            debug_print(f'Setting GW {gateway_id} uplink to {uplink_mode}...')
+            res = self.send_action_to_gateway(gateway_id, payload[uplink_mode])
+            debug_print('Waiting for GW to update... (30 seconds)')
+            time.sleep(30)
+            return res
+        tries = 1
+        if uplink_mode:
+            tries = 3
+        for num in range(tries):
+            res = send_uplink_mode_and_sleep(gateway_id, uplink_mode)
+        return res
 
 class PowerManagementClient(BridgePowerManagementClient, AndroidPowerManagementClient):
     pass
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from numpy import require
 from wiliot_deployment_tools.power_mgmt.power_mgmt import PowerManagementClient
 from wiliot_core import check_user_config_is_ok
 from wiliot_deployment_tools.common.utils_defines import *
 from argparse import ArgumentParser
 import sys
```

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.1.0/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.8
+Version: 4.1.0
 Summary: A library for interacting with Wiliot's Deployment Tools
-Home-page: 
+Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyWiliot: wiliot-deployment-tools #
 
 wiliot-deployment-tools is a python library for accessing Wiliot's Deployment and Automation Tools.
 This python package includes the following CLI utilities:
  - Automatic Configuration Tool (`wlt-config`)
- - Power Management Tool (`wlt-power-mgmt`)
  - Calibration Management Tool (`wlt-clibration-mgmt`)
  - Firmware Update Tool (`wlt-firmware`)
+ - Power Management Tool (`wlt-power-mgmt`)
  - Log Viewer (`wlt-log`)
-
+ - Connectivity Analyzer (`wlt-connectivity-analyzer`)
+ - Gateway Certificate (`wlt-gw-certificate`)
 
 ## Installing wiliot-deployment-tools
 ````commandline
 pip install wiliot-deployment-tools
 ````
 
 ## Using wiliot-deployment-tools
@@ -51,62 +53,65 @@
                         bridges to ignore in the tool - their configuration won't be changed
   -expected_num_brgs EXPECTED_NUM_BRGS
                         Number of expected bridges in location. The tool will try to connect to all bridges (excluding those specified in ignore bridges) until reaching expected number.
 
 example usage: wlt-config --owner wiliot --location "My Deployment" --ota_upgrade --pacing_interval 10 --ignore_bridges 1234ABCD0123
 ```
 
-### Firmware Update
-Update Wiliot Gateways and Bridges firmware version OTA.
- #### Print Available Versions 
- Prints all avaliable Firmware versions for update for every GW Type
-```
-usage: wlt-firmware -owner OWNER [-beta] versions
-
-optional arguments:
-  -beta              show available beta versions / update to beta firmware
-
-example usage: wlt-firmware -o wiliot versions
-```
 ### Calibration Management
-Configure Wiliot Bridge calibration mode
+Configure Wiliot Bridge calibration mode, broadcast is optional
 ```
 usage: wlt-calibration-mgmt -owner OwnerID -brg BridgeID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
+usage (broadcast): wlt-calibration-mgmt -owner OwnerID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
-  -brg BRG      Bridge ID
-  -gw GW        GW ID to configure bridge
+  -brg BRG      Bridge ID (required only for non broadcast)
+  -gw GW        GW ID to configure bridge (required only for broadcast)
   -mode Mode    CalibrationMode on of 3 options: 0-regular, 1-no ch37, 2-ch37 on data only
 
 optional arguments:
-
   -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
 
   example usage: wlt-calibration-mgmt -owner wiliot -brg 0123ABCD -gw AB1234CD -mode 1
 ```
 
+### Firmware Update
+Update Wiliot Gateways and Bridges firmware version OTA.
+ #### Print Available Versions 
+ Prints all avaliable Firmware versions for update for every GW Type
+```
+usage: wlt-firmware -owner OWNER [-beta] versions
+
+optional arguments:
+  -beta              show available beta versions / update to beta firmware
+
+example usage: wlt-firmware -o wiliot versions
+```
+
  #### Firmware Update
  Run OTA Process, first updating specified GWs to latest / specified FW version. Afterwards seuqentially update each specified Bridges / all Bridges to the same Firmware version.
  ```
 usage: wlt-firmware update -owner OWNER [-beta] [-version VERSION] [-gw GW [GW ...]] [-brg BRG [BRG ...]] [-all_brgs] [-ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]] [-action]
 
+
 optional arguments:
   -beta              show available beta versions / update to beta firmware
   -version VERSION      Desired version. if not specified, will update to latest available version
   -gw GW [GW ...]       Gateways to update (multiple allowed)
   -brg BRG [BRG ...]    Bridges to update (multiple allowed)
   -all_brgs             update all bridges connected to Gateways
   -ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]
                         bridges to ignore
   -action               update using action API
   -force                update bridge even if its already in desired version (applicable only with -action)
 
   example usage: wlt-firmware -o wiliot update -gw GW0123 -all_brgs
   ```
+
 ### Power Management
 Use Wiliot Bridge power management functionality
 #### Enter Power Management
 Configure Specified Bridges to work in power management configuration.
 ```
 usage: wlt-power-mgmt -o OwnerID enter -brg BridgeID -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
 
@@ -140,33 +145,109 @@
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
 example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
+  
 
 ### Log Viewer
 View Wiliot Gateway logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
 Log Viewer - CLI Tool to view Wiliot Gateway logs
 
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
 ```
 
+
+
+### Connectivety Analyzer
+Check the rssi connection between gws and bridge (as received at the bridge)
+Can operate by: location, bridges or gateways
+Return the bridges with low connection
+```
+usage: wlt-connectivity-analyzer -owner OWNER -location Location
+
+required arguments:
+  -owner OWNER  Owner ID
+
+
+optional arguments:
+  -gws GwsList         List of gateways IDs to check connection to the bridges they see
+  -brgs BridgesList    List of bridges IDs to check connection 
+  -location Location   Location name (as written in platform) to check all bridges in
+```
+
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
+### Gateway Certificate
+Test Wiliot GWs capabilities.
+The GW Certificate includes different test that run sequentially to test each capability reported by the GW.
+
+#### Coupling Test
+The test switched the GW to an external MQTT Broker and uses a BLE Simulator (Wiliot WIFI GW connected using UART) to simulate bridges and test the coupling capability of the tested GW (Couple together Data and SideInfo packets)
+The test inclued the following stages:
+- STAGES = [InitStage, OneBrgStage, ThreeBrgInitStage, ThreeBrgStage]
+- Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
+- One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
+- Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
+- Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
+The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
+
+#### Release Notes:
+Version 4.1.0:
+* Coupling Test
+* Add CSV Output
+* Calculate test run
+
+Version 4.0.13:
+* Initial Release (Alpha)
+
+```
+usage: wlt-gw-certificate [-h] -owner OWNER -gw GW [-test] [-random] [-legacy]
+
+Gateway Certificate - CLI Tool to test Wiliot GWs
+
+optional arguments:
+  -h, --help    show this help message and exit
+  -test         If flag used, use test environment (prod is used by default)
+  -random       randomize packets (if not used same packets will be sent for each run)
+  -legacy       use legacy DevMode
+
+required arguments:
+  -owner OWNER  Owner ID
+  -gw GW        Gateway ID
+  ```
+
 
 ## Release Notes:
+Version 4.1.0:
+* Custom message support
+* GW Certificate - coupling test
+* Fixes for calibration management
+
+Version 4.0.13:
+* Add Gateway Certificate (Alpha)
+
+Version 4.0.12:
+* Add new Connectivity Analyzer
+
+Version 4.0.11:
+* Add broadcast to calibration management
+* Bugfixes for power management using android GW
+
+Version 4.0.10:
+* Internal fixes
 
 Version 4.0.8:
 * Support for python 3.11
 * Added new calibration mgmt tool
 
 Version 4.0.7:
 * Android power management support
@@ -197,7 +278,9 @@
 /Applications/Python\ 3.7/Install\ Certificates.command
 ~~~~
 
 #### Python 3 on MacOS
 The default Python version on mac is 2.x. Since Wiliot package requires Python 3.x you should download Python3 
 (e.g.  Python3.7) and make python 3 your default.
 There are many ways how to do it such as add python3 to your PATH (one possible solution https://www.educative.io/edpresso/how-to-add-python-to-the-path-variable-in-mac) 
+
+
```

