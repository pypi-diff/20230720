# Comparing `tmp/collective.task-3.0.8.tar.gz` & `tmp/collective.task-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.task-3.0.8.tar", last modified: Fri May 13 15:53:02 2022, max compression
+gzip compressed data, was "collective.task-3.0.9.tar", last modified: Tue Jun 21 08:46:02 2022, max compression
```

## Comparing `collective.task-3.0.8.tar` & `collective.task-3.0.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)     3480 2022-05-13 15:53:02.000000 collective.task-3.0.8/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      124 2022-05-13 15:53:02.000000 collective.task-3.0.8/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      185 2022-05-13 15:53:02.000000 collective.task-3.0.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     8062 2022-05-13 15:53:02.825772 collective.task-3.0.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2181 2022-05-13 15:53:02.000000 collective.task-3.0.8/README.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-05-13 15:53:02.000000 collective.task-3.0.8/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      726 2022-05-13 15:53:02.000000 collective.task-3.0.8/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-05-13 15:53:02.825772 collective.task-3.0.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1814 2022-05-13 15:53:02.000000 collective.task-3.0.8/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.821772 collective.task-3.0.8/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)      268 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/
--rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6388 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/adapters.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6186 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/behaviors.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      756 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/behaviors.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     5545 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/batchactions.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2306 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/browser/static/
--rw-rw-r--   0 sge       (1000) sge       (1000)      248 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/back_in_created.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      269 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/back_in_progress.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      276 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/back_in_realized.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      284 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/back_in_to_assign.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      245 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/back_in_to_do.png
--rw-rw-r--   0 sge       (1000) sge       (1000)     1749 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/collectivetask.css
--rw-rw-r--   0 sge       (1000) sge       (1000)      258 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/do_closed.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      273 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/do_in_progress.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      276 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/do_realized.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      278 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/do_to_assign.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      247 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/do_to_do.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      696 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/static/task_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)     3920 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/table.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1917 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/table.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/browser/templates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1453 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/templates/demoview.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)      240 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/templates/list_tasks.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)      739 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/templates/task_parent.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     1570 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/viewlets.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      882 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/browser/views.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2648 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/content/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/content/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      104 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/content/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      501 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/content/task.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      537 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/field.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2728 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/interfaces.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.821772 collective.task-3.0.8/src/collective/task/locales/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.821772 collective.task-3.0.8/src/collective/task/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1164 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     2872 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/collective.task.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     2463 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.821772 collective.task-3.0.8/src/collective/task/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1540 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     3910 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/collective.task.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     2643 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/plone.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/migrations/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/migrations/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1368 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/migrations/migrate_to_100.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      755 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/migrations/migrate_to_101.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      848 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/migrations/migrate_to_2_2.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      520 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/migrations/migrate_to_2_2_2.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      145 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      531 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/collectivetask_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      354 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/cssregistry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      180 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      325 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/portal_atct.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2178 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/registry.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2363 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/types/task.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      226 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/types.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/default/workflows/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/default/workflows/task_workflow/
--rw-rw-r--   0 sge       (1000) sge       (1000)    20124 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/workflows/task_workflow/definition.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      345 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/default/workflows.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/testing/metadata.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/
--rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      662 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/collectivetask_uninstall_1_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      294 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/import_steps.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      245 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/portlets.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      658 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/registry.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2787 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/profiles.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3491 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2615 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      626 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/subscribers.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1400 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      497 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/testing.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective/task/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2007 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/robot/test_example.robot
--rw-rw-r--   0 sge       (1000) sge       (1000)     7360 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_adapters.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     7227 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_batchactions.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2829 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_behaviors.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      874 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1470 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     6740 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_subscribers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     4078 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_table.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1668 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_utility.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1892 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/tests/test_viewlets.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      787 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective/task/utility.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-05-13 15:53:02.825772 collective.task-3.0.8/src/collective.task.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     8062 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     4252 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      316 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-05-13 15:53:02.000000 collective.task-3.0.8/src/collective.task.egg-info/top_level.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.038378 collective.task-3.0.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3618 2022-06-21 08:46:01.000000 collective.task-3.0.9/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      124 2022-06-21 08:46:01.000000 collective.task-3.0.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      185 2022-06-21 08:46:01.000000 collective.task-3.0.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6453 2022-06-21 08:46:02.038378 collective.task-3.0.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2181 2022-06-21 08:46:01.000000 collective.task-3.0.9/README.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-06-21 08:46:01.000000 collective.task-3.0.9/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      726 2022-06-21 08:46:01.000000 collective.task-3.0.9/docs/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-06-21 08:46:02.038378 collective.task-3.0.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1837 2022-06-21 08:46:01.000000 collective.task-3.0.9/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      268 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6388 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/adapters.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6186 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/behaviors.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      756 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/behaviors.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5545 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/batchactions.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2306 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/browser/static/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      248 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/back_in_created.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      269 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/back_in_progress.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      276 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/back_in_realized.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      284 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/back_in_to_assign.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      245 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/back_in_to_do.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1749 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/collectivetask.css
+-rw-rw-r--   0 sge       (1000) sge       (1000)      258 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/do_closed.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      273 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/do_in_progress.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      276 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/do_realized.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      278 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/do_to_assign.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      247 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/do_to_do.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      696 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/static/task_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3956 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/table.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1917 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/table.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1453 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/templates/demoview.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      240 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/templates/list_tasks.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      739 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/templates/task_parent.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1570 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/viewlets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      882 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/browser/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2648 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/content/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/content/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      104 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/content/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      501 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/content/task.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      537 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/field.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2728 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/interfaces.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/locales/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1164 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2872 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/collective.task.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2463 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1540 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3910 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/collective.task.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2643 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/migrations/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/migrations/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1368 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/migrations/migrate_to_100.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      755 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/migrations/migrate_to_101.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      848 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/migrations/migrate_to_2_2.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      520 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/migrations/migrate_to_2_2_2.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      145 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      531 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/collectivetask_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      354 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/cssregistry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      180 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      325 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/portal_atct.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2178 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/registry.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2363 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/types/task.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      226 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/types.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/default/workflows/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/default/workflows/task_workflow/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    20124 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/workflows/task_workflow/definition.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      345 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/default/workflows.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/testing/metadata.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      163 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/browserlayer.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      662 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/collectivetask_uninstall_1_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      294 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/import_steps.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      245 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/portlets.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      658 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/registry.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2787 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/profiles.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3491 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2615 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/subscribers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      626 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/subscribers.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1400 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      497 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.038378 collective.task-3.0.9/src/collective/task/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.038378 collective.task-3.0.9/src/collective/task/tests/robot/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2007 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/robot/test_example.robot
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7360 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_adapters.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7227 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_batchactions.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2829 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_behaviors.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      874 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_robot.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1470 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6740 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_subscribers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4078 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_table.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1668 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_utility.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1892 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/tests/test_viewlets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      787 2022-06-21 08:46:01.000000 collective.task-3.0.9/src/collective/task/utility.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-06-21 08:46:02.034378 collective.task-3.0.9/src/collective.task.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     6453 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4252 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      328 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-06-21 08:46:02.000000 collective.task-3.0.9/src/collective.task.egg-info/top_level.txt
```

### Comparing `collective.task-3.0.8/CHANGES.rst` & `collective.task-3.0.9/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.9 (2022-06-21)
+------------------
+
+- Required z3c.table 2.2 to include escaping, to avoid xss.
+  Escaped some columns.
+  [sgeulette]
+
 3.0.8 (2022-05-13)
 ------------------
 
 - Added `get_methods_adapter` on Task content class. So it's possible to get the adapter
   in an expression by example.
   [sgeulette]
