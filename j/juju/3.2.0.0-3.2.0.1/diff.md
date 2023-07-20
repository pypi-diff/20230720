# Comparing `tmp/juju-3.2.0.0.tar.gz` & `tmp/juju-3.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juju-3.2.0.0.tar", last modified: Wed Jun  7 09:17:55 2023, max compression
+gzip compressed data, was "juju-3.2.0.1.tar", last modified: Thu Jul 20 21:26:02 2023, max compression
```

## Comparing `juju-3.2.0.0.tar` & `juju-3.2.0.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       65 2023-06-07 08:30:31.000000 juju-3.2.0.0/CONTRIBUTORS
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11344 2023-06-07 08:30:31.000000 juju-3.2.0.0/LICENSE
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      159 2023-06-07 08:30:31.000000 juju-3.2.0.0/MANIFEST.in
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    34081 2023-06-07 09:17:55.208830 juju-3.2.0.0/PKG-INFO
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-06-07 08:30:31.000000 juju-3.2.0.0/README.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        8 2023-06-07 08:30:31.000000 juju-3.2.0.0/VERSION
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.192830 juju-3.2.0.0/docs/
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/api/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.action.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.annotation.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.application.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2352 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.client.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      210 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.constraints.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.controller.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.delta.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      190 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.errors.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      206 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.exceptions.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.juju.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.loop.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      194 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.machine.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.model.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      202 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.placement.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      198 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.relation.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      178 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.tag.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      182 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.unit.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      186 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/juju.utils.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      575 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/api/modules.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    30411 2023-06-07 09:17:40.000000 juju-3.2.0.0/docs/changelog.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      666 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/index.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/narrative/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3213 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/application.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2751 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/controller.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      100 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/index.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8727 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/model.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1469 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/narrative/unit.rst
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3085 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/readme.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.196830 juju-3.2.0.0/docs/upstream-updates/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6676 2023-06-07 08:30:31.000000 juju-3.2.0.0/docs/upstream-updates/index.rst
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/examples/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1159 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1662 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_k8s.py
--rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)     1593 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1689 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1978 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/add_secrets_backend.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      819 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/allwatcher.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      938 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_deploy_k8s.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      830 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_deploy_machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      861 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_find.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      701 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/charmhub_info.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      532 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/cloud.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      556 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/clouds.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1389 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/config.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      703 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/connect_current_model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      955 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1446 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/credential.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2148 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2261 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2466 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2879 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/crossmodel_relation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      841 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/debug-log.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      888 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1462 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      863 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle_charmhub.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1075 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_bundle_with_trust.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      950 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_constraints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      737 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_big_k8s_bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1060 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_bundle_with_resources.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1220 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_file_resource.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1203 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_local_resource.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      803 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/deploy_with_revision.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2457 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/expose-application.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1236 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/formatted_status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      422 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/fullstatus.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1070 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/future.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/get_cloud.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      583 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/leadership.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      250 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/list_secrets.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      669 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/livemodel.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      682 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/local_refresh.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      729 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/localcharm.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1073 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/machine_hostname.py
--rwxrwxr-x   0 jtirado   (1000) jtirado   (1000)      732 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1046 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/modelsummaries.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3239 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/relate.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      853 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/run_action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1114 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/scp.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1195 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1619 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/unitrun.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1194 2023-06-07 08:30:31.000000 juju-3.2.0.0/examples/upgrade_local_charm_k8s.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/juju/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/__init__.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      642 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/action.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      119 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/annotation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1072 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/annotationhelper.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    36725 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/application.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    49702 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/bundle.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      712 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/charm.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     7189 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/charmhub.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/__init__.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8722 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   688237 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client1.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41552 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client10.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   196254 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client11.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   245218 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client12.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   244188 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client13.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   115453 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client14.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   108914 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client15.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client16.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   103511 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client17.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   369150 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client18.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   383690 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client2.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   192763 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client3.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   201969 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client4.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    41639 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client5.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   162109 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client6.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   154579 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client7.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    45251 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client8.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    56944 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_client9.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)  1229695 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/_definitions.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1224 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/client.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1347 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/codegen.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    38886 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/connection.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8034 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/connector.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    31664 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/facade.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      321 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/flags.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3660 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/gocookies.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5968 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/jujudata.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    12465 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/overrides.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/proxy/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      679 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/factory.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.208830 juju-3.2.0.0/juju/client/proxy/kubernetes/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2115 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/kubernetes/proxy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      468 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/proxy/proxy.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      799 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/client/runner.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4478 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/constraints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    37481 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/controller.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2637 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/delta.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3138 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/errors.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       47 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/exceptions.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4219 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/jasyncio.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1162 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/juju.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      136 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/loop.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     8768 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/machine.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)   112234 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/model.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2134 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/names.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6450 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/offerendpoints.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     5798 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/origin.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1829 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/placement.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    11423 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/provisioner.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/py.typed
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4954 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/relation.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1273 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/remoteapplication.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     6521 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/status.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     1313 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/tag.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    14678 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/unit.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     4576 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/url.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2182 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/user.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    17231 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/utils.py
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      415 2023-06-07 08:30:31.000000 juju-3.2.0.0/juju/version.py
-drwxrwxr-x   0 jtirado   (1000) jtirado   (1000)        0 2023-06-07 09:17:55.200830 juju-3.2.0.0/juju.egg-info/
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)    34081 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/PKG-INFO
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     3620 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/SOURCES.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        1 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/dependency_links.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)      308 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/requires.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)        5 2023-06-07 09:17:55.000000 juju-3.2.0.0/juju.egg-info/top_level.txt
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)       38 2023-06-07 09:17:55.208830 juju-3.2.0.0/setup.cfg
--rw-rw-r--   0 jtirado   (1000) jtirado   (1000)     2260 2023-06-07 08:30:31.000000 juju-3.2.0.0/setup.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.754649 juju-3.2.0.1/
+-rw-rw-r--   0 caner     (1000) caner     (1000)      155 2023-07-20 20:43:24.000000 juju-3.2.0.1/CONTRIBUTORS
+-rw-rw-r--   0 caner     (1000) caner     (1000)    11344 2023-07-20 20:43:24.000000 juju-3.2.0.1/LICENSE
+-rw-rw-r--   0 caner     (1000) caner     (1000)      159 2023-07-20 20:43:24.000000 juju-3.2.0.1/MANIFEST.in
+-rw-rw-r--   0 caner     (1000) caner     (1000)    35787 2023-07-20 21:26:02.754649 juju-3.2.0.1/PKG-INFO
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3380 2023-07-20 20:44:25.000000 juju-3.2.0.1/README.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)        8 2023-07-20 20:43:24.000000 juju-3.2.0.1/VERSION
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.654646 juju-3.2.0.1/docs/
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.662646 juju-3.2.0.1/docs/api/
+-rw-rw-r--   0 caner     (1000) caner     (1000)      190 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.action.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      206 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.annotation.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      210 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.application.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2352 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.client.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      210 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.constraints.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      206 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.controller.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      186 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.delta.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      190 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.errors.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      206 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.exceptions.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      182 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.juju.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      182 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.loop.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      194 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.machine.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      186 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.model.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      202 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.placement.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      198 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.relation.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      178 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.tag.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      182 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.unit.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      186 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/juju.utils.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      575 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/api/modules.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)    31635 2023-07-20 20:50:53.000000 juju-3.2.0.1/docs/changelog.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      666 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/index.rst
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.666646 juju-3.2.0.1/docs/narrative/
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3034 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/narrative/application.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2747 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/narrative/controller.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)      100 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/narrative/index.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)     8713 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/narrative/model.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1469 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/narrative/unit.rst
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3380 2023-07-20 20:44:25.000000 juju-3.2.0.1/docs/readme.rst
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.666646 juju-3.2.0.1/docs/upstream-updates/
+-rw-rw-r--   0 caner     (1000) caner     (1000)     6676 2023-07-20 20:43:24.000000 juju-3.2.0.1/docs/upstream-updates/index.rst
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.690647 juju-3.2.0.1/examples/
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1159 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/action.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1662 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/add_k8s.py
+-rwxrwxr-x   0 caner     (1000) caner     (1000)     1593 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/add_machine.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1689 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/add_model.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1978 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/add_secrets_backend.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      819 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/allwatcher.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      938 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/charmhub_deploy_k8s.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      830 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/charmhub_deploy_machine.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      861 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/charmhub_find.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      701 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/charmhub_info.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      532 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/cloud.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      556 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/clouds.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1389 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/config.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      703 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/connect_current_model.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      955 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/controller.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1446 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/credential.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2148 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/crossmodel.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2261 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/crossmodel_bundle.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2466 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/crossmodel_controller.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2879 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/crossmodel_relation.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      841 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/debug-log.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      888 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1462 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_bundle.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      863 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_bundle_charmhub.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1075 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_bundle_with_trust.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      950 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_constraints.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      737 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_local_big_k8s_bundle.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1060 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_local_bundle_with_resources.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1220 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_local_file_resource.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1203 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_local_resource.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      803 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/deploy_with_revision.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2457 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/expose-application.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1236 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/formatted_status.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      422 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/fullstatus.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1070 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/future.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      642 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/get_cloud.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      583 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/leadership.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      250 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/list_secrets.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      669 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/livemodel.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      682 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/local_refresh.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      729 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/localcharm.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1073 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/machine_hostname.py
+-rwxrwxr-x   0 caner     (1000) caner     (1000)      732 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/model.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1046 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/modelsummaries.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3239 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/relate.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      853 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/run_action.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1114 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/scp.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1195 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/status.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1619 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/unitrun.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1194 2023-07-20 20:43:24.000000 juju-3.2.0.1/examples/upgrade_local_charm_k8s.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.710647 juju-3.2.0.1/juju/
+-rw-rw-r--   0 caner     (1000) caner     (1000)        0 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/__init__.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1247 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/access.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      642 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/action.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      119 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/annotation.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1072 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/annotationhelper.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    36991 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/application.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    45144 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/bundle.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      712 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/charm.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     7189 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/charmhub.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.750648 juju-3.2.0.1/juju/client/
+-rw-rw-r--   0 caner     (1000) caner     (1000)        0 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/__init__.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     8722 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   688237 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client1.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    41552 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client10.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   196254 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client11.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   245218 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client12.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   244188 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client13.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   115453 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client14.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   108914 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client15.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   103511 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client16.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   103511 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client17.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   369150 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client18.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   383690 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client2.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   192763 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client3.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   201969 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client4.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    41639 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client5.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   162109 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client6.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   154579 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client7.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    45251 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client8.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    56944 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_client9.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)  1229695 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/_definitions.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1224 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/client.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1347 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/codegen.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    38886 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/connection.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     8034 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/connector.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    31664 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/facade.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      321 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/flags.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3660 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/gocookies.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     5968 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/jujudata.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    12465 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/overrides.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.750648 juju-3.2.0.1/juju/client/proxy/
+-rw-rw-r--   0 caner     (1000) caner     (1000)      679 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/proxy/factory.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.750648 juju-3.2.0.1/juju/client/proxy/kubernetes/
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2115 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/proxy/kubernetes/proxy.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      468 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/proxy/proxy.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      799 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/client/runner.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     4478 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/constraints.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    37437 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/controller.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2637 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/delta.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3366 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/errors.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)       47 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/exceptions.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     4219 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/jasyncio.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1162 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/juju.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      136 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/loop.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     8768 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/machine.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)   115719 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/model.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2134 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/names.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     6450 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/offerendpoints.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     5798 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/origin.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1829 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/placement.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    11423 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/provisioner.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     4954 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/relation.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1455 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/remoteapplication.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     6521 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/status.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     1313 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/tag.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    15342 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/unit.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     4576 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/url.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)     6391 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/user.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)    18524 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/utils.py
+-rw-rw-r--   0 caner     (1000) caner     (1000)      415 2023-07-20 20:43:24.000000 juju-3.2.0.1/juju/version.py
+drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2023-07-20 21:26:02.714647 juju-3.2.0.1/juju.egg-info/
+-rw-rw-r--   0 caner     (1000) caner     (1000)    35787 2023-07-20 21:26:02.000000 juju-3.2.0.1/juju.egg-info/PKG-INFO
+-rw-rw-r--   0 caner     (1000) caner     (1000)     3621 2023-07-20 21:26:02.000000 juju-3.2.0.1/juju.egg-info/SOURCES.txt
+-rw-rw-r--   0 caner     (1000) caner     (1000)        1 2023-07-20 21:26:02.000000 juju-3.2.0.1/juju.egg-info/dependency_links.txt
+-rw-rw-r--   0 caner     (1000) caner     (1000)      315 2023-07-20 21:26:02.000000 juju-3.2.0.1/juju.egg-info/requires.txt
+-rw-rw-r--   0 caner     (1000) caner     (1000)        5 2023-07-20 21:26:02.000000 juju-3.2.0.1/juju.egg-info/top_level.txt
+-rw-rw-r--   0 caner     (1000) caner     (1000)       38 2023-07-20 21:26:02.754649 juju-3.2.0.1/setup.cfg
+-rw-rw-r--   0 caner     (1000) caner     (1000)     2483 2023-07-20 20:44:35.000000 juju-3.2.0.1/setup.py
```

### Comparing `juju-3.2.0.0/LICENSE` & `juju-3.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/PKG-INFO` & `juju-3.2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.2.0.0
+Version: 3.2.0.1
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 A Python library for Juju
 =========================
 
 Source code: https://github.com/juju/python-libjuju
 
