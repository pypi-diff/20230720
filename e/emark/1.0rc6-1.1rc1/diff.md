# Comparing `tmp/emark-1.0rc6.tar.gz` & `tmp/emark-1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emark-1.0rc6.tar", last modified: Tue Apr 25 15:25:13 2023, max compression
+gzip compressed data, was "emark-1.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `emark-1.0rc6.tar` & `emark-1.1rc1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0     1518 2023-04-25 15:24:45.038876 emark-1.0rc6/LICENSE
--rw-r--r--   0        0        0     4038 2023-04-25 15:24:45.038876 emark-1.0rc6/README.md
--rw-r--r--   0        0        0      152 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/__init__.py
--rw-r--r--   0        0        0      158 2023-04-25 15:25:13.895214 emark-1.0rc6/emark/_version.py
--rw-r--r--   0        0        0      281 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/conf.py
--rw-r--r--   0        0        0     6550 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/message.py
--rw-r--r--   0        0        0     2414 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/base.html
--rw-r--r--   0        0        0     1081 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/license.txt
--rw-r--r--   0        0        0     5822 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/styles.css
--rw-r--r--   0        0        0     3780 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/utils.py
--rw-r--r--   0        0        0     2257 2023-04-25 15:24:45.038876 emark-1.0rc6/pyproject.toml
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 emark-1.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-07-20 14:33:00.770370 emark-1.1rc1/LICENSE
+-rw-r--r--   0        0        0     5944 2023-07-20 14:33:00.770370 emark-1.1rc1/README.md
+-rw-r--r--   0        0        0      152 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-20 14:33:46.338776 emark-1.1rc1/emark/_version.py
+-rw-r--r--   0        0        0     2244 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/backends.py
+-rw-r--r--   0        0        0     1030 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/buildapi.py
+-rw-r--r--   0        0        0      309 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/conf.py
+-rw-r--r--   0        0        0      535 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9005 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/message.py
+-rw-r--r--   0        0        0     3474 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/migrations/__init__.py
+-rw-r--r--   0        0        0     2238 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/models.py
+-rw-r--r--   0        0        0     3259 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/base.html
+-rw-r--r--   0        0        0     1081 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/license.txt
+-rw-r--r--   0        0        0     5945 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/templates/emark/styles.css
+-rw-r--r--   0        0        0      325 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/urls.py
+-rw-r--r--   0        0        0     3796 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/utils.py
+-rw-r--r--   0        0        0     2343 2023-07-20 14:33:00.770370 emark-1.1rc1/emark/views.py
+-rw-r--r--   0        0        0     2302 2023-07-20 14:33:00.770370 emark-1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 emark-1.1rc1/PKG-INFO
```

### Comparing `emark-1.0rc6/LICENSE` & `emark-1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `emark-1.0rc6/README.md` & `emark-1.1rc1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Markdown template based HTML and text emails for Django.
 
 * simple email templates with markdown
 * support for HTML and text emails
 * i18n support
 * built-in UTM tracking
+* built-in sent, open and click tracking
 * automatic CSS inliner via [premailer](https://github.com/peterbe/premailer/)
 
 [![PyPi Version](https://img.shields.io/pypi/v/emark.svg)](https://pypi.python.org/pypi/emark/)
 [![Test Coverage](https://codecov.io/gh/voiio/emark/branch/main/graph/badge.svg)](https://codecov.io/gh/voiio/emark)
 [![GitHub License](https://img.shields.io/github/license/voiio/emark)](https://raw.githubusercontent.com/voiio/emark/master/LICENSE)
 
 ## Setup
@@ -112,30 +113,88 @@
         context = super().get_context_data()
         context["my_variable"] = "Hello World"
         return context
 ```
 
 ### Tracking
 
