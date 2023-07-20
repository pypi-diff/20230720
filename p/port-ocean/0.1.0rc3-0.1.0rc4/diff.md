# Comparing `tmp/port_ocean-0.1.0rc3.tar.gz` & `tmp/port_ocean-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0rc3.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0rc4.tar", max compression
```

## Comparing `port_ocean-0.1.0rc3.tar` & `port_ocean-0.1.0rc4.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0    11357 2023-07-19 11:57:29.412104 port_ocean-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0     4585 2023-07-19 11:57:29.412104 port_ocean-0.1.0rc3/README.md
--rw-r--r--   0        0        0      255 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/__init__.py
--rw-r--r--   0        0        0      321 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5561 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
--rw-r--r--   0        0        0       12 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      598 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      653 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
--rw-r--r--   0        0        0      778 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1302 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      722 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2398 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     3049 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5681 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3866 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/config/base.py
--rw-r--r--   0        0        0     1053 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1116 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4058 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/context/event.py
--rw-r--r--   0        0        0     4050 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/base.py
--rw-r--r--   0        0        0      593 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      560 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3083 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     3123 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/sample/__init__.py
--rw-r--r--   0        0        0     1852 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/sample/event_listener.py
--rw-r--r--   0        0        0     2799 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/event_listener/sample/utils.py
--rw-r--r--   0        0        0      716 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      863 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7855 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1339 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      949 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2679 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1912 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11334 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/models.py
--rw-r--r--   0        0        0      563 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/types.py
--rw-r--r--   0        0        0     1916 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-19 11:57:29.440104 port_ocean-0.1.0rc3/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0      554 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2266 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/ocean.py
--rw-r--r--   0        0        0     7212 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/py.typed
--rw-r--r--   0        0        0     2837 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/port_ocean/utils.py
--rw-r--r--   0        0        0     2735 2023-07-19 11:57:29.444104 port_ocean-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 10:20:22.111079 port_ocean-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0     4585 2023-07-20 10:20:22.111079 port_ocean-0.1.0rc4/README.md
+-rw-r--r--   0        0        0      255 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5561 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/defaults/.gitignore
+-rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      598 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      653 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
+-rw-r--r--   0        0        0      778 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-20 10:20:22.143081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1302 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      722 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2398 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     3049 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5681 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3866 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2277 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1218 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1107 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4286 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/base.py
+-rw-r--r--   0        0        0      593 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3083 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     3147 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/utils.py
+-rw-r--r--   0        0        0      716 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7949 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11831 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1683 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0      588 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0      554 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2266 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7234 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/py.typed
+-rw-r--r--   0        0        0     2837 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/port_ocean/utils.py
+-rw-r--r--   0        0        0     2736 2023-07-20 10:20:22.147081 port_ocean-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     6204 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc4/PKG-INFO
```

### Comparing `port_ocean-0.1.0rc3/LICENSE` & `port_ocean-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/README.md` & `port_ocean-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/commands.py` & `port_ocean-0.1.0rc4/port_ocean/cli/commands.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0rc4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0rc4/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0rc4/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/client.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/clients/port/types.py` & `port_ocean-0.1.0rc4/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/config/base.py` & `port_ocean-0.1.0rc4/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/config/dynamic.py` & `port_ocean-0.1.0rc4/port_ocean/config/dynamic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Type, Any
+from typing import Type, Any, Optional
 
 from pydantic import BaseModel, AnyUrl, create_model, Extra, parse_obj_as
 
 
 class Configuration(BaseModel, extra=Extra.allow):
     name: str
     type: str
     required: bool = False
+    default: Optional[Any]
 
 
 def default_config_factory(configurations: Any) -> Type[BaseModel]:
     configurations = parse_obj_as(list[Configuration], configurations)
     fields: dict[str, tuple[Any, Any]] = {}
 
     for config in configurations:
@@ -26,13 +27,16 @@
             case "integer":
                 field_type = int
             case "boolean":
                 field_type = bool
             case _:
                 raise ValueError(f"Unknown type: {config.type}")
 
+        default = ... if config.required else None
+        if config.default is not None:
+            default = parse_obj_as(field_type, config.default)
         fields[config.name] = (
             field_type,
-            ... if config.required else None,
+            default,
         )
 
     return create_model("Config", **fields)  # type: ignore
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/config/integration.py` & `port_ocean-0.1.0rc4/port_ocean/config/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     type: str
     config: dict[str, Any]
 
 
 class IntegrationConfiguration(BaseOceanSettings):
     port: PortSettings
     event_listener: EventListenerSettingsType = Field(alias="eventListener")
-    batch_work_size: int | None = Field(alias="batchWorkSize", default=None)
+    batch_work_size: int = Field(alias="batchWorkSize", default=20)
     initialize_port_resources: bool = Field(
         alias="initializePortResources", default=False
     )
     integration: IntegrationSettings
 
 
 LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0rc4/port_ocean/consumers/kafka_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,17 @@
                 await self.msg_process(message, topic)
             except Exception as e:
                 _type, _, tb = sys.exc_info()
                 logger.opt(exception=(_type, None, tb)).error(
                     f"Failed to process message: {str(e)}"
                 )
 
-        asyncio.run(try_wrapper())
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        loop.run_until_complete(try_wrapper())
 
     def start(self) -> None:
         try:
             logger.info("Start consumer...")
 
             self.consumer.subscribe(
                 [f"{self.org_id}.change.log"],
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/context/event.py` & `port_ocean-0.1.0rc4/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/context/ocean.py` & `port_ocean-0.1.0rc4/port_ocean/context/ocean.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from typing import Callable, TYPE_CHECKING, Any
 
 from fastapi import APIRouter
 from werkzeug.local import LocalProxy, LocalStack
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.models import Entity
-from port_ocean.core.types import (
+from port_ocean.core.ocean_types import (
     RESYNC_EVENT_LISTENER,
     START_EVENT_LISTENER,
     RawEntityDiff,
+    EntityDiff,
 )
 from port_ocean.exceptions.context import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
     from port_ocean.config.integration import IntegrationConfiguration
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.ocean import Ocean
@@ -63,14 +64,21 @@
         self,
         kind: str,
         raw_diff: RawEntityDiff,
         user_agent_type: UserAgentType = UserAgentType.exporter,
     ) -> None:
         await self.integration.update_raw_diff(kind, raw_diff, user_agent_type)
 
+    async def update_diff(
+        self,
+        diff: EntityDiff,
+        user_agent_type: UserAgentType = UserAgentType.exporter,
+    ) -> None:
+        await self.integration.update_diff(diff, user_agent_type)
+
     async def register_raw(
         self,
         kind: str,
         change: list[dict[str, Any]],
         user_agent_type: UserAgentType = UserAgentType.exporter,
     ) -> None:
         await self.integration.register_raw(kind, change, user_agent_type)
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/factory.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/http/event_listener.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/http/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/kafka/event_listener.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/kafka/event_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         return False
 
     async def _handle_message(self, message: dict[Any, Any], topic: str) -> None:
         if not self.should_be_processed(message, topic):
             return
 
-        if "change.log" in topic:
+        if "change.log" in topic and message is not None:
             await self.events["on_resync"](message)
 
     def wrapped_start(
         self, context: PortOceanContext, func: Callable[[], None]
     ) -> Callable[[], None]:
         ocean_app = context.app
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/sample/event_listener.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/event_listener.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/event_listener/sample/utils.py` & `port_ocean-0.1.0rc4/port_ocean/core/event_listener/sample/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.models import Entity
-from port_ocean.core.types import EntityDiff
+from port_ocean.core.ocean_types import EntityDiff
 
 
 class BaseEntitiesStateApplier(BaseWithContext):
     @abstractmethod
     async def apply_diff(
         self,
         entities: EntityDiff,
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     order_by_entities_dependencies,
 )
 from port_ocean.core.handlers.entities_state_applier.port.validate_entity_relations import (
     validate_entity_relations,
 )
 from port_ocean.core.handlers.entity_processor.base import EntityPortDiff
 from port_ocean.core.models import Entity
-from port_ocean.core.types import EntityDiff
+from port_ocean.core.ocean_types import EntityDiff
 from port_ocean.core.utils import is_same_entity, get_unique, get_port_diff
 from port_ocean.exceptions.core import RelationValidationException
 
 
 class HttpEntitiesStateApplier(BaseEntitiesStateApplier):
     async def _validate_delete_dependent_entities(self, entities: list[Entity]) -> None:
         logger.info("Validated deleted entities")
@@ -49,15 +49,15 @@
                 )
 
     async def _validate_entity_diff(self, diff: EntityPortDiff) -> None:
         config = event.port_app_config
         await self._validate_delete_dependent_entities(diff.deleted)
         modified_or_created_entities = diff.modified + diff.created
 