@@ -24,21 +28,24 @@
 
 Documentation: https://pythonlibjuju.readthedocs.io/en/latest/
 
 
 Requirements
 ------------
 
-* Python 3.9/3.10
+This version may support old versions of Juju. However, it has been
+tested with the following requirements.
+
+* Python 3.8/3.9/3.10
 
 
 Design Notes
 ------------
 
-* Asynchronous - Uses asyncio and async/await features of Python
+* Asynchronous - uses asyncio and async/await features of python 3.5
 * Websocket-level bindings are programmatically generated (indirectly) from the
   Juju golang code, ensuring full api coverage
 * Provides an OO layer which encapsulates much of the websocket api and
   provides familiar nouns and verbs (e.g. Model.deploy(), Application.add_unit(),
   etc.)
 
 
@@ -53,14 +60,15 @@
 Quickstart
 ----------
 
 Here's a simple example that shows basic usage of the library. The example
 connects to the currently active Juju model, deploys a single unit of the
 ubuntu charm, then exits:
 
+Note : Pylibjuju requires an already bootstrapped Juju controller to connect to.
 
 .. code:: python
 
   #!/usr/bin/python3
 
   import logging
   import sys
@@ -78,17 +86,15 @@
       await model.connect_current()
 
       try:
           # Deploy a single unit of the ubuntu charm, using the latest revision
           # from the stable channel of the Charm Store.
           ubuntu_app = await model.deploy(
             'ubuntu',
-            application_name='ubuntu',
-            series='xenial',
-            channel='stable',
+            application_name='my-ubuntu',
           )
 
           if '--wait' in sys.argv:
               # optionally block until the application is ready
               await model.block_until(lambda: ubuntu_app.status == 'active')
       finally:
           # Disconnect from the api server and cleanup.
@@ -138,32 +144,54 @@
   >>> await model.connect_current()
   >>> status = await model.get_status()
 
 
 Versioning
 ----------
 
