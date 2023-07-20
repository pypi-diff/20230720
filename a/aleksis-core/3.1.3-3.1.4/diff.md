# Comparing `tmp/aleksis_core-3.1.3.tar.gz` & `tmp/aleksis_core-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-3.1.3.tar", max compression
+gzip compressed data, was "aleksis_core-3.1.4.tar", max compression
```

## Comparing `aleksis_core-3.1.3.tar` & `aleksis_core-3.1.4.tar`

### file list

```diff
@@ -1,490 +1,490 @@
--rw-r--r--   0        0        0    38552 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/LICENCE.rst
--rw-r--r--   0        0        0     3786 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/README.rst
--rw-r--r--   0        0        0      194 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2023-07-18 19:30:55.806599 aleksis_core-3.1.3/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2023-07-18 19:30:57.254654 aleksis_core-3.1.3/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2023-07-18 19:31:01.578817 aleksis_core-3.1.3/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11380 2023-07-18 19:30:58.842714 aleksis_core-3.1.3/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2023-07-18 19:30:55.866602 aleksis_core-3.1.3/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2023-07-18 19:31:01.686821 aleksis_core-3.1.3/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    17897 2023-07-18 19:31:01.106799 aleksis_core-3.1.3/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2023-07-18 19:31:01.698821 aleksis_core-3.1.3/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0     8423 2023-07-18 19:31:01.150801 aleksis_core-3.1.3/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    31446 2023-07-18 19:31:01.114799 aleksis_core-3.1.3/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0    85606 2023-07-18 19:31:00.378772 aleksis_core-3.1.3/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    22237 2023-07-18 19:31:01.794825 aleksis_core-3.1.3/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1370 2023-07-18 19:30:58.866715 aleksis_core-3.1.3/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    16523 2023-07-18 19:31:01.610818 aleksis_core-3.1.3/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    44051 2023-07-18 19:30:57.282655 aleksis_core-3.1.3/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2023-07-18 19:31:01.162801 aleksis_core-3.1.3/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0      950 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/admin.py
--rw-r--r--   0        0        0     8519 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/celery.py
--rw-r--r--   0        0        0     2751 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/checks.py
--rw-r--r--   0        0        0    11534 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5556 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/filters.py
--rw-r--r--   0        0        0    31619 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/forms.py
--rw-r--r--   0        0        0     3175 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1089 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0      793 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     4485 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2411 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0     9590 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1470 2023-07-18 19:29:19.650982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     3778 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      747 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      322 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2558 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1884 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       65 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3482 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     1910 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0      655 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      598 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0      981 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0      408 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0     2017 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0     3232 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0      706 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     3034 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2616 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      200 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1082 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     2892 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      759 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     7423 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      196 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      575 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     3858 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1512 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      390 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2561 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    10763 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0     9741 2023-07-18 19:29:19.654982 aleksis_core-3.1.3/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    12252 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    14534 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     1211 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0      538 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     3441 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     2256 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      736 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     2154 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0     1619 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     6380 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    36573 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74307 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2023-07-18 19:29:19.658983 aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    63806 2023-07-18 19:31:02.266843 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   126085 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2023-07-18 19:31:02.242842 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2023-07-18 19:31:02.210841 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    77782 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-18 19:31:02.206840 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2584 2023-07-18 19:31:02.210841 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    82875 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-18 19:31:02.194840 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74237 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-18 19:31:02.230841 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    80303 2023-07-18 19:31:02.218841 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   144575 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-18 19:31:02.202840 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-18 19:31:02.246842 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74177 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    77610 2023-07-18 19:31:02.226841 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   131787 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-18 19:31:02.214841 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0     1095 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     4690 2023-07-18 19:29:19.662983 aleksis_core-3.1.3/aleksis/core/managers.py
--rw-r--r--   0        0        0    51004 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2473 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1396 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     2311 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2270 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1538 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2177 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1781 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2023-07-18 19:29:19.666983 aleksis_core-3.1.3/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2023-07-18 19:29:19.670983 aleksis_core-3.1.3/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2717 2023-07-18 19:29:19.670983 aleksis_core-3.1.3/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      580 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0        0 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    19769 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/mixins.py
--rw-r--r--   0        0        0    51781 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/models.py
--rw-r--r--   0        0        0    13478 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/preferences.py
--rw-r--r--   0        0        0      692 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/registries.py
--rw-r--r--   0        0        0    16018 2023-07-18 19:29:19.674983 aleksis_core-3.1.3/aleksis/core/rules.py
--rw-r--r--   0        0        0     7486 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     1301 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     3049 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2046 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1743 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1179 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      535 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0     9708 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/person.py
--rw-r--r--   0        0        0      191 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/room.py
--rw-r--r--   0        0        0      163 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1651 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39943 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2023-07-18 19:29:19.678983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4350 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2578 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15745 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     6876 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0      804 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0      888 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_change_disabled.html
--rw-r--r--   0        0        0     1376 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0      483 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/edit.html
--rw-r--r--   0        0        0      594 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/list.html
--rw-r--r--   0        0        0     1053 2023-07-18 19:29:19.682983 aleksis_core-3.1.3/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1212 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0      465 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group_type/edit.html
--rw-r--r--   0        0        0      564 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/group_type/list.html
--rw-r--r--   0        0        0     2504 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2374 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      455 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/create.html
--rw-r--r--   0        0        0      451 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/edit.html
--rw-r--r--   0        0        0      556 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/school_term/list.html
--rw-r--r--   0        0        0      935 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2023-07-18 19:29:19.686984 aleksis_core-3.1.3/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1434 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0      990 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6712 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3312 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1618 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1523 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0     6596 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     6562 2023-07-18 19:29:19.690984 aleksis_core-3.1.3/aleksis/core/tests/models/test_group.py
--rw-r--r--   0        0        0     1520 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    18734 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2023-07-18 19:30:56.514626 aleksis_core-3.1.3/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14902 2023-07-18 19:30:58.866715 aleksis_core-3.1.3/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2023-07-18 19:31:01.162801 aleksis_core-3.1.3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    24932 2023-07-18 19:30:56.522626 aleksis_core-3.1.3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2023-07-18 19:30:57.174651 aleksis_core-3.1.3/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2023-07-18 19:31:01.186802 aleksis_core-3.1.3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5712 2023-07-18 19:31:01.166801 aleksis_core-3.1.3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9548 2023-07-18 19:31:01.610818 aleksis_core-3.1.3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2023-07-18 19:30:58.902716 aleksis_core-3.1.3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      664 2023-07-18 19:30:58.898716 aleksis_core-3.1.3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    10969 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     5970 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    16042 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2901 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3732 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5583 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2023-07-18 19:29:19.694984 aleksis_core-3.1.3/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/search.py
--rw-r--r--   0        0        0      130 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    55996 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/views.py
--rw-r--r--   0        0        0    10257 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       45 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/conftest.py
--rw-r--r--   0        0        0      581 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/Makefile
--rw-r--r--   0        0        0   127432 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2023-07-18 19:29:19.698984 aleksis_core-3.1.3/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2023-07-18 19:29:19.702984 aleksis_core-3.1.3/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2023-07-18 19:29:19.706984 aleksis_core-3.1.3/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8067 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2023-07-18 19:29:19.710985 aleksis_core-3.1.3/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6393 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/conf.py
--rw-r--r--   0        0        0      132 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4058 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/index.rst
--rw-r--r--   0        0        0      787 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/make.bat
--rw-r--r--   0        0        0       95 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     5409 2023-07-18 19:29:40.519767 aleksis_core-3.1.3/pyproject.toml
--rw-r--r--   0        0        0     2599 2023-07-18 19:29:19.714985 aleksis_core-3.1.3/tox.ini
--rw-r--r--   0        0        0     8657 1970-01-01 00:00:00.000000 aleksis_core-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0    38665 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/README.rst
+-rw-r--r--   0        0        0      194 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2023-07-20 17:27:00.636663 aleksis_core-3.1.4/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2023-07-20 17:27:02.232723 aleksis_core-3.1.4/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2023-07-20 17:27:08.300952 aleksis_core-3.1.4/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    11380 2023-07-20 17:27:04.324802 aleksis_core-3.1.4/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2023-07-20 17:27:00.700666 aleksis_core-3.1.4/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2023-07-20 17:27:08.532961 aleksis_core-3.1.4/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    17897 2023-07-20 17:27:07.612926 aleksis_core-3.1.4/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2023-07-20 17:27:08.548961 aleksis_core-3.1.4/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     8423 2023-07-20 17:27:07.684929 aleksis_core-3.1.4/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    31466 2023-07-20 17:27:07.616926 aleksis_core-3.1.4/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    85606 2023-07-20 17:27:06.492884 aleksis_core-3.1.4/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    22237 2023-07-20 17:27:08.720968 aleksis_core-3.1.4/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1370 2023-07-20 17:27:04.356803 aleksis_core-3.1.4/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    16523 2023-07-20 17:27:08.356954 aleksis_core-3.1.4/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    44051 2023-07-20 17:27:02.264725 aleksis_core-3.1.4/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2023-07-20 17:27:07.704929 aleksis_core-3.1.4/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0      950 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8519 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2023-07-20 17:24:58.344057 aleksis_core-3.1.4/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2751 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/checks.py
+-rw-r--r--   0        0        0    11534 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5556 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/filters.py
+-rw-r--r--   0        0        0    31619 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3175 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1089 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0      793 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4485 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2411 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0     9590 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1470 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     3778 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      747 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      322 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2558 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1884 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       65 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3482 2023-07-20 17:24:58.348057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     1910 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0      655 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      598 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0      981 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0      408 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0     2017 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0     3232 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0      706 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     3034 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      200 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1082 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     2892 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      759 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     7423 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      196 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      575 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     3858 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1512 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      390 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2561 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    10763 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0     9741 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    12252 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    14534 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     1211 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0      538 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     3441 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     2256 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      736 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0     2154 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0     1619 2023-07-20 17:24:58.352057 aleksis_core-3.1.4/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     6380 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    36573 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2023-07-20 17:27:09.520998 aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74307 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2023-07-20 17:27:09.492997 aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    63806 2023-07-20 17:27:09.444995 aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   126085 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2023-07-20 17:27:09.428995 aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2023-07-20 17:27:09.460996 aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    77782 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-20 17:27:09.460996 aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2023-07-20 17:24:58.356057 aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2584 2023-07-20 17:27:09.404994 aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    82875 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-20 17:27:09.388993 aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-20 17:27:09.633002 aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74237 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-20 17:27:09.544999 aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    80303 2023-07-20 17:27:09.577000 aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   144575 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-20 17:27:09.536999 aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-20 17:27:09.504997 aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74177 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-20 17:27:09.448995 aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    77610 2023-07-20 17:27:09.633002 aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   131787 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-20 17:27:09.577000 aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0     1095 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     4690 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/managers.py
+-rw-r--r--   0        0        0    51004 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2473 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1396 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     2311 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2270 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2023-07-20 17:24:58.360057 aleksis_core-3.1.4/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1538 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2177 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1781 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2717 2023-07-20 17:24:58.364058 aleksis_core-3.1.4/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2023-07-20 17:24:58.368058 aleksis_core-3.1.4/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      580 2023-07-20 17:24:58.368058 aleksis_core-3.1.4/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.368058 aleksis_core-3.1.4/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    19787 2023-07-20 17:24:58.368058 aleksis_core-3.1.4/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    51781 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/models.py
+-rw-r--r--   0        0        0    13478 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      692 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/registries.py
+-rw-r--r--   0        0        0    16018 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/rules.py
+-rw-r--r--   0        0        0     7486 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     1301 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     3049 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2046 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1743 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1179 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      535 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0     9708 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0      191 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0      163 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1651 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39943 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2023-07-20 17:24:58.372058 aleksis_core-3.1.4/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4350 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2578 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15745 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     6876 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0      804 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0      888 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_change_disabled.html
+-rw-r--r--   0        0        0     1376 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0      483 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/additional_field/edit.html
+-rw-r--r--   0        0        0      594 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/additional_field/list.html
+-rw-r--r--   0        0        0     1053 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1212 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0      465 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group_type/edit.html
+-rw-r--r--   0        0        0      564 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/group_type/list.html
+-rw-r--r--   0        0        0     2504 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2023-07-20 17:24:58.376058 aleksis_core-3.1.4/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2374 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      455 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/school_term/create.html
+-rw-r--r--   0        0        0      451 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/school_term/edit.html
+-rw-r--r--   0        0        0      556 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/school_term/list.html
+-rw-r--r--   0        0        0      935 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1434 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0      990 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6712 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2023-07-20 17:24:58.380058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3312 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1618 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1523 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0     6596 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     6562 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test_group.py
+-rw-r--r--   0        0        0     1520 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    18734 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-20 17:27:01.444694 aleksis_core-3.1.4/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14902 2023-07-20 17:27:04.360803 aleksis_core-3.1.4/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2023-07-20 17:27:07.700929 aleksis_core-3.1.4/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    24932 2023-07-20 17:27:01.448694 aleksis_core-3.1.4/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2023-07-20 17:27:02.128719 aleksis_core-3.1.4/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2023-07-20 17:27:07.736931 aleksis_core-3.1.4/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5712 2023-07-20 17:27:07.708930 aleksis_core-3.1.4/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9548 2023-07-20 17:27:08.360954 aleksis_core-3.1.4/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2023-07-20 17:27:04.416806 aleksis_core-3.1.4/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      664 2023-07-20 17:27:04.400805 aleksis_core-3.1.4/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    10969 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     5970 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    16042 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2901 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2023-07-20 17:24:58.384058 aleksis_core-3.1.4/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3732 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5583 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      130 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    55996 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/views.py
+-rw-r--r--   0        0        0    10257 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       45 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/conftest.py
+-rw-r--r--   0        0        0      581 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/docs/Makefile
+-rw-r--r--   0        0        0   127432 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2023-07-20 17:24:58.388059 aleksis_core-3.1.4/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2023-07-20 17:24:58.392059 aleksis_core-3.1.4/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2023-07-20 17:24:58.396059 aleksis_core-3.1.4/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2023-07-20 17:24:58.396059 aleksis_core-3.1.4/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2023-07-20 17:24:58.396059 aleksis_core-3.1.4/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2023-07-20 17:24:58.396059 aleksis_core-3.1.4/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2023-07-20 17:24:58.396059 aleksis_core-3.1.4/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8067 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6393 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/conf.py
+-rw-r--r--   0        0        0      132 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/make.bat
+-rw-r--r--   0        0        0       95 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5409 2023-07-20 17:25:19.440851 aleksis_core-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2599 2023-07-20 17:24:58.400059 aleksis_core-3.1.4/tox.ini
+-rw-r--r--   0        0        0     8657 1970-01-01 00:00:00.000000 aleksis_core-3.1.4/PKG-INFO
```

### Comparing `aleksis_core-3.1.3/CHANGELOG.rst` & `aleksis_core-3.1.4/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+`3.1.4`_ - 2023-07-20
+---------------------
+
+Fixed
+~~~~~
+
+* Extensible form was broken due to a missing import.
+
 `3.1.3`_ – 2023-07-18
 ---------------------
 
 Fixed
 ~~~~~
 
 * [Docker] The build could silently continue even if frontend bundling failed, resulting