```

### Comparing `collective.task-3.0.8/README.rst` & `collective.task-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/docs/LICENSE.GPL` & `collective.task-3.0.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/docs/LICENSE.rst` & `collective.task-3.0.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/setup.py` & `collective.task-3.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='collective.task',
-    version='3.0.8',
+    version='3.0.9',
     description="Tasks management for Plone.",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
@@ -43,18 +43,19 @@
     install_requires=[
         'dexterity.localrolesfield',
         'plone.api',
         'plone.app.lockingbehavior',
         'plone.directives.form',
         'plone.formwidget.masterselect',
         'plone.principalsource',
+        'future',
         'imio.helpers',
         'imio.migrator',
         'setuptools',
-        'z3c.table',
+        'z3c.table>=2.2',
     ],
     extras_require={
         'test': [
             'collective.eeafaceted.batchactions',
             'imio.prettylink',
             'plone.app.testing',
             'plone.app.contenttypes',
```

### Comparing `collective.task-3.0.8/src/collective/task/adapters.py` & `collective.task-3.0.9/src/collective/task/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/behaviors.py` & `collective.task-3.0.9/src/collective/task/behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/behaviors.zcml` & `collective.task-3.0.9/src/collective/task/behaviors.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/batchactions.py` & `collective.task-3.0.9/src/collective/task/browser/batchactions.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/configure.zcml` & `collective.task-3.0.9/src/collective/task/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/static/collectivetask.css` & `collective.task-3.0.9/src/collective/task/browser/static/collectivetask.css`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/static/task_icon.png` & `collective.task-3.0.9/src/collective/task/browser/static/task_icon.png`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/table.py` & `collective.task-3.0.9/src/collective/task/browser/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """Define tables and columns."""
 
 from collective.task import _
 from collective.task import PMF
 from collective.task.adapters import EMPTY_STRING
+from html import escape
 from plone import api
 from Products.CMFPlone.utils import normalizeString
 from Products.CMFPlone.utils import safe_unicode
 from z3c.table.column import Column
 from z3c.table.column import LinkColumn
 from z3c.table.table import Table
 from zope.cachedescriptors.property import CachedProperty
@@ -16,15 +17,14 @@
 try:
     from imio.prettylink.interfaces import IPrettyLink
 except ImportError:
     pass
 
 
 class TasksTable(Table):
-
     """Table that displays tasks info."""
 
     cssClassEven = u'even'
     cssClassOdd = u'odd'
     cssClasses = {'table': 'listing taskContainerListing icons-on'}
 
     batchSize = 20
@@ -45,45 +45,42 @@
 
     @CachedProperty
     def values(self):
         return self.results
 
 
 class UserColumn(Column):
-
     """Base user column."""
 
     field = NotImplemented
 
     def renderCell(self, value):
         username = getattr(value, self.field, '')
         if username and username != EMPTY_STRING:
             member = api.user.get(username)
-            return member.getUser().getProperty('fullname').decode('utf-8')
+            return escape(member.getUser().getProperty('fullname').decode('utf-8'))
 
         return ""
 
 
 class TitleColumn(LinkColumn):
-
     """Column that displays title."""
 
     header = PMF("Title")
     weight = 10
 
     def getLinkCSS(self, item):
         return ' class="state-%s contenttype-%s"' % (api.content.get_state(obj=item),
                                                      normalizeString(item.portal_type))
 
     def getLinkContent(self, item):
         return safe_unicode(item.title)
 
 
 class PrettyLinkTitleColumn(TitleColumn):
-
     """Column that displays prettylink title."""
 
     header = PMF("Title")
     weight = 10
 
     params = {}
 
@@ -95,71 +92,63 @@
 
     def renderCell(self, item):
         """ """
         return self.getPrettyLink(item)
 
 
 class EnquirerColumn(UserColumn):
-
     """Column that displays enquirer."""
 
     header = _("Enquirer")
     weight = 20
     field = 'enquirer'
 
 
 class AssignedGroupColumn(Column):
-
     """Column that displays assigned group."""
 
     header = _("Assigned group")
     weight = 30
 
     def renderCell(self, value):
         if value.assigned_group:
             group = api.group.get(value.assigned_group).getGroup()
-            return group.getProperty('title').decode('utf-8')
-
+            return escape(group.getProperty('title').decode('utf-8'))
         return ""
 
 
 class AssignedUserColumn(UserColumn):
-
     """Column that displays assigned user."""
 
     header = _("Assigned user")
     weight = 40
     field = 'assigned_user'
 
 
 class DueDateColumn(Column):
-
     """Column that displays due date."""
 
     header = _("Due date")
     weight = 50
     long_format = False
     time_only = False
 
     def renderCell(self, value):
         if value.due_date:
             return api.portal.get_localized_time(datetime=value.due_date, long_format=self.long_format,
                                                  time_only=self.time_only)
-
         return ""
 
 
 class ReviewStateColumn(Column):
-
     """Column that displays value's review state."""
 
     header = PMF("Review state")
     weight = 60
 
     def renderCell(self, value):
         state = api.content.get_state(value)
         if state:
             wtool = api.portal.get_tool('portal_workflow')
             state_title = wtool.getTitleForStateOnType(state, value.portal_type)
-            return translate(PMF(state_title), context=self.request)
-
+            return escape(translate(PMF(state_title), context=self.request))
         return ''
```

### Comparing `collective.task-3.0.8/src/collective/task/browser/table.zcml` & `collective.task-3.0.9/src/collective/task/browser/table.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/templates/demoview.pt` & `collective.task-3.0.9/src/collective/task/browser/templates/demoview.pt`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/templates/task_parent.pt` & `collective.task-3.0.9/src/collective/task/browser/templates/task_parent.pt`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/viewlets.py` & `collective.task-3.0.9/src/collective/task/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/browser/views.py` & `collective.task-3.0.9/src/collective/task/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/configure.zcml` & `collective.task-3.0.9/src/collective/task/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/field.py` & `collective.task-3.0.9/src/collective/task/field.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/interfaces.py` & `collective.task-3.0.9/src/collective/task/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/collective.task.po` & `collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/collective.task.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/en/LC_MESSAGES/plone.po` & `collective.task-3.0.9/src/collective/task/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po` & `collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/collective.eeafaceted.batchactions.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/collective.task.po` & `collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/collective.task.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/locales/fr/LC_MESSAGES/plone.po` & `collective.task-3.0.9/src/collective/task/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/migrations/migrate_to_100.py` & `collective.task-3.0.9/src/collective/task/migrations/migrate_to_100.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/migrations/migrate_to_101.py` & `collective.task-3.0.9/src/collective/task/migrations/migrate_to_101.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/migrations/migrate_to_2_2.py` & `collective.task-3.0.9/src/collective/task/migrations/migrate_to_2_2.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/migrations/migrate_to_2_2_2.py` & `collective.task-3.0.9/src/collective/task/migrations/migrate_to_2_2_2.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/default/catalog.xml` & `collective.task-3.0.9/src/collective/task/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/default/registry.xml` & `collective.task-3.0.9/src/collective/task/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/default/types/task.xml` & `collective.task-3.0.9/src/collective/task/profiles/default/types/task.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/default/workflows/task_workflow/definition.xml` & `collective.task-3.0.9/src/collective/task/profiles/default/workflows/task_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/catalog.xml` & `collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles/uninstall_1.0/registry.xml` & `collective.task-3.0.9/src/collective/task/profiles/uninstall_1.0/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/profiles.zcml` & `collective.task-3.0.9/src/collective/task/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/setuphandlers.py` & `collective.task-3.0.9/src/collective/task/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/subscribers.py` & `collective.task-3.0.9/src/collective/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/subscribers.zcml` & `collective.task-3.0.9/src/collective/task/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/testing.py` & `collective.task-3.0.9/src/collective/task/testing.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/robot/test_example.robot` & `collective.task-3.0.9/src/collective/task/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_adapters.py` & `collective.task-3.0.9/src/collective/task/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_batchactions.py` & `collective.task-3.0.9/src/collective/task/tests/test_batchactions.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_behaviors.py` & `collective.task-3.0.9/src/collective/task/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_robot.py` & `collective.task-3.0.9/src/collective/task/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_setup.py` & `collective.task-3.0.9/src/collective/task/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_subscribers.py` & `collective.task-3.0.9/src/collective/task/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_table.py` & `collective.task-3.0.9/src/collective/task/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_utility.py` & `collective.task-3.0.9/src/collective/task/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/tests/test_viewlets.py` & `collective.task-3.0.9/src/collective/task/tests/test_viewlets.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective/task/utility.py` & `collective.task-3.0.9/src/collective/task/utility.py`

 * *Files identical despite different names*

### Comparing `collective.task-3.0.8/src/collective.task.egg-info/SOURCES.txt` & `collective.task-3.0.9/src/collective.task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

