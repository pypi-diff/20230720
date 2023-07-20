# Comparing `tmp/ai-django-core-7.0.1.tar.gz` & `tmp/ai-django-core-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-django-core-7.0.1.tar", last modified: Thu May  4 13:25:36 2023, max compression
+gzip compressed data, was "ai-django-core-7.0.2.tar", last modified: Thu Jul 20 14:35:12 2023, max compression
```

## Comparing `ai-django-core-7.0.1.tar` & `ai-django-core-7.0.2.tar`

### file list

```diff
@@ -1,216 +1,217 @@
--rw-r--r--   0        0        0       82 2020-04-24 09:15:50.688102 ai-django-core-7.0.1/.coveragerc
--rw-r--r--   0        0        0      288 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/.editorconfig
--rw-r--r--   0        0        0     1736 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      400 2021-03-04 09:37:37.670469 ai-django-core-7.0.1/.gitignore
--rw-r--r--   0        0        0     3941 2023-02-21 14:56:14.192364 ai-django-core-7.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      443 2023-05-02 10:10:53.230359 ai-django-core-7.0.1/.readthedocs.yml
--rw-r--r--   0        0        0    18390 2023-05-04 13:24:40.338660 ai-django-core-7.0.1/CHANGES.md
--rw-r--r--   0        0        0      962 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/Dockerfile
--rw-r--r--   0        0        0     1104 2020-11-11 13:34:13.878022 ai-django-core-7.0.1/LICENSE.md
--rw-r--r--   0        0        0      129 2021-05-12 15:21:27.853419 ai-django-core-7.0.1/MANIFEST.in
--rw-r--r--   0        0        0     4710 2023-05-04 13:15:53.544078 ai-django-core-7.0.1/README.md
--rw-r--r--   0        0        0       91 2023-05-04 13:24:40.338660 ai-django-core-7.0.1/ai_django_core/__init__.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.1/ai_django_core/admin/__init__.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.1/ai_django_core/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2022-05-24 06:31:55.191175 ai-django-core-7.0.1/ai_django_core/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2022-05-24 06:31:55.192174 ai-django-core-7.0.1/ai_django_core/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2022-05-24 06:31:55.194174 ai-django-core-7.0.1/ai_django_core/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/ai_django_core/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2022-05-24 06:31:55.195173 ai-django-core-7.0.1/ai_django_core/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2022-05-24 06:31:55.196174 ai-django-core-7.0.1/ai_django_core/admin/views/mixins.py
--rw-r--r--   0        0        0      205 2023-03-16 14:29:23.656927 ai-django-core-7.0.1/ai_django_core/apps.py
--rw-r--r--   0        0        0      942 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/context_manager.py
--rw-r--r--   0        0        0      147 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/context_processors.py
--rw-r--r--   0        0        0        0 2020-10-30 08:58:27.570199 ai-django-core-7.0.1/ai_django_core/drf/__init__.py
--rw-r--r--   0        0        0     1031 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/drf/fields.py
--rw-r--r--   0        0        0     1143 2022-05-24 06:31:55.197177 ai-django-core-7.0.1/ai_django_core/drf/serializers.py
--rw-r--r--   0        0        0     3226 2022-05-24 06:31:55.198174 ai-django-core-7.0.1/ai_django_core/drf/tests.py
--rw-r--r--   0        0        0        0 2022-01-28 15:09:22.800090 ai-django-core-7.0.1/ai_django_core/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-01-18 08:29:41.824417 ai-django-core-7.0.1/ai_django_core/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2020-11-11 13:34:13.878022 ai-django-core-7.0.1/ai_django_core/graphql/__init__.py
--rw-r--r--   0        0        0        0 2020-11-11 13:34:13.879027 ai-django-core-7.0.1/ai_django_core/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.1/ai_django_core/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2022-05-24 06:31:55.201402 ai-django-core-7.0.1/ai_django_core/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2022-02-04 10:36:09.232865 ai-django-core-7.0.1/ai_django_core/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2022-05-19 13:07:18.117710 ai-django-core-7.0.1/ai_django_core/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2022-05-24 06:31:55.202177 ai-django-core-7.0.1/ai_django_core/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.1/ai_django_core/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/graphql/tests/base_test.py
--rw-r--r--   0        0        0     2011 2022-09-29 17:01:08.183567 ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2948 2022-09-29 17:01:08.186898 ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-10-14 11:54:26.324037 ai-django-core-7.0.1/ai_django_core/mail/__init__.py
--rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.1/ai_django_core/mail/backends/__init__.py
--rw-r--r--   0        0        0     3148 2022-09-29 17:01:08.190635 ai-django-core-7.0.1/ai_django_core/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0      120 2021-04-21 06:44:18.414056 ai-django-core-7.0.1/ai_django_core/mail/errors.py
--rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.1/ai_django_core/mail/services/__init__.py
--rw-r--r--   0        0        0    11273 2022-09-19 13:21:41.288357 ai-django-core-7.0.1/ai_django_core/mail/services/base.py
--rw-r--r--   0        0        0    10121 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/mail/services/tests.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.656927 ai-django-core-7.0.1/ai_django_core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.657928 ai-django-core-7.0.1/ai_django_core/management/commands/__init__.py
--rw-r--r--   0        0        0      302 2023-03-16 14:29:23.658434 ai-django-core-7.0.1/ai_django_core/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2022-05-24 06:31:55.208172 ai-django-core-7.0.1/ai_django_core/managers.py
--rw-r--r--   0        0        0        0 2020-10-14 11:54:26.328426 ai-django-core-7.0.1/ai_django_core/middleware/__init__.py
--rw-r--r--   0        0        0     1050 2022-05-24 06:31:55.209173 ai-django-core-7.0.1/ai_django_core/middleware/current_user.py
--rw-r--r--   0        0        0       31 2022-05-19 13:07:18.127538 ai-django-core-7.0.1/ai_django_core/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2022-05-24 06:31:55.210172 ai-django-core-7.0.1/ai_django_core/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2023-02-13 12:03:20.486464 ai-django-core-7.0.1/ai_django_core/mixins/models.py
--rw-r--r--   0        0        0      246 2022-05-24 06:31:55.211171 ai-django-core-7.0.1/ai_django_core/mixins/validation.py
--rw-r--r--   0        0        0     2591 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/models.py
--rw-r--r--   0        0        0        0 2022-11-28 15:41:36.586624 ai-django-core-7.0.1/ai_django_core/selectors/__init__.py
--rw-r--r--   0        0        0      362 2022-11-28 15:41:36.587626 ai-django-core-7.0.1/ai_django_core/selectors/base.py
--rw-r--r--   0        0        0     1060 2022-11-28 15:41:36.588627 ai-django-core-7.0.1/ai_django_core/selectors/permission.py
--rw-r--r--   0        0        0        0 2021-12-10 09:34:59.322678 ai-django-core-7.0.1/ai_django_core/sentry/__init__.py
--rw-r--r--   0        0        0      668 2022-05-19 13:07:18.127538 ai-django-core-7.0.1/ai_django_core/sentry/helpers.py
--rw-r--r--   0        0        0        0 2020-10-14 11:54:26.334428 ai-django-core-7.0.1/ai_django_core/services/__init__.py
--rw-r--r--   0        0        0     3223 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2020-10-14 11:54:26.435582 ai-django-core-7.0.1/ai_django_core/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      647 2022-09-29 17:01:08.196796 ai-django-core-7.0.1/ai_django_core/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      771 2022-09-29 17:01:08.197793 ai-django-core-7.0.1/ai_django_core/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2020-10-14 11:54:26.432584 ai-django-core-7.0.1/ai_django_core/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2022-05-19 13:07:18.132547 ai-django-core-7.0.1/ai_django_core/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/ai_django_core/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2020-10-29 09:10:12.146622 ai-django-core-7.0.1/ai_django_core/tests/__init__.py
--rw-r--r--   0        0        0       60 2022-06-29 09:25:01.899799 ai-django-core-7.0.1/ai_django_core/tests/errors.py
--rw-r--r--   0        0        0     5006 2023-02-13 12:01:53.840473 ai-django-core-7.0.1/ai_django_core/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.659442 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-03-16 14:29:23.660441 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4633 2023-03-16 14:29:23.660441 ai-django-core-7.0.1/ai_django_core/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2020-10-29 08:14:58.246710 ai-django-core-7.0.1/ai_django_core/utils/__init__.py
--rw-r--r--   0        0        0      127 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/ai_django_core/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/ai_django_core/utils/date.py
--rw-r--r--   0        0        0     1468 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/file.py
--rw-r--r--   0        0        0      343 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2021-01-14 07:19:48.798830 ai-django-core-7.0.1/ai_django_core/utils/math.py
--rw-r--r--   0        0        0      935 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/utils/model.py
--rw-r--r--   0        0        0     3850 2023-03-16 11:00:21.086080 ai-django-core-7.0.1/ai_django_core/utils/named_tuple.py
--rw-r--r--   0        0        0     3694 2022-09-29 17:01:08.210953 ai-django-core-7.0.1/ai_django_core/utils/string.py
--rw-r--r--   0        0        0        0 2021-04-20 12:33:32.484731 ai-django-core-7.0.1/ai_django_core/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2022-05-19 13:07:18.137589 ai-django-core-7.0.1/ai_django_core/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/ai_django_core/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/ai_django_core/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-03-28 10:54:55.241821 ai-django-core-7.0.1/ai_django_core/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2022-06-29 09:25:01.903801 ai-django-core-7.0.1/ai_django_core/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2022-06-29 09:25:01.903801 ai-django-core-7.0.1/ai_django_core/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4120 2022-11-18 09:21:47.406961 ai-django-core-7.0.1/ai_django_core/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-02-21 14:56:14.199514 ai-django-core-7.0.1/ai_django_core/view_layer/views.py
--rw-r--r--   0        0        0      654 2020-10-29 08:14:58.247751 ai-django-core-7.0.1/docs/Makefile
--rw-r--r--   0        0        0     2837 2023-03-16 14:29:23.662561 ai-django-core-7.0.1/docs/conf.py
--rw-r--r--   0        0        0     6729 2021-10-18 07:37:49.515098 ai-django-core-7.0.1/docs/features/admin.md
--rw-r--r--   0        0        0       33 2023-01-11 09:49:34.733879 ai-django-core-7.0.1/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/context_manager.md
--rw-r--r--   0        0        0      548 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2021-11-18 10:19:55.448850 ai-django-core-7.0.1/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2552 2023-01-18 08:29:41.824417 ai-django-core-7.0.1/docs/features/gitlab.md
--rw-r--r--   0        0        0     6339 2022-02-28 07:49:19.065009 ai-django-core-7.0.1/docs/features/graphql.md
--rw-r--r--   0        0        0    10426 2022-02-28 08:13:29.331040 ai-django-core-7.0.1/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2022-11-28 15:41:36.593627 ai-django-core-7.0.1/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2022-12-19 12:58:18.633582 ai-django-core-7.0.1/docs/features/mixins.md
--rw-r--r--   0        0        0     1551 2023-03-28 09:35:16.410380 ai-django-core-7.0.1/docs/features/models.md
--rw-r--r--   0        0        0     4451 2022-11-28 15:41:36.594720 ai-django-core-7.0.1/docs/features/selectors.md
--rw-r--r--   0        0        0     1045 2021-12-10 11:03:41.492786 ai-django-core-7.0.1/docs/features/sentry.md
--rw-r--r--   0        0        0     4977 2021-11-09 07:06:36.578897 ai-django-core-7.0.1/docs/features/services.md
--rw-r--r--   0        0        0     1502 2021-03-17 07:16:57.205815 ai-django-core-7.0.1/docs/features/setup.md
--rw-r--r--   0        0        0    10391 2023-03-16 14:29:23.663545 ai-django-core-7.0.1/docs/features/tests.md
--rw-r--r--   0        0        0      232 2022-06-30 10:27:42.711391 ai-django-core-7.0.1/docs/features/utils.rst
--rw-r--r--   0        0        0      526 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7404 2022-12-01 13:50:38.529789 ai-django-core-7.0.1/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2021-01-14 07:19:48.814455 ai-django-core-7.0.1/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2021-11-09 07:06:36.594530 ai-django-core-7.0.1/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5847 2021-11-09 07:06:36.594530 ai-django-core-7.0.1/docs/features/utils/string.md
--rw-r--r--   0        0        0    15052 2023-02-21 14:56:14.200514 ai-django-core-7.0.1/docs/features/view-layer.md
--rw-r--r--   0        0        0     1152 2022-11-28 15:41:36.595725 ai-django-core-7.0.1/docs/index.rst
--rwxr-xr-x   0        0        0      795 2020-10-29 08:14:58.263559 ai-django-core-7.0.1/docs/make.bat
--rw-r--r--   0        0        0      677 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/manage.py
--rw-r--r--   0        0        0     3912 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/pyproject.toml
--rw-r--r--   0        0        0       56 2020-10-30 08:58:27.573230 ai-django-core-7.0.1/pytest.ini
--rw-r--r--   0        0        0      184 2022-02-28 08:20:10.689851 ai-django-core-7.0.1/scripts/publish_and_update_mirror.ps1
--rw-r--r--   0        0        0      302 2023-03-16 14:36:30.853296 ai-django-core-7.0.1/scripts/update-mirror.ps1
--rw-r--r--   0        0        0     1703 2022-09-29 17:01:08.221675 ai-django-core-7.0.1/settings.py
--rw-r--r--   0        0        0       69 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/setup.cfg
--rw-r--r--   0        0        0        0 2020-10-30 08:58:27.574229 ai-django-core-7.0.1/testapp/__init__.py
--rw-r--r--   0        0        0        0 2021-03-16 07:21:28.693546 ai-django-core-7.0.1/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2022-05-19 13:07:18.142596 ai-django-core-7.0.1/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2021-03-16 07:21:28.693546 ai-django-core-7.0.1/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-03-16 14:29:23.663545 ai-django-core-7.0.1/testapp/forms.py
--rw-r--r--   0        0        0       97 2022-11-28 15:41:36.595725 ai-django-core-7.0.1/testapp/managers.py
--rw-r--r--   0        0        0      829 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0     2529 2023-02-06 12:03:54.242881 ai-django-core-7.0.1/testapp/migrations/0002_auto_210407.py
--rw-r--r--   0        0        0     2194 2022-05-24 06:31:55.228545 ai-django-core-7.0.1/testapp/migrations/0003_modelwithfktoself.py
--rw-r--r--   0        0        0     1866 2023-02-06 12:03:54.226798 ai-django-core-7.0.1/testapp/migrations/0004_auto_20210511_1343.py
--rw-r--r--   0        0        0      613 2023-02-06 12:03:54.191159 ai-django-core-7.0.1/testapp/migrations/0005_modelwithcleanmixin.py
--rw-r--r--   0        0        0      680 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0006_modelwithselector.py
--rw-r--r--   0        0        0      692 2023-02-06 12:03:54.198766 ai-django-core-7.0.1/testapp/migrations/0007_modelwithsavewithoutsignals.py
--rw-r--r--   0        0        0        0 2020-10-30 08:58:27.575702 ai-django-core-7.0.1/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3359 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/testapp/models.py
--rw-r--r--   0        0        0      161 2022-11-28 15:41:36.598713 ai-django-core-7.0.1/testapp/selectors.py
--rw-r--r--   0        0        0     1390 2022-09-29 17:01:08.223215 ai-django-core-7.0.1/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2021-03-04 09:15:39.283083 ai-django-core-7.0.1/testapp/templates/test_email.html
--rw-r--r--   0        0        0      148 2021-03-04 09:15:39.283083 ai-django-core-7.0.1/testapp/templates/test_email.txt
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.1/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.1/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.1/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2022-05-24 06:31:55.232545 ai-django-core-7.0.1/testapp/urls.py
--rw-r--r--   0        0        0      490 2022-09-29 17:18:59.613421 ai-django-core-7.0.1/testapp/views.py
--rw-r--r--   0        0        0        0 2020-10-30 08:58:27.576702 ai-django-core-7.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2605 2023-03-16 14:29:23.667647 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1898 2022-05-24 06:31:55.235544 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1681 2022-05-24 06:31:55.236545 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1182 2022-05-24 06:31:55.237545 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3790 2022-09-29 17:01:08.225217 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1489 2022-05-24 06:31:55.239544 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1907 2022-05-24 06:31:55.240547 ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-03-16 14:29:23.667647 ai-django-core-7.0.1/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7498 2023-04-28 13:00:07.370054 ai-django-core-7.0.1/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/drf/__init__.py
--rw-r--r--   0        0        0     2578 2022-05-24 06:31:55.241566 ai-django-core-7.0.1/tests/drf/test_fields.py
--rw-r--r--   0        0        0       28 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/files/testfile.txt
--rw-r--r--   0        0        0        0 2022-05-24 06:31:55.242545 ai-django-core-7.0.1/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2022-05-24 06:31:55.243544 ai-django-core-7.0.1/tests/mixins/validation.py
--rw-r--r--   0        0        0        0 2022-11-28 15:41:36.598713 ai-django-core-7.0.1/tests/selectors/__init__.py
--rw-r--r--   0        0        0      498 2022-11-28 15:41:36.599713 ai-django-core-7.0.1/tests/selectors/test_base.py
--rw-r--r--   0        0        0     1630 2022-11-28 15:41:36.599713 ai-django-core-7.0.1/tests/selectors/test_permission.py
--rw-r--r--   0        0        0      552 2022-05-24 06:31:55.244544 ai-django-core-7.0.1/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1610 2022-05-24 06:31:55.245548 ai-django-core-7.0.1/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2649 2022-05-24 06:31:55.247546 ai-django-core-7.0.1/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2886 2022-05-24 06:31:55.248546 ai-django-core-7.0.1/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2217 2022-05-24 06:31:55.249546 ai-django-core-7.0.1/tests/test_context_manager.py
--rw-r--r--   0        0        0     9342 2023-01-11 09:40:21.960817 ai-django-core-7.0.1/tests/test_email_test_service.py
--rw-r--r--   0        0        0      821 2020-10-30 08:58:27.625804 ai-django-core-7.0.1/tests/test_log_whodid.py
--rw-r--r--   0        0        0    15502 2022-05-24 06:31:55.250546 ai-django-core-7.0.1/tests/test_mail_services.py
--rw-r--r--   0        0        0     1169 2022-05-24 06:31:55.251544 ai-django-core-7.0.1/tests/test_managers.py
--rw-r--r--   0        0        0     1627 2022-05-24 06:31:55.252553 ai-django-core-7.0.1/tests/test_math.py
--rw-r--r--   0        0        0     2592 2022-05-19 13:07:18.157715 ai-django-core-7.0.1/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2022-12-19 12:58:18.636566 ai-django-core-7.0.1/tests/test_mixins_models.py
--rw-r--r--   0        0        0     1669 2023-03-28 09:35:16.411383 ai-django-core-7.0.1/tests/test_models.py
--rw-r--r--   0        0        0     1779 2022-05-24 06:31:55.254447 ai-django-core-7.0.1/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      663 2022-05-24 06:31:55.255429 ai-django-core-7.0.1/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0     1196 2022-05-24 06:31:55.256430 ai-django-core-7.0.1/tests/test_sentry_helper.py
--rw-r--r--   0        0        0      288 2022-05-24 06:31:55.257429 ai-django-core-7.0.1/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12740 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2022-05-24 06:31:55.259430 ai-django-core-7.0.1/tests/test_utils_file.py
--rw-r--r--   0        0        0      932 2022-05-24 06:31:55.260430 ai-django-core-7.0.1/tests/test_utils_model.py
--rw-r--r--   0        0        0     3806 2022-05-24 06:31:55.261429 ai-django-core-7.0.1/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5342 2022-05-24 06:31:55.262430 ai-django-core-7.0.1/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.1/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-04-08 14:39:10.045967 ai-django-core-7.0.1/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2022-10-12 09:20:31.364313 ai-django-core-7.0.1/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      796 2023-02-13 15:49:17.040360 ai-django-core-7.0.1/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2482 2022-05-24 06:31:55.263431 ai-django-core-7.0.1/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2055 2022-05-24 06:31:55.264429 ai-django-core-7.0.1/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.1/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1890 2023-03-28 10:15:26.101761 ai-django-core-7.0.1/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1562 2023-02-21 14:56:14.201551 ai-django-core-7.0.1/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3369 2022-06-29 11:55:51.396586 ai-django-core-7.0.1/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1323 2022-09-29 17:18:59.613421 ai-django-core-7.0.1/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     7044 1970-01-01 00:00:00.000000 ai-django-core-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-04-24 09:15:50.688102 ai-django-core-7.0.2/.coveragerc
+-rw-r--r--   0        0        0      288 2021-01-14 07:19:48.798830 ai-django-core-7.0.2/.editorconfig
+-rw-r--r--   0        0        0     1736 2023-03-28 10:54:55.241821 ai-django-core-7.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      400 2021-03-04 09:37:37.670469 ai-django-core-7.0.2/.gitignore
+-rw-r--r--   0        0        0     3941 2023-02-21 14:56:14.192364 ai-django-core-7.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      443 2023-05-02 10:10:53.230359 ai-django-core-7.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0    18472 2023-07-20 14:34:48.075794 ai-django-core-7.0.2/CHANGES.md
+-rw-r--r--   0        0        0      962 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/Dockerfile
+-rw-r--r--   0        0        0     1104 2020-11-11 13:34:13.878022 ai-django-core-7.0.2/LICENSE.md
+-rw-r--r--   0        0        0      129 2021-05-12 15:21:27.853419 ai-django-core-7.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     4710 2023-05-04 13:15:53.544078 ai-django-core-7.0.2/README.md
+-rw-r--r--   0        0        0       91 2023-07-20 14:34:48.071640 ai-django-core-7.0.2/ai_django_core/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.2/ai_django_core/admin/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.018823 ai-django-core-7.0.2/ai_django_core/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2022-05-24 06:31:55.191175 ai-django-core-7.0.2/ai_django_core/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2022-05-24 06:31:55.192174 ai-django-core-7.0.2/ai_django_core/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2022-05-24 06:31:55.194174 ai-django-core-7.0.2/ai_django_core/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.2/ai_django_core/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2022-05-24 06:31:55.195173 ai-django-core-7.0.2/ai_django_core/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2022-05-24 06:31:55.196174 ai-django-core-7.0.2/ai_django_core/admin/views/mixins.py
+-rw-r--r--   0        0        0      329 2023-07-20 14:29:48.922902 ai-django-core-7.0.2/ai_django_core/apps.py
+-rw-r--r--   0        0        0      369 2023-07-20 14:34:10.166399 ai-django-core-7.0.2/ai_django_core/checks.py
+-rw-r--r--   0        0        0      942 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/context_manager.py
+-rw-r--r--   0        0        0      147 2022-05-19 13:07:18.117710 ai-django-core-7.0.2/ai_django_core/context_processors.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.570199 ai-django-core-7.0.2/ai_django_core/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2022-05-19 13:07:18.117710 ai-django-core-7.0.2/ai_django_core/drf/fields.py
+-rw-r--r--   0        0        0     1143 2022-05-24 06:31:55.197177 ai-django-core-7.0.2/ai_django_core/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2022-05-24 06:31:55.198174 ai-django-core-7.0.2/ai_django_core/drf/tests.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:09:22.800090 ai-django-core-7.0.2/ai_django_core/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-01-18 08:29:41.824417 ai-django-core-7.0.2/ai_django_core/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.878022 ai-django-core-7.0.2/ai_django_core/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.879027 ai-django-core-7.0.2/ai_django_core/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.2/ai_django_core/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2022-05-24 06:31:55.201402 ai-django-core-7.0.2/ai_django_core/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2022-02-04 10:36:09.232865 ai-django-core-7.0.2/ai_django_core/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2022-05-19 13:07:18.117710 ai-django-core-7.0.2/ai_django_core/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2022-05-24 06:31:55.202177 ai-django-core-7.0.2/ai_django_core/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2020-11-11 13:34:13.880023 ai-django-core-7.0.2/ai_django_core/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     2011 2022-09-29 17:01:08.183567 ai-django-core-7.0.2/ai_django_core/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2948 2022-09-29 17:01:08.186898 ai-django-core-7.0.2/ai_django_core/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.324037 ai-django-core-7.0.2/ai_django_core/mail/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.2/ai_django_core/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3148 2022-09-29 17:01:08.190635 ai-django-core-7.0.2/ai_django_core/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0      120 2021-04-21 06:44:18.414056 ai-django-core-7.0.2/ai_django_core/mail/errors.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.326832 ai-django-core-7.0.2/ai_django_core/mail/services/__init__.py
+-rw-r--r--   0        0        0    11273 2022-09-19 13:21:41.288357 ai-django-core-7.0.2/ai_django_core/mail/services/base.py
+-rw-r--r--   0        0        0    10121 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/mail/services/tests.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.656927 ai-django-core-7.0.2/ai_django_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.657928 ai-django-core-7.0.2/ai_django_core/management/commands/__init__.py
+-rw-r--r--   0        0        0      302 2023-03-16 14:29:23.658434 ai-django-core-7.0.2/ai_django_core/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2022-05-24 06:31:55.208172 ai-django-core-7.0.2/ai_django_core/managers.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.328426 ai-django-core-7.0.2/ai_django_core/middleware/__init__.py
+-rw-r--r--   0        0        0     1050 2022-05-24 06:31:55.209173 ai-django-core-7.0.2/ai_django_core/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2022-05-19 13:07:18.127538 ai-django-core-7.0.2/ai_django_core/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2022-05-24 06:31:55.210172 ai-django-core-7.0.2/ai_django_core/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-02-13 12:03:20.486464 ai-django-core-7.0.2/ai_django_core/mixins/models.py
+-rw-r--r--   0        0        0      246 2022-05-24 06:31:55.211171 ai-django-core-7.0.2/ai_django_core/mixins/validation.py
+-rw-r--r--   0        0        0     2591 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/models.py
+-rw-r--r--   0        0        0        0 2022-11-28 15:41:36.586624 ai-django-core-7.0.2/ai_django_core/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2022-11-28 15:41:36.587626 ai-django-core-7.0.2/ai_django_core/selectors/base.py
+-rw-r--r--   0        0        0     1060 2022-11-28 15:41:36.588627 ai-django-core-7.0.2/ai_django_core/selectors/permission.py
+-rw-r--r--   0        0        0        0 2021-12-10 09:34:59.322678 ai-django-core-7.0.2/ai_django_core/sentry/__init__.py
+-rw-r--r--   0        0        0      668 2022-05-19 13:07:18.127538 ai-django-core-7.0.2/ai_django_core/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2020-10-14 11:54:26.334428 ai-django-core-7.0.2/ai_django_core/services/__init__.py
+-rw-r--r--   0        0        0     3223 2022-05-19 13:07:18.132547 ai-django-core-7.0.2/ai_django_core/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2022-05-19 13:07:18.132547 ai-django-core-7.0.2/ai_django_core/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2020-10-14 11:54:26.435582 ai-django-core-7.0.2/ai_django_core/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      647 2022-09-29 17:01:08.196796 ai-django-core-7.0.2/ai_django_core/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      771 2022-09-29 17:01:08.197793 ai-django-core-7.0.2/ai_django_core/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2020-10-14 11:54:26.432584 ai-django-core-7.0.2/ai_django_core/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2022-05-19 13:07:18.132547 ai-django-core-7.0.2/ai_django_core/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2022-05-19 13:07:18.132547 ai-django-core-7.0.2/ai_django_core/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/ai_django_core/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2020-10-29 09:10:12.146622 ai-django-core-7.0.2/ai_django_core/tests/__init__.py
+-rw-r--r--   0        0        0       60 2022-06-29 09:25:01.899799 ai-django-core-7.0.2/ai_django_core/tests/errors.py
+-rw-r--r--   0        0        0     5006 2023-02-13 12:01:53.840473 ai-django-core-7.0.2/ai_django_core/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.659442 ai-django-core-7.0.2/ai_django_core/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-03-16 14:29:23.660441 ai-django-core-7.0.2/ai_django_core/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4633 2023-03-16 14:29:23.660441 ai-django-core-7.0.2/ai_django_core/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2020-10-29 08:14:58.246710 ai-django-core-7.0.2/ai_django_core/utils/__init__.py
+-rw-r--r--   0        0        0      127 2021-01-14 07:19:48.798830 ai-django-core-7.0.2/ai_django_core/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-03-28 10:54:55.241821 ai-django-core-7.0.2/ai_django_core/utils/date.py
+-rw-r--r--   0        0        0     1468 2022-05-19 13:07:18.137589 ai-django-core-7.0.2/ai_django_core/utils/file.py
+-rw-r--r--   0        0        0      343 2022-05-19 13:07:18.137589 ai-django-core-7.0.2/ai_django_core/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2021-01-14 07:19:48.798830 ai-django-core-7.0.2/ai_django_core/utils/math.py
+-rw-r--r--   0        0        0      935 2022-05-19 13:07:18.137589 ai-django-core-7.0.2/ai_django_core/utils/model.py
+-rw-r--r--   0        0        0     3850 2023-03-16 11:00:21.086080 ai-django-core-7.0.2/ai_django_core/utils/named_tuple.py
+-rw-r--r--   0        0        0     3694 2022-09-29 17:01:08.210953 ai-django-core-7.0.2/ai_django_core/utils/string.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.484731 ai-django-core-7.0.2/ai_django_core/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2022-05-19 13:07:18.137589 ai-django-core-7.0.2/ai_django_core/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2022-05-19 13:07:18.142596 ai-django-core-7.0.2/ai_django_core/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2022-05-19 13:07:18.142596 ai-django-core-7.0.2/ai_django_core/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-03-28 10:54:55.241821 ai-django-core-7.0.2/ai_django_core/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2022-06-29 09:25:01.903801 ai-django-core-7.0.2/ai_django_core/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2022-06-29 09:25:01.903801 ai-django-core-7.0.2/ai_django_core/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4120 2022-11-18 09:21:47.406961 ai-django-core-7.0.2/ai_django_core/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-02-21 14:56:14.199514 ai-django-core-7.0.2/ai_django_core/view_layer/views.py
+-rw-r--r--   0        0        0      654 2020-10-29 08:14:58.247751 ai-django-core-7.0.2/docs/Makefile
+-rw-r--r--   0        0        0     2837 2023-03-16 14:29:23.662561 ai-django-core-7.0.2/docs/conf.py
+-rw-r--r--   0        0        0     6729 2021-10-18 07:37:49.515098 ai-django-core-7.0.2/docs/features/admin.md
+-rw-r--r--   0        0        0       33 2023-01-11 09:49:34.733879 ai-django-core-7.0.2/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2021-01-14 07:19:48.814455 ai-django-core-7.0.2/docs/features/context_manager.md
+-rw-r--r--   0        0        0      548 2021-01-14 07:19:48.814455 ai-django-core-7.0.2/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2021-11-18 10:19:55.448850 ai-django-core-7.0.2/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2021-04-20 12:33:32.500344 ai-django-core-7.0.2/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2552 2023-01-18 08:29:41.824417 ai-django-core-7.0.2/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6339 2022-02-28 07:49:19.065009 ai-django-core-7.0.2/docs/features/graphql.md
+-rw-r--r--   0        0        0    10426 2022-02-28 08:13:29.331040 ai-django-core-7.0.2/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2022-11-28 15:41:36.593627 ai-django-core-7.0.2/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2022-12-19 12:58:18.633582 ai-django-core-7.0.2/docs/features/mixins.md
+-rw-r--r--   0        0        0     1551 2023-03-28 09:35:16.410380 ai-django-core-7.0.2/docs/features/models.md
+-rw-r--r--   0        0        0     4451 2022-11-28 15:41:36.594720 ai-django-core-7.0.2/docs/features/selectors.md
+-rw-r--r--   0        0        0     1045 2021-12-10 11:03:41.492786 ai-django-core-7.0.2/docs/features/sentry.md
+-rw-r--r--   0        0        0     4977 2021-11-09 07:06:36.578897 ai-django-core-7.0.2/docs/features/services.md
+-rw-r--r--   0        0        0     1502 2021-03-17 07:16:57.205815 ai-django-core-7.0.2/docs/features/setup.md
+-rw-r--r--   0        0        0    10391 2023-03-16 14:29:23.663545 ai-django-core-7.0.2/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2022-06-30 10:27:42.711391 ai-django-core-7.0.2/docs/features/utils.rst
+-rw-r--r--   0        0        0      526 2021-01-14 07:19:48.814455 ai-django-core-7.0.2/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7404 2022-12-01 13:50:38.529789 ai-django-core-7.0.2/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2021-01-14 07:19:48.814455 ai-django-core-7.0.2/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2021-01-14 07:19:48.814455 ai-django-core-7.0.2/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2021-11-09 07:06:36.594530 ai-django-core-7.0.2/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5847 2021-11-09 07:06:36.594530 ai-django-core-7.0.2/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15052 2023-02-21 14:56:14.200514 ai-django-core-7.0.2/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1152 2022-11-28 15:41:36.595725 ai-django-core-7.0.2/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2020-10-29 08:14:58.263559 ai-django-core-7.0.2/docs/make.bat
+-rw-r--r--   0        0        0      677 2022-05-19 13:07:18.142596 ai-django-core-7.0.2/manage.py
+-rw-r--r--   0        0        0     3912 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2020-10-30 08:58:27.573230 ai-django-core-7.0.2/pytest.ini
+-rw-r--r--   0        0        0      184 2022-02-28 08:20:10.689851 ai-django-core-7.0.2/scripts/publish_and_update_mirror.ps1
+-rw-r--r--   0        0        0      302 2023-03-16 14:36:30.853296 ai-django-core-7.0.2/scripts/update-mirror.ps1
+-rw-r--r--   0        0        0     1703 2022-09-29 17:01:08.221675 ai-django-core-7.0.2/settings.py
+-rw-r--r--   0        0        0       69 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/setup.cfg
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.574229 ai-django-core-7.0.2/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-16 07:21:28.693546 ai-django-core-7.0.2/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2022-05-19 13:07:18.142596 ai-django-core-7.0.2/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2022-05-19 13:07:18.142596 ai-django-core-7.0.2/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2021-03-16 07:21:28.693546 ai-django-core-7.0.2/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-03-16 14:29:23.663545 ai-django-core-7.0.2/testapp/forms.py
+-rw-r--r--   0        0        0       97 2022-11-28 15:41:36.595725 ai-django-core-7.0.2/testapp/managers.py
+-rw-r--r--   0        0        0      829 2023-02-06 12:03:54.198766 ai-django-core-7.0.2/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2529 2023-02-06 12:03:54.242881 ai-django-core-7.0.2/testapp/migrations/0002_auto_210407.py
+-rw-r--r--   0        0        0     2194 2022-05-24 06:31:55.228545 ai-django-core-7.0.2/testapp/migrations/0003_modelwithfktoself.py
+-rw-r--r--   0        0        0     1866 2023-02-06 12:03:54.226798 ai-django-core-7.0.2/testapp/migrations/0004_auto_20210511_1343.py
+-rw-r--r--   0        0        0      613 2023-02-06 12:03:54.191159 ai-django-core-7.0.2/testapp/migrations/0005_modelwithcleanmixin.py
+-rw-r--r--   0        0        0      680 2023-02-06 12:03:54.198766 ai-django-core-7.0.2/testapp/migrations/0006_modelwithselector.py
+-rw-r--r--   0        0        0      692 2023-02-06 12:03:54.198766 ai-django-core-7.0.2/testapp/migrations/0007_modelwithsavewithoutsignals.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.575702 ai-django-core-7.0.2/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3359 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/testapp/models.py
+-rw-r--r--   0        0        0      161 2022-11-28 15:41:36.598713 ai-django-core-7.0.2/testapp/selectors.py
+-rw-r--r--   0        0        0     1390 2022-09-29 17:01:08.223215 ai-django-core-7.0.2/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2021-03-04 09:15:39.283083 ai-django-core-7.0.2/testapp/templates/test_email.html
+-rw-r--r--   0        0        0      148 2021-03-04 09:15:39.283083 ai-django-core-7.0.2/testapp/templates/test_email.txt
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.2/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.2/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.665545 ai-django-core-7.0.2/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.2/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.666607 ai-django-core-7.0.2/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2022-05-24 06:31:55.232545 ai-django-core-7.0.2/testapp/urls.py
+-rw-r--r--   0        0        0      490 2022-09-29 17:18:59.613421 ai-django-core-7.0.2/testapp/views.py
+-rw-r--r--   0        0        0        0 2020-10-30 08:58:27.576702 ai-django-core-7.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.2/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.2/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2605 2023-03-16 14:29:23.667647 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1898 2022-05-24 06:31:55.235544 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1681 2022-05-24 06:31:55.236545 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1182 2022-05-24 06:31:55.237545 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3790 2022-09-29 17:01:08.225217 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1489 2022-05-24 06:31:55.239544 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1907 2022-05-24 06:31:55.240547 ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-03-16 14:29:23.667647 ai-django-core-7.0.2/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7498 2023-04-28 13:00:07.370054 ai-django-core-7.0.2/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.2/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2578 2022-05-24 06:31:55.241566 ai-django-core-7.0.2/tests/drf/test_fields.py
+-rw-r--r--   0        0        0       28 2021-04-20 12:33:32.500344 ai-django-core-7.0.2/tests/files/testfile.txt
+-rw-r--r--   0        0        0        0 2022-05-24 06:31:55.242545 ai-django-core-7.0.2/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2022-05-24 06:31:55.243544 ai-django-core-7.0.2/tests/mixins/validation.py
+-rw-r--r--   0        0        0        0 2022-11-28 15:41:36.598713 ai-django-core-7.0.2/tests/selectors/__init__.py
+-rw-r--r--   0        0        0      498 2022-11-28 15:41:36.599713 ai-django-core-7.0.2/tests/selectors/test_base.py
+-rw-r--r--   0        0        0     1630 2022-11-28 15:41:36.599713 ai-django-core-7.0.2/tests/selectors/test_permission.py
+-rw-r--r--   0        0        0      552 2022-05-24 06:31:55.244544 ai-django-core-7.0.2/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1610 2022-05-24 06:31:55.245548 ai-django-core-7.0.2/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2649 2022-05-24 06:31:55.247546 ai-django-core-7.0.2/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2886 2022-05-24 06:31:55.248546 ai-django-core-7.0.2/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2217 2022-05-24 06:31:55.249546 ai-django-core-7.0.2/tests/test_context_manager.py
+-rw-r--r--   0        0        0     9342 2023-01-11 09:40:21.960817 ai-django-core-7.0.2/tests/test_email_test_service.py
+-rw-r--r--   0        0        0      821 2020-10-30 08:58:27.625804 ai-django-core-7.0.2/tests/test_log_whodid.py
+-rw-r--r--   0        0        0    15502 2022-05-24 06:31:55.250546 ai-django-core-7.0.2/tests/test_mail_services.py
+-rw-r--r--   0        0        0     1169 2022-05-24 06:31:55.251544 ai-django-core-7.0.2/tests/test_managers.py
+-rw-r--r--   0        0        0     1627 2022-05-24 06:31:55.252553 ai-django-core-7.0.2/tests/test_math.py
+-rw-r--r--   0        0        0     2592 2022-05-19 13:07:18.157715 ai-django-core-7.0.2/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2022-12-19 12:58:18.636566 ai-django-core-7.0.2/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     1669 2023-03-28 09:35:16.411383 ai-django-core-7.0.2/tests/test_models.py
+-rw-r--r--   0        0        0     1779 2022-05-24 06:31:55.254447 ai-django-core-7.0.2/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      663 2022-05-24 06:31:55.255429 ai-django-core-7.0.2/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0     1196 2022-05-24 06:31:55.256430 ai-django-core-7.0.2/tests/test_sentry_helper.py
+-rw-r--r--   0        0        0      288 2022-05-24 06:31:55.257429 ai-django-core-7.0.2/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12740 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2022-05-24 06:31:55.259430 ai-django-core-7.0.2/tests/test_utils_file.py
+-rw-r--r--   0        0        0      932 2022-05-24 06:31:55.260430 ai-django-core-7.0.2/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3806 2022-05-24 06:31:55.261429 ai-django-core-7.0.2/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5342 2022-05-24 06:31:55.262430 ai-django-core-7.0.2/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.030331 ai-django-core-7.0.2/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-08 14:39:10.045967 ai-django-core-7.0.2/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2022-10-12 09:20:31.364313 ai-django-core-7.0.2/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      796 2023-02-13 15:49:17.040360 ai-django-core-7.0.2/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2482 2022-05-24 06:31:55.263431 ai-django-core-7.0.2/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2055 2022-05-24 06:31:55.264429 ai-django-core-7.0.2/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2021-04-20 12:33:32.500344 ai-django-core-7.0.2/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1890 2023-03-28 10:15:26.101761 ai-django-core-7.0.2/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1562 2023-02-21 14:56:14.201551 ai-django-core-7.0.2/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3369 2022-06-29 11:55:51.396586 ai-django-core-7.0.2/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1323 2022-09-29 17:18:59.613421 ai-django-core-7.0.2/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     7044 1970-01-01 00:00:00.000000 ai-django-core-7.0.2/PKG-INFO
```

### Comparing `ai-django-core-7.0.1/.github/workflows/ci.yml` & `ai-django-core-7.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/.gitlab-ci.yml` & `ai-django-core-7.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/.pre-commit-config.yaml` & `ai-django-core-7.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/CHANGES.md` & `ai-django-core-7.0.2/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+* **7.0.2** (2023-05-04)
+  * Added Django system check to warn about deprecation
+
 * **7.0.1** (2023-05-04)
   * **This package was superseded by** [ambient-toolbox](https://pypi.org/project/ambient-toolbox/). Please install the successor package.
 
 * **7.0.0** (2023-03-28)
   * *Breaking change:* Dropped Python 3.7 support due to end of lifetime
   * Added `ALWAYS_UPDATE_FIELDS` flag to `CommonInfo` model
   * Added `ruff` linter and replaced `flake8` and `isort` with it
```

### Comparing `ai-django-core-7.0.1/Dockerfile` & `ai-django-core-7.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/LICENSE.md` & `ai-django-core-7.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/README.md` & `ai-django-core-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/admin/model_admins/classes.py` & `ai-django-core-7.0.2/ai_django_core/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/admin/model_admins/inlines.py` & `ai-django-core-7.0.2/ai_django_core/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/admin/model_admins/mixins.py` & `ai-django-core-7.0.2/ai_django_core/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/admin/views/forms.py` & `ai-django-core-7.0.2/ai_django_core/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/admin/views/mixins.py` & `ai-django-core-7.0.2/ai_django_core/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/context_manager.py` & `ai-django-core-7.0.2/ai_django_core/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/drf/fields.py` & `ai-django-core-7.0.2/ai_django_core/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/drf/serializers.py` & `ai-django-core-7.0.2/ai_django_core/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/drf/tests.py` & `ai-django-core-7.0.2/ai_django_core/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/gitlab/coverage.py` & `ai-django-core-7.0.2/ai_django_core/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/graphql/forms/mutations.py` & `ai-django-core-7.0.2/ai_django_core/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/graphql/schemes/mutations.py` & `ai-django-core-7.0.2/ai_django_core/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/graphql/sentry/views.py` & `ai-django-core-7.0.2/ai_django_core/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/graphql/tests/base_test.py` & `ai-django-core-7.0.2/ai_django_core/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.mo` & `ai-django-core-7.0.2/ai_django_core/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/locale/de/LC_MESSAGES/django.po` & `ai-django-core-7.0.2/ai_django_core/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/mail/backends/whitelist_smtp.py` & `ai-django-core-7.0.2/ai_django_core/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/mail/services/base.py` & `ai-django-core-7.0.2/ai_django_core/mail/services/base.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/mail/services/tests.py` & `ai-django-core-7.0.2/ai_django_core/mail/services/tests.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/managers.py` & `ai-django-core-7.0.2/ai_django_core/managers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/middleware/current_user.py` & `ai-django-core-7.0.2/ai_django_core/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/mixins/bleacher.py` & `ai-django-core-7.0.2/ai_django_core/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/mixins/models.py` & `ai-django-core-7.0.2/ai_django_core/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/models.py` & `ai-django-core-7.0.2/ai_django_core/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/selectors/permission.py` & `ai-django-core-7.0.2/ai_django_core/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/sentry/helpers.py` & `ai-django-core-7.0.2/ai_django_core/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/services/custom_scrubber.py` & `ai-django-core-7.0.2/ai_django_core/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/templatetags/ai_email_tags.py` & `ai-django-core-7.0.2/ai_django_core/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/templatetags/ai_file_tags.py` & `ai-django-core-7.0.2/ai_django_core/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/templatetags/ai_number_tags.py` & `ai-django-core-7.0.2/ai_django_core/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/templatetags/ai_string_tags.py` & `ai-django-core-7.0.2/ai_django_core/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/tests/mixins.py` & `ai-django-core-7.0.2/ai_django_core/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/tests/structure_validator/test_structure_validator.py` & `ai-django-core-7.0.2/ai_django_core/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/date.py` & `ai-django-core-7.0.2/ai_django_core/utils/date.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/file.py` & `ai-django-core-7.0.2/ai_django_core/utils/file.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/math.py` & `ai-django-core-7.0.2/ai_django_core/utils/math.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/model.py` & `ai-django-core-7.0.2/ai_django_core/utils/model.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/named_tuple.py` & `ai-django-core-7.0.2/ai_django_core/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/utils/string.py` & `ai-django-core-7.0.2/ai_django_core/utils/string.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/form_mixins.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/formset_view_mixin.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/htmx_mixins.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/mixins.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/tests/mixins.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/ai_django_core/view_layer/views.py` & `ai-django-core-7.0.2/ai_django_core/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/Makefile` & `ai-django-core-7.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/conf.py` & `ai-django-core-7.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/admin.md` & `ai-django-core-7.0.2/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/context_manager.md` & `ai-django-core-7.0.2/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/context_processors.md` & `ai-django-core-7.0.2/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/database_anonymisation.md` & `ai-django-core-7.0.2/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/djangorestframework.md` & `ai-django-core-7.0.2/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/gitlab.md` & `ai-django-core-7.0.2/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/graphql.md` & `ai-django-core-7.0.2/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/mail.md` & `ai-django-core-7.0.2/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/managers.md` & `ai-django-core-7.0.2/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/mixins.md` & `ai-django-core-7.0.2/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/models.md` & `ai-django-core-7.0.2/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/selectors.md` & `ai-django-core-7.0.2/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/sentry.md` & `ai-django-core-7.0.2/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/services.md` & `ai-django-core-7.0.2/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/setup.md` & `ai-django-core-7.0.2/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/tests.md` & `ai-django-core-7.0.2/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/cache.md` & `ai-django-core-7.0.2/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/date.md` & `ai-django-core-7.0.2/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/math.md` & `ai-django-core-7.0.2/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/model.md` & `ai-django-core-7.0.2/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/named_tuple.md` & `ai-django-core-7.0.2/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/utils/string.md` & `ai-django-core-7.0.2/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/features/view-layer.md` & `ai-django-core-7.0.2/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/index.rst` & `ai-django-core-7.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/docs/make.bat` & `ai-django-core-7.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/manage.py` & `ai-django-core-7.0.2/manage.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/pyproject.toml` & `ai-django-core-7.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/settings.py` & `ai-django-core-7.0.2/settings.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/api/views.py` & `ai-django-core-7.0.2/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0001_initial.py` & `ai-django-core-7.0.2/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0002_auto_210407.py` & `ai-django-core-7.0.2/testapp/migrations/0002_auto_210407.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0003_modelwithfktoself.py` & `ai-django-core-7.0.2/testapp/migrations/0003_modelwithfktoself.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0004_auto_20210511_1343.py` & `ai-django-core-7.0.2/testapp/migrations/0004_auto_20210511_1343.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0005_modelwithcleanmixin.py` & `ai-django-core-7.0.2/testapp/migrations/0005_modelwithcleanmixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0006_modelwithselector.py` & `ai-django-core-7.0.2/testapp/migrations/0006_modelwithselector.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/migrations/0007_modelwithsavewithoutsignals.py` & `ai-django-core-7.0.2/testapp/migrations/0007_modelwithsavewithoutsignals.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/models.py` & `ai-django-core-7.0.2/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/testapp/templates/403.html` & `ai-django-core-7.0.2/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ai-django-core-7.0.2/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/ambient_toolbox/test_test_structure_validator.py` & `ai-django-core-7.0.2/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/drf/test_fields.py` & `ai-django-core-7.0.2/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/selectors/test_permission.py` & `ai-django-core-7.0.2/tests/selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_admin_forms.py` & `ai-django-core-7.0.2/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_admin_inlines.py` & `ai-django-core-7.0.2/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_admin_model_admins_classes.py` & `ai-django-core-7.0.2/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_admin_view_mixins.py` & `ai-django-core-7.0.2/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_context_manager.py` & `ai-django-core-7.0.2/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_email_test_service.py` & `ai-django-core-7.0.2/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_log_whodid.py` & `ai-django-core-7.0.2/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_mail_services.py` & `ai-django-core-7.0.2/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_managers.py` & `ai-django-core-7.0.2/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_math.py` & `ai-django-core-7.0.2/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_middleware.py` & `ai-django-core-7.0.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_mixins_models.py` & `ai-django-core-7.0.2/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_models.py` & `ai-django-core-7.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_rest_api_mixins.py` & `ai-django-core-7.0.2/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_scrubbing_service.py` & `ai-django-core-7.0.2/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_sentry_helper.py` & `ai-django-core-7.0.2/tests/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_utils_date.py` & `ai-django-core-7.0.2/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_utils_file.py` & `ai-django-core-7.0.2/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_utils_model.py` & `ai-django-core-7.0.2/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_utils_named_tuple.py` & `ai-django-core-7.0.2/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/test_utils_string.py` & `ai-django-core-7.0.2/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/tests/mixins/test_django_message_framework.py` & `ai-django-core-7.0.2/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/tests/mixins/test_request_provider_mixin.py` & `ai-django-core-7.0.2/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/tests/test_mail_backends.py` & `ai-django-core-7.0.2/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/view_layer/test_formset_mixins.py` & `ai-django-core-7.0.2/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/view_layer/test_htmx_response_mixin.py` & `ai-django-core-7.0.2/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/view_layer/test_meta_mixins.py` & `ai-django-core-7.0.2/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/tests/view_layer/test_views.py` & `ai-django-core-7.0.2/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ai-django-core-7.0.1/PKG-INFO` & `ai-django-core-7.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-django-core
-Version: 7.0.1
+Version: 7.0.2
 Summary: Ambient toolbox - Lots of helper functions and useful widgets
 Author-email: "Ambient Innovation: GmbH" <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