```

### Comparing `aleksis_core-3.1.3/LICENCE.rst` & `aleksis_core-3.1.4/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/README.rst` & `aleksis_core-3.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 950
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 8519
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 2751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 11534
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 4690
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,50 +1,50 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
-files sz: 19769
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
+files sz: 19787
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d015a010100640064036c026d
       035a036d045a046d055a056d065a066d075a076d085a080100640064046c
       096d0a5a0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e6d
       0f5a0f0100640064076c106d115a110100640064086c126d135a13010064
       0064096c146d155a1501006400640a6c166d175a1701006400640b6c186d
       195a196d1a5a1a01006400640c6c1b6d1c5a1c6d1d5a1d01006400640d6c
-      1e6d1f5a1f01006400640e6c206d215a216d225a2201006400640f6c236d
-      245a240100640064106c256d265a266d275a270100640064116c286d295a
-      2a0100640064126c2b6d2c5a2c6d2d5a2d0100640064136c2e6d2f5a2f6d
-      305a300100640064016c315a31640064146c326d335a330100640064156c
-      346d355a350100640064166c366d375a370100640064176c386d395a3901
-      00640064186c3a6d3b5a3b6d3c5a3c0100640064196c3d6d3e5a3e6d3f5a
-      3f6d405a4001006400641a6c416d425a4201006400641b6c436d445a4401
-      006400641c6c456d465a4601006400641d6c476d485a4801006400641e6c
-      496d4a5a4a6d4b5a4b6d4c5a4c010002004700641f8400642065176a4d00
-      000000000000006a4e0000000000000000a6030000ab0300000000000000
-      005a4f642184005a500200470064228400642365176a5100000000000000
-      00654fac24a6040000ab0400000000000000005a52020047006425840064
-      26654f6542a6040000ab0400000000000000005a53020047006427840064
-      28655265466553ac24a6050000ab0500000000000000005a540200470064
-      298400642a6555a6030000ab0300000000000000005a5602004700642b84
-      00642c65176a510000000000000000a6030000ab0300000000000000005a
-      5702004700642d8400642e6522a6030000ab0300000000000000005a5802
-      004700642f8400643065216558ac24a6040000ab0400000000000000005a
-      590200470064318400643265376548a6040000ab0400000000000000005a
-      5a020047006433840064346530a6030000ab0300000000000000005a5b02
-      004700643584006436650fa6030000ab0300000000000000005a5c020047
-      00643784006438655b652ca6040000ab0400000000000000005a5d020047
-      0064398400643a655b652da6040000ab0400000000000000005a5e020047
-      00643b8400643c652fa6030000ab0300000000000000005a5f0200470064
-      3d8400643e6552a6030000ab0300000000000000005a6002004700643f84
-      0064406559a6030000ab0300000000000000005a61020047006441840064
-      426535a6030000ab0300000000000000005a6202004700644384006444a6
-      020000ab0200000000000000005a6364015300
+      1e6d1f5a1f01006400640e6c206d215a216d225a226d235a230100640064
+      0f6c246d255a250100640064106c266d275a276d285a280100640064116c
+      296d2a5a2b0100640064126c2c6d2d5a2d6d2e5a2e0100640064136c2f6d
+      305a306d315a310100640064016c325a32640064146c336d345a34010064
+      0064156c356d365a360100640064166c376d385a380100640064176c396d
+      3a5a3a0100640064186c3b6d3c5a3c6d3d5a3d0100640064196c3e6d3f5a
+      3f6d405a406d415a4101006400641a6c426d435a4301006400641b6c446d
+      455a4501006400641c6c466d475a4701006400641d6c486d495a49010064
+      00641e6c4a6d4b5a4b6d4c5a4c6d4d5a4d010002004700641f8400642065
+      176a4e00000000000000006a4f0000000000000000a6030000ab03000000
+      00000000005a50642184005a510200470064228400642365176a52000000
+      00000000006550ac24a6040000ab0400000000000000005a530200470064
+      258400642665506543a6040000ab0400000000000000005a540200470064
+      2784006428655365476554ac24a6050000ab0500000000000000005a5502
+      00470064298400642a6556a6030000ab0300000000000000005a57020047
+      00642b8400642c65176a520000000000000000a6030000ab030000000000
+      0000005a5802004700642d8400642e6522a6030000ab0300000000000000
+      005a5902004700642f8400643065216559ac24a6040000ab040000000000
+      0000005a5a0200470064318400643265386549a6040000ab040000000000
+      0000005a5b020047006433840064346531a6030000ab0300000000000000
+      005a5c02004700643584006436650fa6030000ab0300000000000000005a
+      5d02004700643784006438655c652da6040000ab0400000000000000005a
+      5e0200470064398400643a655c652ea6040000ab0400000000000000005a
+      5f02004700643b8400643c6530a6030000ab0300000000000000005a6002
+      004700643d8400643e6553a6030000ab0300000000000000005a61020047
+      00643f84006440655aa6030000ab0300000000000000005a620200470064
+      41840064426536a6030000ab0300000000000000005a6302004700644384
+      006444a6020000ab0200000000000000005a6464015300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -145,356 +145,358 @@
                176 LOAD_CONST              13 (('BaseForm',))
                178 IMPORT_NAME             30 (django.forms.forms)
                180 IMPORT_FROM             31 (BaseForm)
                182 STORE_NAME              31 (BaseForm)
                184 POP_TOP
    
     17         186 LOAD_CONST               0 (0)