-Pylibjuju releases now track the Juju release cadence. New generated schemas
+The current Pylibjuju release policy tracks the Juju release cadence.
+In particular, whenever Juju makes a latest/stable release, pylibjuju pushes out
+a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.2.0.1
+^^^^^^^
+
+Thursday 20th July 2023
+
+This is a point release on the 3.x track, works with any Juju 3.x controller.
+
+What's Changed
+
+* Update readme and add some docstrings for functions by @cderici in https://github.com/juju/python-libjuju/pull/873
+* Forward port subordinate utils by @cderici in https://github.com/juju/python-libjuju/pull/880
+* [JUJU-3952] Revisit access control levels by @cderici in https://github.com/juju/python-libjuju/pull/882
+* [JUJU-3999] Avoid parsing endpoint for overlay offers by @cderici in https://github.com/juju/python-libjuju/pull/887
+* Forward port upgrade resource fixes in app refresh by @cderici in https://github.com/juju/python-libjuju/pull/889
+* [JUJU-4076] Rename `wait_for_units` and make semantics clearer by @cderici in https://github.com/juju/python-libjuju/pull/890
+* Stabilize sphinx build on RTD by @cderici in https://github.com/juju/python-libjuju/pull/899
+* Move test utils into a separate module by @cderici in https://github.com/juju/python-libjuju/pull/903
+* Remove title prefixes from issue templates by @cderici in https://github.com/juju/python-libjuju/pull/904
+* [JUJU-4048] Use GetChangesMapArgs for bundle changes by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/907
+* Forward ports from 2.9 to 3.x by @cderici in https://github.com/juju/python-libjuju/pull/910
+* Remove ceiling on pyyaml version by @cderici in https://github.com/juju/python-libjuju/pull/918
+
 3.2.0.0
 ^^^^^^^
 
 Wednesday 7th June 2023
 
 This release contains the new endpoints for Juju 3.2.0.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
 * Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
 * Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
 * [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
 * Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
 * [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
 * Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
 * [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
@@ -175,17 +203,14 @@
 Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
-
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -195,63 +220,52 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-What's Changed
-""""""""""""""
-
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
 New Contributors
-""""""""""""""""
 
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-What's Changed
-""""""""""""""
-
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
 New Contributors
-""""""""""""""""
 
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-What's Changed
-""""""""""""""
-
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
 * [JUJU-2018] Update 2.9.36 facades & clients by @cderici in https://github.com/juju/python-libjuju/pull/752
@@ -262,17 +276,14 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-What's Changed
-""""""""""""""
-
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
 * [JUJU-1681] Add --attach-storage parameter to model.deploy by @cderici in https://github.com/juju/python-libjuju/pull/720
```

### Comparing `juju-3.2.0.0/README.rst` & `juju-3.2.0.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 Documentation: https://pythonlibjuju.readthedocs.io/en/latest/
 
 
 Requirements
 ------------
 
-* Python 3.9/3.10
+This version may support old versions of Juju. However, it has been
+tested with the following requirements.
+
+* Python 3.8/3.9/3.10
 
 
 Design Notes
 ------------
 
-* Asynchronous - Uses asyncio and async/await features of Python
+* Asynchronous - uses asyncio and async/await features of python 3.5
 * Websocket-level bindings are programmatically generated (indirectly) from the
   Juju golang code, ensuring full api coverage
 * Provides an OO layer which encapsulates much of the websocket api and
   provides familiar nouns and verbs (e.g. Model.deploy(), Application.add_unit(),
   etc.)
 
 
@@ -36,14 +39,15 @@
 Quickstart
 ----------
 
 Here's a simple example that shows basic usage of the library. The example
 connects to the currently active Juju model, deploys a single unit of the
 ubuntu charm, then exits:
 
+Note : Pylibjuju requires an already bootstrapped Juju controller to connect to.
 
 .. code:: python
 
   #!/usr/bin/python3
 
   import logging
   import sys
@@ -61,17 +65,15 @@
       await model.connect_current()
 
       try:
           # Deploy a single unit of the ubuntu charm, using the latest revision
           # from the stable channel of the Charm Store.
           ubuntu_app = await model.deploy(
             'ubuntu',
-            application_name='ubuntu',
-            series='xenial',
-            channel='stable',
+            application_name='my-ubuntu',
           )
 
           if '--wait' in sys.argv:
               # optionally block until the application is ready
               await model.block_until(lambda: ubuntu_app.status == 'active')
       finally:
           # Disconnect from the api server and cleanup.
@@ -121,9 +123,11 @@
   >>> await model.connect_current()
   >>> status = await model.get_status()
 
 
 Versioning
 ----------
 
-Pylibjuju releases now track the Juju release cadence. New generated schemas
+The current Pylibjuju release policy tracks the Juju release cadence.
+In particular, whenever Juju makes a latest/stable release, pylibjuju pushes out
+a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
```

### Comparing `juju-3.2.0.0/docs/api/juju.client.rst` & `juju-3.2.0.1/docs/api/juju.client.rst`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/docs/api/modules.rst` & `juju-3.2.0.1/docs/api/modules.rst`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/docs/changelog.rst` & `juju-3.2.0.1/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,41 @@
 Changelog
 ---------
 
+3.2.0.1
+^^^^^^^
+
+Thursday 20th July 2023
+
+This is a point release on the 3.x track, works with any Juju 3.x controller.
+
+What's Changed
+
+* Update readme and add some docstrings for functions by @cderici in https://github.com/juju/python-libjuju/pull/873
+* Forward port subordinate utils by @cderici in https://github.com/juju/python-libjuju/pull/880
+* [JUJU-3952] Revisit access control levels by @cderici in https://github.com/juju/python-libjuju/pull/882
+* [JUJU-3999] Avoid parsing endpoint for overlay offers by @cderici in https://github.com/juju/python-libjuju/pull/887
+* Forward port upgrade resource fixes in app refresh by @cderici in https://github.com/juju/python-libjuju/pull/889
+* [JUJU-4076] Rename `wait_for_units` and make semantics clearer by @cderici in https://github.com/juju/python-libjuju/pull/890
+* Stabilize sphinx build on RTD by @cderici in https://github.com/juju/python-libjuju/pull/899
+* Move test utils into a separate module by @cderici in https://github.com/juju/python-libjuju/pull/903
+* Remove title prefixes from issue templates by @cderici in https://github.com/juju/python-libjuju/pull/904
+* [JUJU-4048] Use GetChangesMapArgs for bundle changes by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/907
+* Forward ports from 2.9 to 3.x by @cderici in https://github.com/juju/python-libjuju/pull/910
+* Remove ceiling on pyyaml version by @cderici in https://github.com/juju/python-libjuju/pull/918
+
 3.2.0.0
 ^^^^^^^
 
 Wednesday 7th June 2023
 
 This release contains the new endpoints for Juju 3.2.0.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
 * Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
 * Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
 * [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
 * Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
 * [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
 * Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
 * [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
@@ -27,17 +47,14 @@
 Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
-
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -47,63 +64,52 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-What's Changed
-""""""""""""""
-
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
 New Contributors
-""""""""""""""""
 
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-What's Changed
-""""""""""""""
-
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
 New Contributors
-""""""""""""""""
 
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-What's Changed
-""""""""""""""
-
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
 * [JUJU-2018] Update 2.9.36 facades & clients by @cderici in https://github.com/juju/python-libjuju/pull/752
@@ -114,17 +120,14 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-What's Changed
-""""""""""""""
-
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
 * [JUJU-1681] Add --attach-storage parameter to model.deploy by @cderici in https://github.com/juju/python-libjuju/pull/720
```

### Comparing `juju-3.2.0.0/docs/index.rst` & `juju-3.2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/docs/narrative/application.rst` & `juju-3.2.0.1/docs/narrative/application.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 
   from juju.model import Model
 
   model = Model()
   await model.connect_current()
 
   mysql_app = await model.deploy(
-      # If a revision number is not included in the charm url,
-      # the latest revision from the Charm Store will be used.
-      'cs:mysql-55',
-      application_name='mysql',
-      series='trusty',
-      channel='stable',
+      'mysql',
+      application_name='my-mysql',
+      series='jammy',
+      channel='8.0/stable',
       config={
           'tuning-level': 'safest',
       },
       constraints={
           'mem': 256 * MB,
       },
   )
@@ -42,32 +40,31 @@
   from juju.model import Model
 
   model = Model()
   await model.connect_current()
 
   # Deploy a local charm using a path to the charm directory
   await model.deploy(
-      '/home/tvansteenburgh/src/charms/ubuntu',
+      './charms/ubuntu',
       application_name='ubuntu',
-      series='trusty',
+      series='jammy',
   )
 
 
 Adding Units
 ------------
 To add units to a deployed application, use the
 :meth:`juju.application.Application.add_units` method. A list of the newly
 added units (:class:`~juju.unit.Unit` objects) is returned.
 
 .. code:: python
 
   ubuntu_app = await model.deploy(
       'ubuntu',
       application_name='ubuntu',
-      series='trusty',
       channel='stable',
   )
 
   unit_a, unit_b = await ubuntu_app.add_units(count=2)
 
 
 Updating Config and Constraints
@@ -103,26 +100,26 @@
   from juju.model import Model
 
   model = Model()
   await model.connect_current()
 
   # Deploy mysql-master application
   mysql_master = await model.deploy(
-      'cs:mysql-55',
+      'mysql',
       application_name='mysql-master',
-      series='trusty',
-      channel='stable',
+      series='jammy',
+      channel='8.0/stable',
   )
 
   # Deploy mysql-slave application
   mysql_slave = await model.deploy(
-      'cs:mysql-55',
+      'mysql',
       application_name='mysql-slave',
-      series='trusty',
-      channel='stable',
+      series='jammy',
+      channel='8.0/stable',
   )
 
   # Add the master-slave relation
   relation = await mysql_master.relate(
       # Name of the relation on the local (mysql-master) side
       'master',
       # Name of the app:relation on the remote side
```

### Comparing `juju-3.2.0.0/docs/narrative/controller.rst` & `juju-3.2.0.1/docs/narrative/controller.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 ===========
 A Juju controller provides websocket endpoints for itself and each of its
 models. In order to do anything useful, the juju lib must connect to one of
 these endpoints.
 
 Connecting to the controller endpoint is useful if you want to programmatically
 create a new model. If the model you want to use already exists, you can
-connect directly to it (see py:doc:`model`).
+connect directly to it (see :doc:`model`).
 
-For API docs, see py:class:`juju.controller.Controller`.
+For API docs, see :class:`juju.controller.Controller`.
 
 
 Connecting to the Current Controller
 ------------------------------------
 Connect to the currently active Juju controller (the one returned by
 `juju switch`). This only works if you have the Juju CLI client installed.
```

### Comparing `juju-3.2.0.0/docs/narrative/model.rst` & `juju-3.2.0.1/docs/narrative/model.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Models
 ======
 A Juju controller provides websocket endpoints for each of its
 models. In order to do anything useful with a model, the juju lib must
 connect to one of these endpoints. There are several ways to do this.
 
-For api docs, see py:class:`juju.model.Model`.
+For api docs, see :class:`juju.model.Model`.
 
 
 Connecting to the Current Model
 -------------------------------
 Connect to the currently active Juju model (the one returned by
 `juju switch`). This only works if you have the Juju CLI client installed.
 
@@ -88,16 +88,16 @@
                     # of The `juju show-controller` command.
   )
 
 
 Creating and Destroying a Model
 -------------------------------
 Example of creating a new model and then destroying it. See
-py:method:`juju.controller.Controller.add_model` and
-py:method:`juju.controller.Controller.destroy_model` for more info.
+:method:`juju.controller.Controller.add_model` and
+:method:`juju.controller.Controller.destroy_model` for more info.
 
 .. code:: python
 
   from juju.controller import Controller
 
   controller = Controller()
   await controller.connect_current()
@@ -115,16 +115,16 @@
   await controller.destroy_model(model_uuid)
   model = None
 
 
 Adding Machines and Containers
 ------------------------------
 To add a machine or container, connect to a model and then call its
-py:method:`~juju.model.Model.add_machine` method. A
-py:class:`~juju.machine.Machine` instance is returned. The machine id
+:method:`~juju.model.Model.add_machine` method. A
+:class:`~juju.machine.Machine` instance is returned. The machine id
 can be used to deploy a charm to a specific machine or container.
 
 .. code:: python
 
   from juju.model import Model
 
   MB = 1
@@ -173,15 +173,15 @@
   await machine1.destroy(force=True)
 
 
 Reacting to Changes in a Model
 ------------------------------
 To watch for and respond to changes in a model, register an observer with the
 model. The easiest way to do this is by creating a
-py:class:`juju.model.ModelObserver` subclass.
+:class:`juju.model.ModelObserver` subclass.
 
 .. code:: python
 
   from juju.model import Model, ModelObserver
 
   class MyModelObserver(ModelObserver):
       async def on_change(self, delta, old, new, model):
@@ -264,15 +264,15 @@
           pass
 
       async def on_change(self, delta, old, new, model):
           # The catch-all handler - will be called whenever a more
           # specific handler method is not defined.
 
 
-Any py:class:`juju.model.ModelEntity` object can be observed directly by
+Any :class:`juju.model.ModelEntity` object can be observed directly by
 registering callbacks on the object itself.
 
 .. code:: python
 
   import logging
 
   async def on_app_change(delta, old, new, model):
```

### Comparing `juju-3.2.0.0/docs/narrative/unit.rst` & `juju-3.2.0.1/docs/narrative/unit.rst`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/docs/readme.rst` & `juju-3.2.0.1/docs/readme.rst`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 
 Documentation: https://pythonlibjuju.readthedocs.io/en/latest/
 
 
 Requirements
 ------------
 
-* Python 3.9/3.10
+This version may support old versions of Juju. However, it has been
+tested with the following requirements.
+
+* Python 3.8/3.9/3.10
 
 
 Design Notes
 ------------
 
-* Asynchronous - Uses asyncio and async/await features of Python
+* Asynchronous - uses asyncio and async/await features of python 3.5
 * Websocket-level bindings are programmatically generated (indirectly) from the
   Juju golang code, ensuring full api coverage
 * Provides an OO layer which encapsulates much of the websocket api and
   provides familiar nouns and verbs (e.g. Model.deploy(), Application.add_unit(),
   etc.)
 
 
@@ -36,14 +39,15 @@
 Quickstart
 ----------
 
 Here's a simple example that shows basic usage of the library. The example
 connects to the currently active Juju model, deploys a single unit of the
 ubuntu charm, then exits:
 
+Note : Pylibjuju requires an already bootstrapped Juju controller to connect to.
 
 .. code:: python
 
   #!/usr/bin/python3
 
   import logging
   import sys
@@ -61,17 +65,15 @@
       await model.connect_current()
 
       try:
           # Deploy a single unit of the ubuntu charm, using the latest revision
           # from the stable channel of the Charm Store.
           ubuntu_app = await model.deploy(
             'ubuntu',
-            application_name='ubuntu',
-            series='xenial',
-            channel='stable',
+            application_name='my-ubuntu',
           )
 
           if '--wait' in sys.argv:
               # optionally block until the application is ready
               await model.block_until(lambda: ubuntu_app.status == 'active')
       finally:
           # Disconnect from the api server and cleanup.
@@ -121,9 +123,11 @@
   >>> await model.connect_current()
   >>> status = await model.get_status()
 
 
 Versioning
 ----------
 
-Pylibjuju releases now track the Juju release cadence. New generated schemas
+The current Pylibjuju release policy tracks the Juju release cadence.
+In particular, whenever Juju makes a latest/stable release, pylibjuju pushes out
+a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
```

### Comparing `juju-3.2.0.0/docs/upstream-updates/index.rst` & `juju-3.2.0.1/docs/upstream-updates/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/action.py` & `juju-3.2.0.1/examples/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/add_k8s.py` & `juju-3.2.0.1/examples/add_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/add_machine.py` & `juju-3.2.0.1/examples/add_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/add_model.py` & `juju-3.2.0.1/examples/add_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/add_secrets_backend.py` & `juju-3.2.0.1/examples/add_secrets_backend.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/allwatcher.py` & `juju-3.2.0.1/examples/allwatcher.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/charmhub_deploy_k8s.py` & `juju-3.2.0.1/examples/charmhub_deploy_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/charmhub_deploy_machine.py` & `juju-3.2.0.1/examples/charmhub_deploy_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/charmhub_find.py` & `juju-3.2.0.1/examples/charmhub_find.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/charmhub_info.py` & `juju-3.2.0.1/examples/charmhub_info.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/cloud.py` & `juju-3.2.0.1/examples/cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/clouds.py` & `juju-3.2.0.1/examples/clouds.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/config.py` & `juju-3.2.0.1/examples/config.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/connect_current_model.py` & `juju-3.2.0.1/examples/connect_current_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/controller.py` & `juju-3.2.0.1/examples/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/credential.py` & `juju-3.2.0.1/examples/credential.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/crossmodel.py` & `juju-3.2.0.1/examples/crossmodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/crossmodel_bundle.py` & `juju-3.2.0.1/examples/crossmodel_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/crossmodel_controller.py` & `juju-3.2.0.1/examples/crossmodel_controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/crossmodel_relation.py` & `juju-3.2.0.1/examples/crossmodel_relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/debug-log.py` & `juju-3.2.0.1/examples/debug-log.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy.py` & `juju-3.2.0.1/examples/deploy.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_bundle.py` & `juju-3.2.0.1/examples/deploy_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_bundle_charmhub.py` & `juju-3.2.0.1/examples/deploy_bundle_charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_bundle_with_trust.py` & `juju-3.2.0.1/examples/deploy_bundle_with_trust.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_constraints.py` & `juju-3.2.0.1/examples/deploy_constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_local_big_k8s_bundle.py` & `juju-3.2.0.1/examples/deploy_local_big_k8s_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_local_bundle_with_resources.py` & `juju-3.2.0.1/examples/deploy_local_bundle_with_resources.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_local_file_resource.py` & `juju-3.2.0.1/examples/deploy_local_file_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_local_resource.py` & `juju-3.2.0.1/examples/deploy_local_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/deploy_with_revision.py` & `juju-3.2.0.1/examples/deploy_with_revision.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/expose-application.py` & `juju-3.2.0.1/examples/expose-application.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/formatted_status.py` & `juju-3.2.0.1/examples/formatted_status.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/future.py` & `juju-3.2.0.1/examples/future.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/get_cloud.py` & `juju-3.2.0.1/examples/get_cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/leadership.py` & `juju-3.2.0.1/examples/leadership.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/livemodel.py` & `juju-3.2.0.1/examples/livemodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/local_refresh.py` & `juju-3.2.0.1/examples/local_refresh.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/localcharm.py` & `juju-3.2.0.1/examples/localcharm.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/machine_hostname.py` & `juju-3.2.0.1/examples/machine_hostname.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/model.py` & `juju-3.2.0.1/examples/model.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/modelsummaries.py` & `juju-3.2.0.1/examples/modelsummaries.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/relate.py` & `juju-3.2.0.1/examples/relate.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/run_action.py` & `juju-3.2.0.1/examples/run_action.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/scp.py` & `juju-3.2.0.1/examples/scp.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/status.py` & `juju-3.2.0.1/examples/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/unitrun.py` & `juju-3.2.0.1/examples/unitrun.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/examples/upgrade_local_charm_k8s.py` & `juju-3.2.0.1/examples/upgrade_local_charm_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/action.py` & `juju-3.2.0.1/juju/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/annotationhelper.py` & `juju-3.2.0.1/juju/annotationhelper.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/application.py` & `juju-3.2.0.1/juju/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,19 @@
     def units(self):
         return [
             unit for unit in self.model.units.values()
             if unit.application == self.name
         ]
 
     @property
+    def subordinate_units(self):
+        """Returns the subordinate units of this application"""
+        return [u for u in self.units if u.is_subordinate]
+
+    @property
     def relations(self):
         return [rel for rel in self.model.relations if rel.matches(self.name)]
 
     def related_applications(self, endpoint_name=None):
         apps = {}
         for rel in self.relations:
             if rel.is_peer:
@@ -559,18 +564,26 @@
             commands=command,
             machines=[],
             timeout=timeout,
             units=[],
         )
 
     @property
+    def charm_name(self):
+        """Get the charm name of this application
+
+        :return str: The name of the charm
+        """
+        return URL.parse(self.charm_url).name
+
+    @property
     def charm_url(self):
-        """Get the charm url for a given application
+        """Get the charm url for this application
 
-        :return string: The charm url for an application
+        :return str: The charm url
         """
         return self.safe_data['charm-url']
 
     async def get_annotations(self):
         """Get annotations on this application.
 
         :return dict: The annotations for this application
@@ -740,19 +753,18 @@
         response = await resources_facade.ListResources(entities=request_data)
         existing_resources = {
             resource.name: resource
             for resource in response.results[0].resources
         }
 
         # Compute the difference btw resources needed and the existing resources
-        resources_to_update = [
-            resource for resource in charm_resources
-            if resource.get('Name', resource.get('name')) not in existing_resources or
-            existing_resources[resource.get('Name', resource.get('name'))].origin != 'upload'
-        ]
+        resources_to_update = []
+        for resource in charm_resources:
+            if utils.should_upgrade_resource(resource, existing_resources):
+                resources_to_update.append(resource)
 
         # Update the resources
         if resources_to_update:
             request_data = []
             for resource in resources_to_update:
                 request_data.append(client.CharmResource(
                     description=resource.get('Description', resource.get('description')),
```

### Comparing `juju-3.2.0.0/juju/bundle.py` & `juju-3.2.0.1/juju/bundle.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 
 import yaml
 
 from toposort import toposort_flatten
 
 from .client import client
-from .constraints import parse as parse_constraints, parse_storage_constraint, parse_device_constraint
+from .constraints import parse as parse_constraints
 from .errors import JujuError
 from . import utils, jasyncio
 from .origin import Channel, Source
 from .url import Schema, URL
 from .utils import get_base_from_origin_or_channel
 
 log = logging.getLogger(__name__)
@@ -125,15 +125,18 @@
                 pass
             except FileNotFoundError:
                 continue
             series = (app_dict.get('series') or default_series)
             if not series:
                 metadata = utils.get_local_charm_metadata(charm_dir)
                 series = await get_charm_series(metadata, self.model)
-            if not self.model.connection().is_using_old_client and not series:
+            if not series:
+                base = utils.get_local_charm_base(None, charm_path, client.Base)
+                series = utils.base_channel_to_series(base.channel)
+            if not series:
                 raise JujuError(
                     "Couldn't determine series for charm at {}. "
                     "Add a 'series' key to the bundle.".format(charm_dir))
             # Keep track of what we need to update. We keep a list of apps
             # that need to be updated, and a corresponding list of args
             # needed to update those apps.
             apps.append(app_name)
@@ -219,28 +222,43 @@
 
                             # inline the base64 encoded config value
                             base64_contents = base64.b64decode(base64_path.read_text())
                             app['options'][option_key] = base64_contents
 
         return self.bundle, self.overlays
 
-    async def fetch_plan(self, charm_url, origin, overlays=[]):
-        entity_id = charm_url.path()
-        is_local = Schema.LOCAL.matches(charm_url.schema)
+    async def fetch_plan(self, bundle_url, origin, overlays=[]):
+        """fetch_plan is called by the model.deploy(). It gathers the information about the
+        bundle to be deployed (whether local or CharmHub), straightens it up, applies overlays
+        if any overlays are given. Validates the bundle against known issues. Resolves and adds
+        local charms if there's any in the bundle. Resolves and adds --include-file configs if
+        there's any. Finally it calls the BundleFacade.GetChanges() to get the plan for the
+        bundle to be handed to the execute_plan() by the model.deploy(). Note that it doesn't
+        return the plan, just saves it in the self (BundleHandler) to be used later.
+
+        :param client.URL bundle_url: the url of the bundle to be deployed
+        :param client.CharmOrigin origin: the origin of the bundle to be deployed
+        :param [string] overlays: paths for the yaml files containing overlays to be applied to
+        the bundle during deployment
+
+        :returns: None
+        """
+        entity_id = bundle_url.path()
+        is_local = Schema.LOCAL.matches(bundle_url.schema)
         bundle_dir = None
 
         if is_local and os.path.isfile(entity_id):
             bundle_yaml = Path(entity_id).read_text()
             bundle_dir = Path(entity_id).parent
         elif is_local and os.path.isdir(entity_id):
             bundle_yaml = (Path(entity_id) / "bundle.yaml").read_text()
             bundle_dir = Path(entity_id)
 
-        if Schema.CHARM_HUB.matches(charm_url.schema):
-            bundle_yaml = await self._download_bundle(charm_url, origin)
+        if Schema.CHARM_HUB.matches(bundle_url.schema):
+            bundle_yaml = await self._download_bundle(bundle_url, origin)
 
         if not bundle_yaml:
             raise JujuError('empty bundle, nothing to deploy')
 
         _bundles = [b for b in yaml.safe_load_all(bundle_yaml)]
         self.overlays = _bundles[1:]
         self.bundle = _bundles[0]
@@ -269,15 +287,15 @@
         self.bundle, self.overlays = self._resolve_include_file_config(bundle_dir)
 
         _yaml_data = [yaml.dump(self.bundle)]
         for overlay in self.overlays:
             _yaml_data.append(yaml.dump(overlay).replace('null', ''))
         yaml_data = "---\n".join(_yaml_data)
 
-        self.plan = await self.bundle_facade.GetChanges(
+        self.plan = await self.bundle_facade.GetChangesMapArgs(
             bundleurl=entity_id,
             yaml=yaml_data)
 
         if self.plan.errors:
             raise JujuError(self.plan.errors)
 
     async def _download_bundle(self, charm_url, origin):
@@ -469,18 +487,20 @@
                     break
         return results
 
 
 class ChangeInfo:
     _toPy = {}
 
-    def __init__(self, change_id, requires):
+    def __init__(self, change_id, requires, params=None):
         self.change_id = change_id
         self.requires = requires
 
+        type(self).from_dict(self, params)
+
     @classmethod
     def from_dict(cls, self, data):
         """from_dict converts a data bag into fields on a class instance.
         If a value is missing from the data, then None is assigned to the field
         instance value.
         """
         d = (data or {})
@@ -519,47 +539,14 @@
     :devices: optional devices constraints.
     :endpoint_bindings: optional endpoint bindings
     :resources: identifies the revision to use for each resource of the
         application's charm.
     :local_resources: identifies the path to the local resource of the
         application's charm.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(AddApplicationChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.charm = params[0]
-            self.series = params[1]
-            self.application = params[2]
-            self.options = params[3]
-            self.constraints = params[4]
-            self.storage = {k: parse_storage_constraint(v) for k, v in params[5].items()}
-            self.channel = None
-            if len(params) == 8:
-                # Juju 2.4 and below only sends the endpoint bindings and resources
-                self.endpoint_bindings = params[6]
-                self.resources = params[7]
-                self.devices = None
-                self.num_units = None
-            else:
-                # Juju 2.5+ sends devices before endpoint bindings, as well as num_units
-                # There might be placement but we need to ignore that.
-                self.devices = {k: parse_device_constraint(v) for k, v in params[6].items()}
-                self.endpoint_bindings = params[7]
-                self.resources = params[8]
-                self.num_units = params[9]
-                if len(params) > 10:
-                    self.channel = params[10]
-
-        elif isinstance(params, dict):
-            AddApplicationChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "deploy"
 
     async def run(self, context):
@@ -666,34 +653,14 @@
 
     Params holds the following values:
         :charm: URL of the charm to be added.
         :series: series of the charm to be added if the charm default is
            not sufficient.
         :channel: preferred channel for obtaining the charm.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(AddCharmChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.charm = params[0]
-            self.series = params[1]
-            if len(params) > 2 and params[2] != "":
-                self.channel = params[2]
-            else:
-                self.channel = None
-            if len(params) > 3 and params[3] != "":
-                self.architecture = params[3]
-            else:
-                self.architecture = None
-        elif isinstance(params, dict):
-            AddCharmChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "addCharm"
 
     async def run(self, context):
@@ -768,29 +735,14 @@
     Params holds the following values:
         :series: optional machine OS series.
         :constraints: optional machine constraints.
         :container_type: optionally type of the container (for instance
             "lxc" or kvm"). It is not specified for top level machines.
         :parent_id: id of the parent machine.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(AddMachineChange, self).__init__(change_id, requires)
-        # this one is weird, as it returns a set of parameters inside a list.
-        if isinstance(params, list):
-            options = params[0] or {}
-            self.series = options.get("series")
-            self.constraints = options.get("constraints")
-            self.container_type = options.get("containerType")
-            self.parent_id = options.get("parentId")
-        elif isinstance(params, dict):
-            AddMachineChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "addMachines"
 
     async def run(self, context):
@@ -860,26 +812,14 @@
         Endpoint1 and Endpoint2 hold relation endpoints in the
         "application:interface" form, where the application is either a
         placeholder pointing to an application change or in the case of a model
         that already has this application deployed, the name of the
         application, and the interface is optional. Examples are
         "$deploy-42:web", "$deploy-42", "mysql:db".
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(AddRelationChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.endpoint1 = params[0]
-            self.endpoint2 = params[1]
-        elif isinstance(params, dict):
-            AddRelationChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "addRelation"
 
     async def run(self, context):
@@ -922,26 +862,14 @@
 
     Params holds the following values:
         :application: application placeholder name for which a unit is
             added.
         :to: optional location where to add the unit, as a placeholder
             pointing to another unit change or to a machine change.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(AddUnitChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.application = params[0]
-            self.to = params[1]
-        elif isinstance(params, dict):
-            AddUnitChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "addUnit"
 
     async def run(self, context):
@@ -991,27 +919,14 @@
     Params holds the following values:
         :application: is the name of the application to create an offer for.
             added.
         :endpoint: is a list of application endpoint to expose as part of an
             offer.
         :offer_name: describes the offer name.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(CreateOfferChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.application = params[0]
-            self.endpoints = params[1]
-            self.offer_name = params[2]
-        elif isinstance(params, dict):
-            CreateOfferChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "createOffer"
 
     async def run(self, context):
@@ -1024,15 +939,15 @@
         application = context.resolve(self.application)
         for ep in self.endpoints:
             await context.model.create_offer(ep, offer_name=self.offer_name, application_name=application)
 
     def __str__(self):
         endpoints = ""
         if self.endpoints is not None:
-            endpoints = ":{}".format(self.endpoints.join(","))
+            endpoints = ":{}".format(",".join(self.endpoints))
         return "create offer {offer_name} using {application}{endpoints}".format(offer_name=self.offer_name,
                                                                                  application=self.application,
                                                                                  endpoints=endpoints)
 
 
 class ConsumeOfferChange(ChangeInfo):
     _toPy = {'url': 'url',
@@ -1046,26 +961,14 @@
         params could either be a list or a dict. The later being the newer
         return results.
 
     Params holds the following values:
         :url: contains the location of the offer
         :application_name: describes the application name on offer.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(ConsumeOfferChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.url = params[0]
-            self.application_name = params[1]
-        elif isinstance(params, dict):
-            ConsumeOfferChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "consumeOffer"
 
     async def run(self, context):
@@ -1102,26 +1005,14 @@
         :application: placeholder name of the application that must be
             exposed.
         :exposed_endpoints: a an optional dictionary where keys are endpoint
             names and values are dicts that specify the space names and CIDRs
             that should be able to access the port ranges that the application
             has opened for each endpoint.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(ExposeChange, self).__init__(change_id, requires)
-
-        self.exposed_endpoints = None
-        if isinstance(params, list):
-            self.application = params[0]
-        elif isinstance(params, dict):
-            ExposeChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "expose"
 
     async def run(self, context):
@@ -1152,26 +1043,14 @@
         params could either be a list or a dict. The later being the newer
         return results.
 
     Params holds the following values:
         :application: placeholder name of the application to be scaled.
         :scale: is the new scale value to use.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(ScaleChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.application = params[0]
-            self.scale = params[1]
-        elif isinstance(params, dict):
-            ScaleChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "scale"
 
     async def run(self, context):
@@ -1205,27 +1084,14 @@
 
     Params holds the following values:
         :id: is the placeholder for the application or machine change
             corresponding to the entity to be annotated.
         :entity_type: type of the entity, "application" or "machine".
         :ennotations: annotations as key/value pairs.
     """
-
-    def __init__(self, change_id, requires, params=None):
-        super(SetAnnotationsChange, self).__init__(change_id, requires)
-
-        if isinstance(params, list):
-            self.id = params[0]
-            self.entity_type = params[1]
-            self.annotations = params[2]
-        elif isinstance(params, dict):
-            SetAnnotationsChange.from_dict(self, params)
-        else:
-            raise Exception("unexpected params type")
-
     @staticmethod
     def method():
         """method returns an associated ID for the Juju API call.
         """
         return "setAnnotations"
 
     async def run(self, context):
```

### Comparing `juju-3.2.0.0/juju/charm.py` & `juju-3.2.0.1/juju/charm.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/charmhub.py` & `juju-3.2.0.1/juju/charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client.py` & `juju-3.2.0.1/juju/client/_client.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client1.py` & `juju-3.2.0.1/juju/client/_client1.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client10.py` & `juju-3.2.0.1/juju/client/_client10.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client11.py` & `juju-3.2.0.1/juju/client/_client11.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client12.py` & `juju-3.2.0.1/juju/client/_client12.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client13.py` & `juju-3.2.0.1/juju/client/_client13.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client14.py` & `juju-3.2.0.1/juju/client/_client14.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client15.py` & `juju-3.2.0.1/juju/client/_client15.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client16.py` & `juju-3.2.0.1/juju/client/_client16.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client17.py` & `juju-3.2.0.1/juju/client/_client17.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client18.py` & `juju-3.2.0.1/juju/client/_client18.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client2.py` & `juju-3.2.0.1/juju/client/_client2.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client3.py` & `juju-3.2.0.1/juju/client/_client3.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client4.py` & `juju-3.2.0.1/juju/client/_client4.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client5.py` & `juju-3.2.0.1/juju/client/_client5.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client6.py` & `juju-3.2.0.1/juju/client/_client6.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client7.py` & `juju-3.2.0.1/juju/client/_client7.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client8.py` & `juju-3.2.0.1/juju/client/_client8.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_client9.py` & `juju-3.2.0.1/juju/client/_client9.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/_definitions.py` & `juju-3.2.0.1/juju/client/_definitions.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/client.py` & `juju-3.2.0.1/juju/client/client.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/codegen.py` & `juju-3.2.0.1/juju/client/codegen.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/connection.py` & `juju-3.2.0.1/juju/client/connection.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/connector.py` & `juju-3.2.0.1/juju/client/connector.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/facade.py` & `juju-3.2.0.1/juju/client/facade.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/gocookies.py` & `juju-3.2.0.1/juju/client/gocookies.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/jujudata.py` & `juju-3.2.0.1/juju/client/jujudata.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/overrides.py` & `juju-3.2.0.1/juju/client/overrides.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/proxy/factory.py` & `juju-3.2.0.1/juju/client/proxy/factory.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/proxy/kubernetes/proxy.py` & `juju-3.2.0.1/juju/client/proxy/kubernetes/proxy.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/client/runner.py` & `juju-3.2.0.1/juju/client/runner.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/constraints.py` & `juju-3.2.0.1/juju/constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/controller.py` & `juju-3.2.0.1/juju/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,39 +559,22 @@
         current connected user.
 
         :param bool all: Flag to list all models, regardless of
         user accessibility (administrative users only)
 
         :returns: {str name : str UUID}
         """
-
-        if all:
-            facade = client.ControllerFacade.from_connection(
-                self.connection())
-        else:
-            facade = client.ModelManagerFacade.from_connection(
-                self.connection())
-            u_name = username if username else self.get_current_username()
-            user = tag.user(u_name)
-
-        for attempt in (1, 2, 3):
-            try:
-                if all:
-                    userModelList = await facade.AllModels()
-                else:
-                    userModelList = await facade.ListModels(tag=user)
-
-                return {um.model.name: um.model.uuid
-                        for um in userModelList.user_models}
-            except errors.JujuAPIError as e:
-                # retry concurrency error until resolved in Juju
-                # see: https://bugs.launchpad.net/juju/+bug/1721786
-                if 'has been removed' not in e.message or attempt == 3:
-                    raise
-                await jasyncio.sleep(attempt)
+        model_manager_facade = client.ModelManagerFacade.from_connection(self.connection())
+        u_name = username if username else self.get_current_username()
+        user = tag.user(u_name)
+
+        user_model_list = await model_manager_facade.ListModelSummaries(user_tag=user, all_=all)
+        model_summaries = [msr.result for msr in user_model_list.results]
+        return {model_summary.name: model_summary.uuid
+                for model_summary in model_summaries}
 
     async def list_models(self, username=None, all=False):
         """Return list of names of the available models on this controller.
 
         Equivalent to ``sorted((await self.model_uuids()).keys())``
         """
         uuids = await self.model_uuids(username, all)
@@ -741,32 +724,40 @@
 
     async def create_offer(self, model_uuid, endpoint, offer_name=None, application_name=None):
         """
         Offer a deployed application using a series of endpoints for use by
         consumers.
 
         @param endpoint: holds the application and endpoint you want to offer
-        @param offer_name: over ride the offer name to help the consumer
+        @param offer_name: override the offer name to help the consumer
+        @param application_name: overrides the application name in the endpoint
         """
-        try:
-            offer = parse_offer_endpoint(endpoint)
-        except OfferParseError as e:
-            log.error(e.message)
-            raise
 
-        if offer_name is None:
-            offer_name = offer.application
+        # If we have both the offer_name and the application_name
+        # then we're coming from bundle/overlays, so no need to parse the endpoint
+        # Also we accept endpoints without a colon (:) in the overlays
+        if offer_name and application_name:
+            o_name = offer_name
+            a_name = application_name
+            eps = {endpoint: endpoint}
+        else:
+            try:
+                offer = parse_offer_endpoint(endpoint)
+            except OfferParseError as e:
+                log.error(e.message)
+                raise
 
-        if application_name is None:
-            application_name = offer.application
+            o_name = offer_name if offer_name else offer.application
+            a_name = application_name if application_name else offer.application
+            eps = {name: name for name in offer.endpoints}
 
         params = client.AddApplicationOffer()
-        params.application_name = application_name
-        params.endpoints = {name: name for name in offer.endpoints}
-        params.offer_name = offer_name
+        params.application_name = a_name
+        params.endpoints = eps
+        params.offer_name = o_name
         params.model_tag = tag.model(model_uuid)
 
         facade = client.ApplicationOffersFacade.from_connection(self.connection())
         return await facade.Offer(offers=[params])
 
     async def list_offers(self, model_name):
         """
```

### Comparing `juju-3.2.0.0/juju/delta.py` & `juju-3.2.0.1/juju/delta.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/errors.py` & `juju-3.2.0.1/juju/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,21 @@
     pass
 
 
 class JujuBackupError(JujuError):
     pass
 
 
+class JujuNotValid(JujuError):
+    def __init__(self, entity_type, entity_name):
+        self.entity_type = entity_type
+        self.entity_name = entity_name
+        super().__init__(f'Invalid {entity_type} : {entity_name}')
+
+
 class JujuConfigError(JujuError):
     """Exception raised during processing a configuration key-value pair
     in a config set for an application.
     """
     def __init__(self, config, config_pair, message=None):
         self.config = config
         self.config_pair = config_pair
```

### Comparing `juju-3.2.0.0/juju/jasyncio.py` & `juju-3.2.0.1/juju/jasyncio.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/juju.py` & `juju-3.2.0.1/juju/juju.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/machine.py` & `juju-3.2.0.1/juju/machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/model.py` & `juju-3.2.0.1/juju/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,19 @@
         """Return a map of unit-id:Unit for all units currently in
         the model.
 
         """
         return self._live_entity_map('unit')
 
     @property
+    def subordinate_units(self):
+        """Return a map of unit-id:Unit for all subordinate units"""
+        return {u_name: u for u_name, u in self.units.items() if u.is_subordinate}
+
+    @property
     def relations(self):
         """Return a map of relation-id:Relation for all relations currently in
         the model.
 
         """
         return self._live_entity_map('relation')
 
@@ -1075,14 +1080,22 @@
         """Return a map of unit-id:Unit for all units currently in
         the model.
 
         """
         return self.state.units
 
     @property
+    def subordinate_units(self):
+        """Return a map of unit-id:Unit for all subordiante units currently in
+        the model.
+
+        """
+        return self.state.subordinate_units
+
+    @property
     def relations(self):
         """Return a list of all Relations currently in the model.
 
         """
         return list(self.state.relations.values())
 
     @property
@@ -1671,25 +1684,23 @@
         :param to: Placement directive as a string. For example:
 
             '23' - place on machine 23
             'lxd:7' - place in new lxd container on machine 7
             '24/lxd/3' - place in container 3 on machine 24
 
             If None, a new machine is provisioned.
+        :param devices: charm device constraints
         :param bool trust: Trust signifies that the charm should be deployed
             with access to trusted credentials. Hooks run by the charm can access
             cloud credentials and other trusted access credentials.
 
         :param str[] attach_storage: Existing storage to attach to the deployed unit
             (not available on k8s models)
-        TODO::
-
-            - support local file resources
-
         """
+
         if storage:
             storage = {
                 k: client.Constraints(**v)
                 for k, v in storage.items()
             }
         if trust and (self.info.agent_version < client.Number.from_json('2.4.0')):
             raise NotImplementedError("trusted is not supported on model version {}".format(self.info.agent_version))
@@ -1813,14 +1824,23 @@
                 devices=devices,
                 charm_origin=charm_origin,
                 attach_storage=attach_storage,
                 force=force,
             )
 
     async def _add_charm(self, charm_url, origin):
+        """_add_charm sends the given origin and the url to the Juju API too add the charm to the
+        state. Either calls the CharmsFacade.AddCharm for (> version 2), or the
+        ClientFacade.AddCharm (for older versions).
+
+        :param str charm_url: the url of the charm to be added
+        :param client.CharmOrigin origin: the origin for the charm to be added
+
+        :returns client.CharmOriginResult
+        """
         # client facade is deprecated with in Juju, and smaller, more focused
         # facades have been created and we'll use that if it's available.
         charms_cls = client.CharmsFacade
         if charms_cls.best_facade_version(self.connection()) > 2:
             charms_facade = charms_cls.from_connection(self.connection())
             return await charms_facade.AddCharm(charm_origin=origin, url=charm_url, force=False)
 
@@ -1876,27 +1896,43 @@
         selected_series = utils.series_selector(series, url, model_config, supported_series, force)
         result.charm_origin.base = utils.get_base_from_origin_or_channel(resolved_origin, selected_series)
         charm_url.series = selected_series
 
         return str(charm_url), resolved_origin
 
     async def _resolve_architecture(self, url):
+        """_resolve_architecture returns the architecture for a given charm url.
+        :param str url: the client.URL to determine the arch for
+
+        :returns str architecture for the given url
+        """
+
         if url.architecture:
             return url.architecture
 
         constraints = await self.get_constraints()
         if 'arch' in constraints:
             return constraints['arch']
 
         return DEFAULT_ARCHITECTURE
 
     async def _add_charmhub_resources(self, application,
                                       entity_url,
                                       origin,
                                       overrides=None):
+        """_add_charmhub_resources is called by the deploy to add pending resources requested by
+        the charm being deployed. It calls the ResourcesFacade.AddPendingResources.
+
+        :param str application: the name of the application
+        :param client.CharmURL entity_url: url for the charm that we add resources for
+        :param client.CharmOrigin origin: origin for the charm that we add resources for
+
+        :returns [string]string resource_map that is a map of resources to their assigned
+        pendingIDs.
+        """
         charm_facade = client.CharmsFacade.from_connection(self.connection())
         res = await charm_facade.CharmInfo(entity_url)
 
         resources = []
         for resource in res.meta.resources.values():
             resources.append({
                 'description': resource.description,
@@ -1932,14 +1968,28 @@
         resource_map = {resource['name']: pid
                         for resource, pid
                         in zip(resources, response.pending_ids or {})}
 
         return resource_map
 
     async def add_local_resources(self, application, entity_url, metadata, resources):
+        """_add_local_resources is called by the deploy to add pending local  resources requested by
+        the charm being deployed. It calls the ResourcesFacade.AddPendingResources. After getting
+        the pending IDs from the controller it sends an HTTP PUT request to actually upload local
+        resources.
+
+        :param str application: the name of the application
+        :param client.CharmURL entity_url: url for the charm that we add resources for
+        :param [string]string metadata: metadata for the charm that we add resources for
+        :param [string] resources: the paths for the local files (or oci-images) to be added as
+        local resources
+
+        :returns [string]string resource_map that is a map of resources to their assigned
+        pendingIDs.
+        """
         if not resources:
             return None
 
         resource_map = dict()
 
         for name, path in resources.items():
             resource_type = metadata["resources"][name]["type"]
@@ -2520,63 +2570,64 @@
                 if current.controller_name is not None:
                     controller_name = current.controller_name
         await controller.connect(controller_name=controller_name)
         return controller
 
     async def wait_for_idle(self, apps=None, raise_on_error=True, raise_on_blocked=False,
                             wait_for_active=False, timeout=10 * 60, idle_period=15, check_freq=0.5,
-                            status=None, wait_for_units=None, wait_for_exact_units=None):
+                            status=None, wait_for_at_least_units=None, wait_for_exact_units=None):
         """Wait for applications in the model to settle into an idle state.
 
-        :param apps (list[str]): Optional list of specific app names to wait on.
+        :param List[str] apps: Optional list of specific app names to wait on.
             If given, all apps must be present in the model and idle, while other
             apps in the model can still be busy. If not given, all apps currently
             in the model must be idle.
 
-        :param raise_on_error (bool): If True, then any unit or app going into
+        :param bool raise_on_error: If True, then any unit or app going into
             "error" status immediately raises either a JujuAppError or a JujuUnitError.
             Note that machine or agent failures will always raise an exception (either
             JujuMachineError or JujuAgentError), regardless of this param. The default
             is True.
 
-        :param raise_on_blocked (bool): If True, then any unit or app going into
+        :param bool raise_on_blocked: If True, then any unit or app going into
             "blocked" status immediately raises either a JujuAppError or a JujuUnitError.
-            The defaul tis False.
+            The default is False.
 
-        :param wait_for_active (bool): If True, then also wait for all unit workload
+        :param bool wait_for_active: If True, then also wait for all unit workload
             statuses to be "active" as well. The default is False.
 
-        :param timeout (float): How long to wait, in seconds, for the bundle settles
+        :param float timeout: How long to wait, in seconds, for the bundle settles
             before raising an asyncio.TimeoutError. If None, will wait forever.
             The default is 10 minutes.
 
-        :param idle_period (float): How long, in seconds, the agent statuses of all
+        :param float idle_period: How long, in seconds, the agent statuses of all
             units of all apps need to be `idle`. This delay is used to ensure that
             any pending hooks have a chance to start to avoid false positives.
             The default is 15 seconds.
 
-        :param check_freq (float): How frequently, in seconds, to check the model.
+        :param float check_freq: How frequently, in seconds, to check the model.
             The default is every half-second.
 
-        :param status (str): The status to wait for. If None, not waiting.
+        :param str status: The status to wait for. If None, not waiting.
             The default is None (not waiting for any status).
 
-        :param wait_for_units (int): The least number of units to be expected before
-            going into the idle state.
+        :param int wait_for_at_least_units: The least number of units to go into the idle
+        state. wait_for_idle will return after that many units are available (across all the
+        given applications).
             The default is 1 unit.
 
-        :param wait_for_exact_units (int): The exact number of units to be expected before
+        :param int wait_for_exact_units: The exact number of units to be expected before
             going into the idle state. (e.g. useful for scaling down).
             When set, takes precedence over the `wait_for_units` parameter.
         """
         if wait_for_active:
             warnings.warn("wait_for_active is deprecated; use status", DeprecationWarning)
             status = "active"
 
-        _wait_for_units = wait_for_units if wait_for_units is not None else 1
+        _wait_for_units = wait_for_at_least_units if wait_for_at_least_units is not None else 1
 
         timeout = timedelta(seconds=timeout) if timeout is not None else None
         idle_period = timedelta(seconds=idle_period)
         start_time = datetime.now()
         # Type check against the common error of passing a str for apps
         if apps is not None and (not isinstance(apps, list) or
                                  any(not isinstance(o, str)
@@ -2635,37 +2686,51 @@
                                     (wait_for_exact_units, len(app.units)))
                         continue
                 # If we have less # of units then required, then wait a bit more
                 elif len(app.units) < _wait_for_units:
                     busy.append(app.name + " (not enough units yet - %s/%s)" %
                                 (len(app.units), _wait_for_units))
                     continue
-                # User wants to see a certain # of units, and we have enough
-                elif wait_for_units and len(units_ready) >= _wait_for_units:
+                # User is waiting for at least a certain # of units, and we have enough
+                elif wait_for_at_least_units and len(units_ready) >= _wait_for_units:
                     # So no need to keep looking, we have the desired number of units ready to go,
-                    # exit the loop. Don't return, though, we might still have some errors to raise
+                    # exit the loop. Don't just return here, though, we might still have some
+                    # errors to raise at the end
                     break
                 for unit in app.units:
                     if unit.machine is not None and unit.machine.status == "error":
                         errors.setdefault("Machine", []).append(unit.machine.id)
                         continue
                     if unit.agent_status == "error":
                         errors.setdefault("Agent", []).append(unit.name)
                         continue
                     if raise_on_error and unit.workload_status == "error":
                         errors.setdefault("Unit", []).append(unit.name)
                         continue
                     if raise_on_blocked and unit.workload_status == "blocked":
                         blocks.setdefault("Unit", []).append(unit.name)
                         continue
-                    waiting_for_a_particular_status = status and unit.workload_status != status
-                    if not waiting_for_a_particular_status and unit.agent_status == "idle":
-                        # We'll be here in two cases:
-                        # 1) We're not waiting for a particular status and the agent is "idle"
-                        # 2) We're waiting for a particular status and the workload is in that status
+                    # TODO (cderici): we need two versions of wait_for_idle, one for waiting on
+                    #  individual units, another one for waiting for an application.
+                    #  The convoluted logic below is the result of trying to do both at the same
+                    #  time
+                    need_to_wait_more_for_a_particular_status = status and (unit.workload_status != status)
+                    app_is_in_desired_status = (not status) or (app_status == status)
+                    if not need_to_wait_more_for_a_particular_status and \
+                            unit.agent_status == "idle" and \
+                            (wait_for_at_least_units or app_is_in_desired_status):
+                        # A unit is ready if either:
+                        # 1) Don't need to wait more for a particular status and the agent is "idle"
+                        # 2) We're looking for a particular status and the unit's workload,
+                        # as well as the application, is in that status. If the user wants to
+                        # see only a particular number of units in that state -- i.e. a subset of
+                        # the units is needed, then we don't care about the application status
+                        # (because e.g. app can be in 'waiting' while unit.0 is 'active' and unit.1
+                        # is 'waiting')
+
                         # Either way, the unit is ready, start measuring the time period that
                         # it needs to stay in that state (i.e. idle_period)
                         units_ready.add(unit.name)
                         now = datetime.now()
                         idle_start = idle_times.setdefault(unit.name, now)
 
                         if now - idle_start < idle_period:
```

### Comparing `juju-3.2.0.0/juju/names.py` & `juju-3.2.0.1/juju/names.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/offerendpoints.py` & `juju-3.2.0.1/juju/offerendpoints.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/origin.py` & `juju-3.2.0.1/juju/origin.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/placement.py` & `juju-3.2.0.1/juju/placement.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/provisioner.py` & `juju-3.2.0.1/juju/provisioner.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/relation.py` & `juju-3.2.0.1/juju/relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/remoteapplication.py` & `juju-3.2.0.1/juju/remoteapplication.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,7 +40,15 @@
         return tag.application(self.name)
 
 
 class ApplicationOffer(model.ModelEntity):
     @property
     def tag(self):
         return tag.application(self.name)
+
+    @property
+    def offer_name(self):
+        return self.safe_data['offer-name']
+
+    @property
+    def application_name(self):
+        return self.safe_data['application-name']
```

### Comparing `juju-3.2.0.0/juju/status.py` & `juju-3.2.0.1/juju/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/tag.py` & `juju-3.2.0.1/juju/tag.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/unit.py` & `juju-3.2.0.1/juju/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,28 @@
     def agent_status_since(self):
         """Get the time when the `agent_status` was last updated.
 
         """
         return pyrfc3339.parse(self.safe_data['agent-status']['since'])
 
     @property
+    def is_subordinate(self):
+        """True if the unit is subordinate of another unit
+
+        """
+        return self.safe_data['subordinate']
+
+    @property
+    def principal_unit(self):
+        """Returns the name of the unit of which this unit is a subordinate to.
+        Returns '' for principal units themselves.
+        """
+        return self.safe_data['principal']
+
+    @property
     def agent_status_message(self):
         """Get the agent status message.
 
         """
         return self.safe_data['agent-status']['message']
 
     @property
@@ -73,14 +87,22 @@
         """
         return self.safe_data['public-address'] or None
 
     @property
     def tag(self):
         return tag.unit(self.name)
 
+    def get_subordinates(self):
+        """Returns the unit objects that are subordinates to this unit
+
+        :return [Unit]
+        """
+        return [u for u_name, u in self.model.units.items() if u.is_subordinate and
+                u.principal_unit == self.name]
+
     async def destroy(self):
         """Destroy this unit.
 
         """
         app_facade = client.ApplicationFacade.from_connection(self.connection)
 
         log.debug(
```

### Comparing `juju-3.2.0.0/juju/url.py` & `juju-3.2.0.1/juju/url.py`

 * *Files identical despite different names*

### Comparing `juju-3.2.0.0/juju/utils.py` & `juju-3.2.0.1/juju/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -519,7 +519,34 @@
         return user_requested('', supported_series, force)
     except JujuError:
         pass
 
     # Charm hasn't specified a default (likely due to being a local charm
     # deployed by path). Last chance, best we can do is default to LTS.
     return DEFAULT_SUPPORTED_LTS
+
+
+def should_upgrade_resource(available_resource, existing_resources):
+    """Called in the context of upgrade_charm. Given a resource R, takes a look at the resources we
+    already have and decides if we need to refresh R.
+
+    :param dict[str] available_resource: The dict representing the client.Resource coming from the
+    charmhub api. We're considering if we need to refresh this during upgrade_charm.
+    :param dict[str] existing_resources: The dict coming from resources_facade.ListResources
+    representing the resources of the currently deployed charm.
+
+    :result bool: The decision to refresh the given resource
+    """
+    # should upgrade resource?
+    res_name = available_resource.get('Name', available_resource.get('name'))
+    # no, if it's upload
+    if existing_resources[res_name].origin == 'upload':
+        return False
+
+    # no, if we already have it (and upstream doesn't have a newer res available)
+    if res_name in existing_resources:
+        available_rev = available_resource.get('Revision', available_resource.get('revision', -1))
+        u_fields = existing_resources[res_name].unknown_fields
+        existing_rev = u_fields.get('Revision', u_fields.get('revision', -1))
+        if existing_rev >= available_rev:
+            return False
+    return True
```

### Comparing `juju-3.2.0.0/juju.egg-info/PKG-INFO` & `juju-3.2.0.1/juju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.2.0.0
+Version: 3.2.0.1
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 A Python library for Juju
 =========================
 
 Source code: https://github.com/juju/python-libjuju
 
@@ -24,21 +28,24 @@
 
 Documentation: https://pythonlibjuju.readthedocs.io/en/latest/
 
 
 Requirements
 ------------
 
-* Python 3.9/3.10
+This version may support old versions of Juju. However, it has been
+tested with the following requirements.
+
+* Python 3.8/3.9/3.10
 
 
 Design Notes
 ------------
 
-* Asynchronous - Uses asyncio and async/await features of Python
+* Asynchronous - uses asyncio and async/await features of python 3.5
 * Websocket-level bindings are programmatically generated (indirectly) from the
   Juju golang code, ensuring full api coverage
 * Provides an OO layer which encapsulates much of the websocket api and
   provides familiar nouns and verbs (e.g. Model.deploy(), Application.add_unit(),
   etc.)
 
 
@@ -53,14 +60,15 @@
 Quickstart
 ----------
 
 Here's a simple example that shows basic usage of the library. The example
 connects to the currently active Juju model, deploys a single unit of the
 ubuntu charm, then exits:
 
+Note : Pylibjuju requires an already bootstrapped Juju controller to connect to.
 
 .. code:: python
 
   #!/usr/bin/python3
 
   import logging
   import sys
@@ -78,17 +86,15 @@
       await model.connect_current()
 
       try:
           # Deploy a single unit of the ubuntu charm, using the latest revision
           # from the stable channel of the Charm Store.
           ubuntu_app = await model.deploy(
             'ubuntu',
-            application_name='ubuntu',
-            series='xenial',
-            channel='stable',
+            application_name='my-ubuntu',
           )
 
           if '--wait' in sys.argv:
               # optionally block until the application is ready
               await model.block_until(lambda: ubuntu_app.status == 'active')
       finally:
           # Disconnect from the api server and cleanup.
@@ -138,32 +144,54 @@
   >>> await model.connect_current()
   >>> status = await model.get_status()
 
 
 Versioning
 ----------
 
-Pylibjuju releases now track the Juju release cadence. New generated schemas
+The current Pylibjuju release policy tracks the Juju release cadence.
+In particular, whenever Juju makes a latest/stable release, pylibjuju pushes out
+a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.2.0.1
+^^^^^^^
+
+Thursday 20th July 2023
+
+This is a point release on the 3.x track, works with any Juju 3.x controller.
+
+What's Changed
+
+* Update readme and add some docstrings for functions by @cderici in https://github.com/juju/python-libjuju/pull/873
+* Forward port subordinate utils by @cderici in https://github.com/juju/python-libjuju/pull/880
+* [JUJU-3952] Revisit access control levels by @cderici in https://github.com/juju/python-libjuju/pull/882
+* [JUJU-3999] Avoid parsing endpoint for overlay offers by @cderici in https://github.com/juju/python-libjuju/pull/887
+* Forward port upgrade resource fixes in app refresh by @cderici in https://github.com/juju/python-libjuju/pull/889
+* [JUJU-4076] Rename `wait_for_units` and make semantics clearer by @cderici in https://github.com/juju/python-libjuju/pull/890
+* Stabilize sphinx build on RTD by @cderici in https://github.com/juju/python-libjuju/pull/899
+* Move test utils into a separate module by @cderici in https://github.com/juju/python-libjuju/pull/903
+* Remove title prefixes from issue templates by @cderici in https://github.com/juju/python-libjuju/pull/904
+* [JUJU-4048] Use GetChangesMapArgs for bundle changes by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/907
+* Forward ports from 2.9 to 3.x by @cderici in https://github.com/juju/python-libjuju/pull/910
+* Remove ceiling on pyyaml version by @cderici in https://github.com/juju/python-libjuju/pull/918
+
 3.2.0.0
 ^^^^^^^
 
 Wednesday 7th June 2023
 
 This release contains the new endpoints for Juju 3.2.0.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
 * Add base.bootstrapped decorator to integration test by @cderici in https://github.com/juju/python-libjuju/pull/856
 * Add mantic and lunar to list of ubuntu series by @addyess in https://github.com/juju/python-libjuju/pull/853
 * [JUJU-3885] forward port ipv6 support by @cderici in https://github.com/juju/python-libjuju/pull/866
 * Revisit auto documentation generation with sphinx on RTD by @cderici in https://github.com/juju/python-libjuju/pull/871
 * [JUJU-3894] Forward port some fixes from 2.9 to master by @cderici in https://github.com/juju/python-libjuju/pull/870
 * Revisit the secret backend integration test by @cderici in https://github.com/juju/python-libjuju/pull/858
 * [JUJU-3954] Fix incorrect base channel computation by @cderici in https://github.com/juju/python-libjuju/pull/875
@@ -175,17 +203,14 @@
 Friday 5th May 2023
 
 This release has been tested with Juju 3.1.2 and contains the new 
 endpoints for secrets backend.
 
 This release works with any Juju 3.x controller.
 
-What's Changed
-""""""""""""""
-
 * [JUJU-3202] Add facades for 3.1.1. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/807
 * Add destroy units by @cderici in https://github.com/juju/python-libjuju/pull/812
 * [JUJU-3517] Revisit _build_facades in connection by @cderici in https://github.com/juju/python-libjuju/pull/826
 * [JUJU-3527] Added 3.1.2 and 3.2-beta2 schemas. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/828
 * [JUJU-1628] Deploy by revision by @cderici in https://github.com/juju/python-libjuju/pull/830
 * [JUJU-3552] Prepare 3.1.2.1 release by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/836
 
@@ -195,63 +220,52 @@
 Friday 10th February 2023
 
 This release targets juju version 3.1.0 and enables the new secrets backend api.
 Connectivity with juju controllers in the 3.x series is allowed, connections with different major version controllers (e.g. 2.x, 4.x, etc.) will be cancelled.
 
 This version is only tested using Juju 3.1.0.
 
-What's Changed
-""""""""""""""
-
 * setup.py: adjust websockets versions for py38-310 by @mert-kirpici in https://github.com/juju/python-libjuju/pull/731
 * [JUJU-2175] Remove juju 2.9 support on 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/774
 * [JUJU-2276] Series or base for local charms by @cderici in https://github.com/juju/python-libjuju/pull/777
 * [JUJU-2391] Fix wrong bases analysis. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/782
 * [JUJU-2401] Added release candidate workflow. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/784
 * [JUJU-2402] Prepare nightly juju edge testing. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/785
 * [JUJU-2237] Remove charmstore charm support from pylibjuju by @cderici in https://github.com/juju/python-libjuju/pull/786
 * [JUJU-2426] Secrets support by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/791
 * [JUJU-2573] Base argument for model deploy by @cderici in https://github.com/juju/python-libjuju/pull/798
 * Add compatibility for juju 3.1.0 by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/799
 * Replace schemas.json with a wellformed version. by @juanmanuel-tirado in https://github.com/juju/python-libjuju/pull/800
 
 New Contributors
-""""""""""""""""
 
 * @mert-kirpici made their first contribution in https://github.com/juju/python-libjuju/pull/731
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.4...3.1.0.1
 
 3.0.4
 ^^^^^
 
 Wednesday 26th October
 
-What's Changed
-""""""""""""""
-
 * [JUJU-2027] Local refresh with resoruces by @cderici in https://github.com/juju/python-libjuju/pull/757
 * [JUJU-2026] Improve resolve charm by @cderici in https://github.com/juju/python-libjuju/pull/761
 * Add owner and data to license file by @arturo-seijas in https://github.com/juju/python-libjuju/pull/760
 
 New Contributors
-""""""""""""""""
 
 * @arturo-seijas made their first contribution in https://github.com/juju/python-libjuju/pull/760
 
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.3...3.0.4
 
 3.0.3
 ^^^^^
 
 Saturay October 22 2022
 
-What's Changed
-""""""""""""""
-
 * Wait for idle arg type check by @cderici in https://github.com/juju/python-libjuju/pull/741
 * [JUJU-1970] Revise local refresh by @cderici in https://github.com/juju/python-libjuju/pull/742
 * [JUJU-1984] Update facade schemas for juju 3.0-rc1-2 by @cderici in https://github.com/juju/python-libjuju/pull/745
 * [JUJU-1992] Fix charmhub series deploy 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/746
 * [JUJU-2001] Fix base for local charms and bundles for CharmOrigin 3.0 by @cderici in https://github.com/juju/python-libjuju/pull/749
 * [JUJU-2017] Check subordinate field value instead of existence by @cderici in https://github.com/juju/python-libjuju/pull/751
 * [JUJU-2018] Update 2.9.36 facades & clients by @cderici in https://github.com/juju/python-libjuju/pull/752
@@ -262,17 +276,14 @@
 **Full Changelog**: https://github.com/juju/python-libjuju/compare/3.0.2...3.0.3
 
 3.0.2
 ^^^^^
 
 Wednesday October 5 2022
 
-What's Changed
-""""""""""""""
-
 * Model name can now be accessed through model.name by @jack-w-shaw in https://github.com/juju/python-libjuju/pull/702
 * [JUJU-1593] Fix `unit.run()` and update the old client codes by @cderici in https://github.com/juju/python-libjuju/pull/710
 * Add py.typed marker by @sed-i in https://github.com/juju/python-libjuju/pull/709
 * [JUJU-1664] Add force, no-wait, destroy-storage params to app.destroy by @cderici in https://github.com/juju/python-libjuju/pull/714
 * snapcraft.io access should use https requests by @addyess in https://github.com/juju/python-libjuju/pull/715
 * [JUJU-1680] Add issue and PR templates by @cderici in https://github.com/juju/python-libjuju/pull/718
 * [JUJU-1681] Add --attach-storage parameter to model.deploy by @cderici in https://github.com/juju/python-libjuju/pull/720
```

### Comparing `juju-3.2.0.0/juju.egg-info/SOURCES.txt` & `juju-3.2.0.1/juju.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 examples/relate.py
 examples/run_action.py
 examples/scp.py
 examples/status.py
 examples/unitrun.py
 examples/upgrade_local_charm_k8s.py
 juju/__init__.py
+juju/access.py
 juju/action.py
 juju/annotation.py
 juju/annotationhelper.py
 juju/application.py
 juju/bundle.py
 juju/charm.py
 juju/charmhub.py
@@ -101,15 +102,14 @@
 juju/machine.py
 juju/model.py
 juju/names.py
 juju/offerendpoints.py
 juju/origin.py
 juju/placement.py
 juju/provisioner.py
-juju/py.typed
 juju/relation.py
 juju/remoteapplication.py
 juju/status.py
 juju/tag.py
 juju/unit.py
 juju/url.py
 juju/user.py
```

### Comparing `juju-3.2.0.0/setup.py` & `juju-3.2.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,48 +19,52 @@
 here = Path(__file__).absolute().parent
 readme = here / 'docs' / 'readme.rst'
 changelog = here / 'docs' / 'changelog.rst'
 long_description = '{}\n\n{}'.format(
     readme.read_text(),
     changelog.read_text()
 )
+long_description_content_type = 'text/x-rst'
 version = here / 'VERSION'
 
 setup(
     name='juju',
     version=version.read_text().strip(),
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
-    package_data={'juju': ['py.typed']},
     install_requires=[
         'macaroonbakery>=1.1,<2.0',
         'pyRFC3339>=1.0,<2.0',
-        'pyyaml>=5.1.2,<=6.0',
-        'websockets>=8.1,<9.0 ; python_version=="3.8"',
-        'websockets>=9.0,<10.0 ; python_version=="3.9"',
-        'websockets>=10.0; python_version>"3.9"',
+        'pyyaml>=5.1.2',
+        'theblues>=0.5.1,<1.0',
+        'websockets>=7.0,<8.0 ; python_version<"3.9"',
+        'websockets>=8.0,<9.0 ; python_version=="3.9"',
+        'websockets>=9.0; python_version>"3.9"',
         'paramiko>=2.4.0,<3.0.0',
         'pyasn1>=0.4.4',
         'toposort>=1.5,<2',
         'typing_inspect>=0.6.0',
         'kubernetes>=12.0.1',
-        'hvac',
     ],
     include_package_data=True,
     maintainer='Juju Ecosystem Engineering',
     maintainer_email='juju@lists.ubuntu.com',
     description=('Python library for Juju'),
     long_description=long_description,
+    long_description_content_type=long_description_content_type,
     url='https://github.com/juju/python-libjuju',
     license='Apache 2',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     entry_points={
         'console_scripts': [
         ],
```

