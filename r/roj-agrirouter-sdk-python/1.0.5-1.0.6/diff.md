# Comparing `tmp/roj-agrirouter-sdk-python-1.0.5.tar.gz` & `tmp/roj-agrirouter-sdk-python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roj-agrirouter-sdk-python-1.0.5.tar", last modified: Thu Jul 20 12:02:44 2023, max compression
+gzip compressed data, was "roj-agrirouter-sdk-python-1.0.6.tar", last modified: Thu Jul 20 12:47:41 2023, max compression
```

## Comparing `roj-agrirouter-sdk-python-1.0.5.tar` & `roj-agrirouter-sdk-python-1.0.6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      997 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/
--rw-rw-r--   0 user      (1000) user      (1000)     1084 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1356 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/auth.py
--rw-rw-r--   0 user      (1000) user      (1000)     3233 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)      303 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      198 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1235 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     3087 2023-06-15 10:00:14.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/response.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/constants/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/constants/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/constants/media_types.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      508 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/environmental_services.py
--rw-rw-r--   0 user      (1000) user      (1000)     2578 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/environments.py
--rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1363 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/keys.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/cloud_provider_integration/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/cloud_provider_integration/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3522 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/chunk_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     7512 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/message_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/account/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/account/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4230 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/efdi/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/efdi/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)   306464 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9282 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     5278 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.048650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/feed/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/feed/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/gps/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/gps/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    14065 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     9916 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/request_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/account/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/account/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10371 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/endpoint/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/endpoint/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5137 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    37035 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)    12586 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py
--rw-rw-r--   0 user      (1000) user      (1000)     9214 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/response_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/settings/dh_settings_pb2.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     7442 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/builders.py
--rw-rw-r--   0 user      (1000) user      (1000)      571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/certification.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       30 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     2725 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/http.py
--rw-rw-r--   0 user      (1000) user      (1000)     5185 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/mqtt.py
--rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/decode.py
--rw-rw-r--   0 user      (1000) user      (1000)     2438 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/encode.py
--rw-rw-r--   0 user      (1000) user      (1000)     1053 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      441 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/messages.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3200 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)    18534 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/service.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     1571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/result.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.052650 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2986 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     3153 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/commons.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/http/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/http/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      757 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/http/outbox.py
--rw-rw-r--   0 user      (1000) user      (1000)    15502 2023-07-20 10:19:52.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/messaging.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6174 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/dto.py
--rw-rw-r--   0 user      (1000) user      (1000)      169 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/enums.py
--rw-rw-r--   0 user      (1000) user      (1000)      894 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/headers.py
--rw-rw-r--   0 user      (1000) user      (1000)     2376 2023-06-15 10:01:14.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/onboarding.py
--rw-rw-r--   0 user      (1000) user      (1000)     1653 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-06-15 10:01:38.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     2115 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/request_body.py
--rw-rw-r--   0 user      (1000) user      (1000)     6710 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     1035 2023-06-15 10:01:01.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/signature.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      801 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/headers.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     1006 2023-06-15 10:02:01.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/request.py
--rw-rw-r--   0 user      (1000) user      (1000)      860 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/request_body.py
--rw-rw-r--   0 user      (1000) user      (1000)      428 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     1734 2023-06-15 10:02:19.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/revoking.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1936 2023-05-31 09:35:47.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/type_url.py
--rw-rw-r--   0 user      (1000) user      (1000)      202 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/utc_time_util.py
--rw-rw-r--   0 user      (1000) user      (1000)       59 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/uuid_util.py
--rw-rw-r--   0 user      (1000) user      (1000)       90 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.5/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      997 2023-07-20 12:02:43.000000 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4370 2023-07-20 12:02:43.000000 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-20 12:02:43.000000 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      122 2023-07-20 12:02:43.000000 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       11 2023-07-20 12:02:43.000000 roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-20 12:02:44.056650 roj-agrirouter-sdk-python-1.0.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1388 2023-07-20 10:20:47.000000 roj-agrirouter-sdk-python-1.0.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.105928 roj-agrirouter-sdk-python-1.0.6/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-07-20 12:47:41.105928 roj-agrirouter-sdk-python-1.0.6/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.085928 roj-agrirouter-sdk-python-1.0.6/agrirouter/
+-rw-rw-r--   0 user      (1000) user      (1000)     1111 2023-07-20 12:23:55.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.085928 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1356 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/auth.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3233 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)      303 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      198 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1235 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3087 2023-06-15 10:00:14.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/response.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.085928 roj-agrirouter-sdk-python-1.0.6/agrirouter/constants/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/constants/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/constants/media_types.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      508 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/environmental_services.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2578 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/environments.py
+-rw-rw-r--   0 user      (1000) user      (1000)      378 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1363 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/keys.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/cloud_provider_integration/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/cloud_provider_integration/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3522 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/chunk_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7512 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/message_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/account/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/account/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4230 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/efdi/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/efdi/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)   306464 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9282 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5278 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.089928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/feed/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/feed/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/gps/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/gps/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    14065 2022-11-21 14:59:26.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9916 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/request_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/account/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/account/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10371 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/endpoint/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/endpoint/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5137 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    37035 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12586 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9214 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/response_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.093928 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/settings/dh_settings_pb2.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.097928 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7442 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/builders.py
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/certification.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.097928 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       30 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2725 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/http.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5185 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/mqtt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/decode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2438 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/encode.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1053 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      441 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3377 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/messages.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.097928 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3200 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18534 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1571 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/result.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.097928 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2986 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3153 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/commons.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.097928 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/http/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/http/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      757 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/http/outbox.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15502 2023-07-20 10:19:52.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/messaging.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.101928 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6174 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/dto.py
+-rw-rw-r--   0 user      (1000) user      (1000)      169 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/enums.py
+-rw-rw-r--   0 user      (1000) user      (1000)      894 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/headers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2376 2023-06-15 10:01:14.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/onboarding.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1653 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-06-15 10:01:38.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2115 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/request_body.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6710 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1035 2023-06-15 10:01:01.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/signature.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.101928 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      801 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/headers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1006 2023-06-15 10:02:01.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)      860 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/request_body.py
+-rw-rw-r--   0 user      (1000) user      (1000)      428 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1734 2023-06-15 10:02:19.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/revoking.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.101928 roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1936 2023-05-31 09:35:47.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/type_url.py
+-rw-rw-r--   0 user      (1000) user      (1000)      202 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/utc_time_util.py
+-rw-rw-r--   0 user      (1000) user      (1000)       59 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/uuid_util.py
+-rw-rw-r--   0 user      (1000) user      (1000)       90 2023-05-30 12:25:23.000000 roj-agrirouter-sdk-python-1.0.6/pyproject.toml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-20 12:47:41.105928 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-07-20 12:47:41.000000 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4370 2023-07-20 12:47:41.000000 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-20 12:47:41.000000 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      122 2023-07-20 12:47:41.000000 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       11 2023-07-20 12:47:41.000000 roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-20 12:47:41.105928 roj-agrirouter-sdk-python-1.0.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1388 2023-07-20 12:42:15.000000 roj-agrirouter-sdk-python-1.0.6/setup.py
```

### Comparing `roj-agrirouter-sdk-python-1.0.5/LICENSE` & `roj-agrirouter-sdk-python-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/PKG-INFO` & `roj-agrirouter-sdk-python-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roj-agrirouter-sdk-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Agrirouter SDK Python patched by ROJ for experimental test to run on App mobile
 Home-page: https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Author: Stefano Gurrieri
 Author-email: stefano.gurrieri@vandewiele.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Project-URL: Source, https://github.com/ROJ-ITALY/agrirouter-sdk-python
