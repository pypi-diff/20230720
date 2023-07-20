# Comparing `tmp/elefanto_webkassa-0.3.2.tar.gz` & `tmp/elefanto_webkassa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.3.2.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.4.0.tar", max compression
```

## Comparing `elefanto_webkassa-0.3.2.tar` & `elefanto_webkassa-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.3.2/README.md
--rw-r--r--   0        0        0      847 2023-07-20 07:05:06.132583 elefanto_webkassa-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.3.2/webkassa/__init__.py
--rw-r--r--   0        0        0     5375 2023-07-20 06:48:17.909994 elefanto_webkassa-0.3.2/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.3.2/webkassa/apps.py
--rw-r--r--   0        0        0     3528 2023-07-20 06:28:21.251072 elefanto_webkassa-0.3.2/webkassa/forms.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.3.2/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0      469 2023-07-19 10:03:59.733639 elefanto_webkassa-0.3.2/webkassa/migrations/0002_check_order_number.py
--rw-r--r--   0        0        0      352 2023-07-20 07:04:33.293265 elefanto_webkassa-0.3.2/webkassa/migrations/0003_remove_webkassaaccount_is_encrypted_and_more.py
--rw-r--r--   0        0        0      576 2023-07-20 06:19:53.245544 elefanto_webkassa-0.3.2/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.3.2/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     3011 2023-07-20 06:19:38.493854 elefanto_webkassa-0.3.2/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.3.2/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.3.2/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6749 2023-07-19 10:12:09.547417 elefanto_webkassa-0.3.2/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.3.2/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0     2065 2023-07-20 05:53:08.519354 elefanto_webkassa-0.3.2/webkassa/templates/change_password_template.html
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.4.0/README.md
+-rw-r--r--   0        0        0      873 2023-07-20 07:48:35.465180 elefanto_webkassa-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      568 2023-07-20 07:40:50.490900 elefanto_webkassa-0.4.0/webkassa/__init__.py
+-rw-r--r--   0        0        0     5375 2023-07-20 06:48:17.909994 elefanto_webkassa-0.4.0/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.4.0/webkassa/apps.py
+-rw-r--r--   0        0        0     3528 2023-07-20 06:28:21.251072 elefanto_webkassa-0.4.0/webkassa/forms.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.4.0/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0      469 2023-07-19 10:03:59.733639 elefanto_webkassa-0.4.0/webkassa/migrations/0002_check_order_number.py
+-rw-r--r--   0        0        0      352 2023-07-20 07:04:33.293265 elefanto_webkassa-0.4.0/webkassa/migrations/0003_remove_webkassaaccount_is_encrypted_and_more.py
+-rw-r--r--   0        0        0      576 2023-07-20 06:19:53.245544 elefanto_webkassa-0.4.0/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.4.0/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     3011 2023-07-20 06:19:38.493854 elefanto_webkassa-0.4.0/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.4.0/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.4.0/webkassa/services/__init__.py
+-rw-r--r--   0        0        0      777 2023-07-20 07:41:00.042700 elefanto_webkassa-0.4.0/webkassa/services/cron.py
+-rw-r--r--   0        0        0     6749 2023-07-20 07:28:50.118110 elefanto_webkassa-0.4.0/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.4.0/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      328 2023-07-20 07:48:06.765779 elefanto_webkassa-0.4.0/webkassa/settings.py
+-rw-r--r--   0        0        0     2068 2023-07-20 07:17:01.685713 elefanto_webkassa-0.4.0/webkassa/templates/change_password_template.html
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 elefanto_webkassa-0.4.0/PKG-INFO
```

### Comparing `elefanto_webkassa-0.3.2/pyproject.toml` & `elefanto_webkassa-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 django = "^4.0.0"
 cryptography = "^41.0.2"
 httpx = "^0.24.1"
 djangorestframework = "^3.14.0"
+django-crontab = "^0.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
 flake8-quotes = "^3.3.2"
```

### Comparing `elefanto_webkassa-0.3.2/webkassa/admin.py` & `elefanto_webkassa-0.4.0/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/forms.py` & `elefanto_webkassa-0.4.0/webkassa/forms.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.4.0/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py` & `elefanto_webkassa-0.4.0/webkassa/migrations/0004_alter_webkassaaccount_email_and_more.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/models.py` & `elefanto_webkassa-0.4.0/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/serializers.py` & `elefanto_webkassa-0.4.0/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/services/manager.py` & `elefanto_webkassa-0.4.0/webkassa/services/manager.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.3.2/webkassa/templates/change_password_template.html` & `elefanto_webkassa-0.4.0/webkassa/templates/change_password_template.html`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {% if is_popup %}<input type="hidden" name="{{ is_popup_var }}" value="1">{% endif %}
 {% if form.errors %}
     <p class="errornote">
     {% blocktranslate count counter=form.errors.items|length %}Please correct the error below.{% plural %}Please correct the errors below.{% endblocktranslate %}
     </p>
 {% endif %}
 
-<p>{% blocktranslate with username=original %}Enter a new password for the user <strong>{{ username }}</strong>.{% endblocktranslate %}</p>
+<p>{% blocktranslate with username=original %}Enter a new password for the account <strong>{{ username }}</strong>.{% endblocktranslate %}</p>
 
 <fieldset class="module aligned">
 
 <div class="form-row">
   {{ form.password.errors }}
   <div class="flex-container">{{ form.password.label_tag }} {{ form.password }}</div>
   {% if form.password.help_text %}
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 {% endblock %} {% endif %} {% block content %}
 % if form_url %} action="{{ form_url }}"{% endif %} method="post" id="{
 { opts.model_name }}_form">{% csrf_token %}{% block form_top %}{% endblock %}
 {% if is_popup %}{% endif %} {% if form.errors %}
 {% blocktranslate count counter=form.errors.items|length %}Please correct the
 error below.{% plural %}Please correct the errors below.{% endblocktranslate %}
 {% endif %}
-{% blocktranslate with username=original %}Enter a new password for the user {
-{ username }}.{% endblocktranslate %}
+{% blocktranslate with username=original %}Enter a new password for the account
+{{ username }}.{% endblocktranslate %}
 {{ form.password.errors }}
 {{ form.password.label_tag }} {{ form.password }}
 {% if form.password.help_text %}
 % if form.password.id_for_label %} id="{{ form.password.id_for_label
 }}_helptext">{% endif %}{{ form.password.help_text|safe }}
 {% endif %}
 [{% translate 'Change password' %}]
```