+#### Sent, Open & Click Tracking
+
+Django eMark comes with built-in tracking for sent, open and click events.
+The tracking is done via a tracking pixel and a redirect view.
+
+As an added bonus, this feature also comes with an open-in-browser link that
+allows the user to view the email in their browser if their email client does
+not support HTML emails.
+
+This feature is disabled by default. To enable it, you need to use a separate email
+backend. This backend will send the email via SMTP and also add the tracking
+pixel and redirect view. However, it will send a separate email for each
+recipient, which may not be desirable in all cases.
+
+```python
+# settings.py
+EMAIL_BACKEND = "emark.backends.TrackingSMTPEmailBackend"
+```
+
+Furthermore, you need to add the tracking view to your `urls.py`:
+
+```python
+# urls.py
+from django.urls import include, path
+
+urlpatterns = [
+    # … other urls
+    path("emark/", include("emark.urls")),
+]
+```
+
+You will need to provide a domain name for the tracking pixel and redirect view.
+This can be done via the `DOMAIN` setting:
+
+```python
+# settings.py
+EMARK = {
+    "DOMAIN": "example.com"
+}
+```
+
+If the site framework is installed and no settings are provided,
+the domain will be automatically set to the current site's domain.
+
+The tracking data is stored in the database. You need to run migrations to
+create the necessary tables:
+
+```ShellSession
+python3 manage.py migrate
+```
+
+You can analyze the tracking data via the tables `emark_sent`, `emark_open` and
+`emark_click`.
+
+#### UTM Tracking
+
 Every `MarkdownEmail` subclass comes with automatic UTM tracking.
 UTM parameters are added to all links in the email. Existing UTM params on link
 that have been explicitly set, are not overridden. The default parameters are:
 
 * `utm_source`: `website`
 * `utm_medium`: `email`
 * `utm_campaign`: `{{ EMAIL_CLASS_NAME }}`
 
 The global UTM parameters can be overridden via the `EMARK_UTM_PARAMS` setting,
 which is a dictionary of parameters:
 
 ```python
 # settings.py
-EMARK_UTM_PARAMS = {
-    "utm_source": "website",  # default
-    "utm_medium": "email",  # default
+EMARK = {
+  "UTM_PARAMS": {
+      "utm_source": "website",  # default
+      "utm_medium": "email",  # default
+  }
 }
 ```
 
 You may also change the UTM parameters by overriding the `get_utm_params`
 or passing a `utm_params` dictionary to class constructor.
 
 ```python
@@ -156,11 +215,23 @@
     }
 
 
 # or alternatively during instantiation
 MyMessage(utm_params={"utm_campaign": "my-other-campaign"}).send()
 ```
 