-        if modified_or_created_entities:
+        if modified_or_created_entities and not config.create_missing_related_entities:
             logger.info("Validating modified or created entities")
 
             await asyncio.gather(
                 *(
                     self.context.port_client.validate_entity_payload(
                         entity,
                         {
@@ -158,15 +158,16 @@
                     self.context.port_client.upsert_entity(
                         entity,
                         event.port_app_config.get_port_request_options(),
                         user_agent_type,
                         silent=True,
                     )
                     for entity in entities
-                )
+                ),
+                return_exceptions=True,
             )
         else:
             ordered_created_entities = reversed(
                 order_by_entities_dependencies(entities)
             )
 
             for entity in ordered_created_entities:
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass, field
 
 from loguru import logger
 
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
-from port_ocean.core.types import RawEntityDiff, EntityDiff
+from port_ocean.core.ocean_types import RawEntityDiff, EntityDiff
 
 
 @dataclass
 class EntityPortDiff:
     deleted: list[Entity] = field(default_factory=list)
     modified: list[Entity] = field(default_factory=list)
     created: list[Entity] = field(default_factory=list)
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 
 import pyjq as jq  # type: ignore
 
 from port_ocean.core.handlers.entity_processor.base import BaseEntityProcessor
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
-from port_ocean.core.types import RawEntityDiff, EntityDiff
+from port_ocean.core.ocean_types import RawEntityDiff, EntityDiff
 from port_ocean.exceptions.core import EntityProcessorException
 
 
 class JQEntityProcessor(BaseEntityProcessor):
     @lru_cache
     def _compile(self, pattern: str) -> Any:
         return jq.compile(pattern)
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0rc4/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0rc4/port_ocean/core/integrations/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 
-from port_ocean.core.types import (
+from port_ocean.core.ocean_types import (
     IntegrationEventsCallbacks,
     START_EVENT_LISTENER,
     RESYNC_EVENT_LISTENER,
 )
 
 
 class EventsMixin:
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0rc4/port_ocean/core/integrations/mixins/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 import asyncio
-from itertools import chain
-from typing import Any, Awaitable
+import inspect
+import typing
+from typing import Any, Awaitable, Callable
 
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import TriggerType, event_context, EventType
 from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
+from port_ocean.core.integrations.mixins.utils import (
+    resync_function_wrapper,
+    resync_generator_wrapper,
+)
 from port_ocean.core.models import Entity
-from port_ocean.core.types import RawEntityDiff, EntityDiff, RESYNC_EVENT_LISTENER
-from port_ocean.core.utils import validate_result, zip_and_sum
-from port_ocean.exceptions.core import RawObjectValidationException, OceanAbortException
-from port_ocean.utils import get_function_location
+from port_ocean.core.ocean_types import (
+    RawEntityDiff,
+    EntityDiff,
+    RESYNC_RESULT,
+    RAW_RESULT,
+    RESYNC_EVENT_LISTENER,
+    ASYNC_GENERATOR_RESYNC_TYPE,
+)
+from port_ocean.core.utils import zip_and_sum
+from port_ocean.exceptions.core import OceanAbortException
 
 
-class SyncMixin(HandlerMixin, EventsMixin):
+class SyncMixin(HandlerMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
-        EventsMixin.__init__(self)
+
+    async def update_diff(
+        self,
+        desired_state: EntityDiff,
+        user_agent_type: UserAgentType,
+    ) -> None:
+        await self.entities_state_applier.apply_diff(
+            {"before": desired_state["before"], "after": desired_state["after"]},
+            user_agent_type,
+        )
 
     async def register(
         self,
         entities: list[Entity],
         user_agent_type: UserAgentType,
     ) -> None:
         await self.entities_state_applier.upsert(entities, user_agent_type)
@@ -52,78 +72,66 @@
 
 
 class SyncRawMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
         EventsMixin.__init__(self)
 
-    async def _on_resync(self, kind: str) -> list[dict[Any, Any]]:
+    async def _on_resync(self, kind: str) -> RAW_RESULT:
         raise NotImplementedError("on_resync must be implemented")
 
     async def _calculate_raw(
         self, raw_diff: list[tuple[ResourceConfig, RawEntityDiff]]
     ) -> list[EntityDiff]:
         logger.info("Calculating diff in entities between states")
         return await asyncio.gather(
             *(
                 self.entity_processor.parse_items(mapping, results)
                 for mapping, results in raw_diff
             )
         )
 
-    async def _resync_function_wrapper(
-        self, fn: RESYNC_EVENT_LISTENER, kind: str
-    ) -> list[dict[str, Any]]:
-        try:
-            results = await fn(kind)
-            return validate_result(results)
-        except RawObjectValidationException as error:
-            raise OceanAbortException(
-                f"Failed to validate raw data for returned data from {get_function_location(fn)}, error: {error}"
-            ) from error
-        except Exception as error:
-            raise OceanAbortException(
-                f"Failed to execute {get_function_location(fn)}, error: {error}"
-            ) from error
-
     async def _get_resource_raw_results(
         self, resource_config: ResourceConfig
-    ) -> tuple[list[dict[str, Any]], list[Exception]]:
+    ) -> tuple[RESYNC_RESULT, list[Exception]]:
         logger.info(f"Fetching {resource_config.kind} resync results")
-        tasks: list[Awaitable[list[dict[Any, Any]]]] = []
+        tasks: list[Awaitable[RAW_RESULT]] = []
         with logger.contextualize(kind=resource_config.kind):
-            if self.__class__._on_resync != SyncRawMixin._on_resync:
-                tasks.append(
-                    self._resync_function_wrapper(self._on_resync, resource_config.kind)
-                )
-
-            fns = [
+            fns: list[RESYNC_EVENT_LISTENER] = [
                 *self.event_strategy["resync"][resource_config.kind],
                 *self.event_strategy["resync"][None],
             ]
 
-            tasks.extend(
-                [
-                    self._resync_function_wrapper(resync_function, resource_config.kind)
-                    for resync_function in fns
-                ]
+            if self.__class__._on_resync != SyncRawMixin._on_resync:
+                fns.append(self._on_resync)
+
+            results: RESYNC_RESULT = []
+            for task in fns:
+                if inspect.isasyncgenfunction(task):
+                    results.append(resync_generator_wrapper(task, resource_config.kind))
+                else:
+                    task = typing.cast(Callable[[str], Awaitable[RAW_RESULT]], task)
+                    tasks.append(resync_function_wrapper(task, resource_config.kind))
+
+            logger.info(
+                f"Found {len(tasks) + len(results)} resync tasks for {resource_config.kind}"
             )
 
-            logger.info(f"Found {len(tasks)} resync tasks for {resource_config.kind}")
-
-            results_with_error: list[
-                list[dict[Any, Any]] | Exception
-            ] = await asyncio.gather(*tasks, return_exceptions=True)
-            results: list[dict[Any, Any]] = list(
-                chain.from_iterable(
+            results_with_error: list[RAW_RESULT | Exception] = await asyncio.gather(
+                *tasks,
+                return_exceptions=True,
+            )
+            results.extend(
+                sum(
                     [
                         result
                         for result in results_with_error
                         if not isinstance(result, Exception)
-                    ]
+                    ],
+                    [],
                 )
             )
 
             errors = [
                 result for result in results_with_error if isinstance(result, Exception)
             ]
 
@@ -177,34 +185,50 @@
         logger.info("Finished unregistering change")
         return entities_after
 
     async def _register_in_batches(
         self,
         resource_config: ResourceConfig,
         user_agent_type: UserAgentType,
-        batch_work_size: int | None,
+        batch_work_size: int,
     ) -> tuple[list[Entity], list[Exception]]:
         results, errors = await self._get_resource_raw_results(resource_config)
+        async_generators: list[ASYNC_GENERATOR_RESYNC_TYPE] = []
+        raw_results: RAW_RESULT = []
+        for result in results:
+            if isinstance(result, dict):
+                raw_results.append(result)
+            else:
+                async_generators.append(result)
 
-        tasks = []
-
-        batch_size = batch_work_size or len(results) or 1
         batches = [
-            results[i : i + batch_size] for i in range(0, len(results), batch_size)
+            raw_results[i : i + batch_work_size]
+            for i in range(0, len(raw_results), batch_work_size)
         ]
-        for batch in batches:
-            logger.info(f"Creating task for registering batch of {len(batch)} entities")
-            tasks.append(
+
+        registered_entities_results = await asyncio.gather(
+            *(
                 self._register_resource_raw(resource_config, batch, user_agent_type)
+                for batch in batches
             )
+        )
+        for generator in async_generators:
+            try:
+                async for item in generator:
+                    registered_entities_results.append(
+                        await self._register_resource_raw(
+                            resource_config, [item], user_agent_type
+                        )
+                    )
+            except* OceanAbortException as error:
+                errors.append(error)
 
-        registered_entities_results = await asyncio.gather(*tasks)
         entities: list[Entity] = sum(registered_entities_results, [])
         logger.info(
-            f"Finished registering change for {len(results)} raw results for kind: {resource_config.kind}"
+            f"Finished registering change for {len(results)} raw results for kind: {resource_config.kind}. {len(entities)} entities were affected"
         )
         return entities, errors
 
     async def register_raw(
         self,
         kind: str,
         results: list[dict[Any, Any]],
@@ -282,34 +306,31 @@
         logger.info("Resync was triggered")
 
         async with event_context(EventType.RESYNC, trigger_type=trigger_type):
             app_config = await self.port_app_config_handler.get_port_app_config()
 
             entities_at_port = await ocean.port_client.search_entities(user_agent_type)
 
-            creation_results: list[
-                tuple[list[Entity], list[Exception]]
-            ] = await asyncio.gather(
-                *(
-                    self._register_in_batches(
+            creation_results: list[tuple[list[Entity], list[Exception]]] = []
+            for resource in app_config.resources:
+                creation_results.append(
+                    await self._register_in_batches(
                         resource, user_agent_type, ocean.config.batch_work_size
                     )
-                    for resource in app_config.resources
                 )
-            )
             flat_created_entities, errors = zip_and_sum(creation_results)
 
-            if not errors:
+            if errors:
+                message = f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state"
+                error_group = ExceptionGroup(
+                    f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state",
+                    errors,
+                )
+                if not silent:
+                    raise error_group
+
+                logger.error(message, exc_info=error_group)
+            else:
                 await self.entities_state_applier.delete_diff(
                     {"before": entities_at_port, "after": flat_created_entities},
                     user_agent_type,
                 )
-
-            message = f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state"
-            error_group = ExceptionGroup(
-                f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state",
-                errors,
-            )
-            if not silent:
-                raise error_group
-
-            logger.error(message, exc_info=error_group)
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/models.py` & `port_ocean-0.1.0rc4/port_ocean/core/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class Entity(BaseModel):
     identifier: str
     blueprint: str
     title: str | None
     team: str | list[str] = []
     properties: dict[str, Any] = {}
-    relations: dict[str, str] = {}
+    relations: dict[str, Any] = {}
 
 
 class BlueprintRelation(BaseModel):
     many: bool
     required: bool
     target: str
     title: str | None
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/core/utils.py` & `port_ocean-0.1.0rc4/port_ocean/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Iterable, Any, TypeVar
 
 from pydantic import parse_obj_as, ValidationError
 
 from port_ocean.core.handlers.entity_processor.base import EntityPortDiff
 from port_ocean.core.models import Entity
+from port_ocean.core.ocean_types import RAW_RESULT
 from port_ocean.exceptions.core import RawObjectValidationException
 
 T = TypeVar("T", bound=tuple[list[Any], ...])
 
 
 def zip_and_sum(collection: Iterable[T]) -> T:
     return tuple(sum(items, []) for items in zip(*collection))  # type: ignore
 
 
-def validate_result(result: Any) -> list[dict[str, Any]]:
+def validate_result(result: Any) -> RAW_RESULT:
     try:
         return parse_obj_as(list[dict[str, Any]], result)
     except ValidationError as e:
         raise RawObjectValidationException(f"Expected list[dict[str, Any]], Error: {e}")
 
 
 def is_same_entity(first_entity: Entity, second_entity: Entity) -> bool:
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/exceptions/core.py` & `port_ocean-0.1.0rc4/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/logger_setup.py` & `port_ocean-0.1.0rc4/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/middlewares.py` & `port_ocean-0.1.0rc4/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/ocean.py` & `port_ocean-0.1.0rc4/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/port_defaults.py` & `port_ocean-0.1.0rc4/port_ocean/port_defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import json
-from pathlib import Path
 from typing import Type, Any, TypedDict, Optional
 
 import httpx
 import yaml
 from loguru import logger
+from pathlib import Path
 from pydantic import BaseModel, Field
 from starlette import status
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 from port_ocean.exceptions.port_defaults import (
@@ -209,15 +209,16 @@
             raise UnsupportedDefaultFileType(
                 f"Defaults directory should contain only one of the next types: {ALLOWED_FILE_TYPES}. Found: {path}"
             )
 
         if path.stem in allowed_file_names:
             if path.suffix in YAML_EXTENSIONS:
                 default_jsons[path.stem] = yaml.safe_load(path.read_text())
-            default_jsons[path.stem] = json.loads(path.read_text())
+            else:
+                default_jsons[path.stem] = json.loads(path.read_text())
 
     return Defaults(
         blueprints=default_jsons.get("blueprints", []),
         actions=default_jsons.get("actions", []),
         scorecards=default_jsons.get("scorecards", []),
         port_app_config=port_app_config_class(
             **default_jsons.get("port_app_config", {})
```

### Comparing `port_ocean-0.1.0rc3/port_ocean/run.py` & `port_ocean-0.1.0rc4/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/port_ocean/utils.py` & `port_ocean-0.1.0rc4/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0rc3/pyproject.toml` & `port_ocean-0.1.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.rc3"
+version = "0.1.0.rc4"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
@@ -72,15 +72,15 @@
 filename = "CHANGELOG.md"
 package = "port_ocean"
 
 [tool.mypy]
 exclude = [
     'port_ocean/cli/cookiecutter',
     'venv',
-    '.venv',
+    '\.venv',
     'integrations'
 ]
 plugins = [
     "pydantic.mypy"
 ]
 
 follow_imports = "silent"
```

### Comparing `port_ocean-0.1.0rc3/PKG-INFO` & `port_ocean-0.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

