# Comparing `tmp/openedx-events-8.2.0.tar.gz` & `tmp/openedx-events-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-8.2.0.tar", last modified: Fri Jun 23 13:07:01 2023, max compression
+gzip compressed data, was "openedx-events-8.3.0.tar", last modified: Thu Jul 20 10:08:16 2023, max compression
```

## Comparing `openedx-events-8.2.0.tar` & `openedx-events-8.3.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-23 13:06:56.000000 openedx-events-8.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-23 13:06:56.000000 openedx-events-8.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-23 13:06:56.000000 openedx-events-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-06-23 13:07:01.404430 openedx-events-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-23 13:06:56.000000 openedx-events-8.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9087 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.400430 openedx-events-8.2.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-06-23 13:06:56.000000 openedx-events-8.2.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.396429 openedx-events-8.2.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-23 13:07:01.000000 openedx-events-8.2.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-23 13:06:56.000000 openedx-events-8.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-23 13:07:01.404430 openedx-events-8.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-06-23 13:06:56.000000 openedx-events-8.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 13:07:01.404430 openedx-events-8.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-23 13:06:56.000000 openedx-events-8.2.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.791386 openedx-events-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9658 2023-07-20 10:08:11.000000 openedx-events-8.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-20 10:08:11.000000 openedx-events-8.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-20 10:08:11.000000 openedx-events-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15686 2023-07-20 10:08:16.791386 openedx-events-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-07-20 10:08:11.000000 openedx-events-8.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7081 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11516 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12453 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9087 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-07-20 10:08:11.000000 openedx-events-8.3.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.783385 openedx-events-8.3.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15686 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 10:08:16.000000 openedx-events-8.3.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-20 10:08:11.000000 openedx-events-8.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-20 10:08:16.791386 openedx-events-8.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-07-20 10:08:11.000000 openedx-events-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:08:16.787385 openedx-events-8.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-20 10:08:11.000000 openedx-events-8.3.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-8.2.0/CHANGELOG.rst` & `openedx-events-8.3.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.3.0] - 2023-07-10
+--------------------
+Changed
+~~~~~~~
+* Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
+* Added new COURSE_CREATED event in content_authoring.
+* Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
+* Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
+
 [8.2.0] - 2023-06-08
 --------------------
 Changed
 ~~~~~~~
 * Added new USER_NOTIFICATION_REQUESTED event.
 
 [8.1.0] - 2023-06-06
```

### Comparing `openedx-events-8.2.0/LICENSE.txt` & `openedx-events-8.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/PKG-INFO` & `openedx-events-8.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.2.0
+Version: 8.3.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.3.0] - 2023-07-10
+--------------------
+Changed
+~~~~~~~
+* Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
+* Added new COURSE_CREATED event in content_authoring.
+* Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
+* Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
+
 [8.2.0] - 2023-06-08
 --------------------
 Changed
 ~~~~~~~
 * Added new USER_NOTIFICATION_REQUESTED event.
 
 [8.1.0] - 2023-06-06
