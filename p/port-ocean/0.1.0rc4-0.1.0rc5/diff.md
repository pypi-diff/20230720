# Comparing `tmp/port_ocean-0.1.0rc4.tar.gz` & `tmp/port_ocean-0.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0rc4.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0rc5.tar", max compression
```

## Comparing `port_ocean-0.1.0rc4.tar` & `port_ocean-0.1.0rc5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11357 2023-07-20 10:20:22.111079 port_ocean-0.1.0rc4/LICENSE
--rw-r--r--   0        0        0     4585 2023-07-20 10:20:22.111079 port_ocean-0.1.0rc4/README.md
--rw-r--r--   0        0        0      255 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/__init__.py
--rw-r--r--   0        0        0      321 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5561 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
--rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      598 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      653 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
--rw-r--r--   0        0        0      778 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1302 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      722 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2398 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     3049 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5681 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3866 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/base.py
--rw-r--r--   0        0        0     1218 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1107 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/event.py
--rw-r--r--   0        0        0     4286 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/base.py
--rw-r--r--   0        0        0      593 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3083 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     3147 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/utils.py
--rw-r--r--   0        0        0      716 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7949 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11831 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1683 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0      588 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/ocean.py
--rw-r--r--   0        0        0     7234 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/utils.py
--rw-r--r--   0        0        0     2736 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 12:14:21.346149 port_ocean-0.1.0rc5/LICENSE
+-rw-r--r--   0        0        0     4585 2023-07-20 12:14:21.346149 port_ocean-0.1.0rc5/README.md
+-rw-r--r--   0        0        0      255 2023-07-20 12:14:21.370149 port_ocean-0.1.0rc5/port_ocean/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5561 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      598 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      653 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
+-rw-r--r--   0        0        0      778 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1302 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      722 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2398 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     3049 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5730 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3866 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2277 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1218 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1107 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/base.py
+-rw-r--r--   0        0        0      593 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3083 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     3147 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/utils.py
+-rw-r--r--   0        0        0      716 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7949 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11831 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0     1368 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7361 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/port_ocean/utils.py
+-rw-r--r--   0        0        0     2736 2023-07-20 12:14:21.374149 port_ocean-0.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc5/PKG-INFO
```

### Comparing `port_ocean-0.1.0rc4/LICENSE` & `port_ocean-0.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/README.md` & `port_ocean-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/commands.py` & `port_ocean-0.1.0rc5/port_ocean/cli/commands.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0rc5/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0rc5/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0rc5/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/client.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib.parse import quote_plus
+
 import httpx
 from loguru import logger
 
 from port_ocean.clients.port.authentication import PortAuthentication
 from port_ocean.clients.port.types import RequestOptions, UserAgentType
 from port_ocean.clients.port.utils import handle_status_code
 from port_ocean.core.models import Entity
@@ -55,15 +57,15 @@
         user_agent_type: UserAgentType | None = None,
         silent: bool = False,
     ) -> None:
         logger.info(
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         response = await self.client.delete(
-            f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
+            f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{quote_plus(entity.identifier)}",
             headers=await self.auth.headers(user_agent_type),
             params={
                 "delete_dependents": str(
                     request_options.get("delete_dependent_entities", False)
                 ).lower()
             },
         )
```

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/clients/port/types.py` & `port_ocean-0.1.0rc5/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/config/base.py` & `port_ocean-0.1.0rc5/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/config/dynamic.py` & `port_ocean-0.1.0rc5/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/config/integration.py` & `port_ocean-0.1.0rc5/port_ocean/config/integration.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0rc5/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/context/event.py` & `port_ocean-0.1.0rc5/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/context/ocean.py` & `port_ocean-0.1.0rc5/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/event_listener.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/utils.py` & `port_ocean-0.1.0rc5/port_ocean/core/event_listener/sample/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0rc5/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0rc5/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/sync.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.0rc5/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/ocean_types.py` & `port_ocean-0.1.0rc5/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/core/utils.py` & `port_ocean-0.1.0rc5/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/exceptions/core.py` & `port_ocean-0.1.0rc5/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/logger_setup.py` & `port_ocean-0.1.0rc5/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/middlewares.py` & `port_ocean-0.1.0rc5/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/ocean.py` & `port_ocean-0.1.0rc5/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/port_defaults.py` & `port_ocean-0.1.0rc5/port_ocean/port_defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,17 +179,20 @@
 
         raise ExceptionGroup(str(e), e.errors)
 
 
 def initialize_defaults(
     config_class: Type[PortAppConfig], integration_config: IntegrationConfiguration
 ) -> None:
-    asyncio.new_event_loop().run_until_complete(
-        _initialize_defaults(config_class, integration_config)
-    )
+    try:
+        asyncio.new_event_loop().run_until_complete(
+            _initialize_defaults(config_class, integration_config)
+        )
+    except Exception as e:
+        logger.debug(f"Failed to initialize defaults, skipping... Error: {e}")
 
 
 def get_port_integration_defaults(
     port_app_config_class: Type[PortAppConfig], base_path: Path = Path(".")
 ) -> Defaults | None:
     defaults_dir = base_path / ".port/resources"
     if not defaults_dir.exists():
@@ -217,10 +220,10 @@
                 default_jsons[path.stem] = json.loads(path.read_text())
 
     return Defaults(
         blueprints=default_jsons.get("blueprints", []),
         actions=default_jsons.get("actions", []),
         scorecards=default_jsons.get("scorecards", []),
         port_app_config=port_app_config_class(
-            **default_jsons.get("port_app_config", {})
+            **default_jsons.get("port-app-config", {})
         ),
     )
```

### Comparing `port_ocean-0.1.0rc4/port_ocean/run.py` & `port_ocean-0.1.0rc5/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/port_ocean/utils.py` & `port_ocean-0.1.0rc5/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc4/pyproject.toml` & `port_ocean-0.1.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.rc4"
+version = "0.1.0.rc5"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.0rc4/PKG-INFO` & `port_ocean-0.1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