+## Development
+
+Pretty HTML emails are great, unless they spam your console during development.
+To prevent this, you can use the `ConsoleEmailBackend`:
+
+```python
+# settings.py
+EMAIL_BACKEND = "emark.backends.ConsoleEmailBackend"
+```
+
+The `ConsoleEmailBackend` will only print the plain text version of the email.
+
 ## Credits
 
 - Django eMark uses modified version of [Responsive HTML Email Template](https://github.com/leemunroe/responsive-html-email-template/) as a base template
 - For CSS inlining, Django eMark uses [premailer](https://github.com/peterbe/premailer/)
```

### Comparing `emark-1.0rc6/emark/message.py` & `emark-1.1rc1/emark/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 import logging
 import re
 from urllib import parse
 
 import markdown
 import premailer
+from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.core.mail import EmailMultiAlternatives
 from django.template import loader
+from django.urls import reverse
 from django.utils import translation
 from django.utils.safestring import mark_safe
+from django.utils.text import capfirst
+from django.utils.translation import gettext
 
 from emark import conf, utils
 
 INLINE_LINK_RE = re.compile(r"\[[^\]]+\]\(([^)]+)\)")
 INLINE_HTML_LINK_RE = re.compile(r"href=\"([^\"]+)\"")
 CLS_NAME_TO_CAMPAIGN_RE = re.compile(
     r".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)"
@@ -35,86 +39,115 @@
     text body, which extracts a Gmail style plain text version of the fully rendered
     HTML email.
     """
 
     base_html_template = "emark/base.html"
     template = None
     subject = None
+    _tracking_uuid = False
 
     def __init__(
         self,
         language: str,
         subject: str = "",
         context: dict = None,
         utm_params=None,
         template=None,
         **kwargs,
     ):
         """Initialize an email message and attach a rendered HTML version of it."""
-        template = template or self.get_template()
+        self.template = template or self.template
         self.context = context or {}
         self.language = language
-        utm_params = utm_params or {}
+        self.utm_params = utm_params or {}
+        self.subject = subject or self.subject
+        super().__init__(subject=self.subject, **kwargs)
+
+    def get_html(self):
+        """Return the rendered HTML version of the email."""
+        with translation.override(self.language):
+            utm_params = self.get_utm_params()
+            context = self.get_context_data(**utm_params)
+            context |= utm_params
+            template = self.get_template()
+            subject = self.get_subject(**context)
 
-        context = self.get_context_data(**self.context)
-        context |= self.get_utm_params(**utm_params)
-
-        with translation.override(language):
-            subject = subject or self.get_subject(**context)
             markdown_string = self.get_markdown_string(template, context, utm_params)
 
-            self.html = self.render_html(
+            return self.render_html(
                 markdown_string=markdown_string,
                 context={
                     "subject": subject,
                     **context,
                 },
             )
 
-            parser = utils.HTML2TextParser()
-            parser.feed(self.html)
-            lines = str(parser).split("\n")
-            body = "\n".join(lines[1:]).strip()  # remove logo
-            super().__init__(subject=subject, body=body, **kwargs)
-            self.attach_alternative(self.html, "text/html")
+    def get_body(self, html):
+        """Return the parsed plain text version of the rendered HTML email."""
+        parser = utils.HTML2TextParser()
+        parser.feed(html)
+        parser.close()
+        body = str(parser)
+        if self._tracking_uuid:
+            href = reverse("emark:email-detail", kwargs={"pk": self._tracking_uuid})
+            href = parse.urljoin(self.get_site_url(), href)
+            txt = capfirst(gettext("view in browser"))
+            body = f"{txt} <{href}>\n\n" + body
+        return body
+
+    def message(self):
+        # The connection will call .message while sending the email.
+        self.subject = self.get_subject(**self.get_context_data())
+        self.html = self.get_html()
+        self.body = self.get_body(self.html)
+        self.attach_alternative(self.html, "text/html")
+        return super().message()
 
-    @classmethod
-    def get_utm_params(cls, **params: {str: str}) -> {str: str}:
+    def get_utm_params(self, **params: {str: str}) -> {str: str}:
         """Return a dictionary of UTM parameters."""
         return (
             conf.get_settings().UTM_PARAMS
             | {
-                "utm_campaign": cls.get_utm_campaign_name(),
+                "utm_campaign": self.get_utm_campaign_name(),
             }
+            | self.utm_params
             | params
         )
 
     @classmethod
     def get_utm_campaign_name(cls):
         """Return the UTM campaign name for this email."""
         return "_".join(
             (m.group(0) for m in CLS_NAME_TO_CAMPAIGN_RE.finditer(cls.__qualname__))
         ).upper()
 
-    @staticmethod
-    def update_url_params(url, **params):
-        url_parse = parse.urlparse(url)
-        url_params = dict(parse.parse_qsl(url_parse.query))
+    def update_url_params(self, url, **params):
+        """Add UTM parameters to a URL and add the click tracking URL."""
+        redirect_url_parts = parse.urlparse(url)
+        url_params = dict(parse.parse_qsl(redirect_url_parts.query))
         params.update(url_params)
         url_new_query = parse.urlencode(params)
-        url_parse = url_parse._replace(query=url_new_query)
-        return parse.urlunparse(url_parse)
+        redirect_url_parts = redirect_url_parts._replace(query=url_new_query)
+        redirect_url = parse.urlunparse(redirect_url_parts)
+        if not self._tracking_uuid:
+            return redirect_url
+        tracking_url = reverse("emark:email-click", kwargs={"pk": self._tracking_uuid})
+        tracking_url = parse.urljoin(self.get_site_url(), tracking_url)
+        tracking_url_parts = parse.urlparse(tracking_url)
+        tracking_url_parts = tracking_url_parts._replace(
+            query=parse.urlencode({"url": redirect_url})
+        )
+        return parse.urlunparse(tracking_url_parts)
 
-    @classmethod
-    def set_utm_attributes(cls, md, **utm):
+    def set_utm_attributes(self, md, **utm):
         for url in INLINE_LINK_RE.findall(md):
-            md = md.replace(f"({url})", f"({cls.update_url_params(url, **utm)})")
+            md = md.replace(f"({url})", f"({self.update_url_params(url, **utm)})")
         for url in INLINE_HTML_LINK_RE.findall(md):
             md = md.replace(
-                f'href="{url}"', f'href="{cls.update_url_params(url, **utm)}"'
+                f'href="{url}"', f'href="{self.update_url_params(url, **utm)}"'
             )
         return md
 
     @classmethod
     def to_user(cls, user=None, context=None, language=None, **kwargs):
         """Return email with user specific language, context and recipient."""
         if not user.email:
@@ -130,48 +163,71 @@
                     " you must provide a language."
                 ) from e
         context = context or {}
         context |= {
             "short_name": user.get_short_name(),
             "user": user,
         }
-        return cls(
+        obj = cls(
             **{
                 "to": [f'"{user.get_full_name()}" <{user.email}>'],
                 "context": context,
                 "language": language,
             }
             | kwargs
         )
+        obj.user = user
+        return obj
 
     def get_template(self):
         if not self.template:
             raise ImproperlyConfigured(
                 f"{self.__class__.__qualname__} is missing a template."
             )
         return self.template
 
+    def get_site_url(self):
+        protocol = "https" if settings.SECURE_SSL_REDIRECT else "http"
+        if domain := conf.get_settings().DOMAIN:
+            pass
+        elif apps.is_installed("django.contrib.sites"):
+            from django.contrib.sites.models import Site
+
+            domain = Site.objects.get_current().domain
+
+        return parse.urlunparse((protocol, domain, "", "", "", ""))
+
     def get_context_data(self, **context):
         """Return the context data for the email."""
+        if self._tracking_uuid:
+            context |= {
+                "tracking_uuid": self._tracking_uuid,
+                "view_in_browser_url": parse.urljoin(
+                    self.get_site_url(),
+                    reverse("emark:email-detail", kwargs={"pk": self._tracking_uuid}),
+                ),
+                "tracking_pixel_url": parse.urljoin(
+                    self.get_site_url(),
+                    reverse("emark:email-open", kwargs={"pk": self._tracking_uuid}),
+                ),
+            }
+
         return self.context | context
 
     def get_subject(self, **context):
         """Return the email's subject."""
         if not self.subject:
             raise ImproperlyConfigured(
                 f"{self.__class__.__qualname__} is missing a subject."
             )
         return self.subject
 
     def get_markdown_string(self, template, context, utm):
         markdown_string = loader.get_template(template).render(context)
-        markdown_string = self.set_utm_attributes(
-            markdown_string, **self.get_utm_params(**utm)
-        )
-        return markdown_string
+        return self.set_utm_attributes(markdown_string, **self.get_utm_params(**utm))
 
     def render_html(self, markdown_string, context):
         html_message = markdown.markdown(
             markdown_string,
             extensions=[
                 "markdown.extensions.meta",
                 "markdown.extensions.tables",
```

### Comparing `emark-1.0rc6/emark/templates/emark/license.txt` & `emark-1.1rc1/emark/templates/emark/license.txt`

 * *Files identical despite different names*

### Comparing `emark-1.0rc6/emark/templates/emark/styles.css` & `emark-1.1rc1/emark/templates/emark/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
   border-radius: 3px;
   width: 100%;
 }
 
 .wrapper {
   box-sizing: border-box;
   padding: 20px;
+  padding-top: 10px; /* accommodate view-in-browser url */
 }
 
 .content-block {
   padding-bottom: 10px;
   padding-top: 10px;
 }
 
@@ -298,14 +299,19 @@
   table.body .img-responsive {
     height: auto !important;
     max-width: 100% !important;
     width: auto !important;
   }
 }
 
+/* Emark tracking */
+.open-in-browser {
+  text-align: right;
+}
+
 /* -------------------------------------
     PRESERVE THESE STYLES IN THE HEAD
 ------------------------------------- */
 @media all {
   .ExternalClass {
     width: 100%;
   }
```

### Comparing `emark-1.0rc6/emark/utils.py` & `emark-1.1rc1/emark/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,11 +115,11 @@
         """Add text as a leave to the current node."""
         if self.root:
             self.root.children.append(data)
 
     def __str__(self) -> str:
         # remove leading/trailing whitespace
         lines = str(self.root).strip().split("\n")
-        text = "\n".join(line.strip() for line in lines)
+        text = "\n".join(line.strip().strip("\ufeff") for line in lines)
         # sanitize all wide vertical or horizontal spaces
         text = self.DOUBLE_NEWLINE.sub("\n\n", text.strip())
         return self.DOUBLE_SPACE.sub(" ", text)
```

### Comparing `emark-1.0rc6/pyproject.toml` & `emark-1.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 requires = ["flit_core>=3.2", "flit_scm", "wheel"]
-build-backend = "flit_scm:buildapi"
+build-backend = "buildapi"
+backend-path = ["emark"]
 
 [project]
 name = "emark"
 authors = [
   { name = "Rust Saiargaliev", email = "fly.amureki@gmail.com" },
   { name = "Johannes Maron", email = "johannes@maron.family" },
   { name = "Mostafa Mohamed", email = "mostafa.anm91@gmail.com" },
@@ -28,16 +29,16 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 requires-python = ">=3.10"
 dependencies = ["django", "markdown", "premailer"]
 
 [project.optional-dependencies]
 test = [
   "pytest",
@@ -60,14 +61,15 @@
 minversion = "6.0"
 addopts = "--cov --tb=short -rxs"
 testpaths = ["tests"]
 DJANGO_SETTINGS_MODULE = "tests.testapp.settings"
 
 [tool.coverage.run]
 source = ["emark"]
+omit = ["emark/buildapi.py"]
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.isort]
 atomic = true
 line_length = 88
```

### Comparing `emark-1.0rc6/PKG-INFO` & `emark-1.1rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emark
-Version: 1.0rc6
+Version: 1.1rc1
 Summary: Markdown template based HTML and text emails for Django.
 Keywords: Markdown,Django,email,templates,HTML
 Author-email: Rust Saiargaliev <fly.amureki@gmail.com>, Johannes Maron <johannes@maron.family>, Mostafa Mohamed <mostafa.anm91@gmail.com>, Jacqueline Kraus <jacquelinekraus1992@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Dist: django
 Requires-Dist: markdown
 Requires-Dist: premailer
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: model_bakery ; extra == "test"
@@ -42,14 +42,15 @@
 
 Markdown template based HTML and text emails for Django.
 
 * simple email templates with markdown
 * support for HTML and text emails
 * i18n support
 * built-in UTM tracking
+* built-in sent, open and click tracking
 * automatic CSS inliner via [premailer](https://github.com/peterbe/premailer/)
 
 [![PyPi Version](https://img.shields.io/pypi/v/emark.svg)](https://pypi.python.org/pypi/emark/)
 [![Test Coverage](https://codecov.io/gh/voiio/emark/branch/main/graph/badge.svg)](https://codecov.io/gh/voiio/emark)
 [![GitHub License](https://img.shields.io/github/license/voiio/emark)](https://raw.githubusercontent.com/voiio/emark/master/LICENSE)
 
 ## Setup
@@ -150,30 +151,88 @@
         context = super().get_context_data()
         context["my_variable"] = "Hello World"
         return context
 ```
 
 ### Tracking
 
+#### Sent, Open & Click Tracking
+
+Django eMark comes with built-in tracking for sent, open and click events.
+The tracking is done via a tracking pixel and a redirect view.
+
+As an added bonus, this feature also comes with an open-in-browser link that
+allows the user to view the email in their browser if their email client does
+not support HTML emails.
+
+This feature is disabled by default. To enable it, you need to use a separate email
+backend. This backend will send the email via SMTP and also add the tracking
+pixel and redirect view. However, it will send a separate email for each
+recipient, which may not be desirable in all cases.
+
+```python
+# settings.py
+EMAIL_BACKEND = "emark.backends.TrackingSMTPEmailBackend"
+```
+
+Furthermore, you need to add the tracking view to your `urls.py`:
+
+```python
+# urls.py
+from django.urls import include, path
+
+urlpatterns = [
+    # … other urls
+    path("emark/", include("emark.urls")),
+]
+```
+
+You will need to provide a domain name for the tracking pixel and redirect view.
+This can be done via the `DOMAIN` setting:
+
+```python
+# settings.py
+EMARK = {
+    "DOMAIN": "example.com"
+}
+```
+
+If the site framework is installed and no settings are provided,
+the domain will be automatically set to the current site's domain.
+
+The tracking data is stored in the database. You need to run migrations to
+create the necessary tables:
+
+```ShellSession
+python3 manage.py migrate
+```
+
+You can analyze the tracking data via the tables `emark_sent`, `emark_open` and
+`emark_click`.
+
+#### UTM Tracking
+
 Every `MarkdownEmail` subclass comes with automatic UTM tracking.
 UTM parameters are added to all links in the email. Existing UTM params on link
 that have been explicitly set, are not overridden. The default parameters are:
 
 * `utm_source`: `website`
 * `utm_medium`: `email`
 * `utm_campaign`: `{{ EMAIL_CLASS_NAME }}`
 
 The global UTM parameters can be overridden via the `EMARK_UTM_PARAMS` setting,
 which is a dictionary of parameters:
 
 ```python
 # settings.py
-EMARK_UTM_PARAMS = {
-    "utm_source": "website",  # default
-    "utm_medium": "email",  # default
+EMARK = {
+  "UTM_PARAMS": {
+      "utm_source": "website",  # default
+      "utm_medium": "email",  # default
+  }
 }
 ```
 
 You may also change the UTM parameters by overriding the `get_utm_params`
 or passing a `utm_params` dictionary to class constructor.
 
 ```python
@@ -194,12 +253,24 @@
     }
 
 
 # or alternatively during instantiation
 MyMessage(utm_params={"utm_campaign": "my-other-campaign"}).send()
 ```
 
+## Development
+
+Pretty HTML emails are great, unless they spam your console during development.
+To prevent this, you can use the `ConsoleEmailBackend`:
+
+```python
+# settings.py
+EMAIL_BACKEND = "emark.backends.ConsoleEmailBackend"
+```
+
+The `ConsoleEmailBackend` will only print the plain text version of the email.
+
 ## Credits
 
 - Django eMark uses modified version of [Responsive HTML Email Template](https://github.com/leemunroe/responsive-html-email-template/) as a base template
 - For CSS inlining, Django eMark uses [premailer](https://github.com/peterbe/premailer/)
```