-               188 LOAD_CONST              14 (('ModelForm', 'ModelFormMetaclass'))
+               188 LOAD_CONST              14 (('ModelForm', 'ModelFormMetaclass', 'fields_for_model'))
                190 IMPORT_NAME             32 (django.forms.models)
                192 IMPORT_FROM             33 (ModelForm)
                194 STORE_NAME              33 (ModelForm)
                196 IMPORT_FROM             34 (ModelFormMetaclass)
                198 STORE_NAME              34 (ModelFormMetaclass)
-               200 POP_TOP
-   
-    18         202 LOAD_CONST               0 (0)
-               204 LOAD_CONST              15 (('HttpResponse',))
-               206 IMPORT_NAME             35 (django.http)
-               208 IMPORT_FROM             36 (HttpResponse)
-               210 STORE_NAME              36 (HttpResponse)
-               212 POP_TOP
-   
-    19         214 LOAD_CONST               0 (0)
-               216 LOAD_CONST              16 (('classproperty', 'lazy'))
-               218 IMPORT_NAME             37 (django.utils.functional)
-               220 IMPORT_FROM             38 (classproperty)
-               222 STORE_NAME              38 (classproperty)
-               224 IMPORT_FROM             39 (lazy)
-               226 STORE_NAME              39 (lazy)
-               228 POP_TOP
-   
-    20         230 LOAD_CONST               0 (0)
-               232 LOAD_CONST              17 (('gettext',))
-               234 IMPORT_NAME             40 (django.utils.translation)
-               236 IMPORT_FROM             41 (gettext)
-               238 STORE_NAME              42 (_)
-               240 POP_TOP
-   
-    21         242 LOAD_CONST               0 (0)
-               244 LOAD_CONST              18 (('CreateView', 'UpdateView'))
-               246 IMPORT_NAME             43 (django.views.generic)
-               248 IMPORT_FROM             44 (CreateView)
-               250 STORE_NAME              44 (CreateView)
-               252 IMPORT_FROM             45 (UpdateView)
-               254 STORE_NAME              45 (UpdateView)
-               256 POP_TOP
-   
-    22         258 LOAD_CONST               0 (0)
-               260 LOAD_CONST              19 (('DeleteView', 'ModelFormMixin'))
-               262 IMPORT_NAME             46 (django.views.generic.edit)
-               264 IMPORT_FROM             47 (DeleteView)
-               266 STORE_NAME              47 (DeleteView)
-               268 IMPORT_FROM             48 (ModelFormMixin)
-               270 STORE_NAME              48 (ModelFormMixin)
-               272 POP_TOP
-   
-    24         274 LOAD_CONST               0 (0)
-               276 LOAD_CONST               1 (None)
-               278 IMPORT_NAME             49 (reversion)
-               280 STORE_NAME              49 (reversion)
-   
-    25         282 LOAD_CONST               0 (0)
-               284 LOAD_CONST              20 (('preferences_settings',))
-               286 IMPORT_NAME             50 (dynamic_preferences.settings)
-               288 IMPORT_FROM             51 (preferences_settings)
-               290 STORE_NAME              51 (preferences_settings)
-               292 POP_TOP
-   
-    26         294 LOAD_CONST               0 (0)
-               296 LOAD_CONST              21 (('FilePreference',))
-               298 IMPORT_NAME             52 (dynamic_preferences.types)
-               300 IMPORT_FROM             53 (FilePreference)
-               302 STORE_NAME              53 (FilePreference)
-               304 POP_TOP
-   
-    27         306 LOAD_CONST               0 (0)
-               308 LOAD_CONST              22 (('GuardedModelAdmin',))
-               310 IMPORT_NAME             54 (guardian.admin)
-               312 IMPORT_FROM             55 (GuardedModelAdmin)
-               314 STORE_NAME              55 (GuardedModelAdmin)
-               316 POP_TOP
-   
-    28         318 LOAD_CONST               0 (0)
-               320 LOAD_CONST              23 (('ObjectPermissionChecker',))
-               322 IMPORT_NAME             56 (guardian.core)
-               324 IMPORT_FROM             57 (ObjectPermissionChecker)
-               326 STORE_NAME              57 (ObjectPermissionChecker)
-               328 POP_TOP
-   
-    29         330 LOAD_CONST               0 (0)
-               332 LOAD_CONST              24 (('IntegerField', 'JSONFieldMixin'))
-               334 IMPORT_NAME             58 (jsonstore.fields)
-               336 IMPORT_FROM             59 (IntegerField)
-               338 STORE_NAME              59 (IntegerField)
-               340 IMPORT_FROM             60 (JSONFieldMixin)
-               342 STORE_NAME              60 (JSONFieldMixin)
-               344 POP_TOP
-   
-    30         346 LOAD_CONST               0 (0)
-               348 LOAD_CONST              25 (('Fieldset', 'Layout', 'LayoutNode'))
-               350 IMPORT_NAME             61 (material.base)
-               352 IMPORT_FROM             62 (Fieldset)
-               354 STORE_NAME              62 (Fieldset)
-               356 IMPORT_FROM             63 (Layout)
-               358 STORE_NAME              63 (Layout)
-               360 IMPORT_FROM             64 (LayoutNode)
-               362 STORE_NAME              64 (LayoutNode)
-               364 POP_TOP
-   
-    31         366 LOAD_CONST               0 (0)
-               368 LOAD_CONST              26 (('PolymorphicModelBase',))
-               370 IMPORT_NAME             65 (polymorphic.base)
-               372 IMPORT_FROM             66 (PolymorphicModelBase)
-               374 STORE_NAME              66 (PolymorphicModelBase)
-               376 POP_TOP
-   
-    32         378 LOAD_CONST               0 (0)
-               380 LOAD_CONST              27 (('PolymorphicManager',))
-               382 IMPORT_NAME             67 (polymorphic.managers)
-               384 IMPORT_FROM             68 (PolymorphicManager)
-               386 STORE_NAME              68 (PolymorphicManager)
-               388 POP_TOP
-   
-    33         390 LOAD_CONST               0 (0)
-               392 LOAD_CONST              28 (('PolymorphicModel',))
-               394 IMPORT_NAME             69 (polymorphic.models)
-               396 IMPORT_FROM             70 (PolymorphicModel)
-               398 STORE_NAME              70 (PolymorphicModel)
-               400 POP_TOP
-   
-    34         402 LOAD_CONST               0 (0)
-               404 LOAD_CONST              29 (('ObjectPermissionsModelAdmin',))
-               406 IMPORT_NAME             71 (rules.contrib.admin)
-               408 IMPORT_FROM             72 (ObjectPermissionsModelAdmin)
-               410 STORE_NAME              72 (ObjectPermissionsModelAdmin)
-               412 POP_TOP
-   
-    36         414 LOAD_CONST               0 (0)
-               416 LOAD_CONST              30 (('CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet'))
-               418 IMPORT_NAME             73 (aleksis.core.managers)
-               420 IMPORT_FROM             74 (CurrentSiteManagerWithoutMigrations)
-               422 STORE_NAME              74 (CurrentSiteManagerWithoutMigrations)
-               424 IMPORT_FROM             75 (PolymorphicCurrentSiteManager)
-               426 STORE_NAME              75 (PolymorphicCurrentSiteManager)
-               428 IMPORT_FROM             76 (SchoolTermRelatedQuerySet)
-               430 STORE_NAME              76 (SchoolTermRelatedQuerySet)
-               432 POP_TOP
-   
-    43         434 PUSH_NULL
-               436 LOAD_BUILD_CLASS
-               438 LOAD_CONST              31 (<code object _ExtensibleModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 43>)
-               440 MAKE_FUNCTION            0
-               442 LOAD_CONST              32 ('_ExtensibleModelBase')
-               444 LOAD_NAME               23 (models)
-               446 LOAD_ATTR               77 (base)
-               456 LOAD_ATTR               78 (ModelBase)
-               466 PRECALL                  3
-               470 CALL                     3
-               480 STORE_NAME              79 (_ExtensibleModelBase)
-   
-    63         482 LOAD_CONST              33 (<code object _generate_one_to_one_proxy_property, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 63>)
-               484 MAKE_FUNCTION            0
-               486 STORE_NAME              80 (_generate_one_to_one_proxy_property)
-   
-    85         488 PUSH_NULL
-               490 LOAD_BUILD_CLASS
-               492 LOAD_CONST              34 (<code object ExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 85>)
-               494 MAKE_FUNCTION            0
-               496 LOAD_CONST              35 ('ExtensibleModel')
-               498 LOAD_NAME               23 (models)
-               500 LOAD_ATTR               81 (Model)
-               510 LOAD_NAME               79 (_ExtensibleModelBase)
-               512 KW_NAMES                36
-               514 PRECALL                  4
-               518 CALL                     4
-               528 STORE_NAME              82 (ExtensibleModel)
-   
-   374         530 PUSH_NULL
-               532 LOAD_BUILD_CLASS
-               534 LOAD_CONST              37 (<code object _ExtensiblePolymorphicModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 374>)
-               536 MAKE_FUNCTION            0
-               538 LOAD_CONST              38 ('_ExtensiblePolymorphicModelBase')
-               540 LOAD_NAME               79 (_ExtensibleModelBase)
-               542 LOAD_NAME               66 (PolymorphicModelBase)
-               544 PRECALL                  4
-               548 CALL                     4
-               558 STORE_NAME              83 (_ExtensiblePolymorphicModelBase)
-   
-   378         560 PUSH_NULL
-               562 LOAD_BUILD_CLASS
-               564 LOAD_CONST              39 (<code object ExtensiblePolymorphicModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 378>)
-               566 MAKE_FUNCTION            0
-               568 LOAD_CONST              40 ('ExtensiblePolymorphicModel')
-   
-   379         570 LOAD_NAME               82 (ExtensibleModel)
-               572 LOAD_NAME               70 (PolymorphicModel)
-               574 LOAD_NAME               83 (_ExtensiblePolymorphicModelBase)
-   
-   378         576 KW_NAMES                36
-               578 PRECALL                  5
-               582 CALL                     5
-               592 STORE_NAME              84 (ExtensiblePolymorphicModel)
-   
-   390         594 PUSH_NULL
-               596 LOAD_BUILD_CLASS
-               598 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 390>)
-               600 MAKE_FUNCTION            0
-               602 LOAD_CONST              42 ('PureDjangoModel')
-               604 LOAD_NAME               85 (object)
-               606 PRECALL                  3
-               610 CALL                     3
-               620 STORE_NAME              86 (PureDjangoModel)
-   
-   396         622 PUSH_NULL
-               624 LOAD_BUILD_CLASS
-               626 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 396>)
-               628 MAKE_FUNCTION            0
-               630 LOAD_CONST              44 ('GlobalPermissionModel')
-               632 LOAD_NAME               23 (models)
-               634 LOAD_ATTR               81 (Model)
-               644 PRECALL                  3
-               648 CALL                     3
-               658 STORE_NAME              87 (GlobalPermissionModel)
-   
-   407         660 PUSH_NULL
-               662 LOAD_BUILD_CLASS
-               664 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 407>)
-               666 MAKE_FUNCTION            0
-               668 LOAD_CONST              46 ('_ExtensibleFormMetaclass')
-               670 LOAD_NAME               34 (ModelFormMetaclass)
-               672 PRECALL                  3
-               676 CALL                     3
-               686 STORE_NAME              88 (_ExtensibleFormMetaclass)
-   
-   423         688 PUSH_NULL
-               690 LOAD_BUILD_CLASS
-               692 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 423>)
-               694 MAKE_FUNCTION            0
-               696 LOAD_CONST              48 ('ExtensibleForm')
-               698 LOAD_NAME               33 (ModelForm)
-               700 LOAD_NAME               88 (_ExtensibleFormMetaclass)
-               702 KW_NAMES                36
-               704 PRECALL                  4
-               708 CALL                     4
-               718 STORE_NAME              89 (ExtensibleForm)
-   
-   467         720 PUSH_NULL
-               722 LOAD_BUILD_CLASS
-               724 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 467>)
-               726 MAKE_FUNCTION            0
-               728 LOAD_CONST              50 ('BaseModelAdmin')
-               730 LOAD_NAME               55 (GuardedModelAdmin)
-               732 LOAD_NAME               72 (ObjectPermissionsModelAdmin)
-               734 PRECALL                  4
-               738 CALL                     4
-               748 STORE_NAME              90 (BaseModelAdmin)
-   
-   473         750 PUSH_NULL
-               752 LOAD_BUILD_CLASS
-               754 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 473>)
-               756 MAKE_FUNCTION            0
-               758 LOAD_CONST              52 ('SuccessMessageMixin')
-               760 LOAD_NAME               48 (ModelFormMixin)
-               762 PRECALL                  3
-               766 CALL                     3
-               776 STORE_NAME              91 (SuccessMessageMixin)
-   
-   482         778 PUSH_NULL
-               780 LOAD_BUILD_CLASS
-               782 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 482>)
-               784 MAKE_FUNCTION            0
-               786 LOAD_CONST              54 ('SuccessNextMixin')
-               788 LOAD_NAME               15 (RedirectURLMixin)
-               790 PRECALL                  3
-               794 CALL                     3
-               804 STORE_NAME              92 (SuccessNextMixin)
-   
-   489         806 PUSH_NULL
-               808 LOAD_BUILD_CLASS
-               810 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 489>)
-               812 MAKE_FUNCTION            0
-               814 LOAD_CONST              56 ('AdvancedCreateView')
-               816 LOAD_NAME               91 (SuccessMessageMixin)
-               818 LOAD_NAME               44 (CreateView)
-               820 PRECALL                  4
-               824 CALL                     4
-               834 STORE_NAME              93 (AdvancedCreateView)
-   
-   493         836 PUSH_NULL
-               838 LOAD_BUILD_CLASS
-               840 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 493>)
-               842 MAKE_FUNCTION            0
-               844 LOAD_CONST              58 ('AdvancedEditView')
-               846 LOAD_NAME               91 (SuccessMessageMixin)
-               848 LOAD_NAME               45 (UpdateView)
-               850 PRECALL                  4
-               854 CALL                     4
-               864 STORE_NAME              94 (AdvancedEditView)
-   
-   497         866 PUSH_NULL
-               868 LOAD_BUILD_CLASS
-               870 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 497>)
-               872 MAKE_FUNCTION            0
-               874 LOAD_CONST              60 ('AdvancedDeleteView')
-               876 LOAD_NAME               47 (DeleteView)
-               878 PRECALL                  3
-               882 CALL                     3
-               892 STORE_NAME              95 (AdvancedDeleteView)
-   
-   516         894 PUSH_NULL
-               896 LOAD_BUILD_CLASS
-               898 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 516>)
-               900 MAKE_FUNCTION            0
-               902 LOAD_CONST              62 ('SchoolTermRelatedExtensibleModel')
-               904 LOAD_NAME               82 (ExtensibleModel)
-               906 PRECALL                  3
-               910 CALL                     3
-               920 STORE_NAME              96 (SchoolTermRelatedExtensibleModel)
-   
-   534         922 PUSH_NULL
-               924 LOAD_BUILD_CLASS
-               926 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 534>)
-               928 MAKE_FUNCTION            0
-               930 LOAD_CONST              64 ('SchoolTermRelatedExtensibleForm')
-               932 LOAD_NAME               89 (ExtensibleForm)
-               934 PRECALL                  3
-               938 CALL                     3
-               948 STORE_NAME              97 (SchoolTermRelatedExtensibleForm)
-   
-   551         950 PUSH_NULL
-               952 LOAD_BUILD_CLASS
-               954 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 551>)
-               956 MAKE_FUNCTION            0
-               958 LOAD_CONST              66 ('PublicFilePreferenceMixin')
-               960 LOAD_NAME               53 (FilePreference)
-               962 PRECALL                  3
-               966 CALL                     3
-               976 STORE_NAME              98 (PublicFilePreferenceMixin)
-   
-   562         978 PUSH_NULL
-               980 LOAD_BUILD_CLASS
-               982 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 562>)
-               984 MAKE_FUNCTION            0
-               986 LOAD_CONST              68 ('RegistryObject')
-               988 PRECALL                  2
-               992 CALL                     2
-              1002 STORE_NAME              99 (RegistryObject)
-              1004 LOAD_CONST               1 (None)
-              1006 RETURN_VALUE
+               200 IMPORT_FROM             35 (fields_for_model)
+               202 STORE_NAME              35 (fields_for_model)
+               204 POP_TOP
+   
+    18         206 LOAD_CONST               0 (0)
+               208 LOAD_CONST              15 (('HttpResponse',))
+               210 IMPORT_NAME             36 (django.http)
+               212 IMPORT_FROM             37 (HttpResponse)
+               214 STORE_NAME              37 (HttpResponse)
+               216 POP_TOP
+   
+    19         218 LOAD_CONST               0 (0)
+               220 LOAD_CONST              16 (('classproperty', 'lazy'))
+               222 IMPORT_NAME             38 (django.utils.functional)
+               224 IMPORT_FROM             39 (classproperty)
+               226 STORE_NAME              39 (classproperty)
+               228 IMPORT_FROM             40 (lazy)
+               230 STORE_NAME              40 (lazy)
+               232 POP_TOP
+   
+    20         234 LOAD_CONST               0 (0)
+               236 LOAD_CONST              17 (('gettext',))
+               238 IMPORT_NAME             41 (django.utils.translation)
+               240 IMPORT_FROM             42 (gettext)
+               242 STORE_NAME              43 (_)
+               244 POP_TOP
+   
+    21         246 LOAD_CONST               0 (0)
+               248 LOAD_CONST              18 (('CreateView', 'UpdateView'))
+               250 IMPORT_NAME             44 (django.views.generic)
+               252 IMPORT_FROM             45 (CreateView)
+               254 STORE_NAME              45 (CreateView)
+               256 IMPORT_FROM             46 (UpdateView)
+               258 STORE_NAME              46 (UpdateView)
+               260 POP_TOP
+   
+    22         262 LOAD_CONST               0 (0)
+               264 LOAD_CONST              19 (('DeleteView', 'ModelFormMixin'))
+               266 IMPORT_NAME             47 (django.views.generic.edit)
+               268 IMPORT_FROM             48 (DeleteView)
+               270 STORE_NAME              48 (DeleteView)
+               272 IMPORT_FROM             49 (ModelFormMixin)
+               274 STORE_NAME              49 (ModelFormMixin)
+               276 POP_TOP
+   
+    24         278 LOAD_CONST               0 (0)
+               280 LOAD_CONST               1 (None)
+               282 IMPORT_NAME             50 (reversion)
+               284 STORE_NAME              50 (reversion)
+   
+    25         286 LOAD_CONST               0 (0)
+               288 LOAD_CONST              20 (('preferences_settings',))
+               290 IMPORT_NAME             51 (dynamic_preferences.settings)
+               292 IMPORT_FROM             52 (preferences_settings)
+               294 STORE_NAME              52 (preferences_settings)
+               296 POP_TOP
+   
+    26         298 LOAD_CONST               0 (0)
+               300 LOAD_CONST              21 (('FilePreference',))
+               302 IMPORT_NAME             53 (dynamic_preferences.types)
+               304 IMPORT_FROM             54 (FilePreference)
+               306 STORE_NAME              54 (FilePreference)
+               308 POP_TOP
+   
+    27         310 LOAD_CONST               0 (0)
+               312 LOAD_CONST              22 (('GuardedModelAdmin',))
+               314 IMPORT_NAME             55 (guardian.admin)
+               316 IMPORT_FROM             56 (GuardedModelAdmin)
+               318 STORE_NAME              56 (GuardedModelAdmin)
+               320 POP_TOP
+   
+    28         322 LOAD_CONST               0 (0)
+               324 LOAD_CONST              23 (('ObjectPermissionChecker',))
+               326 IMPORT_NAME             57 (guardian.core)
+               328 IMPORT_FROM             58 (ObjectPermissionChecker)
+               330 STORE_NAME              58 (ObjectPermissionChecker)
+               332 POP_TOP
+   
+    29         334 LOAD_CONST               0 (0)
+               336 LOAD_CONST              24 (('IntegerField', 'JSONFieldMixin'))
+               338 IMPORT_NAME             59 (jsonstore.fields)
+               340 IMPORT_FROM             60 (IntegerField)
+               342 STORE_NAME              60 (IntegerField)
+               344 IMPORT_FROM             61 (JSONFieldMixin)
+               346 STORE_NAME              61 (JSONFieldMixin)
+               348 POP_TOP
+   
+    30         350 LOAD_CONST               0 (0)
+               352 LOAD_CONST              25 (('Fieldset', 'Layout', 'LayoutNode'))
+               354 IMPORT_NAME             62 (material.base)
+               356 IMPORT_FROM             63 (Fieldset)
+               358 STORE_NAME              63 (Fieldset)
+               360 IMPORT_FROM             64 (Layout)
+               362 STORE_NAME              64 (Layout)
+               364 IMPORT_FROM             65 (LayoutNode)
+               366 STORE_NAME              65 (LayoutNode)
+               368 POP_TOP
+   
+    31         370 LOAD_CONST               0 (0)
+               372 LOAD_CONST              26 (('PolymorphicModelBase',))
+               374 IMPORT_NAME             66 (polymorphic.base)
+               376 IMPORT_FROM             67 (PolymorphicModelBase)
+               378 STORE_NAME              67 (PolymorphicModelBase)
+               380 POP_TOP
+   
+    32         382 LOAD_CONST               0 (0)
+               384 LOAD_CONST              27 (('PolymorphicManager',))
+               386 IMPORT_NAME             68 (polymorphic.managers)
+               388 IMPORT_FROM             69 (PolymorphicManager)
+               390 STORE_NAME              69 (PolymorphicManager)
+               392 POP_TOP
+   
+    33         394 LOAD_CONST               0 (0)
+               396 LOAD_CONST              28 (('PolymorphicModel',))
+               398 IMPORT_NAME             70 (polymorphic.models)
+               400 IMPORT_FROM             71 (PolymorphicModel)
+               402 STORE_NAME              71 (PolymorphicModel)
+               404 POP_TOP
+   
+    34         406 LOAD_CONST               0 (0)
+               408 LOAD_CONST              29 (('ObjectPermissionsModelAdmin',))
+               410 IMPORT_NAME             72 (rules.contrib.admin)
+               412 IMPORT_FROM             73 (ObjectPermissionsModelAdmin)
+               414 STORE_NAME              73 (ObjectPermissionsModelAdmin)
+               416 POP_TOP
+   
+    36         418 LOAD_CONST               0 (0)
+               420 LOAD_CONST              30 (('CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet'))
+               422 IMPORT_NAME             74 (aleksis.core.managers)
+               424 IMPORT_FROM             75 (CurrentSiteManagerWithoutMigrations)
+               426 STORE_NAME              75 (CurrentSiteManagerWithoutMigrations)
+               428 IMPORT_FROM             76 (PolymorphicCurrentSiteManager)
+               430 STORE_NAME              76 (PolymorphicCurrentSiteManager)
+               432 IMPORT_FROM             77 (SchoolTermRelatedQuerySet)
+               434 STORE_NAME              77 (SchoolTermRelatedQuerySet)
+               436 POP_TOP
+   
+    43         438 PUSH_NULL
+               440 LOAD_BUILD_CLASS
+               442 LOAD_CONST              31 (<code object _ExtensibleModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 43>)
+               444 MAKE_FUNCTION            0
+               446 LOAD_CONST              32 ('_ExtensibleModelBase')
+               448 LOAD_NAME               23 (models)
+               450 LOAD_ATTR               78 (base)
+               460 LOAD_ATTR               79 (ModelBase)
+               470 PRECALL                  3
+               474 CALL                     3
+               484 STORE_NAME              80 (_ExtensibleModelBase)
+   
+    63         486 LOAD_CONST              33 (<code object _generate_one_to_one_proxy_property, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 63>)
+               488 MAKE_FUNCTION            0
+               490 STORE_NAME              81 (_generate_one_to_one_proxy_property)
+   
+    85         492 PUSH_NULL
+               494 LOAD_BUILD_CLASS
+               496 LOAD_CONST              34 (<code object ExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 85>)
+               498 MAKE_FUNCTION            0
+               500 LOAD_CONST              35 ('ExtensibleModel')
+               502 LOAD_NAME               23 (models)
+               504 LOAD_ATTR               82 (Model)
+               514 LOAD_NAME               80 (_ExtensibleModelBase)
+               516 KW_NAMES                36
+               518 PRECALL                  4
+               522 CALL                     4
+               532 STORE_NAME              83 (ExtensibleModel)
+   
+   374         534 PUSH_NULL
+               536 LOAD_BUILD_CLASS
+               538 LOAD_CONST              37 (<code object _ExtensiblePolymorphicModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 374>)
+               540 MAKE_FUNCTION            0
+               542 LOAD_CONST              38 ('_ExtensiblePolymorphicModelBase')
+               544 LOAD_NAME               80 (_ExtensibleModelBase)
+               546 LOAD_NAME               67 (PolymorphicModelBase)
+               548 PRECALL                  4
+               552 CALL                     4
+               562 STORE_NAME              84 (_ExtensiblePolymorphicModelBase)
+   
+   378         564 PUSH_NULL
+               566 LOAD_BUILD_CLASS
+               568 LOAD_CONST              39 (<code object ExtensiblePolymorphicModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 378>)
+               570 MAKE_FUNCTION            0
+               572 LOAD_CONST              40 ('ExtensiblePolymorphicModel')
+   
+   379         574 LOAD_NAME               83 (ExtensibleModel)
+               576 LOAD_NAME               71 (PolymorphicModel)
+               578 LOAD_NAME               84 (_ExtensiblePolymorphicModelBase)
+   
+   378         580 KW_NAMES                36
+               582 PRECALL                  5
+               586 CALL                     5
+               596 STORE_NAME              85 (ExtensiblePolymorphicModel)
+   
+   390         598 PUSH_NULL
+               600 LOAD_BUILD_CLASS
+               602 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 390>)
+               604 MAKE_FUNCTION            0
+               606 LOAD_CONST              42 ('PureDjangoModel')
+               608 LOAD_NAME               86 (object)
+               610 PRECALL                  3
+               614 CALL                     3
+               624 STORE_NAME              87 (PureDjangoModel)
+   
+   396         626 PUSH_NULL
+               628 LOAD_BUILD_CLASS
+               630 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 396>)
+               632 MAKE_FUNCTION            0
+               634 LOAD_CONST              44 ('GlobalPermissionModel')
+               636 LOAD_NAME               23 (models)
+               638 LOAD_ATTR               82 (Model)
+               648 PRECALL                  3
+               652 CALL                     3
+               662 STORE_NAME              88 (GlobalPermissionModel)
+   
+   407         664 PUSH_NULL
+               666 LOAD_BUILD_CLASS
+               668 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 407>)
+               670 MAKE_FUNCTION            0
+               672 LOAD_CONST              46 ('_ExtensibleFormMetaclass')
+               674 LOAD_NAME               34 (ModelFormMetaclass)
+               676 PRECALL                  3
+               680 CALL                     3
+               690 STORE_NAME              89 (_ExtensibleFormMetaclass)
+   
+   423         692 PUSH_NULL
+               694 LOAD_BUILD_CLASS
+               696 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 423>)
+               698 MAKE_FUNCTION            0
+               700 LOAD_CONST              48 ('ExtensibleForm')
+               702 LOAD_NAME               33 (ModelForm)
+               704 LOAD_NAME               89 (_ExtensibleFormMetaclass)
+               706 KW_NAMES                36
+               708 PRECALL                  4
+               712 CALL                     4
+               722 STORE_NAME              90 (ExtensibleForm)
+   
+   467         724 PUSH_NULL
+               726 LOAD_BUILD_CLASS
+               728 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 467>)
+               730 MAKE_FUNCTION            0
+               732 LOAD_CONST              50 ('BaseModelAdmin')
+               734 LOAD_NAME               56 (GuardedModelAdmin)
+               736 LOAD_NAME               73 (ObjectPermissionsModelAdmin)
+               738 PRECALL                  4
+               742 CALL                     4
+               752 STORE_NAME              91 (BaseModelAdmin)
+   
+   473         754 PUSH_NULL
+               756 LOAD_BUILD_CLASS
+               758 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 473>)
+               760 MAKE_FUNCTION            0
+               762 LOAD_CONST              52 ('SuccessMessageMixin')
+               764 LOAD_NAME               49 (ModelFormMixin)
+               766 PRECALL                  3
+               770 CALL                     3
+               780 STORE_NAME              92 (SuccessMessageMixin)
+   
+   482         782 PUSH_NULL
+               784 LOAD_BUILD_CLASS
+               786 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 482>)
+               788 MAKE_FUNCTION            0
+               790 LOAD_CONST              54 ('SuccessNextMixin')
+               792 LOAD_NAME               15 (RedirectURLMixin)
+               794 PRECALL                  3
+               798 CALL                     3
+               808 STORE_NAME              93 (SuccessNextMixin)
+   
+   489         810 PUSH_NULL
+               812 LOAD_BUILD_CLASS
+               814 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 489>)
+               816 MAKE_FUNCTION            0
+               818 LOAD_CONST              56 ('AdvancedCreateView')
+               820 LOAD_NAME               92 (SuccessMessageMixin)
+               822 LOAD_NAME               45 (CreateView)
+               824 PRECALL                  4
+               828 CALL                     4
+               838 STORE_NAME              94 (AdvancedCreateView)
+   
+   493         840 PUSH_NULL
+               842 LOAD_BUILD_CLASS
+               844 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 493>)
+               846 MAKE_FUNCTION            0
+               848 LOAD_CONST              58 ('AdvancedEditView')
+               850 LOAD_NAME               92 (SuccessMessageMixin)
+               852 LOAD_NAME               46 (UpdateView)
+               854 PRECALL                  4
+               858 CALL                     4
+               868 STORE_NAME              95 (AdvancedEditView)
+   
+   497         870 PUSH_NULL
+               872 LOAD_BUILD_CLASS
+               874 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 497>)
+               876 MAKE_FUNCTION            0
+               878 LOAD_CONST              60 ('AdvancedDeleteView')
+               880 LOAD_NAME               48 (DeleteView)
+               882 PRECALL                  3
+               886 CALL                     3
+               896 STORE_NAME              96 (AdvancedDeleteView)
+   
+   516         898 PUSH_NULL
+               900 LOAD_BUILD_CLASS
+               902 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 516>)
+               904 MAKE_FUNCTION            0
+               906 LOAD_CONST              62 ('SchoolTermRelatedExtensibleModel')
+               908 LOAD_NAME               83 (ExtensibleModel)
+               910 PRECALL                  3
+               914 CALL                     3
+               924 STORE_NAME              97 (SchoolTermRelatedExtensibleModel)
+   
+   534         926 PUSH_NULL
+               928 LOAD_BUILD_CLASS
+               930 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 534>)
+               932 MAKE_FUNCTION            0
+               934 LOAD_CONST              64 ('SchoolTermRelatedExtensibleForm')
+               936 LOAD_NAME               90 (ExtensibleForm)
+               938 PRECALL                  3
+               942 CALL                     3
+               952 STORE_NAME              98 (SchoolTermRelatedExtensibleForm)
+   
+   551         954 PUSH_NULL
+               956 LOAD_BUILD_CLASS
+               958 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 551>)
+               960 MAKE_FUNCTION            0
+               962 LOAD_CONST              66 ('PublicFilePreferenceMixin')
+               964 LOAD_NAME               54 (FilePreference)
+               966 PRECALL                  3
+               970 CALL                     3
+               980 STORE_NAME              99 (PublicFilePreferenceMixin)
+   
+   562         982 PUSH_NULL
+               984 LOAD_BUILD_CLASS
+               986 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 562>)
+               988 MAKE_FUNCTION            0
+               990 LOAD_CONST              68 ('RegistryObject')
+               992 PRECALL                  2
+               996 CALL                     2
+              1006 STORE_NAME             100 (RegistryObject)
+              1008 LOAD_CONST               1 (None)
+              1010 RETURN_VALUE
    consts
       0
       None
       ('datetime',)
       ('Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union')
       ('settings',)
       ('messages',)