```

### Comparing `openedx-events-8.2.0/README.rst` & `openedx-events-8.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/content_authoring/data.py` & `openedx-events-8.3.0/openedx_events/content_authoring/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 (see deprecation proposal at https://github.com/openedx/public-engineering/issues/160)
 """
 from datetime import datetime
 from typing import BinaryIO, List
 
 import attr
 from opaque_keys.edx.keys import CourseKey, UsageKey
+from opaque_keys.edx.locator import LibraryLocatorV2, LibraryUsageLocatorV2
+
+
+@attr.s(frozen=True)
+class CourseData:
+    """
+    Attributes defined for Open edX Course object.
+
+    Arguments:
+        course_key (CourseKey): identifier of the Course object.
+    """
+
+    course_key = attr.ib(type=CourseKey)
 
 
 @attr.s(frozen=True)
 class CourseScheduleData:
     """
     Data describing course scheduling.
 
@@ -61,18 +74,21 @@
 class XBlockData:
     """
     Data about changed XBlock.
 
     Arguments:
         usage_key (UsageKey): identifier of the XBlock object.
         block_type (str): type of block.
+        version (UsageKey): identifier of the XBlock object with branch and version data (optional). This
+        could be used to get the exact version of the XBlock object.
     """
 
     usage_key = attr.ib(type=UsageKey)
     block_type = attr.ib(type=str)
+    version = attr.ib(type=UsageKey, default=None, kw_only=True)
 
 
 @attr.s(frozen=True)
 class DuplicatedXBlockData(XBlockData):
     """
     Data about duplicated XBlock.
 
@@ -132,7 +148,35 @@
     """
 
     certificate_type = attr.ib(type=str)
     course_key = attr.ib(type=CourseKey)
     title = attr.ib(type=str)
     signatories = attr.ib(type=List[CertificateSignatoryData], factory=list)
     is_active = attr.ib(type=bool, default=False)
+
+
+@attr.s(frozen=True)
+class ContentLibraryData:
+    """
+    Data about changed ContentLibrary.
+
+    Arguments:
+        library_key (LibraryLocatorV2): a key that represents a Blockstore-based content library.
+        update_blocks (bool): flag that indicates whether the content library blocks indexes should be updated
+    """
+
+    library_key = attr.ib(type=LibraryLocatorV2)
+    update_blocks = attr.ib(type=bool, default=False)
+
+
+@attr.s(frozen=True)
+class LibraryBlockData:
+    """
+    Data about changed LibraryBlock.
+
+    Arguments:
+        library_key (LibraryLocatorV2): a key that represents a Blockstore-based content library.
+        usage_key (LibraryUsageLocatorV2): a key that represents a XBlock in a Blockstore-based content library.
+    """
+
+    library_key = attr.ib(type=LibraryLocatorV2)
+    usage_key = attr.ib(type=LibraryUsageLocatorV2)
```

### Comparing `openedx-events-8.2.0/openedx_events/data.py` & `openedx-events-8.3.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/__init__.py` & `openedx-events-8.3.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 Classes to serialize and deserialize custom types used by openedx events. See README for usage.
 """
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 from opaque_keys.edx.keys import CourseKey, UsageKey
+from opaque_keys.edx.locator import LibraryLocatorV2, LibraryUsageLocatorV2
 
 from openedx_events.event_bus.avro.types import PYTHON_TYPE_TO_AVRO_MAPPING
 
 
 class BaseCustomTypeAvroSerializer(ABC):
     """
     Used by openedx_events.avro_utilities class to serialize/deserialize custom types.
@@ -86,8 +87,52 @@
 
     @staticmethod
     def deserialize(data: str):
         """Deserialize string into obj."""
         return UsageKey.from_string(data)
 
 
-DEFAULT_CUSTOM_SERIALIZERS = [CourseKeyAvroSerializer, DatetimeAvroSerializer, UsageKeyAvroSerializer]
+class LibraryLocatorV2AvroSerializer(BaseCustomTypeAvroSerializer):
+    """
+    CustomTypeAvroSerializer for LibraryLocatorV2 class.
+    """
+
+    cls = LibraryLocatorV2
+    field_type = PYTHON_TYPE_TO_AVRO_MAPPING[str]
+
+    @staticmethod
+    def serialize(obj) -> str:
+        """Serialize obj into string."""
+        return str(obj)
+
+    @staticmethod
+    def deserialize(data: str):
+        """Deserialize string into obj."""
+        return LibraryLocatorV2.from_string(data)
+
+
+class LibraryUsageLocatorV2AvroSerializer(BaseCustomTypeAvroSerializer):
+    """
+    CustomTypeAvroSerializer for LibraryUsageLocatorV2 class.
+    """
+
+    cls = LibraryUsageLocatorV2
+    field_type = PYTHON_TYPE_TO_AVRO_MAPPING[str]
+
+    @staticmethod
+    def serialize(obj) -> str:
+        """Serialize obj into string."""
+        return str(obj)
+
+    @staticmethod
+    def deserialize(data: str):
+        """Deserialize string into obj."""
+        return LibraryUsageLocatorV2.from_string(data)
+
+
+DEFAULT_CUSTOM_SERIALIZERS = [
+    CourseKeyAvroSerializer,
+    DatetimeAvroSerializer,
+    LibraryLocatorV2AvroSerializer,
+    LibraryUsageLocatorV2AvroSerializer,
+    UsageKeyAvroSerializer,
+]
```

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import List
 from unittest import TestCase
 
 from fastavro import schemaless_reader, schemaless_writer
 from fastavro.repository.base import SchemaRepositoryError
 from fastavro.schema import load_schema
 from opaque_keys.edx.keys import CourseKey, UsageKey
+from opaque_keys.edx.locator import LibraryLocatorV2, LibraryUsageLocatorV2
 
 from openedx_events.event_bus.avro.deserializer import AvroSignalDeserializer, deserialize_bytes_to_event_data
 from openedx_events.event_bus.avro.serializer import AvroSignalSerializer, serialize_event_data_to_bytes
 from openedx_events.event_bus.avro.tests.test_utilities import (
     EventData,
     NestedAttrsWithDefaults,
     SimpleAttrsWithDefaults,
@@ -98,14 +99,16 @@
         bool: True,
         str: "default",
         float: 1.0,
         CourseKey: CourseKey.from_string("course-v1:edX+DemoX.1+2014"),
         UsageKey: UsageKey.from_string(
             "block-v1:edx+DemoX+Demo_course+type@video+block@UaEBjyMjcLW65gaTXggB93WmvoxGAJa0JeHRrDThk",
         ),
+        LibraryLocatorV2: LibraryLocatorV2.from_string('lib:MITx:reallyhardproblems'),
+        LibraryUsageLocatorV2: LibraryUsageLocatorV2.from_string('lb:MITx:reallyhardproblems:problem:problem1'),
         List[int]: [1, 2, 3],
         datetime: datetime.now(),
     }
     data_dict = {}
     for attribute in data_type.__attrs_attrs__:
         result = defaults_per_type.get(attribute.type, None)
         if result is not None:
```

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for avro.deserializer"""
 import json
 from datetime import datetime
 from typing import List
 from unittest import TestCase
 
 from opaque_keys.edx.keys import CourseKey, UsageKey
+from opaque_keys.edx.locator import LibraryLocatorV2, LibraryUsageLocatorV2
 
 from openedx_events.event_bus.avro.deserializer import AvroSignalDeserializer, deserialize_bytes_to_event_data
 from openedx_events.event_bus.avro.tests.test_utilities import (
     EventData,
     NestedAttrsWithDefaults,
     NestedNonAttrs,
     NonAttrs,
@@ -115,14 +116,40 @@
         )
         as_dict = {"usage_key": str(usage_key)}
         event_data = deserializer.from_dict(as_dict)
         usage_key_deserialized = event_data["usage_key"]
         self.assertIsInstance(usage_key_deserialized, UsageKey)
         self.assertEqual(usage_key_deserialized, usage_key)
 
+    def test_default_librarylocatorv2_deserialization(self):
+        """
+        Test deserialization of LibraryLocatorV2
+        """
+        SIGNAL = create_simple_signal({"library_key": LibraryLocatorV2})
+        deserializer = AvroSignalDeserializer(SIGNAL)
+        library_key = LibraryLocatorV2.from_string("lib:MITx:reallyhardproblems")
+        as_dict = {"library_key": str(library_key)}
+        event_data = deserializer.from_dict(as_dict)
+        library_key_deserialized = event_data["library_key"]
+        self.assertIsInstance(library_key_deserialized, LibraryLocatorV2)
+        self.assertEqual(library_key_deserialized, library_key)
+
+    def test_default_libraryusagelocatorv2_deserialization(self):
+        """
+        Test deserialization of LibraryUsageLocatorV2
+        """
+        SIGNAL = create_simple_signal({"usage_key": LibraryUsageLocatorV2})
+        deserializer = AvroSignalDeserializer(SIGNAL)
+        usage_key = LibraryUsageLocatorV2.from_string("lb:MITx:reallyhardproblems:problem:problem1")
+        as_dict = {"usage_key": str(usage_key)}
+        event_data = deserializer.from_dict(as_dict)
+        usage_key_deserialized = event_data["usage_key"]
+        self.assertIsInstance(usage_key_deserialized, LibraryUsageLocatorV2)
+        self.assertEqual(usage_key_deserialized, usage_key)
+
     def test_deserialization_with_custom_serializer(self):
         SIGNAL = create_simple_signal({"test_data": NonAttrs})
         deserializer = SpecialDeserializer(SIGNAL)
         as_dict = {
             "test_data": "a.val:a.nother.val"
         }
         event_data = deserializer.from_dict(as_dict)
```

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import json
 from datetime import datetime
 
 import pytest
 from django.test import TestCase
 from opaque_keys.edx.keys import CourseKey, UsageKey
+from opaque_keys.edx.locator import LibraryLocatorV2, LibraryUsageLocatorV2
 
 from openedx_events.event_bus.avro.serializer import AvroSignalSerializer, serialize_event_data_to_bytes
 from openedx_events.event_bus.avro.tests.test_utilities import (
     CustomAttrsWithDefaults,
     CustomAttrsWithoutDefaults,
     EventData,
     NestedAttrsWithDefaults,
@@ -115,14 +116,36 @@
         usage_key = UsageKey.from_string(
             "block-v1:edx+DemoX+Demo_course+type@video+block@UaEBjyMjcLW65gaTXggB93WmvoxGAJa0JeHRrDThk",
         )
         test_data = {"usage_key": usage_key}
         data_dict = serializer.to_dict(test_data)
         self.assertDictEqual(data_dict, {"usage_key": str(usage_key)})
 
+    def test_default_librarylocatorv2_serialization(self):
+        """
+        Test serialization of LibraryLocatorV2
+        """
+        SIGNAL = create_simple_signal({"library_key": LibraryLocatorV2})
+        serializer = AvroSignalSerializer(SIGNAL)
+        library_key = LibraryLocatorV2.from_string("lib:MITx:reallyhardproblems")
+        test_data = {"library_key": library_key}
+        data_dict = serializer.to_dict(test_data)
+        self.assertDictEqual(data_dict, {"library_key": str(library_key)})
+
+    def test_default_libraryusagelocatorv2_serialization(self):
+        """
+        Test serialization of LibraryUsageLocatorV2
+        """
+        SIGNAL = create_simple_signal({"usage_key": LibraryUsageLocatorV2})
+        serializer = AvroSignalSerializer(SIGNAL)
+        usage_key = LibraryUsageLocatorV2.from_string("lb:MITx:reallyhardproblems:problem:problem1")
+        test_data = {"usage_key": usage_key}
+        data_dict = serializer.to_dict(test_data)
+        self.assertDictEqual(data_dict, {"usage_key": str(usage_key)})
+
     def test_serialization_with_custom_serializer(self):
         SIGNAL = create_simple_signal({"test_data": NonAttrs})
 
         serializer = SpecialSerializer(SIGNAL)
         test_data = {
             "test_data": NonAttrs("a.val", "a.nother.val")
         }
```

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-8.3.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-8.3.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/exceptions.py` & `openedx-events-8.3.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/learning/data.py` & `openedx-events-8.3.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/learning/signals.py` & `openedx-events-8.3.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/management/commands/consume_events.py` & `openedx-events-8.3.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-8.3.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-8.3.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-8.3.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/tests/test_tooling.py` & `openedx-events-8.3.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/tests/utils.py` & `openedx-events-8.3.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/tooling.py` & `openedx-events-8.3.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events/utils.py` & `openedx-events-8.3.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-8.3.0/openedx_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.2.0
+Version: 8.3.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,23 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.3.0] - 2023-07-10
+--------------------
+Changed
+~~~~~~~
+* Added new XBLOCK_CREATED and XBLOCK_UPDATED events in content_authoring.
+* Added new COURSE_CREATED event in content_authoring.
+* Added new CONTENT_LIBRARY_CREATED, CONTENT_LIBRARY_UPDATED and CONTENT_LIBRARY_DELETED events in content_authoring.
+* Added new LIBRARY_BLOCK_CREATED, LIBRARY_BLOCK_UPDATED and LIBRARY_BLOCK_DELETED events in content_authoring.
+
 [8.2.0] - 2023-06-08
 --------------------
 Changed
 ~~~~~~~
 * Added new USER_NOTIFICATION_REQUESTED event.
 
 [8.1.0] - 2023-06-06
```

### Comparing `openedx-events-8.2.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-8.3.0/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.2.0/setup.py` & `openedx-events-8.3.0/setup.py`

 * *Files identical despite different names*