```

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/__init__.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 from agrirouter.messaging.parameters.service import MessageHeaderParameters, MessagePayloadParameters, \
     QueryMessageParameters, QueryHeaderParameters, CloudOffboardParameters, CloudOnboardParameters, \
     CapabilityParameters, FeedConfirmParameters, FeedDeleteParameters, ListEndpointsParameters, MessageParameters, \
     SubscriptionParameters, ImageParameters, EfdiParameters
 from agrirouter.messaging.services.cloud import CloudOnboardService, CloudOffboardService
 from agrirouter.messaging.services.messaging import SubscriptionService, CapabilityService, FeedConfirmService,\
-    FeedDeleteService, QueryHeaderService, QueryMessagesService, ListEndpointsService, ImageService, EfdiTimelogService, EfdiDeviceDscService
+    FeedDeleteService, QueryHeaderService, QueryMessagesService, ListEndpointsService, ImageService, EfdiTimelogService, EfdiTimelogPublishService, EfdiDeviceDscService
```

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/auth.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/auth.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/dto.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/parameters.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/auth/response.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/auth/response.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/environments.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/environments.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/environments/keys.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/environments/keys.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/cloud_provider_integration/cloud_virtualized_app_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/chunk_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/chunk_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/commons/message_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/commons/message_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/account/endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/efdi/efdi_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/endpoint/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/feed/feed_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/payload/gps/gps_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/request/request_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/request/request_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/account/endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/endpoint/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/feed_response_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/payload/feed/push_notification_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/messaging/response/response_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/messaging/response/response_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/generated/settings/dh_settings_pb2.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/generated/settings/dh_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/builders.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/builders.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/certification.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/certification.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/http.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/http.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/clients/mqtt.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/clients/mqtt.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/decode.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/decode.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/encode.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/encode.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/enums.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/enums.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/messages.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/messages.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/dto.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/parameters/service.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/parameters/service.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/request.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/request.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/result.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/result.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/cloud.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/cloud.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/commons.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/commons.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/http/outbox.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/http/outbox.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/messaging/services/messaging.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/messaging/services/messaging.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/dto.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/dto.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/exceptions.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/exceptions.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/headers.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/headers.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/onboarding.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/onboarding.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/parameters.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/request.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/request.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/request_body.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/request_body.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/response.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/response.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/onboarding/signature.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/onboarding/signature.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/headers.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/headers.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/parameters.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/parameters.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/request.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/request.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/request_body.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/request_body.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/revoking/revoking.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/revoking/revoking.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/agrirouter/utils/type_url.py` & `roj-agrirouter-sdk-python-1.0.6/agrirouter/utils/type_url.py`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/PKG-INFO` & `roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roj-agrirouter-sdk-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: Agrirouter SDK Python patched by ROJ for experimental test to run on App mobile
 Home-page: https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Author: Stefano Gurrieri
 Author-email: stefano.gurrieri@vandewiele.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ROJ-ITALY/agrirouter-sdk-python
 Project-URL: Source, https://github.com/ROJ-ITALY/agrirouter-sdk-python
```

### Comparing `roj-agrirouter-sdk-python-1.0.5/roj_agrirouter_sdk_python.egg-info/SOURCES.txt` & `roj-agrirouter-sdk-python-1.0.6/roj_agrirouter_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roj-agrirouter-sdk-python-1.0.5/setup.py` & `roj-agrirouter-sdk-python-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='roj-agrirouter-sdk-python',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),	
     include_package_data=True,
     python_requires=">= 3.6",
     url='https://github.com/ROJ-ITALY/agrirouter-sdk-python',
     license='Apache-2.0',
     author='Stefano Gurrieri',
     author_email='stefano.gurrieri@vandewiele.com',
```