@@ -502,15 +504,15 @@
       ('ContentType',)
       ('CurrentSiteManager',)
       ('Site',)
       ('models',)
       ('JSONField', 'QuerySet')
       ('CharField', 'TextField')
       ('BaseForm',)
-      ('ModelForm', 'ModelFormMetaclass')
+      ('ModelForm', 'ModelFormMetaclass', 'fields_for_model')
       ('HttpResponse',)
       ('classproperty', 'lazy')
       ('gettext',)
       ('CreateView', 'UpdateView')
       ('DeleteView', 'ModelFormMixin')
       ('preferences_settings',)
       ('FilePreference',)
@@ -3984,19 +3986,19 @@
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'RegistryObject'
          firstlineno 562
          lnotab
             0x0c01040236011a020608020104ff0e010204020104ff0e010203020104
             ff0e010203020104ff0e01
       'RegistryObject'
-   names      ('os', 'datetime', 'typing', 'Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union', 'django.conf', 'settings', 'django.contrib', 'messages', 'django.contrib.auth.views', 'LoginView', 'RedirectURLMixin', 'django.contrib.contenttypes.models', 'ContentType', 'django.contrib.sites.managers', 'CurrentSiteManager', 'django.contrib.sites.models', 'Site', 'django.db', 'models', 'django.db.models', 'JSONField', 'QuerySet', 'django.db.models.fields', 'CharField', 'TextField', 'django.forms.forms', 'BaseForm', 'django.forms.models', 'ModelForm', 'ModelFormMetaclass', 'django.http', 'HttpResponse', 'django.utils.functional', 'classproperty', 'lazy', 'django.utils.translation', 'gettext', '_', 'django.views.generic', 'CreateView', 'UpdateView', 'django.views.generic.edit', 'DeleteView', 'ModelFormMixin', 'reversion', 'dynamic_preferences.settings', 'preferences_settings', 'dynamic_preferences.types', 'FilePreference', 'guardian.admin', 'GuardedModelAdmin', 'guardian.core', 'ObjectPermissionChecker', 'jsonstore.fields', 'IntegerField', 'JSONFieldMixin', 'material.base', 'Fieldset', 'Layout', 'LayoutNode', 'polymorphic.base', 'PolymorphicModelBase', 'polymorphic.managers', 'PolymorphicManager', 'polymorphic.models', 'PolymorphicModel', 'rules.contrib.admin', 'ObjectPermissionsModelAdmin', 'aleksis.core.managers', 'CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet', 'base', 'ModelBase', '_ExtensibleModelBase', '_generate_one_to_one_proxy_property', 'Model', 'ExtensibleModel', '_ExtensiblePolymorphicModelBase', 'ExtensiblePolymorphicModel', 'object', 'PureDjangoModel', 'GlobalPermissionModel', '_ExtensibleFormMetaclass', 'ExtensibleForm', 'BaseModelAdmin', 'SuccessMessageMixin', 'SuccessNextMixin', 'AdvancedCreateView', 'AdvancedEditView', 'AdvancedDeleteView', 'SchoolTermRelatedExtensibleModel', 'SchoolTermRelatedExtensibleForm', 'PublicFilePreferenceMixin', 'RegistryObject')
+   names      ('os', 'datetime', 'typing', 'Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union', 'django.conf', 'settings', 'django.contrib', 'messages', 'django.contrib.auth.views', 'LoginView', 'RedirectURLMixin', 'django.contrib.contenttypes.models', 'ContentType', 'django.contrib.sites.managers', 'CurrentSiteManager', 'django.contrib.sites.models', 'Site', 'django.db', 'models', 'django.db.models', 'JSONField', 'QuerySet', 'django.db.models.fields', 'CharField', 'TextField', 'django.forms.forms', 'BaseForm', 'django.forms.models', 'ModelForm', 'ModelFormMetaclass', 'fields_for_model', 'django.http', 'HttpResponse', 'django.utils.functional', 'classproperty', 'lazy', 'django.utils.translation', 'gettext', '_', 'django.views.generic', 'CreateView', 'UpdateView', 'django.views.generic.edit', 'DeleteView', 'ModelFormMixin', 'reversion', 'dynamic_preferences.settings', 'preferences_settings', 'dynamic_preferences.types', 'FilePreference', 'guardian.admin', 'GuardedModelAdmin', 'guardian.core', 'ObjectPermissionChecker', 'jsonstore.fields', 'IntegerField', 'JSONFieldMixin', 'material.base', 'Fieldset', 'Layout', 'LayoutNode', 'polymorphic.base', 'PolymorphicModelBase', 'polymorphic.managers', 'PolymorphicManager', 'polymorphic.models', 'PolymorphicModel', 'rules.contrib.admin', 'ObjectPermissionsModelAdmin', 'aleksis.core.managers', 'CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet', 'base', 'ModelBase', '_ExtensibleModelBase', '_generate_one_to_one_proxy_property', 'Model', 'ExtensibleModel', '_ExtensiblePolymorphicModelBase', 'ExtensiblePolymorphicModel', 'object', 'PureDjangoModel', 'GlobalPermissionModel', '_ExtensibleFormMetaclass', 'ExtensibleForm', 'BaseModelAdmin', 'SuccessMessageMixin', 'SuccessNextMixin', 'AdvancedCreateView', 'AdvancedEditView', 'AdvancedDeleteView', 'SchoolTermRelatedExtensibleModel', 'SchoolTermRelatedExtensibleForm', 'PublicFilePreferenceMixin', 'RegistryObject')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020308010c0120020c010c0110010c010c010c010c01100110010c
-      0110010c0110010c011001100208010c010c010c010c01100114010c010c
+      0114010c0110010c011001100208010c010c010c010c01100114010c010c
       010c010c021407301406162a7f007f00231e040a0106ff120c1c06260b1c
       10202c1e061c091c071e041e041c131c121c111c0b
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 51781
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 13478
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 692
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 16018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 39943
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/admin.py` & `aleksis_core-3.1.4/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/apps.py` & `aleksis_core-3.1.4/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/celery.py` & `aleksis_core-3.1.4/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/checks.py` & `aleksis_core-3.1.4/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/data_checks.py` & `aleksis_core-3.1.4/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/decorators.py` & `aleksis_core-3.1.4/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/filters.py` & `aleksis_core-3.1.4/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/forms.py` & `aleksis_core-3.1.4/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/app/apollo.js` & `aleksis_core-3.1.4/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-3.1.4/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-3.1.4/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-3.1.4/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-3.1.4/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/index.js` & `aleksis_core-3.1.4/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/messages/de.json` & `aleksis_core-3.1.4/aleksis/core/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/messages/en.json` & `aleksis_core-3.1.4/aleksis/core/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/messages/ru.json` & `aleksis_core-3.1.4/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/messages/uk.json` & `aleksis_core-3.1.4/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-3.1.4/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-3.1.4/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/frontend/routes.js` & `aleksis_core-3.1.4/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/health_checks.py` & `aleksis_core-3.1.4/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.4/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-3.1.4/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/management/commands/vite.py` & `aleksis_core-3.1.4/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/managers.py` & `aleksis_core-3.1.4/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0001_initial.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-3.1.4/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/mixins.py` & `aleksis_core-3.1.4/aleksis/core/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.sites.managers import CurrentSiteManager
 from django.contrib.sites.models import Site
 from django.db import models
 from django.db.models import JSONField, QuerySet
 from django.db.models.fields import CharField, TextField
 from django.forms.forms import BaseForm
-from django.forms.models import ModelForm, ModelFormMetaclass
+from django.forms.models import ModelForm, ModelFormMetaclass, fields_for_model
 from django.http import HttpResponse
 from django.utils.functional import classproperty, lazy
 from django.utils.translation import gettext as _
 from django.views.generic import CreateView, UpdateView
 from django.views.generic.edit import DeleteView, ModelFormMixin
 
 import reversion
```

### Comparing `aleksis_core-3.1.3/aleksis/core/models.py` & `aleksis_core-3.1.4/aleksis/core/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/preferences.py` & `aleksis_core-3.1.4/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/registries.py` & `aleksis_core-3.1.4/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/rules.py` & `aleksis_core-3.1.4/aleksis/core/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/__init__.py` & `aleksis_core-3.1.4/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/base.py` & `aleksis_core-3.1.4/aleksis/core/schema/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/celery_progress.py` & `aleksis_core-3.1.4/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/custom_menu.py` & `aleksis_core-3.1.4/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/group.py` & `aleksis_core-3.1.4/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/installed_apps.py` & `aleksis_core-3.1.4/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/notification.py` & `aleksis_core-3.1.4/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/oauth.py` & `aleksis_core-3.1.4/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/pdf.py` & `aleksis_core-3.1.4/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/person.py` & `aleksis_core-3.1.4/aleksis/core/schema/person.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/search.py` & `aleksis_core-3.1.4/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/site_preferences.py` & `aleksis_core-3.1.4/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/system_properties.py` & `aleksis_core-3.1.4/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/two_factor.py` & `aleksis_core-3.1.4/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/schema/user.py` & `aleksis_core-3.1.4/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/settings.py` & `aleksis_core-3.1.4/aleksis/core/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-3.1.4/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/fallback.png` & `aleksis_core-3.1.4/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/img/hero.svg` & `aleksis_core-3.1.4/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-3.1.4/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/helper.js` & `aleksis_core-3.1.4/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-3.1.4/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/main.js` & `aleksis_core-3.1.4/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/multi_select.js` & `aleksis_core-3.1.4/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/search.js` & `aleksis_core-3.1.4/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/js/serviceworker.js` & `aleksis_core-3.1.4/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/print.css` & `aleksis_core-3.1.4/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-3.1.4/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/public/style.scss` & `aleksis_core-3.1.4/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/static/public/theme.scss` & `aleksis_core-3.1.4/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tables.py` & `aleksis_core-3.1.4/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tasks.py` & `aleksis_core-3.1.4/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/403.html` & `aleksis_core-3.1.4/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/404.html` & `aleksis_core-3.1.4/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/500.html` & `aleksis_core-3.1.4/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-3.1.4/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_change.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_change_disabled.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_change_disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/signup.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-3.1.4/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/components/chips.html` & `aleksis_core-3.1.4/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/components/pagination.html` & `aleksis_core-3.1.4/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/additional_field/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/additional_field/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/base.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/base_print.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/group/edit.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/group/full.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/group/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/group_type/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/group_type/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/index.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/perms/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/person/create.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/person/edit.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/person/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/school_term/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/school_term/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/core/vue_index.html` & `aleksis_core-3.1.4/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-3.1.4/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-3.1.4/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-3.1.4/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/invitations/enter.html` & `aleksis_core-3.1.4/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-3.1.4/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-3.1.4/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-3.1.4/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-3.1.4/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-3.1.4/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-3.1.4/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/offline.html` & `aleksis_core-3.1.4/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/search/search.html` & `aleksis_core-3.1.4/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-3.1.4/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/base.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/email.css` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-3.1.4/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-3.1.4/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-3.1.4/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-3.1.4/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-3.1.4/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/models/test.pdf` & `aleksis_core-3.1.4/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/models/test_group.py` & `aleksis_core-3.1.4/aleksis/core/tests/models/test_group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-3.1.4/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/models/test_notification.py` & `aleksis_core-3.1.4/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-3.1.4/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-3.1.4/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-3.1.4/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-3.1.4/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/tests/views/test_account.py` & `aleksis_core-3.1.4/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/urls.py` & `aleksis_core-3.1.4/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 10969
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 16042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 3732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 5583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-3.1.4/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0fe8b664 (Tue Jul 18 19:29:19 2023 UTC)
+moddate:  0xea6db964 (Thu Jul 20 17:24:58 2023 UTC)
 files sz: 130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.3/aleksis/core/util/apps.py` & `aleksis_core-3.1.4/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/auth_helpers.py` & `aleksis_core-3.1.4/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/celery_progress.py` & `aleksis_core-3.1.4/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/core_helpers.py` & `aleksis_core-3.1.4/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/email.py` & `aleksis_core-3.1.4/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/forms.py` & `aleksis_core-3.1.4/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/frontend_helpers.py` & `aleksis_core-3.1.4/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/ldap.py` & `aleksis_core-3.1.4/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/licenses.json` & `aleksis_core-3.1.4/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/messages.py` & `aleksis_core-3.1.4/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/middlewares.py` & `aleksis_core-3.1.4/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/model_helpers.py` & `aleksis_core-3.1.4/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/notifications.py` & `aleksis_core-3.1.4/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/pdf.py` & `aleksis_core-3.1.4/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/predicates.py` & `aleksis_core-3.1.4/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/sass_helpers.py` & `aleksis_core-3.1.4/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/search.py` & `aleksis_core-3.1.4/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/util/tables.py` & `aleksis_core-3.1.4/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/views.py` & `aleksis_core-3.1.4/aleksis/core/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/aleksis/core/vite.config.js` & `aleksis_core-3.1.4/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/Makefile` & `aleksis_core-3.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/2fa.png` & `aleksis_core-3.1.4/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/accept_invite.png` & `aleksis_core-3.1.4/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/create_dashboard_widget.png` & `aleksis_core-3.1.4/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/create_social_application.png` & `aleksis_core-3.1.4/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/dashboard.png` & `aleksis_core-3.1.4/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/dashboard_widgets.png` & `aleksis_core-3.1.4/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/data_checks.png` & `aleksis_core-3.1.4/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/edit_dashboard.png` & `aleksis_core-3.1.4/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/edit_default_dashboard.png` & `aleksis_core-3.1.4/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/invitations.png` & `aleksis_core-3.1.4/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/invite_existing.png` & `aleksis_core-3.1.4/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-3.1.4/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-3.1.4/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-3.1.4/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/pwa_mobile_safari.png` & `aleksis_core-3.1.4/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/_static/signup.png` & `aleksis_core-3.1.4/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/01_core_concepts.rst` & `aleksis_core-3.1.4/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/10_install.rst` & `aleksis_core-3.1.4/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/15_config_files.rst` & `aleksis_core-3.1.4/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/16_config_options.rst` & `aleksis_core-3.1.4/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/17_storage.rst` & `aleksis_core-3.1.4/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/18_mail.rst` & `aleksis_core-3.1.4/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/21_ldap.rst` & `aleksis_core-3.1.4/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/22_registration.rst` & `aleksis_core-3.1.4/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/23_socialaccounts.rst` & `aleksis_core-3.1.4/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/31_monitoring.rst` & `aleksis_core-3.1.4/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/32_tasks.rst` & `aleksis_core-3.1.4/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/33_data_checks.rst` & `aleksis_core-3.1.4/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/admin/50_dashboard.rst` & `aleksis_core-3.1.4/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/conf.py` & `aleksis_core-3.1.4/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-Core"
 copyright = "2019-2023 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.1"
 # The full version, including alpha/beta/rc tags
-release = "3.1.3"
+release = "3.1.4"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_core-3.1.3/docs/dev/01_setup.rst` & `aleksis_core-3.1.4/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/dev/02_install_apps.rst` & `aleksis_core-3.1.4/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/dev/03_run_tests.rst` & `aleksis_core-3.1.4/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/dev/04_materialize_templates.rst` & `aleksis_core-3.1.4/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/dev/06_merging_app_settings.rst` & `aleksis_core-3.1.4/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-3.1.4/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/index.rst` & `aleksis_core-3.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/make.bat` & `aleksis_core-3.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/ref/core/09_utils.rst` & `aleksis_core-3.1.4/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/user/01_registration.rst` & `aleksis_core-3.1.4/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/user/02_personal_account.rst` & `aleksis_core-3.1.4/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/user/10_dashboard.rst` & `aleksis_core-3.1.4/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/docs/user/20_pwa.rst` & `aleksis_core-3.1.4/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/pyproject.toml` & `aleksis_core-3.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "3.1.3"
+version = "3.1.4"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_core-3.1.3/tox.ini` & `aleksis_core-3.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.3/PKG-INFO` & `aleksis_core-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-core
-Version: 3.1.3
+Version: 3.1.4
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
```

