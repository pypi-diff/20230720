# Comparing `tmp/django-reactor-5.2.0b0.tar.gz` & `tmp/django-reactor-5.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reactor-5.2.0b0.tar", last modified: Thu Jul 13 13:01:45 2023, max compression
+gzip compressed data, was "django-reactor-5.3.0b0.tar", last modified: Thu Jul 20 13:00:16 2023, max compression
```

## Comparing `django-reactor-5.2.0b0.tar` & `django-reactor-5.3.0b0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       65 2023-06-13 10:33:48.000000 django-reactor-5.2.0b0/MANIFEST.in
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17423 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16564 2023-07-11 15:11:18.000000 django-reactor-5.2.0b0/README.md
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.592571 django-reactor-5.2.0b0/django_reactor.egg-info/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17423 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/django_reactor.egg-info/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      800 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/django_reactor.egg-info/SOURCES.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/django_reactor.egg-info/dependency_links.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.2.0b0/django_reactor.egg-info/not-zip-safe
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/django_reactor.egg-info/requires.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/django_reactor.egg-info/top_level.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.2.0b0/pyproject.toml
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.2.0b0/reactor/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.2.0b0/reactor/apps.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.2.0b0/reactor/auto_broadcast.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13891 2023-07-11 13:13:59.000000 django-reactor-5.2.0b0/reactor/component.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6427 2023-07-12 12:45:39.000000 django-reactor-5.2.0b0/reactor/consumer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3958 2023-07-07 13:06:43.000000 django-reactor-5.2.0b0/reactor/event_transpiler.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.2.0b0/reactor/log.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3930 2023-07-11 13:05:45.000000 django-reactor-5.2.0b0/reactor/repository.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.2.0b0/reactor/schemas.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-30 09:52:16.000000 django-reactor-5.2.0b0/reactor/serializer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.2.0b0/reactor/settings.py
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.592571 django-reactor-5.2.0b0/reactor/static/
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/reactor/static/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2886 2023-07-11 14:28:47.000000 django-reactor-5.2.0b0/reactor/static/reactor/reactor-boost.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     8895 2023-07-11 14:43:33.000000 django-reactor-5.2.0b0/reactor/static/reactor/reactor.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    21384 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/reactor/static/reactor/reactor.min.js
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    83825 2023-07-13 13:01:45.000000 django-reactor-5.2.0b0/reactor/static/reactor/reactor.min.js.map
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/reactor/templates/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.2.0b0/reactor/templates/reactor_header.html
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/reactor/templatetags/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.2.0b0/reactor/templatetags/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3727 2023-07-11 13:13:27.000000 django-reactor-5.2.0b0/reactor/templatetags/reactor.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.2.0b0/reactor/urls.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2950 2023-07-12 12:56:18.000000 django-reactor-5.2.0b0/reactor/utils.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-07-13 13:01:45.595904 django-reactor-5.2.0b0/setup.cfg
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.2.0b0/setup.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       65 2023-06-13 10:33:48.000000 django-reactor-5.3.0b0/MANIFEST.in
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17536 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16677 2023-07-19 12:51:05.000000 django-reactor-5.3.0b0/README.md
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.035996 django-reactor-5.3.0b0/django_reactor.egg-info/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    17536 2023-07-20 13:00:16.000000 django-reactor-5.3.0b0/django_reactor.egg-info/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      800 2023-07-20 13:00:16.000000 django-reactor-5.3.0b0/django_reactor.egg-info/SOURCES.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-07-20 13:00:16.000000 django-reactor-5.3.0b0/django_reactor.egg-info/dependency_links.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.3.0b0/django_reactor.egg-info/not-zip-safe
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-07-20 13:00:16.000000 django-reactor-5.3.0b0/django_reactor.egg-info/requires.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-07-20 13:00:16.000000 django-reactor-5.3.0b0/django_reactor.egg-info/top_level.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.3.0b0/pyproject.toml
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.3.0b0/reactor/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.3.0b0/reactor/apps.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.3.0b0/reactor/auto_broadcast.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    14072 2023-07-19 20:43:31.000000 django-reactor-5.3.0b0/reactor/component.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     7071 2023-07-19 21:49:25.000000 django-reactor-5.3.0b0/reactor/consumer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3958 2023-07-07 13:06:43.000000 django-reactor-5.3.0b0/reactor/event_transpiler.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.3.0b0/reactor/log.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     4191 2023-07-19 21:49:39.000000 django-reactor-5.3.0b0/reactor/repository.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.3.0b0/reactor/schemas.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-30 09:52:16.000000 django-reactor-5.3.0b0/reactor/serializer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.3.0b0/reactor/settings.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.035996 django-reactor-5.3.0b0/reactor/static/
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/reactor/static/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3073 2023-07-20 06:44:22.000000 django-reactor-5.3.0b0/reactor/static/reactor/reactor-boost.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     9301 2023-07-20 11:49:34.000000 django-reactor-5.3.0b0/reactor/static/reactor/reactor.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    23900 2023-07-20 13:00:15.000000 django-reactor-5.3.0b0/reactor/static/reactor/reactor.min.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    94438 2023-07-20 13:00:15.000000 django-reactor-5.3.0b0/reactor/static/reactor/reactor.min.js.map
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/reactor/templates/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      282 2023-07-19 10:11:13.000000 django-reactor-5.3.0b0/reactor/templates/reactor_header.html
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/reactor/templatetags/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.3.0b0/reactor/templatetags/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3561 2023-07-19 21:50:07.000000 django-reactor-5.3.0b0/reactor/templatetags/reactor.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.3.0b0/reactor/urls.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3158 2023-07-19 13:21:26.000000 django-reactor-5.3.0b0/reactor/utils.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-07-20 13:00:16.039329 django-reactor-5.3.0b0/setup.cfg
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.3.0b0/setup.py
```

### Comparing `django-reactor-5.2.0b0/PKG-INFO` & `django-reactor-5.3.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.2.0b0
+Version: 5.3.0b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -80,20 +80,20 @@
 
 Note: Reactor since version 2, autoloads any `live.py` file in your applications with the hope to find there Reactor Components so they get registered and can be instantiated.
 
 In the templates where you want to use reactive components you have to load the reactor static files. So do something like this so the right JavaScript gets loaded:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    ... {% reactor_header %}
-  </head>
-  ...
+    <head>
+        ... {% reactor_header %}
+    </head>
+    ...
 </html>
 ```
 
 Don't worry if you put this as early as possible, the scripts are loaded using `<script defer>` so they will be downloaded in parallel with the html, and when all is loaded they are executed.
 
 ## Simple example of a counter
 
@@ -143,25 +143,25 @@
     return render(request, 'index.html')
 ```
 
 And the index template being:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    .... {% reactor_header %}
-  </head>
-  <body>
-    {% component 'XCounter' %}
-
-    <!-- or passing an initial state -->
-    {% component 'XCounter' amount=100 %}
-  </body>
+    <head>
+        .... {% reactor_header %}
+    </head>
+    <body>
+        {% component 'XCounter' %}
+
+        <!-- or passing an initial state -->
+        {% component 'XCounter' amount=100 %}
+    </body>
 </html>
 ```
 
 Don't forget to update your `urls.py` to call the index view.
 
 ### Persisting the state of the Counter in the URL as a GET parameter
 
@@ -188,15 +188,14 @@
 
 This will make that everytime that method gets called the query string on the browser will get updated to include "query=blahblah". Never replace the `self.reactor.params`, mutate it instead.
 
 Here is another example, suppose you have a list of items that can be expanded, like nodes in a tree view:
 
 ```python
 class Node(Component):
-    _extends = "li"
     name: str
     expanded: bool = False
 
     @classmethod
     def new(cls, reactor: ReactorMeta, id: str, **kwargs):
         kwargs["expanded"] = id in reactor.params.get("expanded.json", [])
         return cls(reactor=reactor, id=id, **kwargs)
@@ -239,28 +238,28 @@
         # this is a set of tuples of ('app_label', 'ModelName')
         # to subscribe for the auto broadcast
         senders: set[tuple[str, str]] = Field(default_factory=set)
     ),
 }
 ```
 
-- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
-- `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
-- `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
+-   `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
+-   `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
+-   `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
+-   `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
-- `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
-- `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
-- `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
-- `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
-- `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
+-   `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
+-   `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
+-   `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
+-   `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
+-   `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
 
 ## Component live cycle
 
 ### Initialization & Rendering
 
 This happens when in a "normal" template you include a component.
 
@@ -280,93 +279,93 @@
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
-- In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
+-   In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
+-   In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
-- `_template_name`: Contains the path of the template of the component.
-- `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
+-   `_template_name`: Contains the path of the template of the component.
+-   `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 
 #### Subscriptions
 
-- `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
-- `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
+-   `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
+-   `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+-   `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
-- `destroy()`: Removes the component from the interface.
-- `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `skip_render()`: Prevents the component from being rendered once.
-- `send_render()`: Send a signal to request render the component ahead of time.
-- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
-- `freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
-- `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
-- `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
+-   `destroy()`: Removes the component from the interface.
+-   `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
+-   `skip_render()`: Prevents the component from being rendered once.
+-   `send_render()`: Send a signal to request render the component ahead of time.
+-   `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+-   `freeze()`: Prevents the component from being rendered again.
+-   `deffer(f, *args, **kwargs)`: Send a message to the current event to be executed after the current function is executed.
+-   `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
+-   `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
+-   `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
+-   `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
-- `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
+-   `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
 
 Look at this:
 
 ```html
   <button {% on "click.prevent" "submit" %}>Submit</button>
 ```
 
 Syntax: {% on <event-and-modifiers> <event-handler> [<event-handler-arguments-as-kwargs>] %}
 The format for event and modifiers is `@<event>[.modifier1][.modifier2][.modifier2-argument1][.modifier2-argument2]`
 
 Examples:
 
-- `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
-- `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
+-   `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
+-   `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
 
 Misc:
 
-- `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
-- `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
+-   `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
+-   `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
 
-  Available modifiers are:
+    Available modifiers are:
 
-  - `inlinejs`: takes the next "event handler" argument as literal JS code.
-  - `prevent`: calls `event.preventDefault()`
-  - `stop`: calls `event.StopPropagation()`
-  - `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
-  - `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
-  - `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
-  - `enter`: alias for `key.enter`
-  - `tab`: alias for `key.tab`
-  - `delete`: alias for `key.delete`
-  - `backspace`: alias for `key.backspace`
-  - `space`: alias for `key. `
-  - `up`: alias for `key.arrowup`
-  - `down`: alias for `key.arrowdown`
-  - `left`: alias for `key.arrowleft`
-  - `right`: alias for `key.arrowright`
+    -   `inlinejs`: takes the next "event handler" argument as literal JS code.
+    -   `prevent`: calls `event.preventDefault()`
+    -   `stop`: calls `event.StopPropagation()`
+    -   `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
+    -   `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
+    -   `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
+    -   `enter`: alias for `key.enter`
+    -   `tab`: alias for `key.tab`
+    -   `delete`: alias for `key.delete`
+    -   `backspace`: alias for `key.backspace`
+    -   `space`: alias for `key. `
+    -   `up`: alias for `key.arrowup`
+    -   `down`: alias for `key.arrowdown`
+    -   `left`: alias for `key.arrowleft`
+    -   `right`: alias for `key.arrowright`
 
 #### Event arguments
 
 Reactor sends the implicit arguments you pass on the `on` template tag, but also sends implicit arguments.
 The implicit arguments are taken from the `form` the element handling the event is in or from the whole component otherwise.
 
 Examples:
```

### Comparing `django-reactor-5.2.0b0/README.md` & `django-reactor-5.3.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,20 @@
 
 Note: Reactor since version 2, autoloads any `live.py` file in your applications with the hope to find there Reactor Components so they get registered and can be instantiated.
 
 In the templates where you want to use reactive components you have to load the reactor static files. So do something like this so the right JavaScript gets loaded:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    ... {% reactor_header %}
-  </head>
-  ...
+    <head>
+        ... {% reactor_header %}
+    </head>
+    ...
 </html>
 ```
 
 Don't worry if you put this as early as possible, the scripts are loaded using `<script defer>` so they will be downloaded in parallel with the html, and when all is loaded they are executed.
 
 ## Simple example of a counter
 
@@ -119,25 +119,25 @@
     return render(request, 'index.html')
 ```
 
 And the index template being:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    .... {% reactor_header %}
-  </head>
-  <body>
-    {% component 'XCounter' %}
-
-    <!-- or passing an initial state -->
-    {% component 'XCounter' amount=100 %}
-  </body>
+    <head>
+        .... {% reactor_header %}
+    </head>
+    <body>
+        {% component 'XCounter' %}
+
+        <!-- or passing an initial state -->
+        {% component 'XCounter' amount=100 %}
+    </body>
 </html>
 ```
 
 Don't forget to update your `urls.py` to call the index view.
 
 ### Persisting the state of the Counter in the URL as a GET parameter
 
@@ -164,15 +164,14 @@
 
 This will make that everytime that method gets called the query string on the browser will get updated to include "query=blahblah". Never replace the `self.reactor.params`, mutate it instead.
 
 Here is another example, suppose you have a list of items that can be expanded, like nodes in a tree view:
 
 ```python
 class Node(Component):
-    _extends = "li"
     name: str
     expanded: bool = False
 
     @classmethod
     def new(cls, reactor: ReactorMeta, id: str, **kwargs):
         kwargs["expanded"] = id in reactor.params.get("expanded.json", [])
         return cls(reactor=reactor, id=id, **kwargs)
@@ -215,28 +214,28 @@
         # this is a set of tuples of ('app_label', 'ModelName')
         # to subscribe for the auto broadcast
         senders: set[tuple[str, str]] = Field(default_factory=set)
     ),
 }
 ```
 
-- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
-- `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
-- `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
+-   `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
+-   `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
+-   `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
+-   `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
-- `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
-- `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
-- `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
-- `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
-- `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
+-   `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
+-   `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
+-   `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
+-   `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
+-   `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
 
 ## Component live cycle
 
 ### Initialization & Rendering
 
 This happens when in a "normal" template you include a component.
 
@@ -256,93 +255,93 @@
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
-- In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
+-   In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
+-   In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
-- `_template_name`: Contains the path of the template of the component.
-- `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
+-   `_template_name`: Contains the path of the template of the component.
+-   `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 
 #### Subscriptions
 
-- `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
-- `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
+-   `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
+-   `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+-   `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
-- `destroy()`: Removes the component from the interface.
-- `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `skip_render()`: Prevents the component from being rendered once.
-- `send_render()`: Send a signal to request render the component ahead of time.
-- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
-- `freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
-- `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
-- `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
+-   `destroy()`: Removes the component from the interface.
+-   `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
+-   `skip_render()`: Prevents the component from being rendered once.
+-   `send_render()`: Send a signal to request render the component ahead of time.
+-   `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+-   `freeze()`: Prevents the component from being rendered again.
+-   `deffer(f, *args, **kwargs)`: Send a message to the current event to be executed after the current function is executed.
+-   `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
+-   `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
+-   `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
+-   `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
-- `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
+-   `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
 
 Look at this:
 
 ```html
   <button {% on "click.prevent" "submit" %}>Submit</button>
 ```
 
 Syntax: {% on <event-and-modifiers> <event-handler> [<event-handler-arguments-as-kwargs>] %}
 The format for event and modifiers is `@<event>[.modifier1][.modifier2][.modifier2-argument1][.modifier2-argument2]`
 
 Examples:
 
-- `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
-- `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
+-   `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
+-   `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
 
 Misc:
 
-- `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
-- `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
+-   `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
+-   `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
 
-  Available modifiers are:
+    Available modifiers are:
 
-  - `inlinejs`: takes the next "event handler" argument as literal JS code.
-  - `prevent`: calls `event.preventDefault()`
-  - `stop`: calls `event.StopPropagation()`
-  - `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
-  - `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
-  - `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
-  - `enter`: alias for `key.enter`
-  - `tab`: alias for `key.tab`
-  - `delete`: alias for `key.delete`
-  - `backspace`: alias for `key.backspace`
-  - `space`: alias for `key. `
-  - `up`: alias for `key.arrowup`
-  - `down`: alias for `key.arrowdown`
-  - `left`: alias for `key.arrowleft`
-  - `right`: alias for `key.arrowright`
+    -   `inlinejs`: takes the next "event handler" argument as literal JS code.
+    -   `prevent`: calls `event.preventDefault()`
+    -   `stop`: calls `event.StopPropagation()`
+    -   `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
+    -   `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
+    -   `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
+    -   `enter`: alias for `key.enter`
+    -   `tab`: alias for `key.tab`
+    -   `delete`: alias for `key.delete`
+    -   `backspace`: alias for `key.backspace`
+    -   `space`: alias for `key. `
+    -   `up`: alias for `key.arrowup`
+    -   `down`: alias for `key.arrowdown`
+    -   `left`: alias for `key.arrowleft`
+    -   `right`: alias for `key.arrowright`
 
 #### Event arguments
 
 Reactor sends the implicit arguments you pass on the `on` template tag, but also sends implicit arguments.
 The implicit arguments are taken from the `form` the element handling the event is in or from the whole component otherwise.
 
 Examples:
```

### Comparing `django-reactor-5.2.0b0/django_reactor.egg-info/PKG-INFO` & `django-reactor-5.3.0b0/django_reactor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.2.0b0
+Version: 5.3.0b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -80,20 +80,20 @@
 
 Note: Reactor since version 2, autoloads any `live.py` file in your applications with the hope to find there Reactor Components so they get registered and can be instantiated.
 
 In the templates where you want to use reactive components you have to load the reactor static files. So do something like this so the right JavaScript gets loaded:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    ... {% reactor_header %}
-  </head>
-  ...
+    <head>
+        ... {% reactor_header %}
+    </head>
+    ...
 </html>
 ```
 
 Don't worry if you put this as early as possible, the scripts are loaded using `<script defer>` so they will be downloaded in parallel with the html, and when all is loaded they are executed.
 
 ## Simple example of a counter
 
@@ -143,25 +143,25 @@
     return render(request, 'index.html')
 ```
 
 And the index template being:
 
 ```html
 {% load reactor %}
-<!DOCTYPE html>
+<!doctype html>
 <html>
-  <head>
-    .... {% reactor_header %}
-  </head>
-  <body>
-    {% component 'XCounter' %}
-
-    <!-- or passing an initial state -->
-    {% component 'XCounter' amount=100 %}
-  </body>
+    <head>
+        .... {% reactor_header %}
+    </head>
+    <body>
+        {% component 'XCounter' %}
+
+        <!-- or passing an initial state -->
+        {% component 'XCounter' amount=100 %}
+    </body>
 </html>
 ```
 
 Don't forget to update your `urls.py` to call the index view.
 
 ### Persisting the state of the Counter in the URL as a GET parameter
 
@@ -188,15 +188,14 @@
 
 This will make that everytime that method gets called the query string on the browser will get updated to include "query=blahblah". Never replace the `self.reactor.params`, mutate it instead.
 
 Here is another example, suppose you have a list of items that can be expanded, like nodes in a tree view:
 
 ```python
 class Node(Component):
-    _extends = "li"
     name: str
     expanded: bool = False
 
     @classmethod
     def new(cls, reactor: ReactorMeta, id: str, **kwargs):
         kwargs["expanded"] = id in reactor.params.get("expanded.json", [])
         return cls(reactor=reactor, id=id, **kwargs)
@@ -239,28 +238,28 @@
         # this is a set of tuples of ('app_label', 'ModelName')
         # to subscribe for the auto broadcast
         senders: set[tuple[str, str]] = Field(default_factory=set)
     ),
 }
 ```
 
-- `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
-- `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
-- `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
-- `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
+-   `TRANSPILER_CACHE_SIZE`: this is the size of an LRU dict used to cache javascript event halder transpilations.
+-   `USE_HTML_DIFF`: when enabled uses `difflib` to create diffs to patch the front-end, reducing bandwidth. If disabled it sends the full HTML content every time.
+-   `REACTOR_USE_HMIN`: when enabled and django-hmin is installed will use it to minified the HTML of the components and save bandwidth.
+-   `AUTO_BROADCAST`: Controls which signals are sent to `Component.mutation` when a model is mutated.
 
 ## Back-end APIs
 
 ### Template tags and filters of `reactor` library
 
-- `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
-- `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
-- `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
-- `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
-- `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
+-   `{% reactor_header %}`: that includes the necessary JavaScript to make this library work. ~10Kb of minified JS, compressed with gz or brotli.
+-   `{% component 'Component' param1=1 param2=2 %}`: Renders a component by its name and passing whatever parameters you put there to the `XComponent.new` method that constructs the component instance.
+-   `{% on 'click' 'event_handler' param1=1 param2=2 %}`: Binds an event handler with paramters to some event. Look at [Event binding in the front-end](#event-binding-in-the-front-end)
+-   `cond`: Allows simple conditional presence of a string: `{% cond {'hidden': is_hidden } %}`.
+-   `class`: Use it to handle conditional classes: `<div {% class {'nav_bar': True, 'hidden': is_hidden} %}></div>`.
 
 ## Component live cycle
 
 ### Initialization & Rendering
 
 This happens when in a "normal" template you include a component.
 
@@ -280,93 +279,93 @@
 
 When a component or its parent has joined it can send user events to the client. Using the `on` template tag, this events are sent to the backend and then the componet is rendered again.
 
 ### Subscriptions
 
 Every time a component joins or responds to an event the `Componet._subscriptions` set is reviewed to check if the component subscribes or not to some channel.
 
-- In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
-- In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
+-   In case a mutation in a model occurs `Component.mutation(channel: str, action: reactor.auto_broadcast.Action, instance: Model)` will be called.
+-   In case you broadcast a message using `reactor.component.broadcast(channel, **kwargs)` this message will be sent to any component subscribed to `channel` using the method `Component.notification(channel, **kwargs)`.
 
 ### Disconnection
 
 If the component is destroyed using the `Component.destroy` or just desapears from the front-end it is removed from the backend. If the the websocket closes all components in that connection are removed from the backend and the state of those componets stay just in the front-end in the seralized form awaiting for the front-end to join again.
 
 #### Component API
 
 Each component is a Pydantic model so it can serialize itself. I would advice not to mess with the `__init__` method.
 Instead use the class method `new` to create the instance.
 
 ##### Rendering
 
-- `_extends`: (default: `"div"`) Tag name HTML element the component extends. (Each component is a HTML5 component so it should extend some HTML tag)
-- `_template_name`: Contains the path of the template of the component.
-- `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
+-   `_template_name`: Contains the path of the template of the component.
+-   `_exclude_fields`: (default: `{"user", "reactor"}`) Which fields to exclude from state serialization during rendering
 
 #### Subscriptions
 
-- `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
-- `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
-- `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
+-   `_subscriptions`: (default: `set()`) Defines which channels is this component subscribed to.
+-   `mutation(channel, action, instance)` Called when autobroadcast is enabled and a model you are subscribed to changes.
+-   `notification(channel, **kwargs)` Called when `reactor.component.broadcast(channel, **kwargs)` is used to send an arbitrary notification to components.
 
 #### Actions
 
-- `destroy()`: Removes the component from the interface.
-- `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
-- `skip_render()`: Prevents the component from being rendered once.
-- `send_render()`: Send a signal to request render the component ahead of time.
-- `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
-- `freeze()`: Prevents the component from being rendered again.
-- `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
-- `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
-- `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
-- `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
+-   `destroy()`: Removes the component from the interface.
+-   `focus_on(selector: str)`: Makes the front-end look for that `selector` and run `.focus()` on it.
+-   `skip_render()`: Prevents the component from being rendered once.
+-   `send_render()`: Send a signal to request render the component ahead of time.
+-   `dom(_action: DomAction, id: str, component_or_template, **kwargs)`: Can append, prepend, insert befor or after certain HTMLElement ID in the dom, the component or template, rendered using the `kwargs`.
+-   `freeze()`: Prevents the component from being rendered again.
+-   `deffer(f, *args, **kwargs)`: Send a message to the current event to be executed after the current function is executed.
+-   `reactor.redirect_to(to, **kwargs)`: Changes the URL of the front-end and triggers a page load for that new URL
+-   `reactor.replace_to(to, **kwargs)`: Changes the current URL for another one.
+-   `reactor.push_to(to, **kwargs)`: Changs the URL of the front-end adding a new history entry but does not fetch the new URL from the backend.
+-   `reactor.send(_channel: str, _topic: str, **kwargs)`: Sends a message over a channel.
 
 ## Front-end APIs
 
-- `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
+-   `reactor.send(element, name, args)`: Sends a reactor user event to `element`, where `name` is the event handler and `args` is a JS object containing the implicit arguments of the call.
 
 ### Event binding in the front-end
 
 Look at this:
 
 ```html
   <button {% on "click.prevent" "submit" %}>Submit</button>
 ```
 
 Syntax: {% on <event-and-modifiers> <event-handler> [<event-handler-arguments-as-kwargs>] %}
 The format for event and modifiers is `@<event>[.modifier1][.modifier2][.modifier2-argument1][.modifier2-argument2]`
 
 Examples:
 
-- `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
-- `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
+-   `{% on "click.ctrl" "decrement" %}>`: Clicking with Ctrl pressed calls "decrement".
+-   `{% on "click" "increment" amount=1 %}>`: Clicking calls "increment" passing `amount=1` as argument.
 
 Misc:
 
-- `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
-- `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
+-   `event`: is the name of the HTMLElement event: `click`, `blur`, `change`, `keypress`, `keyup`, `keydown`...
+-   `modifier`: can be concatenated after the event name and represent actions or conditions to be met before the event execution. This is very similar as [how VueJS does event binding](https://vuejs.org/v2/guide/events.html#Event-Modifiers):
 
-  Available modifiers are:
+    Available modifiers are:
 
-  - `inlinejs`: takes the next "event handler" argument as literal JS code.
-  - `prevent`: calls `event.preventDefault()`
-  - `stop`: calls `event.StopPropagation()`
-  - `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
-  - `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
-  - `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
-  - `enter`: alias for `key.enter`
-  - `tab`: alias for `key.tab`
-  - `delete`: alias for `key.delete`
-  - `backspace`: alias for `key.backspace`
-  - `space`: alias for `key. `
-  - `up`: alias for `key.arrowup`
-  - `down`: alias for `key.arrowdown`
-  - `left`: alias for `key.arrowleft`
-  - `right`: alias for `key.arrowright`
+    -   `inlinejs`: takes the next "event handler" argument as literal JS code.
+    -   `prevent`: calls `event.preventDefault()`
+    -   `stop`: calls `event.StopPropagation()`
+    -   `ctrl`, `alt`, `shift`, `meta`: continues processing the event if any of those keys is pressed
+    -   `debounce`: debounces the event, it needs a delay in milliseconds. Example: `keypress.debounce.100`.
+    -   `key.<keycode>`: continues processing the event if the key with `keycode` is pressed
+    -   `enter`: alias for `key.enter`
+    -   `tab`: alias for `key.tab`
+    -   `delete`: alias for `key.delete`
+    -   `backspace`: alias for `key.backspace`
+    -   `space`: alias for `key. `
+    -   `up`: alias for `key.arrowup`
+    -   `down`: alias for `key.arrowdown`
+    -   `left`: alias for `key.arrowleft`
+    -   `right`: alias for `key.arrowright`
 
 #### Event arguments
 
 Reactor sends the implicit arguments you pass on the `on` template tag, but also sends implicit arguments.
 The implicit arguments are taken from the `form` the element handling the event is in or from the whole component otherwise.
 
 Examples:
```

### Comparing `django-reactor-5.2.0b0/django_reactor.egg-info/SOURCES.txt` & `django-reactor-5.3.0b0/django_reactor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/auto_broadcast.py` & `django-reactor-5.3.0b0/reactor/auto_broadcast.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/component.py` & `django-reactor-5.3.0b0/reactor/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import difflib
 import typing as t
 from asyncio import iscoroutine, iscoroutinefunction
 from functools import reduce
 from uuid import uuid4
 
 from asgiref.sync import async_to_sync
-from channels.db import database_sync_to_async as db
 from channels.layers import BaseChannelLayer
 from django.apps import apps
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.db import models
 from django.http import HttpRequest
 from django.shortcuts import resolve_url  # type: ignore
@@ -17,14 +16,15 @@
 from django.utils.html import format_html
 from django.utils.safestring import SafeString, SafeText, mark_safe
 from pydantic import BaseModel, validate_arguments
 from pydantic.fields import Field, ModelField
 
 from . import settings, utils
 from .schemas import DomAction, ModelAction
+from .utils import db
 
 if settings.USE_HMIN:
     try:
         from hmin.base import html_minify  # type: ignore
     except ImportError as e:
         raise ImportError(
             "If you enable REACTOR['USE_HMIN'] you need to install django-hmin"
@@ -74,20 +74,18 @@
     _last_sent_html: list[str]
 
     def __init__(
         self,
         params: dict[str, t.Any],
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
-        parent_id: str | None = None,
     ):
         self.params = params
         self.channel_name = channel_name
         self.channel_layer = channel_layer
-        self.parent_id = parent_id
         self._is_frozen: bool = False
         self._redirected_to: str | None = None
         self._last_sent_html: list[str] = []
         self._skip_render: bool = False
 
     def clone(self):
         return type(self)(
@@ -187,14 +185,29 @@
             "scroll_into_view",
             id=id,
             behavoir=behavoir,
             block=block,
             inline=inline,
         )
 
+    async def deffer(
+        self,
+        _id: str,
+        _f: t.Callable[P, t.Coroutine],
+        *args: P.args,
+        **kwargs: P.kwargs,
+    ):
+        await self.send(
+            "dispatch_event",
+            command=_f.__name__,
+            id=_id,
+            args=args,
+            kwargs=kwargs,
+        )
+
     async def send(self, _command: str, **kwargs: t.Any):
         if self.channel_name:
             await self.send_to(self.channel_name, _command, **kwargs)
 
     async def send_to(self, _channel: str, _command: str, **kwargs: t.Any):
         if self.channel_layer:
             await self.channel_layer.send(
@@ -260,18 +273,14 @@
 
     _all: dict[str, t.Type["Component"]] = {}
     _urls = {}
     _name: str = ...  # type: ignore
     _template_name: str = ...  # type: ignore
     _templates: dict[str, Template] = {}
     _fqn: str
-    _tag_name: str
-
-    # HTML tag that this component extends
-    _extends = "div"
 
     # fields to exclude from the component state during serialization
     _exclude_fields = {"user", "reactor"}
 
     # Subscriptions: you can define here which channels this component is
     # subscribed to
     _subscriptions: set[str] = set()
@@ -295,19 +304,14 @@
             name = name or cls.__name__
             cls._all[name] = cls
             # Component name
             cls._name = name
             # Fully qualified name
             cls._fqn = f"{cls.__module__}.{name}"
 
-            # Compote a valid HTML tag from the component name
-            name = "".join([("-" + c if c.isupper() else c) for c in name])
-            name = name.strip("-").lower()
-            cls._tag_name = "x-" + name
-
         for attr_name in vars(cls):
             attr = getattr(cls, attr_name)
             if (
                 not attr_name.startswith("_")
                 and attr_name.islower()
                 and callable(attr)
             ):
@@ -341,15 +345,14 @@
         cls,
         _component_name: str,
         state: ComponentState,
         params: dict[str, t.Any],
         user: AnonymousUser | AbstractBaseUser | None = None,
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
-        parent_id: str | None = None,
     ) -> "Component":
         if _component_name not in cls._all:
             raise ComponentNotFound(
                 (
                     f"Could not find requested component '{_component_name}'. "
                     f"Did you load the component?"
                 )
@@ -358,15 +361,14 @@
         # TODO: rename state to initial_state
         instance = cls._all[_component_name].new(
             user=user or AnonymousUser(),
             reactor=ReactorMeta(
                 params=params,
                 channel_name=channel_name,
                 channel_layer=channel_layer,
-                parent_id=parent_id,
             ),
             **state,
         )
         return instance
 
     @classmethod
     def _get_template(cls, template_name: str | None = None) -> Template:
@@ -412,14 +414,25 @@
 
     def skip_render(self):
         self.reactor.skip_render()
 
     def force_render(self):
         self.reactor.force_render()
 
+    async def deffer(
+        self,
+        _f: t.Callable[P, t.Coroutine],
+        *args: P.args,
+        **kwargs: P.kwargs,
+    ):
+        await self.reactor.deffer(self.id, _f, *args, **kwargs)
+
+    def freeze(self):
+        self.reactor.freeze()
+
     async def dom(
         self,
         _action: DomAction,
         _id: str,
         _component_class_or_template_name: t.Type["Component"] | str,
         **kwargs,
     ):
@@ -431,15 +444,19 @@
 
             component = _component_class_or_template_name.new(
                 reactor=self.reactor.clone(),
                 user=self.user,
                 **kwargs,
             )
             html = await db(component._render)(
-                ComponentRepository(user=self.user, params=self.reactor.params)
+                ComponentRepository(
+                    is_live=False,
+                    user=self.user,
+                    params=self.reactor.params,
+                )
             )
         await self.reactor.send_dom_action(_action, _id, html)
 
     # Internal render operations
 
     def _render(self, repo: Repo):
         return self.reactor.render(self, repo)
```

### Comparing `django-reactor-5.2.0b0/reactor/consumer.py` & `django-reactor-5.3.0b0/reactor/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,40 @@
 import logging
 import typing as t
 
 from channels.generic.websocket import AsyncJsonWebsocketConsumer
 from django.contrib.auth.models import AnonymousUser
 from django.core.signing import Signer
 from django.utils.datastructures import MultiValueDict
+
 from reactor.component import Component
 
 from . import serializer
 from .repository import ComponentRepository
 from .utils import parse_request_data
 
 log = logging.getLogger("reactor")
 
 
+class ChildComponent(t.TypedDict):
+    name: str
+    state: str
+
+
 class ReactorConsumer(AsyncJsonWebsocketConsumer):
     @property
     def user(self):
         return self.scope.get("user") or AnonymousUser()
 
     async def connect(self):
         await super().connect()
         self.subscriptions = set()
         self.query_stirng: str = ""
         self.repo = ComponentRepository(
+            is_live=True,
             user=self.user,
             channel_name=self.channel_name,
             channel_layer=self.channel_layer,
         )
 
     # Fronted commands
 
@@ -37,29 +44,35 @@
             **content["payload"]
         )
 
     async def command_join(
         self,
         name: str,
         state: str,
-        parent_id: str | None = None,
+        children: dict[str, ChildComponent] | None = None,
     ):
-        decoded_state: dict[str, t.Any] = json.loads(Signer().unsign(state))
+        signer = Signer()
+        decoded_state: dict[str, t.Any] = json.loads(signer.unsign(state))
+        decoded_children: dict[str, tuple[str, dict[str, t.Any]]] = {
+            id: (name, json.loads(signer.unsign(state)))
+            for id, (name, state) in (children or {}).items()
+        }
         log.debug(f"<<< JOIN {name} {decoded_state}")
         try:
-            component, created = await self.repo.join(
-                name, decoded_state, parent_id=parent_id
+            component = await self.repo.join(
+                name,
+                decoded_state,
+                children=decoded_children,
             )
         except Exception as e:
             log.exception(e)
             if id := decoded_state.get("id"):
                 await self.component_remove(id)
         else:
-            if created:
-                await self.send_render(component)
+            await self.send_render(component)
             await self.after_mutation_schores()
 
     async def command_leave(self, id):
         log.debug(f"<<< LEAVE {id}")
         self.repo.remove(id)
 
     async def command_query_string(self, qs: str):
@@ -69,23 +82,29 @@
     async def command_user_event(
         self, id, command, implicit_args, explicit_args
     ):
         kwargs = dict(
             parse_request_data(MultiValueDict(implicit_args)), **explicit_args
         )
         log.debug(f"<<< USER-EVENT {id} {command} {kwargs}")
-        component = await self.repo.dispatch_event(id, command, kwargs)
+        component = await self.repo.dispatch_event(id, command, [], kwargs)
         await self.send_render(component)
         await self.after_mutation_schores()
 
     # Component commands
 
     async def message_from_component(self, data):
         await getattr(self, f"component_{data['command']}")(**data["kwargs"])
 
+    async def component_dispatch_event(self, id, command, args, kwargs):
+        log.debug(f"<<< EVENT {id} {command} {args} {kwargs}")
+        component = await self.repo.dispatch_event(id, command, args, kwargs)
+        await self.send_render(component)
+        await self.after_mutation_schores()
+
     async def component_remove(self, id):
         log.debug(f">>> REMOVE {id}")
         await self.send_command("remove", {"id": id})
 
     async def component_send_render(self, id):
         log.debug(f">>> SEND-RENDER {id}")
         if component := self.repo.get(id):
```

### Comparing `django-reactor-5.2.0b0/reactor/event_transpiler.py` & `django-reactor-5.3.0b0/reactor/event_transpiler.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/repository.py` & `django-reactor-5.3.0b0/reactor/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 from channels.db import database_sync_to_async as db
 from channels.layers import BaseChannelLayer
 from django.contrib.auth.models import AbstractBaseUser, AnonymousUser
 
 from .component import Component, MessagePayload
 from .utils import filter_parameters
 
+ChildrenRepo = dict[str, tuple[str, dict[str, t.Any]]]
+
 
 class ComponentRepository:
     user: AnonymousUser | AbstractBaseUser
 
     def __init__(
         self,
+        *,
+        is_live: bool,
         user: AnonymousUser | AbstractBaseUser | None = None,
         params: dict[str, t.Any] | None = None,
         channel_name: str | None = None,
         channel_layer: BaseChannelLayer | None = None,
     ):
         self.params = params or {}
         self.channel_name = channel_name
         self.channel_layer = channel_layer
         self.user = user or AnonymousUser()
         self.components: dict[str, Component] = {}
+        self.children: ChildrenRepo = {}
+        self.is_live = is_live
 
     @staticmethod
     def extract_params(qs: str):
         return {
             key: json.loads(value) if key.endswith(".json") else value
             for key, value in parse_qsl(qs)
         }
@@ -52,58 +58,66 @@
             }
         )
 
     def get(self, component_id: str) -> Component | None:
         return self.components.get(component_id)
 
     def build(
-        self, name: str, state: MessagePayload, parent_id: str | None = None
-    ) -> tuple[Component, bool]:
-        if (component_id := state.get("id")) and (
-            component := self.components.get(component_id)
-        ):
-            # override with the passed state but preserve the rest of the state
-            for key, value in state.items():
-                setattr(component, key, value)
-            component.reactor.parent_id = parent_id
-            return component, False
-        else:
-            component = Component._build(
-                name,
-                state,
-                params=self.params,
-                user=self.user,
-                channel_name=self.channel_name,
-                channel_layer=self.channel_layer,
-                parent_id=parent_id,
-            )
-            return self.register_component(component), True
+        self,
+        name: str,
+        state: MessagePayload,
+    ) -> Component:
+        if component_id := state.get("id"):
+            if component := self.components.get(component_id):
+                # override with the passed state but preserve the rest of the state
+                for key, value in state.items():
+                    setattr(component, key, value)
+                return component
+            elif child := self.children.get(component_id):
+                child_name, child_state = child
+                if child_name == name:
+                    state = child_state | state
+                    self.children.pop(component_id)
+
+        component = Component._build(
+            name,
+            state,
+            params=self.params,
+            user=self.user,
+            channel_name=self.channel_name,
+            channel_layer=self.channel_layer,
+        )
+        return self.register_component(component)
 
     async def join(
-        self, name: str, state: MessagePayload, parent_id: str | None = None
-    ) -> tuple[Component, bool]:
-        component, created = await db(self.build)(
-            name, state, parent_id=parent_id
+        self,
+        name: str,
+        state: MessagePayload,
+        children: ChildrenRepo | None = None,
+    ) -> Component:
+        self.children.update(children or {})
+        component = await db(self.build)(
+            name,
+            state,
         )
-        if created:
-            await component.joined()
-        return component, created
+        await component.joined()
+        return component
 
     def register_component(self, component: Component):
         self.components[component.id] = component
         return component
 
     def remove(self, id):
         self.components.pop(id, None)
 
-    async def dispatch_event(self, id, command, kwargs):
+    async def dispatch_event(self, id, command, args, kwargs):
         assert not command.startswith("_")
         component = self.components[id]
         handler = getattr(component, command)
-        await handler(**filter_parameters(handler, kwargs))
+        await handler(*args, **filter_parameters(handler, kwargs))
         return component
 
     def components_subscribed_to(self, channel):
         # XXX: There is a list() here because the dict can change size during
         # iteration
         for component in list(self.components.values()):
             if channel in component._subscriptions:
```

### Comparing `django-reactor-5.2.0b0/reactor/schemas.py` & `django-reactor-5.3.0b0/reactor/schemas.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/serializer.py` & `django-reactor-5.3.0b0/reactor/serializer.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/settings.py` & `django-reactor-5.3.0b0/reactor/settings.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.2.0b0/reactor/static/reactor/reactor-boost.js` & `django-reactor-5.3.0b0/reactor/static/reactor/reactor-boost.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,28 @@
-import morphdom from "morphdom";
+import _load from "idiomorph";
 
 function morph(oldNode, newNode) {
-    morphdom(oldNode, newNode);
+    Idiomorph.morph(oldNode, newNode);
 }
 
 const BOOST_PAGES = JSON.parse(
     document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false"
 );
 
 console.log("BOOST_PAGES", BOOST_PAGES);
 
 class NavEvents extends EventTarget {
-    send() {
+    sendNewLocation() {
         console.log("LOAD", document.location.href);
         this.dispatchEvent(new Event("newLocation"));
     }
+
+    sendNewContent() {
+        this.dispatchEvent(new Event("newContent"));
+    }
 }
 
 let navEvent = new NavEvents();
 
 if (BOOST_PAGES) {
     document.addEventListener("click", (e) => {
         let link = e.target;
@@ -37,20 +41,23 @@
             e.preventDefault();
             HistoryCache.load(link.href);
         }
     });
 }
 
 function replaceBodyContent(newBody, scrollY = undefined) {
-    document.body.innerHTML = newBody;
-    if (scrollY === undefined) {
-        document.querySelector("[autofocus]")?.focus();
-    } else {
-        window.scrollTo(0, scrollY);
-    }
+    window.requestAnimationFrame(() => {
+        morph(document.body, newBody);
+        if (scrollY === undefined) {
+            document.querySelector("[autofocus]")?.focus();
+        } else {
+            window.scrollTo(0, scrollY);
+        }
+        navEvent.sendNewContent();
+    });
 }
 
 function hasSameOriginAsDocument(url) {
     if (url.startsWith("http://") || url.startsWith("https://")) {
         return new URL(url).origin === document.location.origin;
     } else {
         return true;
@@ -74,40 +81,40 @@
     static back() {
         window.history.back();
     }
 
     static async push(path) {
         if (document.body == null) debugger;
         history.replaceState({
-                content: document.body.innerHTML,
+                content: document.body.outerHTML,
                 scrollY: window.scrollY,
             },
             document.title,
             document.location.href
         );
         history.pushState({}, document.title, path);
         this.replaceContentFromUrl(path);
     }
 
     static async replaceContentFromUrl(url) {
-        navEvent.send();
+        navEvent.sendNewLocation();
         let response = await fetch(url);
         let content = await response.text();
         let doc = new DOMParser().parseFromString(content, "text/html");
         document.title = doc.querySelector("title")?.text ?? "";
-        replaceBodyContent(doc.body.innerHTML);
+        replaceBodyContent(doc.body);
     }
 
     static replace(path) {
         history.replaceState({}, document.title, path);
     }
 }
 
 window.addEventListener("popstate", (event) => {
-    navEvent.send();
+    navEvent.sendNewLocation();
     if (event.state?.content !== undefined) {
         replaceBodyContent(event.state.content, event.state.scrollY);
     }
     HistoryCache.replaceContentFromUrl(document.location.href);
 });
 
 export default {
```

### Comparing `django-reactor-5.2.0b0/reactor/static/reactor/reactor.js` & `django-reactor-5.3.0b0/reactor/static/reactor/reactor.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,60 +1,90 @@
 import ReconnectingWebSocket from "reconnecting-websocket";
 import boost from "./reactor-boost";
 
 // Connection
 
 const parser = new DOMParser();
 
-class ServerConnection extends EventTarget {
+class ServerConnection {
+    constructor() {
+        this.components = {};
+    }
+
     open(path = "__reactor__") {
         let protocol = location.protocol.replace("http", "ws");
         this.socket = new ReconnectingWebSocket(
             `${protocol}//${location.host}/${path}`,
             [], {
                 maxEnqueuedMessages: 0,
             }
         );
 
         this.socket.addEventListener("open", () => {
             console.log("WS: OPEN");
             this.sendQueryString();
-            this.dispatchEvent(new Event("open"));
+            this.components = {};
+            this.joinAllComponents();
         });
 
         this.socket.addEventListener("message", (event) =>
             this._processMessage(event)
         );
 
         this.socket.addEventListener("close", () => {
             console.log("WS: CLOSE");
-            this.dispatchEvent(new Event("close"));
+            this.components = {};
+            document.querySelectorAll("[reactor-component]").forEach((element) => {
+                element.classList.add("reactor-disconnected");
+                element.dataset.isLive = "false";
+            });
         });
 
         boost.navEvent.addEventListener("newLocation", () => {
             this.sendQueryString();
         });
+
+        boost.navEvent.addEventListener("newContent", () => {
+            this.joinAllComponents();
+        });
     }
 
     get isOpen() {
         return this.socket?.readyState == ReconnectingWebSocket.OPEN;
     }
 
+    joinAllComponents() {
+        let registeredIds = new Set(Object.keys(this.components));
+        for (let element of document.querySelectorAll("[reactor-component]")) {
+            if (registeredIds.delete(element.id)) {
+                this.components[element.id].join();
+            } else {
+                let component = new ReactorComponent(element.id);
+                this.components[element.id] = component;
+                component.join();
+            }
+        }
+        for (let id of registeredIds.keys()) {
+            delete this.components[id];
+            this.sendLeave(id);
+        }
+    }
+
     _processMessage(event) {
         let {
             command,
             payload
         } = JSON.parse(event.data);
         switch (command) {
             case "render":
                 var {
                     id, diff
                 } = payload;
                 console.log("<<< RENDER", id);
-                document.getElementById(id)?.applyDiff(diff);
+                this.components[id]?.applyDiff(diff);
                 break;
             case "append":
             case "prepend":
             case "insert_after":
             case "insert_before":
             case "replace_with":
                 var {
@@ -77,22 +107,24 @@
                         case "insert_before":
                             element.before(html);
                             break;
                         case "replace_with":
                             boost.morph(element, html);
                             break;
                     }
+                    boost.navEvent.sendNewContent();
                 }
                 break;
             case "remove":
                 var {
                     id
                 } = payload;
                 console.log("<<< REMOVE", id);
                 document.getElementById(id)?.remove();
+                boost.navEvent.sendNewContent();
                 break;
             case "focus_on":
                 var {
                     selector
                 } = payload;
                 console.log(
                     "<<< FOCUS-ON",
@@ -157,20 +189,20 @@
         let qs = document.location.search.slice(1);
         console.log("QS", qs);
         this._send("query_string", {
             qs
         });
     }
 
-    sendJoin(name, component_id, parent_id, state) {
+    sendJoin(name, component_id, state, children) {
         console.log(">>> JOIN", name, component_id);
         this._send("join", {
             name,
-            parent_id,
-            state
+            state,
+            children
         });
     }
 
     sendLeave(id) {
         console.log(">>> LEAVE", id);
         this._send("leave", {
             id
@@ -195,171 +227,147 @@
             }));
         }
     }
 }
 
 let connection = new ServerConnection();
 
-for ({
-        dataset
+class ReactorComponent {
+    /**
+     * Returns the id of the parent component
+     *
+     * @param {HTMLElement} el
+     */
+    constructor(id) {
+        this.id = id;
+        this.lastReceivedHtml = [];
     }
-    of document.querySelectorAll("meta[name=reactor-component]")) {
-    let baseElement = document.createElement(dataset.extends);
-
-    class ReactorComponent extends baseElement.constructor {
-        constructor(...args) {
-            super(...args);
-            this._lastReceivedHtml = [];
-            this.joinBind = () => this.join();
-            this.wentOffline = () => this.classList.add("reactor-disconnected");
-        }
 
-        connectedCallback() {
-            connection.addEventListener("open", this.joinBind);
-            connection.addEventListener("close", this.wentOffline);
-            this.join();
-        }
-
-        disconnectedCallback() {
-            connection.removeEventListener("open", this.joinBind);
-            connection.removeEventListener("close", this.wentOffline);
-            this.leave();
-        }
-
-        join() {
-            this.classList.remove("reactor-disconnected");
-            connection.sendJoin(
-                this.dataset.name,
-                this.id,
-                this.parentId,
-                this.dataset.state
-            );
-        }
-
-        leave() {
-            connection.sendLeave(this.id);
-        }
+    getElemenet() {
+        return document.getElementById(this.id);
+    }
 
-        applyDiff(diff) {
-            window.requestAnimationFrame(() => {
+    applyDiff(diff) {
+        window.requestAnimationFrame(() => {
+            let el = this.getElemenet();
+            if (el) {
                 let html = this.getHtml(diff);
-                boost.morph(this, html);
-            });
-        }
-
-        getHtml(diff) {
-            let fragments = [];
-            let cursor = 0;
-            for (let fragment of diff) {
-                if (typeof fragment === "string") {
-                    fragments.push(fragment);
-                } else if (fragment < 0) {
-                    cursor -= fragment;
-                } else {
-                    fragments.push(
-                        ...this._lastReceivedHtml.slice(cursor, cursor + fragment)
-                    );
-                    cursor += fragment;
-                }
+                boost.morph(el, html);
+                boost.navEvent.sendNewContent();
             }
-            this._lastReceivedHtml = fragments;
-            return fragments.join(" ");
-        }
+        });
+    }
 
-        /**
-         * Returns the id of the parent component
-         *
-         * @returns {?String}
-         */
-        get parentId() {
-            return this.parentComponent?.id;
+    getHtml(diff) {
+        let fragments = [];
+        let cursor = 0;
+        for (let fragment of diff) {
+            if (typeof fragment === "string") {
+                fragments.push(fragment);
+            } else if (fragment < 0) {
+                cursor -= fragment;
+            } else {
+                fragments.push(
+                    ...this.lastReceivedHtml.slice(cursor, cursor + fragment)
+                );
+                cursor += fragment;
+            }
         }
+        this.lastReceivedHtml = fragments;
+        return fragments.join(" ");
+    }
 
-        /**
-         * Returns the high parent reactor component if any is found component
-         *
-         * @returns {?ReactorComponent}
-         */
-        get parentComponent() {
-            return this.parentElement?.closest("[reactor-component]");
+    join() {
+        let element = this.getElemenet();
+        if (element && element.dataset.isLive === "false") {
+            let parent = element?.parentElement?.closest("[reactor-component]");
+            if (!parent || parent.dataset.isLive === "true") {
+                element.dataset.isLive = "true";
+                let children = Array.from(
+                    element.querySelectorAll("[reactor-component]")
+                ).reduce((children, el) => {
+                    children[el.id] = [el.dataset.name, el.dataset.state];
+                    return children;
+                }, {});
+
+                connection.sendJoin(
+                    element.dataset.name,
+                    element.id,
+                    element.dataset.state,
+                    children
+                );
+            }
         }
+    }
 
-        /**
-         * Dispatches a command to this component and sends it to the backend
-         * @param {String} command
-         * @param {Object} args
-         * @param {?HTMLFormElement} form
-         */
-        dispatch(command, args, formScope) {
-            connection.sendUserEvent(
-                this.id,
-                command,
-                this.serialize(formScope),
-                args
-            );
-        }
+    /**
+     * Dispatches a command to this component and sends it to the backend
+     * @param {String} command
+     * @param {Object} args
+     * @param {?HTMLFormElement} form
+     */
+    dispatch(command, args, formScope) {
+        connection.sendUserEvent(this.id, command, this.serialize(formScope), args);
+    }
 
-        /**
-         * Serialize all elements inside `element` with a [name] attribute into
-         * a an array of `[element[name], element[value]]`
-         * @param {HTMLElement} element
-         */
-        serialize(element) {
-            let result = {};
-            for (let el of element.querySelectorAll("[name]")) {
-                // Avoid serializing data of a nested component
-                if (el.closest("[reactor-component]") !== this) {
-                    continue;
-                }
+    /**
+     * Serialize all elements inside `element` with a [name] attribute into
+     * a an array of `[element[name], element[value]]`
+     * @param {HTMLElement} element
+     */
+    serialize(element) {
+        let result = {};
+        let thisElement = this.getElemenet();
+        for (let el of element.querySelectorAll("[name]")) {
+            // Avoid serializing data of a nested component
+            if (el.closest("[reactor-component]") !== thisElement) {
+                continue;
+            }
 
-                let value = null;
-                switch (el.type.toLowerCase()) {
-                    case "checkbox":
-                    case "radio":
-                        value = el.checked ? el.value || true : null;
-                        break;
-                    case "select-multiple":
-                        value = el.selectedOptions.map((option) => option.value);
-                        break;
-                    default:
-                        value = el.value;
-                        break;
-                }
+            let value = null;
+            switch (el.type.toLowerCase()) {
+                case "checkbox":
+                case "radio":
+                    value = el.checked ? el.value || true : null;
+                    break;
+                case "select-multiple":
+                    value = el.selectedOptions.map((option) => option.value);
+                    break;
+                default:
+                    value = el.value;
+                    break;
+            }
 
-                if (value !== null) {
-                    let key = el.getAttribute("name");
-                    let values = result[key] ?? [];
-                    values.push(value);
-                    result[key] = values;
-                }
+            if (value !== null) {
+                let key = el.getAttribute("name");
+                let values = result[key] ?? [];
+                values.push(value);
+                result[key] = values;
             }
-            return result;
         }
+        return result;
     }
-
-    customElements.define(dataset.tagName, ReactorComponent, {
-        extends: dataset.extends,
-    });
 }
 
 connection.open();
 var debounceTimeout = undefined;
 
 window.reactor = {
     /**
      * Forwards a user event to a component
      * @param {HTMLElement} element
      * @param {String} name
      * @param {Object} args
      */
     send(element, name, args) {
-        let component = element.closest("[reactor-component]");
-        if (component !== null) {
+        let component_el = element.closest("[reactor-component]");
+        let component = connection.components[component_el.id];
+        if (component_el !== null && component !== undefined) {
             let form = element.closest("form");
-            let formScope = component.contains(form) ? form : component;
+            let formScope = component_el.contains(form) ? form : component_el;
             component.dispatch(name, args, formScope);
         }
     },
 
     /**
      * Debounce a function call
      * @param {Number} delay
```

### Comparing `django-reactor-5.2.0b0/reactor/static/reactor/reactor.min.js` & `django-reactor-5.3.0b0/reactor/static/reactor/reactor.min.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,371 @@
 (() => {
-    var K = function(t, e) {
-        return K = Object.setPrototypeOf || {
+    var le = Object.create;
+    var P = Object.defineProperty;
+    var ce = Object.getOwnPropertyDescriptor;
+    var ue = Object.getOwnPropertyNames;
+    var de = Object.getPrototypeOf,
+        fe = Object.prototype.hasOwnProperty;
+    var he = t => P(t, "__esModule", {
+        value: !0
+    });
+    var pe = (t, e) => () => (e || t((e = {
+        exports: {}
+    }).exports, e), e.exports);
+    var me = (t, e, n) => {
+            if (e && typeof e == "object" || typeof e == "function")
+                for (let a of ue(e)) !fe.call(t, a) && a !== "default" && P(t, a, {
+                    get: () => e[a],
+                    enumerable: !(n = ce(e, a)) || n.enumerable
+                });
+            return t
+        },
+        _e = t => me(he(P(t != null ? le(de(t)) : {}, "default", t && t.__esModule && "default" in t ? {
+            get: () => t.default,
+            enumerable: !0
+        } : {
+            value: t,
+            enumerable: !0
+        })), t);
+    var V = pe(G => {
+        (function(t, e) {
+            typeof define == "function" && define.amd ? define([], e) : t.Idiomorph = t.Idiomorph || e()
+        })(typeof self != "undefined" ? self : G, function() {
+            return function() {
+                "use strict";
+                let t = new Set;
+
+                function e(r, o, i = {}) {
+                    r instanceof Document && (r = r.documentElement), typeof o == "string" && (o = Z(o));
+                    let l = ee(o),
+                        c = R(r, l, i);
+                    return n(r, l, c)
+                }
+
+                function n(r, o, i) {
+                    if (i.head.block) {
+                        let l = r.querySelector("head"),
+                            c = o.querySelector("head");
+                        if (l && c) {
+                            let u = h(c, l, i);
+                            Promise.all(u).then(function() {
+                                n(r, o, Object.assign(i, {
+                                    head: {
+                                        block: !1,
+                                        ignore: !0
+                                    }
+                                }))
+                            });
+                            return
+                        }
+                    }
+                    if (i.morphStyle === "innerHTML") return s(o, r, i), r.children;
+                    if (i.morphStyle === "outerHTML" || i.morphStyle == null) {
+                        let l = ne(o, r, i),
+                            c = l?.previousSibling,
+                            u = l?.nextSibling,
+                            p = a(r, l, i);
+                        return l ? te(c, p, u) : []
+                    } else throw "Do not understand how to morph style " + i.morphStyle
+                }
+
+                function a(r, o, i) {
+                    if (!(i.ignoreActive && r === document.activeElement)) return o == null ? (i.callbacks.beforeNodeRemoved(r), r.remove(), i.callbacks.afterNodeRemoved(r), null) : E(r, o) ? (i.callbacks.beforeNodeMorphed(r, o), r instanceof HTMLHeadElement && i.head.ignore || (r instanceof HTMLHeadElement && i.head.style !== "morph" ? h(o, r, i) : (d(o, r), s(o, r, i))), i.callbacks.afterNodeMorphed(r, o), r) : (i.callbacks.beforeNodeRemoved(r), i.callbacks.beforeNodeAdded(o), r.parentElement.replaceChild(o, r), i.callbacks.afterNodeAdded(o), i.callbacks.afterNodeRemoved(r), o)
+                }
+
+                function s(r, o, i) {
+                    let l = r.firstChild,
+                        c = o.firstChild;
+                    for (; l;) {
+                        let u = l;
+                        if (l = u.nextSibling, c == null) i.callbacks.beforeNodeAdded(u), o.appendChild(u), i.callbacks.afterNodeAdded(u);
+                        else if (T(u, c, i)) a(c, u, i), c = c.nextSibling;
+                        else {
+                            let p = x(r, o, u, c, i);
+                            if (p) c = w(c, p, i), a(p, u, i);
+                            else {
+                                let y = X(r, o, u, c, i);
+                                y ? (c = w(c, y, i), a(y, u, i)) : (i.callbacks.beforeNodeAdded(u), o.insertBefore(u, c), i.callbacks.afterNodeAdded(u))
+                            }
+                        }
+                        N(i, u)
+                    }
+                    for (; c !== null;) {
+                        let u = c;
+                        c = c.nextSibling, q(u, i)
+                    }
+                }
+
+                function d(r, o) {
+                    let i = r.nodeType;
+                    if (i === 1) {
+                        let l = r.attributes,
+                            c = o.attributes;
+                        for (let u of l) o.getAttribute(u.name) !== u.value && o.setAttribute(u.name, u.value);
+                        for (let u of c) r.hasAttribute(u.name) || o.removeAttribute(u.name)
+                    }
+                    if ((i === 8 || i === 3) && o.nodeValue !== r.nodeValue && (o.nodeValue = r.nodeValue), r instanceof HTMLInputElement && o instanceof HTMLInputElement && r.type !== "file") {
+                        let l = r.value,
+                            c = o.value;
+                        f(r, o, "checked"), f(r, o, "disabled"), r.hasAttribute("value") ? l !== c && (o.setAttribute("value", l), o.value = l) : (o.value = "", o.removeAttribute("value"))
+                    } else if (r instanceof HTMLOptionElement) f(r, o, "selected");
+                    else if (r instanceof HTMLTextAreaElement && o instanceof HTMLTextAreaElement) {
+                        let l = r.value,
+                            c = o.value;
+                        l !== c && (o.value = l), o.firstChild && o.firstChild.nodeValue !== l && (o.firstChild.nodeValue = l)
+                    }
+                }
+
+                function f(r, o, i) {
+                    r[i] !== o[i] && (o[i] = r[i], r[i] ? o.setAttribute(i, "") : o.removeAttribute(i))
+                }
+
+                function h(r, o, i) {
+                    let l = [],
+                        c = [],
+                        u = [],
+                        p = [],
+                        y = i.head.style,
+                        S = new Map;
+                    for (let _ of r.children) S.set(_.outerHTML, _);
+                    for (let _ of o.children) {
+                        let v = S.has(_.outerHTML),
+                            C = i.head.shouldReAppend(_),
+                            I = i.head.shouldPreserve(_);
+                        v || I ? C ? c.push(_) : (S.delete(_.outerHTML), u.push(_)) : y === "append" ? C && (c.push(_), p.push(_)) : i.head.shouldRemove(_) !== !1 && c.push(_)
+                    }
+                    p.push(...S.values()), m("to append: ", p);
+                    let F = [];
+                    for (let _ of p) {
+                        m("adding: ", _);
+                        let v = document.createRange().createContextualFragment(_.outerHTML).firstChild;
+                        if (m(v), i.callbacks.beforeNodeAdded(v) !== !1) {
+                            if (v.href || v.src) {
+                                let C = null,
+                                    I = new Promise(function(ae) {
+                                        C = ae
+                                    });
+                                v.addEventListener("load", function() {
+                                    C()
+                                }), F.push(I)
+                            }
+                            o.appendChild(v), i.callbacks.afterNodeAdded(v), l.push(v)
+                        }
+                    }
+                    for (let _ of c) i.callbacks.beforeNodeRemoved(_) !== !1 && (o.removeChild(_), i.callbacks.afterNodeRemoved(_));
+                    return i.head.afterHeadMorphed(o, {
+                        added: l,
+                        kept: u,
+                        removed: c
+                    }), F
+                }
+
+                function m() {}
+
+                function b() {}
+
+                function R(r, o, i) {
+                    return {
+                        target: r,
+                        newContent: o,
+                        config: i,
+                        morphStyle: i.morphStyle,
+                        ignoreActive: i.ignoreActive,
+                        idMap: se(r, o),
+                        deadIds: new Set,
+                        callbacks: Object.assign({
+                            beforeNodeAdded: b,
+                            afterNodeAdded: b,
+                            beforeNodeMorphed: b,
+                            afterNodeMorphed: b,
+                            beforeNodeRemoved: b,
+                            afterNodeRemoved: b
+                        }, i.callbacks),
+                        head: Object.assign({
+                            style: "merge",
+                            shouldPreserve: function(l) {
+                                return l.getAttribute("im-preserve") === "true"
+                            },
+                            shouldReAppend: function(l) {
+                                return l.getAttribute("im-re-append") === "true"
+                            },
+                            shouldRemove: b,
+                            afterHeadMorphed: b
+                        }, i.head)
+                    }
+                }
+
+                function T(r, o, i) {
+                    return r == null || o == null ? !1 : r.nodeType === o.nodeType && r.tagName === o.tagName ? r.id !== "" && r.id === o.id ? !0 : k(i, r, o) > 0 : !1
+                }
+
+                function E(r, o) {
+                    return r == null || o == null ? !1 : r.nodeType === o.nodeType && r.tagName === o.tagName
+                }
+
+                function w(r, o, i) {
+                    for (; r !== o;) {
+                        let l = r;
+                        r = r.nextSibling, q(l, i)
+                    }
+                    return N(i, o), o.nextSibling
+                }
+
+                function x(r, o, i, l, c) {
+                    let u = k(c, i, o),
+                        p = null;
+                    if (u > 0) {
+                        let y = l,
+                            S = 0;
+                        for (; y != null;) {
+                            if (T(i, y, c)) return y;
+                            if (S += k(c, y, r), S > u) return null;
+                            y = y.nextSibling
+                        }
+                    }
+                    return p
+                }
+
+                function X(r, o, i, l, c) {
+                    let u = l,
+                        p = i.nextSibling,
+                        y = 0;
+                    for (; u != null;) {
+                        if (k(c, u, r) > 0) return null;
+                        if (E(i, u)) return u;
+                        if (E(p, u) && (y++, p = p.nextSibling, y >= 2)) return null;
+                        u = u.nextSibling
+                    }
+                    return u
+                }
+
+                function Z(r) {
+                    let o = new DOMParser,
+                        i = r.replace(/<svg(\s[^>]*>|>)([\s\S]*?)<\/svg>/gim, "");
+                    if (i.match(/<\/html>/) || i.match(/<\/head>/) || i.match(/<\/body>/)) {
+                        let l = o.parseFromString(r, "text/html");
+                        if (i.match(/<\/html>/)) return l.generatedByIdiomorph = !0, l; {
+                            let c = l.firstChild;
+                            return c ? (c.generatedByIdiomorph = !0, c) : null
+                        }
+                    } else {
+                        let c = o.parseFromString("<body><template>" + r + "</template></body>", "text/html").body.querySelector("template").content;
+                        return c.generatedByIdiomorph = !0, c
+                    }
+                }
+
+                function ee(r) {
+                    if (r == null) return document.createElement("div");
+                    if (r.generatedByIdiomorph) return r;
+                    if (r instanceof Node) {
+                        let o = document.createElement("div");
+                        return o.append(r), o
+                    } else {
+                        let o = document.createElement("div");
+                        for (let i of [...r]) o.append(i);
+                        return o
+                    }
+                }
+
+                function te(r, o, i) {
+                    let l = [],
+                        c = [];
+                    for (; r != null;) l.push(r), r = r.previousSibling;
+                    for (; l.length > 0;) {
+                        let u = l.pop();
+                        c.push(u), o.parentElement.insertBefore(u, o)
+                    }
+                    for (c.push(o); i != null;) l.push(i), c.push(i), i = i.nextSibling;
+                    for (; l.length > 0;) o.parentElement.insertBefore(l.pop(), o.nextSibling);
+                    return c
+                }
+
+                function ne(r, o, i) {
+                    let l;
+                    l = r.firstChild;
+                    let c = l,
+                        u = 0;
+                    for (; l;) {
+                        let p = re(l, o, i);
+                        p > u && (c = l, u = p), l = l.nextSibling
+                    }
+                    return c
+                }
+
+                function re(r, o, i) {
+                    return E(r, o) ? .5 + k(i, r, o) : 0
+                }
+
+                function q(r, o) {
+                    N(o, r), o.callbacks.beforeNodeRemoved(r), r.remove(), o.callbacks.afterNodeRemoved(r)
+                }
+
+                function oe(r, o) {
+                    return !r.deadIds.has(o)
+                }
+
+                function ie(r, o, i) {
+                    return (r.idMap.get(i) || t).has(o)
+                }
+
+                function N(r, o) {
+                    let i = r.idMap.get(o) || t;
+                    for (let l of i) r.deadIds.add(l)
+                }
+
+                function k(r, o, i) {
+                    let l = r.idMap.get(o) || t,
+                        c = 0;
+                    for (let u of l) oe(r, u) && ie(r, u, i) && ++c;
+                    return c
+                }
+
+                function U(r, o) {
+                    let i = r.parentElement,
+                        l = r.querySelectorAll("[id]");
+                    for (let c of l) {
+                        let u = c;
+                        for (; u !== i && u != null;) {
+                            let p = o.get(u);
+                            p == null && (p = new Set, o.set(u, p)), p.add(c.id), u = u.parentElement
+                        }
+                    }
+                }
+
+                function se(r, o) {
+                    let i = new Map;
+                    return U(r, i), U(o, i), i
+                }
+                return {
+                    morph: e
+                }
+            }()
+        })
+    });
+    var D = function(t, e) {
+        return D = Object.setPrototypeOf || {
             __proto__: []
         }
-        instanceof Array && function(n, i) {
-            n.__proto__ = i
-        } || function(n, i) {
-            for (var r in i) i.hasOwnProperty(r) && (n[r] = i[r])
-        }, K(t, e)
+        instanceof Array && function(n, a) {
+            n.__proto__ = a
+        } || function(n, a) {
+            for (var s in a) a.hasOwnProperty(s) && (n[s] = a[s])
+        }, D(t, e)
     };
 
-    function re(t, e) {
-        K(t, e);
+    function B(t, e) {
+        D(t, e);
 
         function n() {
             this.constructor = t
         }
         t.prototype = e === null ? Object.create(e) : (n.prototype = e.prototype, new n)
     }
 
-    function ge(t) {
+    function ye(t) {
         var e = typeof Symbol == "function" && t[Symbol.iterator],
             n = 0;
         return e ? e.call(t) : {
             next: function() {
                 return t && n >= t.length && (t = void 0), {
                     value: t && t[n++],
                     done: !t
@@ -31,112 +373,112 @@
             }
         }
     }
 
     function be(t, e) {
         var n = typeof Symbol == "function" && t[Symbol.iterator];
         if (!n) return t;
-        var i = n.call(t),
-            r, o = [],
-            s;
+        var a = n.call(t),
+            s, d = [],
+            f;
         try {
             for (;
-                (e === void 0 || e-- > 0) && !(r = i.next()).done;) o.push(r.value)
-        } catch (l) {
-            s = {
-                error: l
+                (e === void 0 || e-- > 0) && !(s = a.next()).done;) d.push(s.value)
+        } catch (h) {
+            f = {
+                error: h
             }
         } finally {
             try {
-                r && !r.done && (n = i.return) && n.call(i)
+                s && !s.done && (n = a.return) && n.call(a)
             } finally {
-                if (s) throw s.error
+                if (f) throw f.error
             }
         }
-        return o
+        return d
     }
 
-    function we() {
+    function ge() {
         for (var t = [], e = 0; e < arguments.length; e++) t = t.concat(be(arguments[e]));
         return t
     }
-    var ie = function() {
+    var W = function() {
             function t(e, n) {
                 this.target = n, this.type = e
             }
             return t
         }(),
-        Ee = function(t) {
-            re(e, t);
+        ve = function(t) {
+            B(e, t);
 
-            function e(n, i) {
-                var r = t.call(this, "error", i) || this;
-                return r.message = n.message, r.error = n, r
+            function e(n, a) {
+                var s = t.call(this, "error", a) || this;
+                return s.message = n.message, s.error = n, s
             }
             return e
-        }(ie),
-        Se = function(t) {
-            re(e, t);
+        }(W),
+        Ee = function(t) {
+            B(e, t);
 
-            function e(n, i, r) {
-                n === void 0 && (n = 1e3), i === void 0 && (i = "");
-                var o = t.call(this, "close", r) || this;
-                return o.wasClean = !0, o.code = n, o.reason = i, o
+            function e(n, a, s) {
+                n === void 0 && (n = 1e3), a === void 0 && (a = "");
+                var d = t.call(this, "close", s) || this;
+                return d.wasClean = !0, d.code = n, d.reason = a, d
             }
             return e
-        }(ie);
-    var Te = function() {
+        }(W);
+    var we = function() {
             if (typeof WebSocket != "undefined") return WebSocket
         },
-        Oe = function(t) {
+        Se = function(t) {
             return typeof t != "undefined" && !!t && t.CLOSING === 2
         },
-        C = {
+        L = {
             maxReconnectionDelay: 1e4,
             minReconnectionDelay: 1e3 + Math.random() * 4e3,
             minUptime: 5e3,
             reconnectionDelayGrowFactor: 1.3,
             connectionTimeout: 4e3,
             maxRetries: 1 / 0,
             maxEnqueuedMessages: 1 / 0,
             startClosed: !1,
             debug: !1
         },
-        Ce = function() {
-            function t(e, n, i) {
-                var r = this;
-                i === void 0 && (i = {}), this._listeners = {
+        Le = function() {
+            function t(e, n, a) {
+                var s = this;
+                a === void 0 && (a = {}), this._listeners = {
                     error: [],
                     message: [],
                     open: [],
                     close: []
-                }, this._retryCount = -1, this._shouldReconnect = !0, this._connectLock = !1, this._binaryType = "blob", this._closeCalled = !1, this._messageQueue = [], this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this._handleOpen = function(o) {
-                    r._debug("open event");
-                    var s = r._options.minUptime,
-                        l = s === void 0 ? C.minUptime : s;
-                    clearTimeout(r._connectTimeout), r._uptimeTimeout = setTimeout(function() {
-                        return r._acceptOpen()
-                    }, l), r._ws.binaryType = r._binaryType, r._messageQueue.forEach(function(d) {
-                        return r._ws.send(d)
-                    }), r._messageQueue = [], r.onopen && r.onopen(o), r._listeners.open.forEach(function(d) {
-                        return r._callEventListener(o, d)
+                }, this._retryCount = -1, this._shouldReconnect = !0, this._connectLock = !1, this._binaryType = "blob", this._closeCalled = !1, this._messageQueue = [], this.onclose = null, this.onerror = null, this.onmessage = null, this.onopen = null, this._handleOpen = function(d) {
+                    s._debug("open event");
+                    var f = s._options.minUptime,
+                        h = f === void 0 ? L.minUptime : f;
+                    clearTimeout(s._connectTimeout), s._uptimeTimeout = setTimeout(function() {
+                        return s._acceptOpen()
+                    }, h), s._ws.binaryType = s._binaryType, s._messageQueue.forEach(function(m) {
+                        return s._ws.send(m)
+                    }), s._messageQueue = [], s.onopen && s.onopen(d), s._listeners.open.forEach(function(m) {
+                        return s._callEventListener(d, m)
                     })
-                }, this._handleMessage = function(o) {
-                    r._debug("message event"), r.onmessage && r.onmessage(o), r._listeners.message.forEach(function(s) {
-                        return r._callEventListener(o, s)
+                }, this._handleMessage = function(d) {
+                    s._debug("message event"), s.onmessage && s.onmessage(d), s._listeners.message.forEach(function(f) {
+                        return s._callEventListener(d, f)
                     })
-                }, this._handleError = function(o) {
-                    r._debug("error event", o.message), r._disconnect(void 0, o.message === "TIMEOUT" ? "timeout" : void 0), r.onerror && r.onerror(o), r._debug("exec error listeners"), r._listeners.error.forEach(function(s) {
-                        return r._callEventListener(o, s)
-                    }), r._connect()
-                }, this._handleClose = function(o) {
-                    r._debug("close event"), r._clearTimeouts(), r._shouldReconnect && r._connect(), r.onclose && r.onclose(o), r._listeners.close.forEach(function(s) {
-                        return r._callEventListener(o, s)
+                }, this._handleError = function(d) {
+                    s._debug("error event", d.message), s._disconnect(void 0, d.message === "TIMEOUT" ? "timeout" : void 0), s.onerror && s.onerror(d), s._debug("exec error listeners"), s._listeners.error.forEach(function(f) {
+                        return s._callEventListener(d, f)
+                    }), s._connect()
+                }, this._handleClose = function(d) {
+                    s._debug("close event"), s._clearTimeouts(), s._shouldReconnect && s._connect(), s.onclose && s.onclose(d), s._listeners.close.forEach(function(f) {
+                        return s._callEventListener(d, f)
                     })
-                }, this._url = e, this._protocols = n, this._options = i, this._options.startClosed && (this._shouldReconnect = !1), this._connect()
+                }, this._url = e, this._protocols = n, this._options = a, this._options.startClosed && (this._shouldReconnect = !1), this._connect()
             }
             return Object.defineProperty(t, "CONNECTING", {
                 get: function() {
                     return 0
                 },
                 enumerable: !0,
                 configurable: !0
@@ -195,16 +537,16 @@
                 get: function() {
                     return Math.max(this._retryCount, 0)
                 },
                 enumerable: !0,
                 configurable: !0
             }), Object.defineProperty(t.prototype, "bufferedAmount", {
                 get: function() {
-                    var e = this._messageQueue.reduce(function(n, i) {
-                        return typeof i == "string" ? n += i.length : i instanceof Blob ? n += i.size : n += i.byteLength, n
+                    var e = this._messageQueue.reduce(function(n, a) {
+                        return typeof a == "string" ? n += a.length : a instanceof Blob ? n += a.size : n += a.byteLength, n
                     }, 0);
                     return e + (this._ws ? this._ws.bufferedAmount : 0)
                 },
                 enumerable: !0,
                 configurable: !0
             }), Object.defineProperty(t.prototype, "extensions", {
                 get: function() {
@@ -242,55 +584,55 @@
                 this._ws.close(e, n)
             }, t.prototype.reconnect = function(e, n) {
                 this._shouldReconnect = !0, this._closeCalled = !1, this._retryCount = -1, !this._ws || this._ws.readyState === this.CLOSED ? this._connect() : (this._disconnect(e, n), this._connect())
             }, t.prototype.send = function(e) {
                 if (this._ws && this._ws.readyState === this.OPEN) this._debug("send", e), this._ws.send(e);
                 else {
                     var n = this._options.maxEnqueuedMessages,
-                        i = n === void 0 ? C.maxEnqueuedMessages : n;
-                    this._messageQueue.length < i && (this._debug("enqueue", e), this._messageQueue.push(e))
+                        a = n === void 0 ? L.maxEnqueuedMessages : n;
+                    this._messageQueue.length < a && (this._debug("enqueue", e), this._messageQueue.push(e))
                 }
             }, t.prototype.addEventListener = function(e, n) {
                 this._listeners[e] && this._listeners[e].push(n)
             }, t.prototype.dispatchEvent = function(e) {
-                var n, i, r = this._listeners[e.type];
-                if (r) try {
-                    for (var o = ge(r), s = o.next(); !s.done; s = o.next()) {
-                        var l = s.value;
-                        this._callEventListener(e, l)
+                var n, a, s = this._listeners[e.type];
+                if (s) try {
+                    for (var d = ye(s), f = d.next(); !f.done; f = d.next()) {
+                        var h = f.value;
+                        this._callEventListener(e, h)
                     }
-                } catch (d) {
+                } catch (m) {
                     n = {
-                        error: d
+                        error: m
                     }
                 } finally {
                     try {
-                        s && !s.done && (i = o.return) && i.call(o)
+                        f && !f.done && (a = d.return) && a.call(d)
                     } finally {
                         if (n) throw n.error
                     }
                 }
                 return !0
             }, t.prototype.removeEventListener = function(e, n) {
-                this._listeners[e] && (this._listeners[e] = this._listeners[e].filter(function(i) {
-                    return i !== n
+                this._listeners[e] && (this._listeners[e] = this._listeners[e].filter(function(a) {
+                    return a !== n
                 }))
             }, t.prototype._debug = function() {
                 for (var e = [], n = 0; n < arguments.length; n++) e[n] = arguments[n];
-                this._options.debug && console.log.apply(console, we(["RWS>"], e))
+                this._options.debug && console.log.apply(console, ge(["RWS>"], e))
             }, t.prototype._getNextDelay = function() {
                 var e = this._options,
                     n = e.reconnectionDelayGrowFactor,
-                    i = n === void 0 ? C.reconnectionDelayGrowFactor : n,
-                    r = e.minReconnectionDelay,
-                    o = r === void 0 ? C.minReconnectionDelay : r,
-                    s = e.maxReconnectionDelay,
-                    l = s === void 0 ? C.maxReconnectionDelay : s,
-                    d = 0;
-                return this._retryCount > 0 && (d = o * Math.pow(i, this._retryCount - 1), d > l && (d = l)), this._debug("next delay", d), d
+                    a = n === void 0 ? L.reconnectionDelayGrowFactor : n,
+                    s = e.minReconnectionDelay,
+                    d = s === void 0 ? L.minReconnectionDelay : s,
+                    f = e.maxReconnectionDelay,
+                    h = f === void 0 ? L.maxReconnectionDelay : f,
+                    m = 0;
+                return this._retryCount > 0 && (m = d * Math.pow(a, this._retryCount - 1), m > h && (m = h)), this._debug("next delay", m), m
             }, t.prototype._wait = function() {
                 var e = this;
                 return new Promise(function(n) {
                     setTimeout(n, e._getNextDelay())
                 })
             }, t.prototype._getNextUrl = function(e) {
                 if (typeof e == "string") return Promise.resolve(e);
@@ -301,579 +643,359 @@
                 }
                 throw Error("Invalid URL")
             }, t.prototype._connect = function() {
                 var e = this;
                 if (!(this._connectLock || !this._shouldReconnect)) {
                     this._connectLock = !0;
                     var n = this._options,
-                        i = n.maxRetries,
-                        r = i === void 0 ? C.maxRetries : i,
-                        o = n.connectionTimeout,
-                        s = o === void 0 ? C.connectionTimeout : o,
-                        l = n.WebSocket,
-                        d = l === void 0 ? Te() : l;
-                    if (this._retryCount >= r) {
-                        this._debug("max retries reached", this._retryCount, ">=", r);
+                        a = n.maxRetries,
+                        s = a === void 0 ? L.maxRetries : a,
+                        d = n.connectionTimeout,
+                        f = d === void 0 ? L.connectionTimeout : d,
+                        h = n.WebSocket,
+                        m = h === void 0 ? we() : h;
+                    if (this._retryCount >= s) {
+                        this._debug("max retries reached", this._retryCount, ">=", s);
                         return
                     }
-                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Oe(d)) throw Error("No valid WebSocket class provided");
+                    if (this._retryCount++, this._debug("connect", this._retryCount), this._removeListeners(), !Se(m)) throw Error("No valid WebSocket class provided");
                     this._wait().then(function() {
                         return e._getNextUrl(e._url)
-                    }).then(function(_) {
+                    }).then(function(b) {
                         e._closeCalled || (e._debug("connect", {
-                            url: _,
+                            url: b,
                             protocols: e._protocols
-                        }), e._ws = e._protocols ? new d(_, e._protocols) : new d(_), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
+                        }), e._ws = e._protocols ? new m(b, e._protocols) : new m(b), e._ws.binaryType = e._binaryType, e._connectLock = !1, e._addListeners(), e._connectTimeout = setTimeout(function() {
                             return e._handleTimeout()
-                        }, s))
+                        }, f))
                     })
                 }
             }, t.prototype._handleTimeout = function() {
-                this._debug("timeout event"), this._handleError(new Ee(Error("TIMEOUT"), this))
+                this._debug("timeout event"), this._handleError(new ve(Error("TIMEOUT"), this))
             }, t.prototype._disconnect = function(e, n) {
                 if (e === void 0 && (e = 1e3), this._clearTimeouts(), !!this._ws) {
                     this._removeListeners();
                     try {
-                        this._ws.close(e, n), this._handleClose(new Se(e, n, this))
+                        this._ws.close(e, n), this._handleClose(new Ee(e, n, this))
                     } catch {}
                 }
             }, t.prototype._acceptOpen = function() {
                 this._debug("accept open"), this._retryCount = 0
             }, t.prototype._callEventListener = function(e, n) {
                 "handleEvent" in n ? n.handleEvent(e) : n(e)
             }, t.prototype._removeListeners = function() {
                 !this._ws || (this._debug("removeListeners"), this._ws.removeEventListener("open", this._handleOpen), this._ws.removeEventListener("close", this._handleClose), this._ws.removeEventListener("message", this._handleMessage), this._ws.removeEventListener("error", this._handleError))
             }, t.prototype._addListeners = function() {
                 !this._ws || (this._debug("addListeners"), this._ws.addEventListener("open", this._handleOpen), this._ws.addEventListener("close", this._handleClose), this._ws.addEventListener("message", this._handleMessage), this._ws.addEventListener("error", this._handleError))
             }, t.prototype._clearTimeouts = function() {
                 clearTimeout(this._connectTimeout), clearTimeout(this._uptimeTimeout)
             }, t
         }(),
-        $ = Ce;
-    var oe = 11;
-
-    function Le(t, e) {
-        var n = e.attributes,
-            i, r, o, s, l;
-        if (!(e.nodeType === oe || t.nodeType === oe)) {
-            for (var d = n.length - 1; d >= 0; d--) i = n[d], r = i.name, o = i.namespaceURI, s = i.value, o ? (r = i.localName || r, l = t.getAttributeNS(o, r), l !== s && (i.prefix === "xmlns" && (r = i.name), t.setAttributeNS(o, r, s))) : (l = t.getAttribute(r), l !== s && t.setAttribute(r, s));
-            for (var _ = t.attributes, T = _.length - 1; T >= 0; T--) i = _[T], r = i.name, o = i.namespaceURI, o ? (r = i.localName || r, e.hasAttributeNS(o, r) || t.removeAttributeNS(o, r)) : e.hasAttribute(r) || t.removeAttribute(r)
-        }
-    }
-    var j, Ne = "http://www.w3.org/1999/xhtml",
-        v = typeof document == "undefined" ? void 0 : document,
-        xe = !!v && "content" in v.createElement("template"),
-        Ae = !!v && v.createRange && "createContextualFragment" in v.createRange();
-
-    function ke(t) {
-        var e = v.createElement("template");
-        return e.innerHTML = t, e.content.childNodes[0]
-    }
-
-    function Re(t) {
-        j || (j = v.createRange(), j.selectNode(v.body));
-        var e = j.createContextualFragment(t);
-        return e.childNodes[0]
-    }
-
-    function De(t) {
-        var e = v.createElement("body");
-        return e.innerHTML = t, e.childNodes[0]
-    }
-
-    function Ue(t) {
-        return t = t.trim(), xe ? ke(t) : Ae ? Re(t) : De(t)
-    }
-
-    function H(t, e) {
-        var n = t.nodeName,
-            i = e.nodeName,
-            r, o;
-        return n === i ? !0 : (r = n.charCodeAt(0), o = i.charCodeAt(0), r <= 90 && o >= 97 ? n === i.toUpperCase() : o <= 90 && r >= 97 ? i === n.toUpperCase() : !1)
-    }
-
-    function Pe(t, e) {
-        return !e || e === Ne ? v.createElement(t) : v.createElementNS(e, t)
-    }
-
-    function Me(t, e) {
-        for (var n = t.firstChild; n;) {
-            var i = n.nextSibling;
-            e.appendChild(n), n = i
-        }
-        return e
-    }
-
-    function z(t, e, n) {
-        t[n] !== e[n] && (t[n] = e[n], t[n] ? t.setAttribute(n, "") : t.removeAttribute(n))
-    }
-    var se = {
-            OPTION: function(t, e) {
-                var n = t.parentNode;
-                if (n) {
-                    var i = n.nodeName.toUpperCase();
-                    i === "OPTGROUP" && (n = n.parentNode, i = n && n.nodeName.toUpperCase()), i === "SELECT" && !n.hasAttribute("multiple") && (t.hasAttribute("selected") && !e.selected && (t.setAttribute("selected", "selected"), t.removeAttribute("selected")), n.selectedIndex = -1)
-                }
-                z(t, e, "selected")
-            },
-            INPUT: function(t, e) {
-                z(t, e, "checked"), z(t, e, "disabled"), t.value !== e.value && (t.value = e.value), e.hasAttribute("value") || t.removeAttribute("value")
-            },
-            TEXTAREA: function(t, e) {
-                var n = e.value;
-                t.value !== n && (t.value = n);
-                var i = t.firstChild;
-                if (i) {
-                    var r = i.nodeValue;
-                    if (r == n || !n && r == t.placeholder) return;
-                    i.nodeValue = n
-                }
-            },
-            SELECT: function(t, e) {
-                if (!e.hasAttribute("multiple")) {
-                    for (var n = -1, i = 0, r = t.firstChild, o, s; r;)
-                        if (s = r.nodeName && r.nodeName.toUpperCase(), s === "OPTGROUP") o = r, r = o.firstChild;
-                        else {
-                            if (s === "OPTION") {
-                                if (r.hasAttribute("selected")) {
-                                    n = i;
-                                    break
-                                }
-                                i++
-                            }
-                            r = r.nextSibling, !r && o && (r = o.nextSibling, o = null)
-                        } t.selectedIndex = n
-                }
-            }
-        },
-        A = 1,
-        ae = 11,
-        ce = 3,
-        ue = 8;
-
-    function E() {}
-
-    function Ie(t) {
-        if (t) return t.getAttribute && t.getAttribute("id") || t.id
-    }
-
-    function je(t) {
-        return function(n, i, r) {
-            if (r || (r = {}), typeof i == "string")
-                if (n.nodeName === "#document" || n.nodeName === "HTML" || n.nodeName === "BODY") {
-                    var o = i;
-                    i = v.createElement("html"), i.innerHTML = o
-                } else i = Ue(i);
-            else i.nodeType === ae && (i = i.firstElementChild);
-            var s = r.getNodeKey || Ie,
-                l = r.onBeforeNodeAdded || E,
-                d = r.onNodeAdded || E,
-                _ = r.onBeforeElUpdated || E,
-                T = r.onElUpdated || E,
-                G = r.onBeforeNodeDiscarded || E,
-                m = r.onNodeDiscarded || E,
-                O = r.onBeforeElChildrenUpdated || E,
-                ve = r.skipFromChildren || E,
-                Y = r.addChild || function(c, a) {
-                    return c.appendChild(a)
-                },
-                B = r.childrenOnly === !0,
-                L = Object.create(null),
-                k = [];
-
-            function R(c) {
-                k.push(c)
-            }
-
-            function Z(c, a) {
-                if (c.nodeType === A)
-                    for (var h = c.firstChild; h;) {
-                        var u = void 0;
-                        a && (u = s(h)) ? R(u) : (m(h), h.firstChild && Z(h, a)), h = h.nextSibling
-                    }
-            }
-
-            function D(c, a, h) {
-                G(c) !== !1 && (a && a.removeChild(c), m(c), Z(c, h))
-            }
-
-            function ee(c) {
-                if (c.nodeType === A || c.nodeType === ae)
-                    for (var a = c.firstChild; a;) {
-                        var h = s(a);
-                        h && (L[h] = a), ee(a), a = a.nextSibling
-                    }
-            }
-            ee(n);
-
-            function V(c) {
-                d(c);
-                for (var a = c.firstChild; a;) {
-                    var h = a.nextSibling,
-                        u = s(a);
-                    if (u) {
-                        var f = L[u];
-                        f && H(a, f) ? (a.parentNode.replaceChild(f, a), U(f, a)) : V(a)
-                    } else V(a);
-                    a = h
-                }
-            }
-
-            function _e(c, a, h) {
-                for (; a;) {
-                    var u = a.nextSibling;
-                    (h = s(a)) ? R(h): D(a, c, !0), a = u
-                }
-            }
-
-            function U(c, a, h) {
-                var u = s(a);
-                u && delete L[u], !(!h && (_(c, a) === !1 || (t(c, a), T(c), O(c, a) === !1))) && (c.nodeName !== "TEXTAREA" ? me(c, a) : se.TEXTAREA(c, a))
-            }
-
-            function me(c, a) {
-                var h = ve(c),
-                    u = a.firstChild,
-                    f = c.firstChild,
-                    N, g, x, M, b;
-                e: for (; u;) {
-                    for (M = u.nextSibling, N = s(u); !h && f;) {
-                        if (x = f.nextSibling, u.isSameNode && u.isSameNode(f)) {
-                            u = M, f = x;
-                            continue e
-                        }
-                        g = s(f);
-                        var I = f.nodeType,
-                            w = void 0;
-                        if (I === u.nodeType && (I === A ? (N ? N !== g && ((b = L[N]) ? x === b ? w = !1 : (c.insertBefore(b, f), g ? R(g) : D(f, c, !0), f = b) : w = !1) : g && (w = !1), w = w !== !1 && H(f, u), w && U(f, u)) : (I === ce || I == ue) && (w = !0, f.nodeValue !== u.nodeValue && (f.nodeValue = u.nodeValue))), w) {
-                            u = M, f = x;
-                            continue e
-                        }
-                        g ? R(g) : D(f, c, !0), f = x
-                    }
-                    if (N && (b = L[N]) && H(b, u)) h || Y(c, b), U(b, u);
-                    else {
-                        var Q = l(u);
-                        Q !== !1 && (Q && (u = Q), u.actualize && (u = u.actualize(c.ownerDocument || v)), Y(c, u), V(u))
-                    }
-                    u = M, f = x
-                }
-                _e(c, f, g);
-                var ne = se[c.nodeName];
-                ne && ne(c, a)
-            }
-            var p = n,
-                P = p.nodeType,
-                te = i.nodeType;
-            if (!B) {
-                if (P === A) te === A ? H(n, i) || (m(n), p = Me(n, Pe(i.nodeName, i.namespaceURI))) : p = i;
-                else if (P === ce || P === ue) {
-                    if (te === P) return p.nodeValue !== i.nodeValue && (p.nodeValue = i.nodeValue), p;
-                    p = i
-                }
-            }
-            if (p === i) m(n);
-            else {
-                if (i.isSameNode && i.isSameNode(p)) return;
-                if (U(p, i, B), k)
-                    for (var W = 0, ye = k.length; W < ye; W++) {
-                        var q = L[k[W]];
-                        q && D(q, q.parentNode, !1)
-                    }
-            }
-            return !B && p !== n && n.parentNode && (p.actualize && (p = p.actualize(n.ownerDocument || v)), n.parentNode.replaceChild(p, n)), p
-        }
-    }
-    var He = je(Le),
-        le = He;
+        H = Le;
+    var Ae = _e(V());
 
-    function Fe(t, e) {
-        le(t, e)
+    function Q(t, e) {
+        Idiomorph.morph(t, e)
     }
-    var J = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
-    console.log("BOOST_PAGES", J);
-    var de = class extends EventTarget {
-            send() {
+    var j = JSON.parse(document.querySelector("meta[name=reactor-boost]")?.dataset.enabled || "false");
+    console.log("BOOST_PAGES", j);
+    var $ = class extends EventTarget {
+            sendNewLocation() {
                 console.log("LOAD", document.location.href), this.dispatchEvent(new Event("newLocation"))
             }
+            sendNewContent() {
+                this.dispatchEvent(new Event("newContent"))
+            }
         },
-        X = new de;
-    J && document.addEventListener("click", t => {
+        O = new $;
+    j && document.addEventListener("click", t => {
         let e = t.target;
-        e = e.tagName.toLowerCase() !== "a" ? e.closest("a") : e, e && e.href && (!e.target || e.target === "_self") && e.origin == document.location.origin && t.button === 0 && !t.metaKey && !t.ctrlKey && !t.altKey && !t.shiftKey && (t.preventDefault(), F.load(e.href))
+        e = e.tagName.toLowerCase() !== "a" ? e.closest("a") : e, e && e.href && (!e.target || e.target === "_self") && e.origin == document.location.origin && t.button === 0 && !t.metaKey && !t.ctrlKey && !t.altKey && !t.shiftKey && (t.preventDefault(), M.load(e.href))
     });
 
-    function fe(t, e = void 0) {
-        document.body.innerHTML = t, e === void 0 ? document.querySelector("[autofocus]")?.focus() : window.scrollTo(0, e)
+    function J(t, e = void 0) {
+        window.requestAnimationFrame(() => {
+            Q(document.body, t), e === void 0 ? document.querySelector("[autofocus]")?.focus() : window.scrollTo(0, e), O.sendNewContent()
+        })
     }
 
-    function Ge(t) {
+    function ke(t) {
         return t.startsWith("http://") || t.startsWith("https://") ? new URL(t).origin === document.location.origin : !0
     }
-    var F = class {
+    var M = class {
         static async load(e) {
-            J && Ge(e) ? this.push(e) : document.location.assign(e)
+            j && ke(e) ? this.push(e) : document.location.assign(e)
         }
         static back() {
             window.history.back()
         }
         static async push(e) {
             if (document.body == null) debugger;
             history.replaceState({
-                content: document.body.innerHTML,
+                content: document.body.outerHTML,
                 scrollY: window.scrollY
             }, document.title, document.location.href), history.pushState({}, document.title, e), this.replaceContentFromUrl(e)
         }
         static async replaceContentFromUrl(e) {
-            X.send();
-            let i = await (await fetch(e)).text(),
-                r = new DOMParser().parseFromString(i, "text/html");
-            document.title = r.querySelector("title")?.text ?? "", fe(r.body.innerHTML)
+            O.sendNewLocation();
+            let a = await (await fetch(e)).text(),
+                s = new DOMParser().parseFromString(a, "text/html");
+            document.title = s.querySelector("title")?.text ?? "", J(s.body)
         }
         static replace(e) {
             history.replaceState({}, document.title, e)
         }
     };
     window.addEventListener("popstate", t => {
-        X.send(), t.state?.content !== void 0 && fe(t.state.content, t.state.scrollY), F.replaceContentFromUrl(document.location.href)
+        O.sendNewLocation(), t.state?.content !== void 0 && J(t.state.content, t.state.scrollY), M.replaceContentFromUrl(document.location.href)
     });
-    var y = {
-        HistoryCache: F,
-        morph: Fe,
-        navEvent: X
+    var g = {
+        HistoryCache: M,
+        morph: Q,
+        navEvent: O
     };
-    var Be = new DOMParser,
-        he = class extends EventTarget {
+    var Ce = new DOMParser,
+        K = class {
+            constructor() {
+                this.components = {}
+            }
             open(e = "__reactor__") {
                 let n = location.protocol.replace("http", "ws");
-                this.socket = new $(`${n}//${location.host}/${e}`, [], {
+                this.socket = new H(`${n}//${location.host}/${e}`, [], {
                     maxEnqueuedMessages: 0
                 }), this.socket.addEventListener("open", () => {
-                    console.log("WS: OPEN"), this.sendQueryString(), this.dispatchEvent(new Event("open"))
-                }), this.socket.addEventListener("message", i => this._processMessage(i)), this.socket.addEventListener("close", () => {
-                    console.log("WS: CLOSE"), this.dispatchEvent(new Event("close"))
-                }), y.navEvent.addEventListener("newLocation", () => {
+                    console.log("WS: OPEN"), this.sendQueryString(), this.components = {}, this.joinAllComponents()
+                }), this.socket.addEventListener("message", a => this._processMessage(a)), this.socket.addEventListener("close", () => {
+                    console.log("WS: CLOSE"), this.components = {}, document.querySelectorAll("[reactor-component]").forEach(a => {
+                        a.classList.add("reactor-disconnected"), a.dataset.isLive = "false"
+                    })
+                }), g.navEvent.addEventListener("newLocation", () => {
                     this.sendQueryString()
+                }), g.navEvent.addEventListener("newContent", () => {
+                    this.joinAllComponents()
                 })
             }
             get isOpen() {
-                return this.socket?.readyState == $.OPEN
+                return this.socket?.readyState == H.OPEN
+            }
+            joinAllComponents() {
+                let e = new Set(Object.keys(this.components));
+                for (let n of document.querySelectorAll("[reactor-component]"))
+                    if (e.delete(n.id)) this.components[n.id].join();
+                    else {
+                        let a = new z(n.id);
+                        this.components[n.id] = a, a.join()
+                    } for (let n of e.keys()) delete this.components[n], this.sendLeave(n)
             }
             _processMessage(e) {
                 let {
                     command: n,
-                    payload: i
+                    payload: a
                 } = JSON.parse(e.data);
                 switch (n) {
                     case "render":
                         var {
-                            id: r, diff: o
-                        } = i;
-                        console.log("<<< RENDER", r), document.getElementById(r)?.applyDiff(o);
+                            id: s, diff: d
+                        } = a;
+                        console.log("<<< RENDER", s), this.components[s]?.applyDiff(d);
                         break;
                     case "append":
                     case "prepend":
                     case "insert_after":
                     case "insert_before":
                     case "replace_with":
                         var {
-                            id: r, html: s
-                        } = i;
-                        console.log(`<<< ${n.toUpperCase()}`, r), s = Be.parseFromString(s, "text/html").body.firstChild;
-                        var l = document.getElementById(r);
-                        if (l) switch (n) {
-                            case "append":
-                                l.append(s);
-                                break;
-                            case "prepend":
-                                l.prepend(s);
-                                break;
-                            case "insert_after":
-                                l.after(s);
-                                break;
-                            case "insert_before":
-                                l.before(s);
-                                break;
-                            case "replace_with":
-                                y.morph(l, s);
-                                break
+                            id: s, html: f
+                        } = a;
+                        console.log(`<<< ${n.toUpperCase()}`, s), f = Ce.parseFromString(f, "text/html").body.firstChild;
+                        var h = document.getElementById(s);
+                        if (h) {
+                            switch (n) {
+                                case "append":
+                                    h.append(f);
+                                    break;
+                                case "prepend":
+                                    h.prepend(f);
+                                    break;
+                                case "insert_after":
+                                    h.after(f);
+                                    break;
+                                case "insert_before":
+                                    h.before(f);
+                                    break;
+                                case "replace_with":
+                                    g.morph(h, f);
+                                    break
+                            }
+                            g.navEvent.sendNewContent()
                         }
                         break;
                     case "remove":
                         var {
-                            id: r
-                        } = i;
-                        console.log("<<< REMOVE", r), document.getElementById(r)?.remove();
+                            id: s
+                        } = a;
+                        console.log("<<< REMOVE", s), document.getElementById(s)?.remove(), g.navEvent.sendNewContent();
                         break;
                     case "focus_on":
                         var {
-                            selector: d
-                        } = i;
-                        console.log("<<< FOCUS-ON", `"${d}"`, document.querySelector(d)), window.requestAnimationFrame(() => document.querySelector(d)?.focus());
+                            selector: m
+                        } = a;
+                        console.log("<<< FOCUS-ON", `"${m}"`, document.querySelector(m)), window.requestAnimationFrame(() => document.querySelector(m)?.focus());
                         break;
                     case "scroll_into_view":
                         var {
-                            id: r, behavior: _, block: T, inline: G
-                        } = i;
-                        window.requestAnimationFrame(() => document.getElementById(r)?.scrollIntoView({
-                            behavior: _,
-                            block: T,
-                            inline: G
+                            id: s, behavior: b, block: R, inline: T
+                        } = a;
+                        window.requestAnimationFrame(() => document.getElementById(s)?.scrollIntoView({
+                            behavior: b,
+                            block: R,
+                            inline: T
                         }));
                         break;
                     case "url_change":
                         var {
-                            url: m
-                        } = i;
-                        switch (console.log("<< URL", i.command, m), i.command) {
+                            url: E
+                        } = a;
+                        switch (console.log("<< URL", a.command, E), a.command) {
                             case "redirect":
-                                y.HistoryCache.load(m);
+                                g.HistoryCache.load(E);
                                 break;
                             case "replace":
-                                y.HistoryCache.replace(m);
+                                g.HistoryCache.replace(E);
                                 break;
                             case "push":
-                                y.HistoryCache.push(m);
+                                g.HistoryCache.push(E);
                                 break
                         }
                         break;
                     case "set_query_string":
                         var {
-                            qs: O
-                        } = i;
-                        O = O.length ? `?${O}` : "", console.log("<< SET URL PARAMS", O), y.HistoryCache.replace(document.location.pathname + O);
+                            qs: w
+                        } = a;
+                        w = w.length ? `?${w}` : "", console.log("<< SET URL PARAMS", w), g.HistoryCache.replace(document.location.pathname + w);
                         break;
                     case "back":
-                        y.HistoryCache.back();
+                        g.HistoryCache.back();
                         break;
                     default:
-                        console.error(`Unknown command "${n}"`, i)
+                        console.error(`Unknown command "${n}"`, a)
                 }
             }
             sendQueryString() {
                 let e = document.location.search.slice(1);
                 console.log("QS", e), this._send("query_string", {
                     qs: e
                 })
             }
-            sendJoin(e, n, i, r) {
+            sendJoin(e, n, a, s) {
                 console.log(">>> JOIN", e, n), this._send("join", {
                     name: e,
-                    parent_id: i,
-                    state: r
+                    state: a,
+                    children: s
                 })
             }
             sendLeave(e) {
                 console.log(">>> LEAVE", e), this._send("leave", {
                     id: e
                 })
             }
-            sendUserEvent(e, n, i, r) {
-                console.log(">>> USER_EVENT", e, n, r), this._send("user_event", {
+            sendUserEvent(e, n, a, s) {
+                console.log(">>> USER_EVENT", e, n, s), this._send("user_event", {
                     id: e,
                     command: n,
-                    implicit_args: i,
-                    explicit_args: r
+                    implicit_args: a,
+                    explicit_args: s
                 })
             }
             _send(e, n) {
                 this.isOpen && this.socket.send(JSON.stringify({
                     command: e,
                     payload: n
                 }))
             }
         },
-        S = new he;
-    for ({
-            dataset
-        }
-        of document.querySelectorAll("meta[name=reactor-component]")) {
-        let t = document.createElement(dataset.extends);
-        class e extends t.constructor {
-            constructor(...i) {
-                super(...i);
-                this._lastReceivedHtml = [], this.joinBind = () => this.join(), this.wentOffline = () => this.classList.add("reactor-disconnected")
-            }
-            connectedCallback() {
-                S.addEventListener("open", this.joinBind), S.addEventListener("close", this.wentOffline), this.join()
+        A = new K,
+        z = class {
+            constructor(e) {
+                this.id = e, this.lastReceivedHtml = []
             }
-            disconnectedCallback() {
-                S.removeEventListener("open", this.joinBind), S.removeEventListener("close", this.wentOffline), this.leave()
+            getElemenet() {
+                return document.getElementById(this.id)
             }
-            join() {
-                this.classList.remove("reactor-disconnected"), S.sendJoin(this.dataset.name, this.id, this.parentId, this.dataset.state)
-            }
-            leave() {
-                S.sendLeave(this.id)
-            }
-            applyDiff(i) {
+            applyDiff(e) {
                 window.requestAnimationFrame(() => {
-                    let r = this.getHtml(i);
-                    y.morph(this, r)
+                    let n = this.getElemenet();
+                    if (n) {
+                        let a = this.getHtml(e);
+                        g.morph(n, a), g.navEvent.sendNewContent()
+                    }
                 })
             }
-            getHtml(i) {
-                let r = [],
-                    o = 0;
-                for (let s of i) typeof s == "string" ? r.push(s) : s < 0 ? o -= s : (r.push(...this._lastReceivedHtml.slice(o, o + s)), o += s);
-                return this._lastReceivedHtml = r, r.join(" ")
-            }
-            get parentId() {
-                return this.parentComponent?.id
-            }
-            get parentComponent() {
-                return this.parentElement?.closest("[reactor-component]")
-            }
-            dispatch(i, r, o) {
-                S.sendUserEvent(this.id, i, this.serialize(o), r)
-            }
-            serialize(i) {
-                let r = {};
-                for (let o of i.querySelectorAll("[name]")) {
-                    if (o.closest("[reactor-component]") !== this) continue;
-                    let s = null;
-                    switch (o.type.toLowerCase()) {
+            getHtml(e) {
+                let n = [],
+                    a = 0;
+                for (let s of e) typeof s == "string" ? n.push(s) : s < 0 ? a -= s : (n.push(...this.lastReceivedHtml.slice(a, a + s)), a += s);
+                return this.lastReceivedHtml = n, n.join(" ")
+            }
+            join() {
+                let e = this.getElemenet();
+                if (e && e.dataset.isLive === "false") {
+                    let n = e?.parentElement?.closest("[reactor-component]");
+                    if (!n || n.dataset.isLive === "true") {
+                        e.dataset.isLive = "true";
+                        let a = Array.from(e.querySelectorAll("[reactor-component]")).reduce((s, d) => (s[d.id] = [d.dataset.name, d.dataset.state], s), {});
+                        A.sendJoin(e.dataset.name, e.id, e.dataset.state, a)
+                    }
+                }
+            }
+            dispatch(e, n, a) {
+                A.sendUserEvent(this.id, e, this.serialize(a), n)
+            }
+            serialize(e) {
+                let n = {},
+                    a = this.getElemenet();
+                for (let s of e.querySelectorAll("[name]")) {
+                    if (s.closest("[reactor-component]") !== a) continue;
+                    let d = null;
+                    switch (s.type.toLowerCase()) {
                         case "checkbox":
                         case "radio":
-                            s = o.checked ? o.value || !0 : null;
+                            d = s.checked ? s.value || !0 : null;
                             break;
                         case "select-multiple":
-                            s = o.selectedOptions.map(l => l.value);
+                            d = s.selectedOptions.map(f => f.value);
                             break;
                         default:
-                            s = o.value;
+                            d = s.value;
                             break
                     }
-                    if (s !== null) {
-                        let l = o.getAttribute("name"),
-                            d = r[l] ?? [];
-                        d.push(s), r[l] = d
+                    if (d !== null) {
+                        let f = s.getAttribute("name"),
+                            h = n[f] ?? [];
+                        h.push(d), n[f] = h
                     }
                 }
-                return r
+                return n
             }
-        }
-        customElements.define(dataset.tagName, e, {
-            extends: dataset.extends
-        })
-    }
-    S.open();
-    var pe = void 0;
+        };
+    A.open();
+    var Y = void 0;
     window.reactor = {
         send(t, e, n) {
-            let i = t.closest("[reactor-component]");
-            if (i !== null) {
-                let r = t.closest("form"),
-                    o = i.contains(r) ? r : i;
-                i.dispatch(e, n, o)
+            let a = t.closest("[reactor-component]"),
+                s = A.components[a.id];
+            if (a !== null && s !== void 0) {
+                let d = t.closest("form"),
+                    f = a.contains(d) ? d : a;
+                s.dispatch(e, n, f)
             }
         },
         debounce(t) {
             return e => (...n) => {
-                clearTimeout(pe), pe = setTimeout(() => e(...n), t)
+                clearTimeout(Y), Y = setTimeout(() => e(...n), t)
             }
         }
     };
 })();
 /*!
  * Reconnecting WebSocket
  * by Pedro Ladaria <pedro.ladaria@gmail.com>
```

### Comparing `django-reactor-5.2.0b0/reactor/static/reactor/reactor.min.js.map` & `django-reactor-5.3.0b0/reactor/static/reactor/reactor.min.js.map`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7742857142857142%*

 * *Differences: {"'mappings'": "'wmBAAA,aAKA,AAAC,UAAU,EAAM,EAAS,CAEtB,AAAI,MAAO,SAAW,YAAc,OAAO,IAGvC,OAAO,GAAI,GAGX,EAAK,UAAY,EAAK,WAAa,MAEzC,MAAO,OAAS,YAAc,KAAO,EACnC,UAAY,CACR,MAAQ,WAAY,CAChB,aAKA,GAAI,GAAY,GAAI,KAKpB,WAAe,EAAS,EAAY,EAAS,GAAI,CAE7C,AAAI,YAAmB,WACnB,GAAU,EAAQ,iBAGlB,MAAO,IAAe,UACtB,GAAa,EAAa,IAG9B,GAAI,GAAoB,GAAiB,GAErC,EAAM,EAAmB,EAAS,EAAmB,GAEzD,MAAO,GAAuB,EAAS,EAAmB,GAG9D,WAAgC,EAAS,EAAsB,EAAK,CAChE,GAAI,EAAI,KAAK,MAAO,CAChB,GAAI,GAAU,EAAQ,cAAc,QAChC,EAAU,EAAqB,cAAc,QACjD,GAAI,GAAW,EAAS,CACpB,GAAI,GAA […]*

```diff
@@ -1,17 +1,17 @@
 {
-    "mappings": "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",
+    "mappings": "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",
     "names": [],
     "sources": [
+        "../../../node_modules/idiomorph/dist/idiomorph.js",
         "../../../node_modules/reconnecting-websocket/dist/reconnecting-websocket-mjs.js",
-        "../../../node_modules/morphdom/dist/morphdom-esm.js",
         "reactor-boost.js",
         "reactor.js"
     ],
     "sourcesContent": [
+        "//=============================================================================\n// AMD insanity... i hate javascript so much\n//\n// IGNORE EVERYTHING FROM HERE UNTIL THE COMMENT SAYING 'AND NOW IT BEGINS...\"\n//=============================================================================\n(function (root, factory) {\n    //@ts-ignore\n    if (typeof define === 'function' && define.amd) {\n        // AMD. Register as an anonymous module.\n        //@ts-ignore\n        define([], factory);\n    } else {\n        // Browser globals\n        root.Idiomorph = root.Idiomorph || factory();\n    }\n}(typeof self !== 'undefined' ? self : this,\n    function () {\n        return (function () {\n            'use strict';\n\n            //=============================================================================\n            // AND NOW IT BEGINS...\n            //=============================================================================\n            let EMPTY_SET = new Set();\n\n            //=============================================================================\n            // Core Morphing Algorithm - morph, morphNormalizedContent, morphOldNodeTo, morphChildren\n            //=============================================================================\n            function morph(oldNode, newContent, config = {}) {\n\n                if (oldNode instanceof Document) {\n                    oldNode = oldNode.documentElement;\n                }\n\n                if (typeof newContent === 'string') {\n                    newContent = parseContent(newContent);\n                }\n\n                let normalizedContent = normalizeContent(newContent);\n\n                let ctx = createMorphContext(oldNode, normalizedContent, config);\n\n                return morphNormalizedContent(oldNode, normalizedContent, ctx);\n            }\n\n            function morphNormalizedContent(oldNode, normalizedNewContent, ctx) {\n                if (ctx.head.block) {\n                    let oldHead = oldNode.querySelector('head');\n                    let newHead = normalizedNewContent.querySelector('head');\n                    if (oldHead && newHead) {\n                        let promises = handleHeadElement(newHead, oldHead, ctx);\n                        // when head promises resolve, call morph again, ignoring the head tag\n                        Promise.all(promises).then(function () {\n                            morphNormalizedContent(oldNode, normalizedNewContent, Object.assign(ctx, {\n                                head: {\n                                    block: false,\n                                    ignore: true\n                                }\n                            }));\n                        });\n                        return;\n                    }\n                }\n\n                if (ctx.morphStyle === \"innerHTML\") {\n\n                    // innerHTML, so we are only updating the children\n                    morphChildren(normalizedNewContent, oldNode, ctx);\n                    return oldNode.children;\n\n                } else if (ctx.morphStyle === \"outerHTML\" || ctx.morphStyle == null) {\n                    // otherwise find the best element match in the new content, morph that, and merge its siblings\n                    // into either side of the best match\n                    let bestMatch = findBestNodeMatch(normalizedNewContent, oldNode, ctx);\n\n                    // stash the siblings that will need to be inserted on either side of the best match\n                    let previousSibling = bestMatch?.previousSibling;\n                    let nextSibling = bestMatch?.nextSibling;\n\n                    // morph it\n                    let morphedNode = morphOldNodeTo(oldNode, bestMatch, ctx);\n\n                    if (bestMatch) {\n                        // if there was a best match, merge the siblings in too and return the\n                        // whole bunch\n                        return insertSiblings(previousSibling, morphedNode, nextSibling);\n                    } else {\n                        // otherwise nothing was added to the DOM\n                        return []\n                    }\n                } else {\n                    throw \"Do not understand how to morph style \" + ctx.morphStyle;\n                }\n            }\n\n\n\n            /**\n             * @param oldNode root node to merge content into\n             * @param newContent new content to merge\n             * @param ctx the merge context\n             * @returns {Element} the element that ended up in the DOM\n             */\n            function morphOldNodeTo(oldNode, newContent, ctx) {\n                if (ctx.ignoreActive && oldNode === document.activeElement) {\n                    // don't morph focused element\n                } else if (newContent == null) {\n                    ctx.callbacks.beforeNodeRemoved(oldNode);\n                    oldNode.remove();\n                    ctx.callbacks.afterNodeRemoved(oldNode);\n                    return null;\n                } else if (!isSoftMatch(oldNode, newContent)) {\n                    ctx.callbacks.beforeNodeRemoved(oldNode);\n                    ctx.callbacks.beforeNodeAdded(newContent);\n                    oldNode.parentElement.replaceChild(newContent, oldNode);\n                    ctx.callbacks.afterNodeAdded(newContent);\n                    ctx.callbacks.afterNodeRemoved(oldNode);\n                    return newContent;\n                } else {\n                    ctx.callbacks.beforeNodeMorphed(oldNode, newContent);\n                    if (oldNode instanceof HTMLHeadElement && ctx.head.ignore) {\n                        // ignore the head element\n                    } else if (oldNode instanceof HTMLHeadElement && ctx.head.style !== \"morph\") {\n                        handleHeadElement(newContent, oldNode, ctx);\n                    } else {\n                        syncNodeFrom(newContent, oldNode);\n                        morphChildren(newContent, oldNode, ctx);\n                    }\n                    ctx.callbacks.afterNodeMorphed(oldNode, newContent);\n                    return oldNode;\n                }\n            }\n\n            /**\n             * This is the core algorithm for matching up children.  The idea is to use id sets to try to match up\n             * nodes as faithfully as possible.  We greedily match, which allows us to keep the algorithm fast, but\n             * by using id sets, we are able to better match up with content deeper in the DOM.\n             *\n             * Basic algorithm is, for each node in the new content:\n             *\n             * - if we have reached the end of the old parent, append the new content\n             * - if the new content has an id set match with the current insertion point, morph\n             * - search for an id set match\n             * - if id set match found, morph\n             * - otherwise search for a \"soft\" match\n             * - if a soft match is found, morph\n             * - otherwise, prepend the new node before the current insertion point\n             *\n             * The two search algorithms terminate if competing node matches appear to outweigh what can be achieved\n             * with the current node.  See findIdSetMatch() and findSoftMatch() for details.\n             *\n             * @param {Element} newParent the parent element of the new content\n             * @param {Element } oldParent the old content that we are merging the new content into\n             * @param ctx the merge context\n             */\n            function morphChildren(newParent, oldParent, ctx) {\n\n                let nextNewChild = newParent.firstChild;\n                let insertionPoint = oldParent.firstChild;\n\n                // run through all the new content\n                while (nextNewChild) {\n\n                    let newChild = nextNewChild;\n                    nextNewChild = newChild.nextSibling;\n\n                    // if we are at the end of the exiting parent's children, just append\n                    if (insertionPoint == null) {\n\n                        ctx.callbacks.beforeNodeAdded(newChild);\n                        oldParent.appendChild(newChild);\n                        ctx.callbacks.afterNodeAdded(newChild);\n\n                        // if the current node has an id set match then morph\n                    } else if (isIdSetMatch(newChild, insertionPoint, ctx)) {\n\n                        morphOldNodeTo(insertionPoint, newChild, ctx);\n                        insertionPoint = insertionPoint.nextSibling;\n\n                    } else {\n\n                        // otherwise search forward in the existing old children for an id set match\n                        let idSetMatch = findIdSetMatch(newParent, oldParent, newChild, insertionPoint, ctx);\n\n                        // if we found a potential match, remove the nodes until that point and morph\n                        if (idSetMatch) {\n\n                            insertionPoint = removeNodesBetween(insertionPoint, idSetMatch, ctx);\n                            morphOldNodeTo(idSetMatch, newChild, ctx);\n\n                        } else {\n\n                            // no id set match found, so scan forward for a soft match for the current node\n                            let softMatch = findSoftMatch(newParent, oldParent, newChild, insertionPoint, ctx);\n\n                            // if we found a soft match for the current node, morph\n                            if (softMatch) {\n\n                                insertionPoint = removeNodesBetween(insertionPoint, softMatch, ctx);\n                                morphOldNodeTo(softMatch, newChild, ctx);\n\n                            } else {\n\n                                // abandon all hope of morphing, just insert the new child before the insertion point\n                                // and move on\n                                ctx.callbacks.beforeNodeAdded(newChild);\n                                oldParent.insertBefore(newChild, insertionPoint);\n                                ctx.callbacks.afterNodeAdded(newChild);\n\n                            }\n                        }\n                    }\n\n                    // remove the processed new contents ids from consideration in future merge decisions\n                    removeIdsFromConsideration(ctx, newChild);\n                }\n\n                // remove any remaining old nodes that didn't match up with new content\n                while (insertionPoint !== null) {\n\n                    let tempNode = insertionPoint;\n                    insertionPoint = insertionPoint.nextSibling;\n                    removeNode(tempNode, ctx);\n                }\n            }\n\n            //=============================================================================\n            // Attribute Syncing Code\n            //=============================================================================\n\n            /**\n             * syncs a given node with another node, copying over all attributes and\n             * inner element state from the 'from' node to the 'to' node\n             *\n             * @param {Element} from the element to copy attributes & state from\n             * @param {Element} to the element to copy attributes & state to\n             */\n            function syncNodeFrom(from, to) {\n                let type = from.nodeType\n\n                // if is an element type, sync the attributes from the\n                // new node into the new node\n                if (type === 1 /* element type */) {\n                    const fromAttributes = from.attributes;\n                    const toAttributes = to.attributes;\n                    for (const fromAttribute of fromAttributes) {\n                        if (to.getAttribute(fromAttribute.name) !== fromAttribute.value) {\n                            to.setAttribute(fromAttribute.name, fromAttribute.value);\n                        }\n                    }\n                    for (const toAttribute of toAttributes) {\n                        if (!from.hasAttribute(toAttribute.name)) {\n                            to.removeAttribute(toAttribute.name);\n                        }\n                    }\n                }\n\n                // sync text nodes\n                if (type === 8 /* comment */ || type === 3 /* text */) {\n                    if (to.nodeValue !== from.nodeValue) {\n                        to.nodeValue = from.nodeValue;\n                    }\n                }\n\n                // NB: many bothans died to bring us information:\n                //\n                // https://github.com/patrick-steele-idem/morphdom/blob/master/src/specialElHandlers.js\n                // https://github.com/choojs/nanomorph/blob/master/lib/morph.jsL113\n\n                // sync input value\n                if (from instanceof HTMLInputElement &&\n                    to instanceof HTMLInputElement &&\n                    from.type !== 'file') {\n\n                    let fromValue = from.value;\n                    let toValue = to.value;\n\n                    // sync boolean attributes\n                    syncBooleanAttribute(from, to, 'checked');\n                    syncBooleanAttribute(from, to, 'disabled');\n\n                    if (!from.hasAttribute('value')) {\n                        to.value = '';\n                        to.removeAttribute('value');\n                    } else if (fromValue !== toValue) {\n                        to.setAttribute('value', fromValue);\n                        to.value = fromValue;\n                    }\n                } else if (from instanceof HTMLOptionElement) {\n                    syncBooleanAttribute(from, to, 'selected')\n                } else if (from instanceof HTMLTextAreaElement && to instanceof HTMLTextAreaElement) {\n                    let fromValue = from.value;\n                    let toValue = to.value;\n                    if (fromValue !== toValue) {\n                        to.value = fromValue;\n                    }\n                    if (to.firstChild && to.firstChild.nodeValue !== fromValue) {\n                        to.firstChild.nodeValue = fromValue\n                    }\n                }\n            }\n\n            function syncBooleanAttribute(from, to, attributeName) {\n                if (from[attributeName] !== to[attributeName]) {\n                    to[attributeName] = from[attributeName];\n                    if (from[attributeName]) {\n                        to.setAttribute(attributeName, '');\n                    } else {\n                        to.removeAttribute(attributeName);\n                    }\n                }\n            }\n\n            //=============================================================================\n            // the HEAD tag can be handled specially, either w/ a 'merge' or 'append' style\n            //=============================================================================\n            function handleHeadElement(newHeadTag, currentHead, ctx) {\n\n                let added = []\n                let removed = []\n                let preserved = []\n                let nodesToAppend = []\n\n                let headMergeStyle = ctx.head.style;\n\n                // put all new head elements into a Map, by their outerHTML\n                let srcToNewHeadNodes = new Map();\n                for (const newHeadChild of newHeadTag.children) {\n                    srcToNewHeadNodes.set(newHeadChild.outerHTML, newHeadChild);\n                }\n\n                // for each elt in the current head\n                for (const currentHeadElt of currentHead.children) {\n\n                    // If the current head element is in the map\n                    let inNewContent = srcToNewHeadNodes.has(currentHeadElt.outerHTML);\n                    let isReAppended = ctx.head.shouldReAppend(currentHeadElt);\n                    let isPreserved = ctx.head.shouldPreserve(currentHeadElt);\n                    if (inNewContent || isPreserved) {\n                        if (isReAppended) {\n                            // remove the current version and let the new version replace it and re-execute\n                            removed.push(currentHeadElt);\n                        } else {\n                            // this element already exists and should not be re-appended, so remove it from\n                            // the new content map, preserving it in the DOM\n                            srcToNewHeadNodes.delete(currentHeadElt.outerHTML);\n                            preserved.push(currentHeadElt);\n                        }\n                    } else {\n                        if (headMergeStyle === \"append\") {\n                            // we are appending and this existing element is not new content\n                            // so if and only if it is marked for re-append do we do anything\n                            if (isReAppended) {\n                                removed.push(currentHeadElt);\n                                nodesToAppend.push(currentHeadElt);\n                            }\n                        } else {\n                            // if this is a merge, we remove this content since it is not in the new head\n                            if (ctx.head.shouldRemove(currentHeadElt) !== false) {\n                                removed.push(currentHeadElt);\n                            }\n                        }\n                    }\n                }\n\n                // Push the remaining new head elements in the Map into the\n                // nodes to append to the head tag\n                nodesToAppend.push(...srcToNewHeadNodes.values());\n                log(\"to append: \", nodesToAppend);\n\n                let promises = [];\n                for (const newNode of nodesToAppend) {\n                    log(\"adding: \", newNode);\n                    let newElt = document.createRange().createContextualFragment(newNode.outerHTML).firstChild;\n                    log(newElt);\n                    if (ctx.callbacks.beforeNodeAdded(newElt) !== false) {\n                        if (newElt.href || newElt.src) {\n                            let resolve = null;\n                            let promise = new Promise(function (_resolve) {\n                                resolve = _resolve;\n                            });\n                            newElt.addEventListener('load',function() {\n                                resolve();\n                            });\n                            promises.push(promise);\n                        }\n                        currentHead.appendChild(newElt);\n                        ctx.callbacks.afterNodeAdded(newElt);\n                        added.push(newElt);\n                    }\n                }\n\n                // remove all removed elements, after we have appended the new elements to avoid\n                // additional network requests for things like style sheets\n                for (const removedElement of removed) {\n                    if (ctx.callbacks.beforeNodeRemoved(removedElement) !== false) {\n                        currentHead.removeChild(removedElement);\n                        ctx.callbacks.afterNodeRemoved(removedElement);\n                    }\n                }\n\n                ctx.head.afterHeadMorphed(currentHead, {added: added, kept: preserved, removed: removed});\n                return promises;\n            }\n\n            //=============================================================================\n            // Misc\n            //=============================================================================\n\n            function log() {\n                //console.log(arguments);\n            }\n\n            function noOp() {}\n\n            function createMorphContext(oldNode, newContent, config) {\n                return {\n                    target:oldNode,\n                    newContent: newContent,\n                    config: config,\n                    morphStyle : config.morphStyle,\n                    ignoreActive : config.ignoreActive,\n                    idMap: createIdMap(oldNode, newContent),\n                    deadIds: new Set(),\n                    callbacks: Object.assign({\n                        beforeNodeAdded: noOp,\n                        afterNodeAdded : noOp,\n                        beforeNodeMorphed: noOp,\n                        afterNodeMorphed : noOp,\n                        beforeNodeRemoved: noOp,\n                        afterNodeRemoved : noOp,\n\n                    }, config.callbacks),\n                    head: Object.assign({\n                        style: 'merge',\n                        shouldPreserve : function(elt) {\n                            return elt.getAttribute(\"im-preserve\") === \"true\";\n                        },\n                        shouldReAppend : function(elt) {\n                            return elt.getAttribute(\"im-re-append\") === \"true\";\n                        },\n                        shouldRemove : noOp,\n                        afterHeadMorphed : noOp,\n                    }, config.head),\n                }\n            }\n\n            function isIdSetMatch(node1, node2, ctx) {\n                if (node1 == null || node2 == null) {\n                    return false;\n                }\n                if (node1.nodeType === node2.nodeType && node1.tagName === node2.tagName) {\n                    if (node1.id !== \"\" && node1.id === node2.id) {\n                        return true;\n                    } else {\n                        return getIdIntersectionCount(ctx, node1, node2) > 0;\n                    }\n                }\n                return false;\n            }\n\n            function isSoftMatch(node1, node2) {\n                if (node1 == null || node2 == null) {\n                    return false;\n                }\n                return node1.nodeType === node2.nodeType && node1.tagName === node2.tagName\n            }\n\n            function removeNodesBetween(startInclusive, endExclusive, ctx) {\n                while (startInclusive !== endExclusive) {\n                    let tempNode = startInclusive;\n                    startInclusive = startInclusive.nextSibling;\n                    removeNode(tempNode, ctx);\n                }\n                removeIdsFromConsideration(ctx, endExclusive);\n                return endExclusive.nextSibling;\n            }\n\n            //=============================================================================\n            // Scans forward from the insertionPoint in the old parent looking for a potential id match\n            // for the newChild.  We stop if we find a potential id match for the new child OR\n            // if the number of potential id matches we are discarding is greater than the\n            // potential id matches for the new child\n            //=============================================================================\n            function findIdSetMatch(newContent, oldParent, newChild, insertionPoint, ctx) {\n\n                // max id matches we are willing to discard in our search\n                let newChildPotentialIdCount = getIdIntersectionCount(ctx, newChild, oldParent);\n\n                let potentialMatch = null;\n\n                // only search forward if there is a possibility of an id match\n                if (newChildPotentialIdCount > 0) {\n                    let potentialMatch = insertionPoint;\n                    // if there is a possibility of an id match, scan forward\n                    // keep track of the potential id match count we are discarding (the\n                    // newChildPotentialIdCount must be greater than this to make it likely\n                    // worth it)\n                    let otherMatchCount = 0;\n                    while (potentialMatch != null) {\n\n                        // If we have an id match, return the current potential match\n                        if (isIdSetMatch(newChild, potentialMatch, ctx)) {\n                            return potentialMatch;\n                        }\n\n                        // computer the other potential matches of this new content\n                        otherMatchCount += getIdIntersectionCount(ctx, potentialMatch, newContent);\n                        if (otherMatchCount > newChildPotentialIdCount) {\n                            // if we have more potential id matches in _other_ content, we\n                            // do not have a good candidate for an id match, so return null\n                            return null;\n                        }\n\n                        // advanced to the next old content child\n                        potentialMatch = potentialMatch.nextSibling;\n                    }\n                }\n                return potentialMatch;\n            }\n\n            //=============================================================================\n            // Scans forward from the insertionPoint in the old parent looking for a potential soft match\n            // for the newChild.  We stop if we find a potential soft match for the new child OR\n            // if we find a potential id match in the old parents children OR if we find two\n            // potential soft matches for the next two pieces of new content\n            //=============================================================================\n            function findSoftMatch(newContent, oldParent, newChild, insertionPoint, ctx) {\n\n                let potentialSoftMatch = insertionPoint;\n                let nextSibling = newChild.nextSibling;\n                let siblingSoftMatchCount = 0;\n\n                while (potentialSoftMatch != null) {\n\n                    if (getIdIntersectionCount(ctx, potentialSoftMatch, newContent) > 0) {\n                        // the current potential soft match has a potential id set match with the remaining new\n                        // content so bail out of looking\n                        return null;\n                    }\n\n                    // if we have a soft match with the current node, return it\n                    if (isSoftMatch(newChild, potentialSoftMatch)) {\n                        return potentialSoftMatch;\n                    }\n\n                    if (isSoftMatch(nextSibling, potentialSoftMatch)) {\n                        // the next new node has a soft match with this node, so\n                        // increment the count of future soft matches\n                        siblingSoftMatchCount++;\n                        nextSibling = nextSibling.nextSibling;\n\n                        // If there are two future soft matches, bail to allow the siblings to soft match\n                        // so that we don't consume future soft matches for the sake of the current node\n                        if (siblingSoftMatchCount >= 2) {\n                            return null;\n                        }\n                    }\n\n                    // advanced to the next old content child\n                    potentialSoftMatch = potentialSoftMatch.nextSibling;\n                }\n\n                return potentialSoftMatch;\n            }\n\n            function parseContent(newContent) {\n                let parser = new DOMParser();\n\n                // remove svgs to avoid false-positive matches on head, etc.\n                let contentWithSvgsRemoved = newContent.replace(/<svg(\\s[^>]*>|>)([\\s\\S]*?)<\\/svg>/gim, '');\n\n                // if the newContent contains a html, head or body tag, we can simply parse it w/o wrapping\n                if (contentWithSvgsRemoved.match(/<\\/html>/) || contentWithSvgsRemoved.match(/<\\/head>/) || contentWithSvgsRemoved.match(/<\\/body>/)) {\n                    let content = parser.parseFromString(newContent, \"text/html\");\n                    // if it is a full HTML document, return the document itself as the parent container\n                    if (contentWithSvgsRemoved.match(/<\\/html>/)) {\n                        content.generatedByIdiomorph = true;\n                        return content;\n                    } else {\n                        // otherwise return the html element as the parent container\n                        let htmlElement = content.firstChild;\n                        if (htmlElement) {\n                            htmlElement.generatedByIdiomorph = true;\n                            return htmlElement;\n                        } else {\n                            return null;\n                        }\n                    }\n                } else {\n                    // if it is partial HTML, wrap it in a template tag to provide a parent element and also to help\n                    // deal with touchy tags like tr, tbody, etc.\n                    let responseDoc = parser.parseFromString(\"<body><template>\" + newContent + \"</template></body>\", \"text/html\");\n                    let content = responseDoc.body.querySelector('template').content;\n                    content.generatedByIdiomorph = true;\n                    return content\n                }\n            }\n\n            function normalizeContent(newContent) {\n                if (newContent == null) {\n                    // noinspection UnnecessaryLocalVariableJS\n                    const dummyParent = document.createElement('div');\n                    return dummyParent;\n                } else if (newContent.generatedByIdiomorph) {\n                    // the template tag created by idiomorph parsing can serve as a dummy parent\n                    return newContent;\n                } else if (newContent instanceof Node) {\n                    // a single node is added as a child to a dummy parent\n                    const dummyParent = document.createElement('div');\n                    dummyParent.append(newContent);\n                    return dummyParent;\n                } else {\n                    // all nodes in the array or HTMLElement collection are consolidated under\n                    // a single dummy parent element\n                    const dummyParent = document.createElement('div');\n                    for (const elt of [...newContent]) {\n                        dummyParent.append(elt);\n                    }\n                    return dummyParent;\n                }\n            }\n\n            function insertSiblings(previousSibling, morphedNode, nextSibling) {\n                let stack = []\n                let added = []\n                while (previousSibling != null) {\n                    stack.push(previousSibling);\n                    previousSibling = previousSibling.previousSibling;\n                }\n                while (stack.length > 0) {\n                    let node = stack.pop();\n                    added.push(node); // push added preceding siblings on in order and insert\n                    morphedNode.parentElement.insertBefore(node, morphedNode);\n                }\n                added.push(morphedNode);\n                while (nextSibling != null) {\n                    stack.push(nextSibling);\n                    added.push(nextSibling); // here we are going in order, so push on as we scan, rather than add\n                    nextSibling = nextSibling.nextSibling;\n                }\n                while (stack.length > 0) {\n                    morphedNode.parentElement.insertBefore(stack.pop(), morphedNode.nextSibling);\n                }\n                return added;\n            }\n\n            function findBestNodeMatch(newContent, oldNode, ctx) {\n                let currentElement;\n                currentElement = newContent.firstChild;\n                let bestElement = currentElement;\n                let score = 0;\n                while (currentElement) {\n                    let newScore = scoreElement(currentElement, oldNode, ctx);\n                    if (newScore > score) {\n                        bestElement = currentElement;\n                        score = newScore;\n                    }\n                    currentElement = currentElement.nextSibling;\n                }\n                return bestElement;\n            }\n\n            function scoreElement(node1, node2, ctx) {\n                if (isSoftMatch(node1, node2)) {\n                    return .5 + getIdIntersectionCount(ctx, node1, node2);\n                }\n                return 0;\n            }\n\n            function removeNode(tempNode, ctx) {\n                removeIdsFromConsideration(ctx, tempNode)\n                ctx.callbacks.beforeNodeRemoved(tempNode);\n                tempNode.remove();\n                ctx.callbacks.afterNodeRemoved(tempNode);\n            }\n\n            //=============================================================================\n            // ID Set Functions\n            //=============================================================================\n\n            function isIdInConsideration(ctx, id) {\n                return !ctx.deadIds.has(id);\n            }\n\n            function idIsWithinNode(ctx, id, targetNode) {\n                let idSet = ctx.idMap.get(targetNode) || EMPTY_SET;\n                return idSet.has(id);\n            }\n\n            function removeIdsFromConsideration(ctx, node) {\n                let idSet = ctx.idMap.get(node) || EMPTY_SET;\n                for (const id of idSet) {\n                    ctx.deadIds.add(id);\n                }\n            }\n\n            function getIdIntersectionCount(ctx, node1, node2) {\n                let sourceSet = ctx.idMap.get(node1) || EMPTY_SET;\n                let matchCount = 0;\n                for (const id of sourceSet) {\n                    // a potential match is an id in the source and potentialIdsSet, but\n                    // that has not already been merged into the DOM\n                    if (isIdInConsideration(ctx, id) && idIsWithinNode(ctx, id, node2)) {\n                        ++matchCount;\n                    }\n                }\n                return matchCount;\n            }\n\n            /**\n             * A bottom up algorithm that finds all elements with ids inside of the node\n             * argument and populates id sets for those nodes and all their parents, generating\n             * a set of ids contained within all nodes for the entire hierarchy in the DOM\n             *\n             * @param node {Element}\n             * @param {Map<Node, Set<String>>} idMap\n             */\n            function populateIdMapForNode(node, idMap) {\n                let nodeParent = node.parentElement;\n                // find all elements with an id property\n                let idElements = node.querySelectorAll('[id]');\n                for (const elt of idElements) {\n                    let current = elt;\n                    // walk up the parent hierarchy of that element, adding the id\n                    // of element to the parent's id set\n                    while (current !== nodeParent && current != null) {\n                        let idSet = idMap.get(current);\n                        // if the id set doesn't exist, create it and insert it in the  map\n                        if (idSet == null) {\n                            idSet = new Set();\n                            idMap.set(current, idSet);\n                        }\n                        idSet.add(elt.id);\n                        current = current.parentElement;\n                    }\n                }\n            }\n\n            /**\n             * This function computes a map of nodes to all ids contained within that node (inclusive of the\n             * node).  This map can be used to ask if two nodes have intersecting sets of ids, which allows\n             * for a looser definition of \"matching\" than tradition id matching, and allows child nodes\n             * to contribute to a parent nodes matching.\n             *\n             * @param {Element} oldContent  the old content that will be morphed\n             * @param {Element} newContent  the new content to morph to\n             * @returns {Map<Node, Set<String>>} a map of nodes to id sets for the\n             */\n            function createIdMap(oldContent, newContent) {\n                let idMap = new Map();\n                populateIdMapForNode(oldContent, idMap);\n                populateIdMapForNode(newContent, idMap);\n                return idMap;\n            }\n\n            //=============================================================================\n            // This is what ends up becoming the Idiomorph global object\n            //=============================================================================\n            return {\n                morph\n            }\n        })()\n    }));\n\n",
         "/*! *****************************************************************************\r\nCopyright (c) Microsoft Corporation. All rights reserved.\r\nLicensed under the Apache License, Version 2.0 (the \"License\"); you may not use\r\nthis file except in compliance with the License. You may obtain a copy of the\r\nLicense at http://www.apache.org/licenses/LICENSE-2.0\r\n\r\nTHIS CODE IS PROVIDED ON AN *AS IS* BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY\r\nKIND, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY IMPLIED\r\nWARRANTIES OR CONDITIONS OF TITLE, FITNESS FOR A PARTICULAR PURPOSE,\r\nMERCHANTABLITY OR NON-INFRINGEMENT.\r\n\r\nSee the Apache Version 2.0 License for specific language governing permissions\r\nand limitations under the License.\r\n***************************************************************************** */\r\n/* global Reflect, Promise */\r\n\r\nvar extendStatics = function(d, b) {\r\n    extendStatics = Object.setPrototypeOf ||\r\n        ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\r\n        function (d, b) { for (var p in b) if (b.hasOwnProperty(p)) d[p] = b[p]; };\r\n    return extendStatics(d, b);\r\n};\r\n\r\nfunction __extends(d, b) {\r\n    extendStatics(d, b);\r\n    function __() { this.constructor = d; }\r\n    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\r\n}\r\n\r\nfunction __values(o) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator], i = 0;\r\n    if (m) return m.call(o);\r\n    return {\r\n        next: function () {\r\n            if (o && i >= o.length) o = void 0;\r\n            return { value: o && o[i++], done: !o };\r\n        }\r\n    };\r\n}\r\n\r\nfunction __read(o, n) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator];\r\n    if (!m) return o;\r\n    var i = m.call(o), r, ar = [], e;\r\n    try {\r\n        while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\r\n    }\r\n    catch (error) { e = { error: error }; }\r\n    finally {\r\n        try {\r\n            if (r && !r.done && (m = i[\"return\"])) m.call(i);\r\n        }\r\n        finally { if (e) throw e.error; }\r\n    }\r\n    return ar;\r\n}\r\n\r\nfunction __spread() {\r\n    for (var ar = [], i = 0; i < arguments.length; i++)\r\n        ar = ar.concat(__read(arguments[i]));\r\n    return ar;\r\n}\n\nvar Event = /** @class */ (function () {\r\n    function Event(type, target) {\r\n        this.target = target;\r\n        this.type = type;\r\n    }\r\n    return Event;\r\n}());\r\nvar ErrorEvent = /** @class */ (function (_super) {\r\n    __extends(ErrorEvent, _super);\r\n    function ErrorEvent(error, target) {\r\n        var _this = _super.call(this, 'error', target) || this;\r\n        _this.message = error.message;\r\n        _this.error = error;\r\n        return _this;\r\n    }\r\n    return ErrorEvent;\r\n}(Event));\r\nvar CloseEvent = /** @class */ (function (_super) {\r\n    __extends(CloseEvent, _super);\r\n    function CloseEvent(code, reason, target) {\r\n        if (code === void 0) { code = 1000; }\r\n        if (reason === void 0) { reason = ''; }\r\n        var _this = _super.call(this, 'close', target) || this;\r\n        _this.wasClean = true;\r\n        _this.code = code;\r\n        _this.reason = reason;\r\n        return _this;\r\n    }\r\n    return CloseEvent;\r\n}(Event));\n\n/*!\r\n * Reconnecting WebSocket\r\n * by Pedro Ladaria <pedro.ladaria@gmail.com>\r\n * https://github.com/pladaria/reconnecting-websocket\r\n * License MIT\r\n */\r\nvar getGlobalWebSocket = function () {\r\n    if (typeof WebSocket !== 'undefined') {\r\n        // @ts-ignore\r\n        return WebSocket;\r\n    }\r\n};\r\n/**\r\n * Returns true if given argument looks like a WebSocket class\r\n */\r\nvar isWebSocket = function (w) { return typeof w !== 'undefined' && !!w && w.CLOSING === 2; };\r\nvar DEFAULT = {\r\n    maxReconnectionDelay: 10000,\r\n    minReconnectionDelay: 1000 + Math.random() * 4000,\r\n    minUptime: 5000,\r\n    reconnectionDelayGrowFactor: 1.3,\r\n    connectionTimeout: 4000,\r\n    maxRetries: Infinity,\r\n    maxEnqueuedMessages: Infinity,\r\n    startClosed: false,\r\n    debug: false,\r\n};\r\nvar ReconnectingWebSocket = /** @class */ (function () {\r\n    function ReconnectingWebSocket(url, protocols, options) {\r\n        var _this = this;\r\n        if (options === void 0) { options = {}; }\r\n        this._listeners = {\r\n            error: [],\r\n            message: [],\r\n            open: [],\r\n            close: [],\r\n        };\r\n        this._retryCount = -1;\r\n        this._shouldReconnect = true;\r\n        this._connectLock = false;\r\n        this._binaryType = 'blob';\r\n        this._closeCalled = false;\r\n        this._messageQueue = [];\r\n        /**\r\n         * An event listener to be called when the WebSocket connection's readyState changes to CLOSED\r\n         */\r\n        this.onclose = null;\r\n        /**\r\n         * An event listener to be called when an error occurs\r\n         */\r\n        this.onerror = null;\r\n        /**\r\n         * An event listener to be called when a message is received from the server\r\n         */\r\n        this.onmessage = null;\r\n        /**\r\n         * An event listener to be called when the WebSocket connection's readyState changes to OPEN;\r\n         * this indicates that the connection is ready to send and receive data\r\n         */\r\n        this.onopen = null;\r\n        this._handleOpen = function (event) {\r\n            _this._debug('open event');\r\n            var _a = _this._options.minUptime, minUptime = _a === void 0 ? DEFAULT.minUptime : _a;\r\n            clearTimeout(_this._connectTimeout);\r\n            _this._uptimeTimeout = setTimeout(function () { return _this._acceptOpen(); }, minUptime);\r\n            _this._ws.binaryType = _this._binaryType;\r\n            // send enqueued messages (messages sent before websocket open event)\r\n            _this._messageQueue.forEach(function (message) { return _this._ws.send(message); });\r\n            _this._messageQueue = [];\r\n            if (_this.onopen) {\r\n                _this.onopen(event);\r\n            }\r\n            _this._listeners.open.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._handleMessage = function (event) {\r\n            _this._debug('message event');\r\n            if (_this.onmessage) {\r\n                _this.onmessage(event);\r\n            }\r\n            _this._listeners.message.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._handleError = function (event) {\r\n            _this._debug('error event', event.message);\r\n            _this._disconnect(undefined, event.message === 'TIMEOUT' ? 'timeout' : undefined);\r\n            if (_this.onerror) {\r\n                _this.onerror(event);\r\n            }\r\n            _this._debug('exec error listeners');\r\n            _this._listeners.error.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n            _this._connect();\r\n        };\r\n        this._handleClose = function (event) {\r\n            _this._debug('close event');\r\n            _this._clearTimeouts();\r\n            if (_this._shouldReconnect) {\r\n                _this._connect();\r\n            }\r\n            if (_this.onclose) {\r\n                _this.onclose(event);\r\n            }\r\n            _this._listeners.close.forEach(function (listener) { return _this._callEventListener(event, listener); });\r\n        };\r\n        this._url = url;\r\n        this._protocols = protocols;\r\n        this._options = options;\r\n        if (this._options.startClosed) {\r\n            this._shouldReconnect = false;\r\n        }\r\n        this._connect();\r\n    }\r\n    Object.defineProperty(ReconnectingWebSocket, \"CONNECTING\", {\r\n        get: function () {\r\n            return 0;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"OPEN\", {\r\n        get: function () {\r\n            return 1;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"CLOSING\", {\r\n        get: function () {\r\n            return 2;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket, \"CLOSED\", {\r\n        get: function () {\r\n            return 3;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CONNECTING\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CONNECTING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"OPEN\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.OPEN;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CLOSING\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CLOSING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"CLOSED\", {\r\n        get: function () {\r\n            return ReconnectingWebSocket.CLOSED;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"binaryType\", {\r\n        get: function () {\r\n            return this._ws ? this._ws.binaryType : this._binaryType;\r\n        },\r\n        set: function (value) {\r\n            this._binaryType = value;\r\n            if (this._ws) {\r\n                this._ws.binaryType = value;\r\n            }\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"retryCount\", {\r\n        /**\r\n         * Returns the number or connection retries\r\n         */\r\n        get: function () {\r\n            return Math.max(this._retryCount, 0);\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"bufferedAmount\", {\r\n        /**\r\n         * The number of bytes of data that have been queued using calls to send() but not yet\r\n         * transmitted to the network. This value resets to zero once all queued data has been sent.\r\n         * This value does not reset to zero when the connection is closed; if you keep calling send(),\r\n         * this will continue to climb. Read only\r\n         */\r\n        get: function () {\r\n            var bytes = this._messageQueue.reduce(function (acc, message) {\r\n                if (typeof message === 'string') {\r\n                    acc += message.length; // not byte size\r\n                }\r\n                else if (message instanceof Blob) {\r\n                    acc += message.size;\r\n                }\r\n                else {\r\n                    acc += message.byteLength;\r\n                }\r\n                return acc;\r\n            }, 0);\r\n            return bytes + (this._ws ? this._ws.bufferedAmount : 0);\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"extensions\", {\r\n        /**\r\n         * The extensions selected by the server. This is currently only the empty string or a list of\r\n         * extensions as negotiated by the connection\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.extensions : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"protocol\", {\r\n        /**\r\n         * A string indicating the name of the sub-protocol the server selected;\r\n         * this will be one of the strings specified in the protocols parameter when creating the\r\n         * WebSocket object\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.protocol : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"readyState\", {\r\n        /**\r\n         * The current state of the connection; this is one of the Ready state constants\r\n         */\r\n        get: function () {\r\n            if (this._ws) {\r\n                return this._ws.readyState;\r\n            }\r\n            return this._options.startClosed\r\n                ? ReconnectingWebSocket.CLOSED\r\n                : ReconnectingWebSocket.CONNECTING;\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    Object.defineProperty(ReconnectingWebSocket.prototype, \"url\", {\r\n        /**\r\n         * The URL as resolved by the constructor\r\n         */\r\n        get: function () {\r\n            return this._ws ? this._ws.url : '';\r\n        },\r\n        enumerable: true,\r\n        configurable: true\r\n    });\r\n    /**\r\n     * Closes the WebSocket connection or connection attempt, if any. If the connection is already\r\n     * CLOSED, this method does nothing\r\n     */\r\n    ReconnectingWebSocket.prototype.close = function (code, reason) {\r\n        if (code === void 0) { code = 1000; }\r\n        this._closeCalled = true;\r\n        this._shouldReconnect = false;\r\n        this._clearTimeouts();\r\n        if (!this._ws) {\r\n            this._debug('close enqueued: no ws instance');\r\n            return;\r\n        }\r\n        if (this._ws.readyState === this.CLOSED) {\r\n            this._debug('close: already closed');\r\n            return;\r\n        }\r\n        this._ws.close(code, reason);\r\n    };\r\n    /**\r\n     * Closes the WebSocket connection or connection attempt and connects again.\r\n     * Resets retry counter;\r\n     */\r\n    ReconnectingWebSocket.prototype.reconnect = function (code, reason) {\r\n        this._shouldReconnect = true;\r\n        this._closeCalled = false;\r\n        this._retryCount = -1;\r\n        if (!this._ws || this._ws.readyState === this.CLOSED) {\r\n            this._connect();\r\n        }\r\n        else {\r\n            this._disconnect(code, reason);\r\n            this._connect();\r\n        }\r\n    };\r\n    /**\r\n     * Enqueue specified data to be transmitted to the server over the WebSocket connection\r\n     */\r\n    ReconnectingWebSocket.prototype.send = function (data) {\r\n        if (this._ws && this._ws.readyState === this.OPEN) {\r\n            this._debug('send', data);\r\n            this._ws.send(data);\r\n        }\r\n        else {\r\n            var _a = this._options.maxEnqueuedMessages, maxEnqueuedMessages = _a === void 0 ? DEFAULT.maxEnqueuedMessages : _a;\r\n            if (this._messageQueue.length < maxEnqueuedMessages) {\r\n                this._debug('enqueue', data);\r\n                this._messageQueue.push(data);\r\n            }\r\n        }\r\n    };\r\n    /**\r\n     * Register an event handler of a specific event type\r\n     */\r\n    ReconnectingWebSocket.prototype.addEventListener = function (type, listener) {\r\n        if (this._listeners[type]) {\r\n            // @ts-ignore\r\n            this._listeners[type].push(listener);\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype.dispatchEvent = function (event) {\r\n        var e_1, _a;\r\n        var listeners = this._listeners[event.type];\r\n        if (listeners) {\r\n            try {\r\n                for (var listeners_1 = __values(listeners), listeners_1_1 = listeners_1.next(); !listeners_1_1.done; listeners_1_1 = listeners_1.next()) {\r\n                    var listener = listeners_1_1.value;\r\n                    this._callEventListener(event, listener);\r\n                }\r\n            }\r\n            catch (e_1_1) { e_1 = { error: e_1_1 }; }\r\n            finally {\r\n                try {\r\n                    if (listeners_1_1 && !listeners_1_1.done && (_a = listeners_1.return)) _a.call(listeners_1);\r\n                }\r\n                finally { if (e_1) throw e_1.error; }\r\n            }\r\n        }\r\n        return true;\r\n    };\r\n    /**\r\n     * Removes an event listener\r\n     */\r\n    ReconnectingWebSocket.prototype.removeEventListener = function (type, listener) {\r\n        if (this._listeners[type]) {\r\n            // @ts-ignore\r\n            this._listeners[type] = this._listeners[type].filter(function (l) { return l !== listener; });\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._debug = function () {\r\n        var args = [];\r\n        for (var _i = 0; _i < arguments.length; _i++) {\r\n            args[_i] = arguments[_i];\r\n        }\r\n        if (this._options.debug) {\r\n            // not using spread because compiled version uses Symbols\r\n            // tslint:disable-next-line\r\n            console.log.apply(console, __spread(['RWS>'], args));\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._getNextDelay = function () {\r\n        var _a = this._options, _b = _a.reconnectionDelayGrowFactor, reconnectionDelayGrowFactor = _b === void 0 ? DEFAULT.reconnectionDelayGrowFactor : _b, _c = _a.minReconnectionDelay, minReconnectionDelay = _c === void 0 ? DEFAULT.minReconnectionDelay : _c, _d = _a.maxReconnectionDelay, maxReconnectionDelay = _d === void 0 ? DEFAULT.maxReconnectionDelay : _d;\r\n        var delay = 0;\r\n        if (this._retryCount > 0) {\r\n            delay =\r\n                minReconnectionDelay * Math.pow(reconnectionDelayGrowFactor, this._retryCount - 1);\r\n            if (delay > maxReconnectionDelay) {\r\n                delay = maxReconnectionDelay;\r\n            }\r\n        }\r\n        this._debug('next delay', delay);\r\n        return delay;\r\n    };\r\n    ReconnectingWebSocket.prototype._wait = function () {\r\n        var _this = this;\r\n        return new Promise(function (resolve) {\r\n            setTimeout(resolve, _this._getNextDelay());\r\n        });\r\n    };\r\n    ReconnectingWebSocket.prototype._getNextUrl = function (urlProvider) {\r\n        if (typeof urlProvider === 'string') {\r\n            return Promise.resolve(urlProvider);\r\n        }\r\n        if (typeof urlProvider === 'function') {\r\n            var url = urlProvider();\r\n            if (typeof url === 'string') {\r\n                return Promise.resolve(url);\r\n            }\r\n            if (!!url.then) {\r\n                return url;\r\n            }\r\n        }\r\n        throw Error('Invalid URL');\r\n    };\r\n    ReconnectingWebSocket.prototype._connect = function () {\r\n        var _this = this;\r\n        if (this._connectLock || !this._shouldReconnect) {\r\n            return;\r\n        }\r\n        this._connectLock = true;\r\n        var _a = this._options, _b = _a.maxRetries, maxRetries = _b === void 0 ? DEFAULT.maxRetries : _b, _c = _a.connectionTimeout, connectionTimeout = _c === void 0 ? DEFAULT.connectionTimeout : _c, _d = _a.WebSocket, WebSocket = _d === void 0 ? getGlobalWebSocket() : _d;\r\n        if (this._retryCount >= maxRetries) {\r\n            this._debug('max retries reached', this._retryCount, '>=', maxRetries);\r\n            return;\r\n        }\r\n        this._retryCount++;\r\n        this._debug('connect', this._retryCount);\r\n        this._removeListeners();\r\n        if (!isWebSocket(WebSocket)) {\r\n            throw Error('No valid WebSocket class provided');\r\n        }\r\n        this._wait()\r\n            .then(function () { return _this._getNextUrl(_this._url); })\r\n            .then(function (url) {\r\n            // close could be called before creating the ws\r\n            if (_this._closeCalled) {\r\n                return;\r\n            }\r\n            _this._debug('connect', { url: url, protocols: _this._protocols });\r\n            _this._ws = _this._protocols\r\n                ? new WebSocket(url, _this._protocols)\r\n                : new WebSocket(url);\r\n            _this._ws.binaryType = _this._binaryType;\r\n            _this._connectLock = false;\r\n            _this._addListeners();\r\n            _this._connectTimeout = setTimeout(function () { return _this._handleTimeout(); }, connectionTimeout);\r\n        });\r\n    };\r\n    ReconnectingWebSocket.prototype._handleTimeout = function () {\r\n        this._debug('timeout event');\r\n        this._handleError(new ErrorEvent(Error('TIMEOUT'), this));\r\n    };\r\n    ReconnectingWebSocket.prototype._disconnect = function (code, reason) {\r\n        if (code === void 0) { code = 1000; }\r\n        this._clearTimeouts();\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._removeListeners();\r\n        try {\r\n            this._ws.close(code, reason);\r\n            this._handleClose(new CloseEvent(code, reason, this));\r\n        }\r\n        catch (error) {\r\n            // ignore\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._acceptOpen = function () {\r\n        this._debug('accept open');\r\n        this._retryCount = 0;\r\n    };\r\n    ReconnectingWebSocket.prototype._callEventListener = function (event, listener) {\r\n        if ('handleEvent' in listener) {\r\n            // @ts-ignore\r\n            listener.handleEvent(event);\r\n        }\r\n        else {\r\n            // @ts-ignore\r\n            listener(event);\r\n        }\r\n    };\r\n    ReconnectingWebSocket.prototype._removeListeners = function () {\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._debug('removeListeners');\r\n        this._ws.removeEventListener('open', this._handleOpen);\r\n        this._ws.removeEventListener('close', this._handleClose);\r\n        this._ws.removeEventListener('message', this._handleMessage);\r\n        // @ts-ignore\r\n        this._ws.removeEventListener('error', this._handleError);\r\n    };\r\n    ReconnectingWebSocket.prototype._addListeners = function () {\r\n        if (!this._ws) {\r\n            return;\r\n        }\r\n        this._debug('addListeners');\r\n        this._ws.addEventListener('open', this._handleOpen);\r\n        this._ws.addEventListener('close', this._handleClose);\r\n        this._ws.addEventListener('message', this._handleMessage);\r\n        // @ts-ignore\r\n        this._ws.addEventListener('error', this._handleError);\r\n    };\r\n    ReconnectingWebSocket.prototype._clearTimeouts = function () {\r\n        clearTimeout(this._connectTimeout);\r\n        clearTimeout(this._uptimeTimeout);\r\n    };\r\n    return ReconnectingWebSocket;\r\n}());\n\nexport default ReconnectingWebSocket;\n",
-        "var DOCUMENT_FRAGMENT_NODE = 11;\n\nfunction morphAttrs(fromNode, toNode) {\n    var toNodeAttrs = toNode.attributes;\n    var attr;\n    var attrName;\n    var attrNamespaceURI;\n    var attrValue;\n    var fromValue;\n\n    // document-fragments dont have attributes so lets not do anything\n    if (toNode.nodeType === DOCUMENT_FRAGMENT_NODE || fromNode.nodeType === DOCUMENT_FRAGMENT_NODE) {\n      return;\n    }\n\n    // update attributes on original DOM element\n    for (var i = toNodeAttrs.length - 1; i >= 0; i--) {\n        attr = toNodeAttrs[i];\n        attrName = attr.name;\n        attrNamespaceURI = attr.namespaceURI;\n        attrValue = attr.value;\n\n        if (attrNamespaceURI) {\n            attrName = attr.localName || attrName;\n            fromValue = fromNode.getAttributeNS(attrNamespaceURI, attrName);\n\n            if (fromValue !== attrValue) {\n                if (attr.prefix === 'xmlns'){\n                    attrName = attr.name; // It's not allowed to set an attribute with the XMLNS namespace without specifying the `xmlns` prefix\n                }\n                fromNode.setAttributeNS(attrNamespaceURI, attrName, attrValue);\n            }\n        } else {\n            fromValue = fromNode.getAttribute(attrName);\n\n            if (fromValue !== attrValue) {\n                fromNode.setAttribute(attrName, attrValue);\n            }\n        }\n    }\n\n    // Remove any extra attributes found on the original DOM element that\n    // weren't found on the target element.\n    var fromNodeAttrs = fromNode.attributes;\n\n    for (var d = fromNodeAttrs.length - 1; d >= 0; d--) {\n        attr = fromNodeAttrs[d];\n        attrName = attr.name;\n        attrNamespaceURI = attr.namespaceURI;\n\n        if (attrNamespaceURI) {\n            attrName = attr.localName || attrName;\n\n            if (!toNode.hasAttributeNS(attrNamespaceURI, attrName)) {\n                fromNode.removeAttributeNS(attrNamespaceURI, attrName);\n            }\n        } else {\n            if (!toNode.hasAttribute(attrName)) {\n                fromNode.removeAttribute(attrName);\n            }\n        }\n    }\n}\n\nvar range; // Create a range object for efficently rendering strings to elements.\nvar NS_XHTML = 'http://www.w3.org/1999/xhtml';\n\nvar doc = typeof document === 'undefined' ? undefined : document;\nvar HAS_TEMPLATE_SUPPORT = !!doc && 'content' in doc.createElement('template');\nvar HAS_RANGE_SUPPORT = !!doc && doc.createRange && 'createContextualFragment' in doc.createRange();\n\nfunction createFragmentFromTemplate(str) {\n    var template = doc.createElement('template');\n    template.innerHTML = str;\n    return template.content.childNodes[0];\n}\n\nfunction createFragmentFromRange(str) {\n    if (!range) {\n        range = doc.createRange();\n        range.selectNode(doc.body);\n    }\n\n    var fragment = range.createContextualFragment(str);\n    return fragment.childNodes[0];\n}\n\nfunction createFragmentFromWrap(str) {\n    var fragment = doc.createElement('body');\n    fragment.innerHTML = str;\n    return fragment.childNodes[0];\n}\n\n/**\n * This is about the same\n * var html = new DOMParser().parseFromString(str, 'text/html');\n * return html.body.firstChild;\n *\n * @method toElement\n * @param {String} str\n */\nfunction toElement(str) {\n    str = str.trim();\n    if (HAS_TEMPLATE_SUPPORT) {\n      // avoid restrictions on content for things like `<tr><th>Hi</th></tr>` which\n      // createContextualFragment doesn't support\n      // <template> support not available in IE\n      return createFragmentFromTemplate(str);\n    } else if (HAS_RANGE_SUPPORT) {\n      return createFragmentFromRange(str);\n    }\n\n    return createFragmentFromWrap(str);\n}\n\n/**\n * Returns true if two node's names are the same.\n *\n * NOTE: We don't bother checking `namespaceURI` because you will never find two HTML elements with the same\n *       nodeName and different namespace URIs.\n *\n * @param {Element} a\n * @param {Element} b The target element\n * @return {boolean}\n */\nfunction compareNodeNames(fromEl, toEl) {\n    var fromNodeName = fromEl.nodeName;\n    var toNodeName = toEl.nodeName;\n    var fromCodeStart, toCodeStart;\n\n    if (fromNodeName === toNodeName) {\n        return true;\n    }\n\n    fromCodeStart = fromNodeName.charCodeAt(0);\n    toCodeStart = toNodeName.charCodeAt(0);\n\n    // If the target element is a virtual DOM node or SVG node then we may\n    // need to normalize the tag name before comparing. Normal HTML elements that are\n    // in the \"http://www.w3.org/1999/xhtml\"\n    // are converted to upper case\n    if (fromCodeStart <= 90 && toCodeStart >= 97) { // from is upper and to is lower\n        return fromNodeName === toNodeName.toUpperCase();\n    } else if (toCodeStart <= 90 && fromCodeStart >= 97) { // to is upper and from is lower\n        return toNodeName === fromNodeName.toUpperCase();\n    } else {\n        return false;\n    }\n}\n\n/**\n * Create an element, optionally with a known namespace URI.\n *\n * @param {string} name the element name, e.g. 'div' or 'svg'\n * @param {string} [namespaceURI] the element's namespace URI, i.e. the value of\n * its `xmlns` attribute or its inferred namespace.\n *\n * @return {Element}\n */\nfunction createElementNS(name, namespaceURI) {\n    return !namespaceURI || namespaceURI === NS_XHTML ?\n        doc.createElement(name) :\n        doc.createElementNS(namespaceURI, name);\n}\n\n/**\n * Copies the children of one DOM element to another DOM element\n */\nfunction moveChildren(fromEl, toEl) {\n    var curChild = fromEl.firstChild;\n    while (curChild) {\n        var nextChild = curChild.nextSibling;\n        toEl.appendChild(curChild);\n        curChild = nextChild;\n    }\n    return toEl;\n}\n\nfunction syncBooleanAttrProp(fromEl, toEl, name) {\n    if (fromEl[name] !== toEl[name]) {\n        fromEl[name] = toEl[name];\n        if (fromEl[name]) {\n            fromEl.setAttribute(name, '');\n        } else {\n            fromEl.removeAttribute(name);\n        }\n    }\n}\n\nvar specialElHandlers = {\n    OPTION: function(fromEl, toEl) {\n        var parentNode = fromEl.parentNode;\n        if (parentNode) {\n            var parentName = parentNode.nodeName.toUpperCase();\n            if (parentName === 'OPTGROUP') {\n                parentNode = parentNode.parentNode;\n                parentName = parentNode && parentNode.nodeName.toUpperCase();\n            }\n            if (parentName === 'SELECT' && !parentNode.hasAttribute('multiple')) {\n                if (fromEl.hasAttribute('selected') && !toEl.selected) {\n                    // Workaround for MS Edge bug where the 'selected' attribute can only be\n                    // removed if set to a non-empty value:\n                    // https://developer.microsoft.com/en-us/microsoft-edge/platform/issues/12087679/\n                    fromEl.setAttribute('selected', 'selected');\n                    fromEl.removeAttribute('selected');\n                }\n                // We have to reset select element's selectedIndex to -1, otherwise setting\n                // fromEl.selected using the syncBooleanAttrProp below has no effect.\n                // The correct selectedIndex will be set in the SELECT special handler below.\n                parentNode.selectedIndex = -1;\n            }\n        }\n        syncBooleanAttrProp(fromEl, toEl, 'selected');\n    },\n    /**\n     * The \"value\" attribute is special for the <input> element since it sets\n     * the initial value. Changing the \"value\" attribute without changing the\n     * \"value\" property will have no effect since it is only used to the set the\n     * initial value.  Similar for the \"checked\" attribute, and \"disabled\".\n     */\n    INPUT: function(fromEl, toEl) {\n        syncBooleanAttrProp(fromEl, toEl, 'checked');\n        syncBooleanAttrProp(fromEl, toEl, 'disabled');\n\n        if (fromEl.value !== toEl.value) {\n            fromEl.value = toEl.value;\n        }\n\n        if (!toEl.hasAttribute('value')) {\n            fromEl.removeAttribute('value');\n        }\n    },\n\n    TEXTAREA: function(fromEl, toEl) {\n        var newValue = toEl.value;\n        if (fromEl.value !== newValue) {\n            fromEl.value = newValue;\n        }\n\n        var firstChild = fromEl.firstChild;\n        if (firstChild) {\n            // Needed for IE. Apparently IE sets the placeholder as the\n            // node value and vise versa. This ignores an empty update.\n            var oldValue = firstChild.nodeValue;\n\n            if (oldValue == newValue || (!newValue && oldValue == fromEl.placeholder)) {\n                return;\n            }\n\n            firstChild.nodeValue = newValue;\n        }\n    },\n    SELECT: function(fromEl, toEl) {\n        if (!toEl.hasAttribute('multiple')) {\n            var selectedIndex = -1;\n            var i = 0;\n            // We have to loop through children of fromEl, not toEl since nodes can be moved\n            // from toEl to fromEl directly when morphing.\n            // At the time this special handler is invoked, all children have already been morphed\n            // and appended to / removed from fromEl, so using fromEl here is safe and correct.\n            var curChild = fromEl.firstChild;\n            var optgroup;\n            var nodeName;\n            while(curChild) {\n                nodeName = curChild.nodeName && curChild.nodeName.toUpperCase();\n                if (nodeName === 'OPTGROUP') {\n                    optgroup = curChild;\n                    curChild = optgroup.firstChild;\n                } else {\n                    if (nodeName === 'OPTION') {\n                        if (curChild.hasAttribute('selected')) {\n                            selectedIndex = i;\n                            break;\n                        }\n                        i++;\n                    }\n                    curChild = curChild.nextSibling;\n                    if (!curChild && optgroup) {\n                        curChild = optgroup.nextSibling;\n                        optgroup = null;\n                    }\n                }\n            }\n\n            fromEl.selectedIndex = selectedIndex;\n        }\n    }\n};\n\nvar ELEMENT_NODE = 1;\nvar DOCUMENT_FRAGMENT_NODE$1 = 11;\nvar TEXT_NODE = 3;\nvar COMMENT_NODE = 8;\n\nfunction noop() {}\n\nfunction defaultGetNodeKey(node) {\n  if (node) {\n    return (node.getAttribute && node.getAttribute('id')) || node.id;\n  }\n}\n\nfunction morphdomFactory(morphAttrs) {\n\n  return function morphdom(fromNode, toNode, options) {\n    if (!options) {\n      options = {};\n    }\n\n    if (typeof toNode === 'string') {\n      if (fromNode.nodeName === '#document' || fromNode.nodeName === 'HTML' || fromNode.nodeName === 'BODY') {\n        var toNodeHtml = toNode;\n        toNode = doc.createElement('html');\n        toNode.innerHTML = toNodeHtml;\n      } else {\n        toNode = toElement(toNode);\n      }\n    } else if (toNode.nodeType === DOCUMENT_FRAGMENT_NODE$1) {\n      toNode = toNode.firstElementChild;\n    }\n\n    var getNodeKey = options.getNodeKey || defaultGetNodeKey;\n    var onBeforeNodeAdded = options.onBeforeNodeAdded || noop;\n    var onNodeAdded = options.onNodeAdded || noop;\n    var onBeforeElUpdated = options.onBeforeElUpdated || noop;\n    var onElUpdated = options.onElUpdated || noop;\n    var onBeforeNodeDiscarded = options.onBeforeNodeDiscarded || noop;\n    var onNodeDiscarded = options.onNodeDiscarded || noop;\n    var onBeforeElChildrenUpdated = options.onBeforeElChildrenUpdated || noop;\n    var skipFromChildren = options.skipFromChildren || noop;\n    var addChild = options.addChild || function(parent, child){ return parent.appendChild(child); };\n    var childrenOnly = options.childrenOnly === true;\n\n    // This object is used as a lookup to quickly find all keyed elements in the original DOM tree.\n    var fromNodesLookup = Object.create(null);\n    var keyedRemovalList = [];\n\n    function addKeyedRemoval(key) {\n      keyedRemovalList.push(key);\n    }\n\n    function walkDiscardedChildNodes(node, skipKeyedNodes) {\n      if (node.nodeType === ELEMENT_NODE) {\n        var curChild = node.firstChild;\n        while (curChild) {\n\n          var key = undefined;\n\n          if (skipKeyedNodes && (key = getNodeKey(curChild))) {\n            // If we are skipping keyed nodes then we add the key\n            // to a list so that it can be handled at the very end.\n            addKeyedRemoval(key);\n          } else {\n            // Only report the node as discarded if it is not keyed. We do this because\n            // at the end we loop through all keyed elements that were unmatched\n            // and then discard them in one final pass.\n            onNodeDiscarded(curChild);\n            if (curChild.firstChild) {\n              walkDiscardedChildNodes(curChild, skipKeyedNodes);\n            }\n          }\n\n          curChild = curChild.nextSibling;\n        }\n      }\n    }\n\n    /**\n    * Removes a DOM node out of the original DOM\n    *\n    * @param  {Node} node The node to remove\n    * @param  {Node} parentNode The nodes parent\n    * @param  {Boolean} skipKeyedNodes If true then elements with keys will be skipped and not discarded.\n    * @return {undefined}\n    */\n    function removeNode(node, parentNode, skipKeyedNodes) {\n      if (onBeforeNodeDiscarded(node) === false) {\n        return;\n      }\n\n      if (parentNode) {\n        parentNode.removeChild(node);\n      }\n\n      onNodeDiscarded(node);\n      walkDiscardedChildNodes(node, skipKeyedNodes);\n    }\n\n    // // TreeWalker implementation is no faster, but keeping this around in case this changes in the future\n    // function indexTree(root) {\n    //     var treeWalker = document.createTreeWalker(\n    //         root,\n    //         NodeFilter.SHOW_ELEMENT);\n    //\n    //     var el;\n    //     while((el = treeWalker.nextNode())) {\n    //         var key = getNodeKey(el);\n    //         if (key) {\n    //             fromNodesLookup[key] = el;\n    //         }\n    //     }\n    // }\n\n    // // NodeIterator implementation is no faster, but keeping this around in case this changes in the future\n    //\n    // function indexTree(node) {\n    //     var nodeIterator = document.createNodeIterator(node, NodeFilter.SHOW_ELEMENT);\n    //     var el;\n    //     while((el = nodeIterator.nextNode())) {\n    //         var key = getNodeKey(el);\n    //         if (key) {\n    //             fromNodesLookup[key] = el;\n    //         }\n    //     }\n    // }\n\n    function indexTree(node) {\n      if (node.nodeType === ELEMENT_NODE || node.nodeType === DOCUMENT_FRAGMENT_NODE$1) {\n        var curChild = node.firstChild;\n        while (curChild) {\n          var key = getNodeKey(curChild);\n          if (key) {\n            fromNodesLookup[key] = curChild;\n          }\n\n          // Walk recursively\n          indexTree(curChild);\n\n          curChild = curChild.nextSibling;\n        }\n      }\n    }\n\n    indexTree(fromNode);\n\n    function handleNodeAdded(el) {\n      onNodeAdded(el);\n\n      var curChild = el.firstChild;\n      while (curChild) {\n        var nextSibling = curChild.nextSibling;\n\n        var key = getNodeKey(curChild);\n        if (key) {\n          var unmatchedFromEl = fromNodesLookup[key];\n          // if we find a duplicate #id node in cache, replace `el` with cache value\n          // and morph it to the child node.\n          if (unmatchedFromEl && compareNodeNames(curChild, unmatchedFromEl)) {\n            curChild.parentNode.replaceChild(unmatchedFromEl, curChild);\n            morphEl(unmatchedFromEl, curChild);\n          } else {\n            handleNodeAdded(curChild);\n          }\n        } else {\n          // recursively call for curChild and it's children to see if we find something in\n          // fromNodesLookup\n          handleNodeAdded(curChild);\n        }\n\n        curChild = nextSibling;\n      }\n    }\n\n    function cleanupFromEl(fromEl, curFromNodeChild, curFromNodeKey) {\n      // We have processed all of the \"to nodes\". If curFromNodeChild is\n      // non-null then we still have some from nodes left over that need\n      // to be removed\n      while (curFromNodeChild) {\n        var fromNextSibling = curFromNodeChild.nextSibling;\n        if ((curFromNodeKey = getNodeKey(curFromNodeChild))) {\n          // Since the node is keyed it might be matched up later so we defer\n          // the actual removal to later\n          addKeyedRemoval(curFromNodeKey);\n        } else {\n          // NOTE: we skip nested keyed nodes from being removed since there is\n          //       still a chance they will be matched up later\n          removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n        }\n        curFromNodeChild = fromNextSibling;\n      }\n    }\n\n    function morphEl(fromEl, toEl, childrenOnly) {\n      var toElKey = getNodeKey(toEl);\n\n      if (toElKey) {\n        // If an element with an ID is being morphed then it will be in the final\n        // DOM so clear it out of the saved elements collection\n        delete fromNodesLookup[toElKey];\n      }\n\n      if (!childrenOnly) {\n        // optional\n        if (onBeforeElUpdated(fromEl, toEl) === false) {\n          return;\n        }\n\n        // update attributes on original DOM element first\n        morphAttrs(fromEl, toEl);\n        // optional\n        onElUpdated(fromEl);\n\n        if (onBeforeElChildrenUpdated(fromEl, toEl) === false) {\n          return;\n        }\n      }\n\n      if (fromEl.nodeName !== 'TEXTAREA') {\n        morphChildren(fromEl, toEl);\n      } else {\n        specialElHandlers.TEXTAREA(fromEl, toEl);\n      }\n    }\n\n    function morphChildren(fromEl, toEl) {\n      var skipFrom = skipFromChildren(fromEl);\n      var curToNodeChild = toEl.firstChild;\n      var curFromNodeChild = fromEl.firstChild;\n      var curToNodeKey;\n      var curFromNodeKey;\n\n      var fromNextSibling;\n      var toNextSibling;\n      var matchingFromEl;\n\n      // walk the children\n      outer: while (curToNodeChild) {\n        toNextSibling = curToNodeChild.nextSibling;\n        curToNodeKey = getNodeKey(curToNodeChild);\n\n        // walk the fromNode children all the way through\n        while (!skipFrom && curFromNodeChild) {\n          fromNextSibling = curFromNodeChild.nextSibling;\n\n          if (curToNodeChild.isSameNode && curToNodeChild.isSameNode(curFromNodeChild)) {\n            curToNodeChild = toNextSibling;\n            curFromNodeChild = fromNextSibling;\n            continue outer;\n          }\n\n          curFromNodeKey = getNodeKey(curFromNodeChild);\n\n          var curFromNodeType = curFromNodeChild.nodeType;\n\n          // this means if the curFromNodeChild doesnt have a match with the curToNodeChild\n          var isCompatible = undefined;\n\n          if (curFromNodeType === curToNodeChild.nodeType) {\n            if (curFromNodeType === ELEMENT_NODE) {\n              // Both nodes being compared are Element nodes\n\n              if (curToNodeKey) {\n                // The target node has a key so we want to match it up with the correct element\n                // in the original DOM tree\n                if (curToNodeKey !== curFromNodeKey) {\n                  // The current element in the original DOM tree does not have a matching key so\n                  // let's check our lookup to see if there is a matching element in the original\n                  // DOM tree\n                  if ((matchingFromEl = fromNodesLookup[curToNodeKey])) {\n                    if (fromNextSibling === matchingFromEl) {\n                      // Special case for single element removals. To avoid removing the original\n                      // DOM node out of the tree (since that can break CSS transitions, etc.),\n                      // we will instead discard the current node and wait until the next\n                      // iteration to properly match up the keyed target element with its matching\n                      // element in the original tree\n                      isCompatible = false;\n                    } else {\n                      // We found a matching keyed element somewhere in the original DOM tree.\n                      // Let's move the original DOM node into the current position and morph\n                      // it.\n\n                      // NOTE: We use insertBefore instead of replaceChild because we want to go through\n                      // the `removeNode()` function for the node that is being discarded so that\n                      // all lifecycle hooks are correctly invoked\n                      fromEl.insertBefore(matchingFromEl, curFromNodeChild);\n\n                      // fromNextSibling = curFromNodeChild.nextSibling;\n\n                      if (curFromNodeKey) {\n                        // Since the node is keyed it might be matched up later so we defer\n                        // the actual removal to later\n                        addKeyedRemoval(curFromNodeKey);\n                      } else {\n                        // NOTE: we skip nested keyed nodes from being removed since there is\n                        //       still a chance they will be matched up later\n                        removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n                      }\n\n                      curFromNodeChild = matchingFromEl;\n                    }\n                  } else {\n                    // The nodes are not compatible since the \"to\" node has a key and there\n                    // is no matching keyed node in the source tree\n                    isCompatible = false;\n                  }\n                }\n              } else if (curFromNodeKey) {\n                // The original has a key\n                isCompatible = false;\n              }\n\n              isCompatible = isCompatible !== false && compareNodeNames(curFromNodeChild, curToNodeChild);\n              if (isCompatible) {\n                // We found compatible DOM elements so transform\n                // the current \"from\" node to match the current\n                // target DOM node.\n                // MORPH\n                morphEl(curFromNodeChild, curToNodeChild);\n              }\n\n            } else if (curFromNodeType === TEXT_NODE || curFromNodeType == COMMENT_NODE) {\n              // Both nodes being compared are Text or Comment nodes\n              isCompatible = true;\n              // Simply update nodeValue on the original node to\n              // change the text value\n              if (curFromNodeChild.nodeValue !== curToNodeChild.nodeValue) {\n                curFromNodeChild.nodeValue = curToNodeChild.nodeValue;\n              }\n\n            }\n          }\n\n          if (isCompatible) {\n            // Advance both the \"to\" child and the \"from\" child since we found a match\n            // Nothing else to do as we already recursively called morphChildren above\n            curToNodeChild = toNextSibling;\n            curFromNodeChild = fromNextSibling;\n            continue outer;\n          }\n\n          // No compatible match so remove the old node from the DOM and continue trying to find a\n          // match in the original DOM. However, we only do this if the from node is not keyed\n          // since it is possible that a keyed node might match up with a node somewhere else in the\n          // target tree and we don't want to discard it just yet since it still might find a\n          // home in the final DOM tree. After everything is done we will remove any keyed nodes\n          // that didn't find a home\n          if (curFromNodeKey) {\n            // Since the node is keyed it might be matched up later so we defer\n            // the actual removal to later\n            addKeyedRemoval(curFromNodeKey);\n          } else {\n            // NOTE: we skip nested keyed nodes from being removed since there is\n            //       still a chance they will be matched up later\n            removeNode(curFromNodeChild, fromEl, true /* skip keyed nodes */);\n          }\n\n          curFromNodeChild = fromNextSibling;\n        } // END: while(curFromNodeChild) {}\n\n        // If we got this far then we did not find a candidate match for\n        // our \"to node\" and we exhausted all of the children \"from\"\n        // nodes. Therefore, we will just append the current \"to\" node\n        // to the end\n        if (curToNodeKey && (matchingFromEl = fromNodesLookup[curToNodeKey]) && compareNodeNames(matchingFromEl, curToNodeChild)) {\n          // MORPH\n          if(!skipFrom){ addChild(fromEl, matchingFromEl); }\n          morphEl(matchingFromEl, curToNodeChild);\n        } else {\n          var onBeforeNodeAddedResult = onBeforeNodeAdded(curToNodeChild);\n          if (onBeforeNodeAddedResult !== false) {\n            if (onBeforeNodeAddedResult) {\n              curToNodeChild = onBeforeNodeAddedResult;\n            }\n\n            if (curToNodeChild.actualize) {\n              curToNodeChild = curToNodeChild.actualize(fromEl.ownerDocument || doc);\n            }\n            addChild(fromEl, curToNodeChild);\n            handleNodeAdded(curToNodeChild);\n          }\n        }\n\n        curToNodeChild = toNextSibling;\n        curFromNodeChild = fromNextSibling;\n      }\n\n      cleanupFromEl(fromEl, curFromNodeChild, curFromNodeKey);\n\n      var specialElHandler = specialElHandlers[fromEl.nodeName];\n      if (specialElHandler) {\n        specialElHandler(fromEl, toEl);\n      }\n    } // END: morphChildren(...)\n\n    var morphedNode = fromNode;\n    var morphedNodeType = morphedNode.nodeType;\n    var toNodeType = toNode.nodeType;\n\n    if (!childrenOnly) {\n      // Handle the case where we are given two DOM nodes that are not\n      // compatible (e.g. <div> --> <span> or <div> --> TEXT)\n      if (morphedNodeType === ELEMENT_NODE) {\n        if (toNodeType === ELEMENT_NODE) {\n          if (!compareNodeNames(fromNode, toNode)) {\n            onNodeDiscarded(fromNode);\n            morphedNode = moveChildren(fromNode, createElementNS(toNode.nodeName, toNode.namespaceURI));\n          }\n        } else {\n          // Going from an element node to a text node\n          morphedNode = toNode;\n        }\n      } else if (morphedNodeType === TEXT_NODE || morphedNodeType === COMMENT_NODE) { // Text or comment node\n        if (toNodeType === morphedNodeType) {\n          if (morphedNode.nodeValue !== toNode.nodeValue) {\n            morphedNode.nodeValue = toNode.nodeValue;\n          }\n\n          return morphedNode;\n        } else {\n          // Text node to something else\n          morphedNode = toNode;\n        }\n      }\n    }\n\n    if (morphedNode === toNode) {\n      // The \"to node\" was not compatible with the \"from node\" so we had to\n      // toss out the \"from node\" and use the \"to node\"\n      onNodeDiscarded(fromNode);\n    } else {\n      if (toNode.isSameNode && toNode.isSameNode(morphedNode)) {\n        return;\n      }\n\n      morphEl(morphedNode, toNode, childrenOnly);\n\n      // We now need to loop over any keyed nodes that might need to be\n      // removed. We only do the removal if we know that the keyed node\n      // never found a match. When a keyed node is matched up we remove\n      // it out of fromNodesLookup and we use fromNodesLookup to determine\n      // if a keyed node has been matched up or not\n      if (keyedRemovalList) {\n        for (var i=0, len=keyedRemovalList.length; i<len; i++) {\n          var elToRemove = fromNodesLookup[keyedRemovalList[i]];\n          if (elToRemove) {\n            removeNode(elToRemove, elToRemove.parentNode, false);\n          }\n        }\n      }\n    }\n\n    if (!childrenOnly && morphedNode !== fromNode && fromNode.parentNode) {\n      if (morphedNode.actualize) {\n        morphedNode = morphedNode.actualize(fromNode.ownerDocument || doc);\n      }\n      // If we had to swap out the from node with a new node because the old\n      // node was not compatible with the target node then we need to\n      // replace the old DOM node in the original DOM tree. This is only\n      // possible if the original DOM node was part of a DOM tree which\n      // we know is the case if it has a parent node.\n      fromNode.parentNode.replaceChild(morphedNode, fromNode);\n    }\n\n    return morphedNode;\n  };\n}\n\nvar morphdom = morphdomFactory(morphAttrs);\n\nexport default morphdom;\n",
-        "import morphdom from \"morphdom\";\n\nfunction morph(oldNode, newNode) {\n  morphdom(oldNode, newNode);\n}\n\nconst BOOST_PAGES = JSON.parse(\n  document.querySelector(\"meta[name=reactor-boost]\")?.dataset.enabled || \"false\"\n);\n\nconsole.log(\"BOOST_PAGES\", BOOST_PAGES);\n\nclass NavEvents extends EventTarget {\n  send() {\n    console.log(\"LOAD\", document.location.href);\n    this.dispatchEvent(new Event(\"newLocation\"));\n  }\n}\n\nlet navEvent = new NavEvents();\n\nif (BOOST_PAGES) {\n  document.addEventListener(\"click\", (e) => {\n    let link = e.target;\n    link = link.tagName.toLowerCase() !== \"a\" ? link.closest(\"a\") : link;\n    if (\n      link &&\n      link.href &&\n      (!link.target || link.target === \"_self\") &&\n      link.origin == document.location.origin &&\n      e.button === 0 && // left click only\n      !e.metaKey && // open in new tab (mac)\n      !e.ctrlKey && // open in new tab (win & linux)\n      !e.altKey && // download\n      !e.shiftKey\n    ) {\n      e.preventDefault();\n      HistoryCache.load(link.href);\n    }\n  });\n}\n\nfunction replaceBodyContent(newBody, scrollY = undefined) {\n  document.body.innerHTML = newBody;\n  if (scrollY === undefined) {\n    document.querySelector(\"[autofocus]\")?.focus();\n  } else {\n    window.scrollTo(0, scrollY);\n  }\n}\n\nfunction hasSameOriginAsDocument(url) {\n  if (url.startsWith(\"http://\") || url.startsWith(\"https://\")) {\n    return new URL(url).origin === document.location.origin;\n  } else {\n    return true;\n  }\n}\n\nclass HistoryCache {\n  static async load(url) {\n    if (BOOST_PAGES) {\n      // this._saveCurrentPage();\n      if (hasSameOriginAsDocument(url)) {\n        this.push(url);\n      } else {\n        document.location.assign(url);\n      }\n    } else {\n      document.location.assign(url);\n    }\n  }\n\n  static back() {\n    window.history.back();\n  }\n\n  static async push(path) {\n    if (document.body == null) debugger;\n    history.replaceState(\n      {\n        content: document.body.innerHTML,\n        scrollY: window.scrollY,\n      },\n      document.title,\n      document.location.href\n    );\n    history.pushState({}, document.title, path);\n    this.replaceContentFromUrl(path);\n  }\n\n  static async replaceContentFromUrl(url) {\n    navEvent.send();\n    let response = await fetch(url);\n    let content = await response.text();\n    let doc = new DOMParser().parseFromString(content, \"text/html\");\n    document.title = doc.querySelector(\"title\")?.text ?? \"\";\n    replaceBodyContent(doc.body.innerHTML);\n  }\n\n  static replace(path) {\n    history.replaceState({}, document.title, path);\n  }\n}\n\nwindow.addEventListener(\"popstate\", (event) => {\n  navEvent.send();\n  if (event.state?.content !== undefined) {\n    replaceBodyContent(event.state.content, event.state.scrollY);\n  }\n  HistoryCache.replaceContentFromUrl(document.location.href);\n});\n\nexport default {\n  HistoryCache: HistoryCache,\n  morph: morph,\n  navEvent: navEvent,\n};\n",
-        "import ReconnectingWebSocket from \"reconnecting-websocket\";\nimport boost from \"./reactor-boost\";\n\n// Connection\n\nconst parser = new DOMParser();\n\nclass ServerConnection extends EventTarget {\n  open(path = \"__reactor__\") {\n    let protocol = location.protocol.replace(\"http\", \"ws\");\n    this.socket = new ReconnectingWebSocket(\n      `${protocol}//${location.host}/${path}`,\n      [],\n      {\n        maxEnqueuedMessages: 0,\n      }\n    );\n\n    this.socket.addEventListener(\"open\", () => {\n      console.log(\"WS: OPEN\");\n      this.sendQueryString();\n      this.dispatchEvent(new Event(\"open\"));\n    });\n\n    this.socket.addEventListener(\"message\", (event) =>\n      this._processMessage(event)\n    );\n\n    this.socket.addEventListener(\"close\", () => {\n      console.log(\"WS: CLOSE\");\n      this.dispatchEvent(new Event(\"close\"));\n    });\n\n    boost.navEvent.addEventListener(\"newLocation\", () => {\n      this.sendQueryString();\n    });\n  }\n\n  get isOpen() {\n    return this.socket?.readyState == ReconnectingWebSocket.OPEN;\n  }\n\n  _processMessage(event) {\n    let { command, payload } = JSON.parse(event.data);\n    switch (command) {\n      case \"render\":\n        var { id, diff } = payload;\n        console.log(\"<<< RENDER\", id);\n        document.getElementById(id)?.applyDiff(diff);\n        break;\n      case \"append\":\n      case \"prepend\":\n      case \"insert_after\":\n      case \"insert_before\":\n      case \"replace_with\":\n        var { id, html } = payload;\n        console.log(`<<< ${command.toUpperCase()}`, id);\n        html = parser.parseFromString(html, \"text/html\").body.firstChild;\n        var element = document.getElementById(id);\n        if (element) {\n          switch (command) {\n            case \"append\":\n              element.append(html);\n              break;\n            case \"prepend\":\n              element.prepend(html);\n              break;\n            case \"insert_after\":\n              element.after(html);\n              break;\n            case \"insert_before\":\n              element.before(html);\n              break;\n            case \"replace_with\":\n              boost.morph(element, html);\n              break;\n          }\n        }\n        break;\n      case \"remove\":\n        var { id } = payload;\n        console.log(\"<<< REMOVE\", id);\n        document.getElementById(id)?.remove();\n        break;\n      case \"focus_on\":\n        var { selector } = payload;\n        console.log(\n          \"<<< FOCUS-ON\",\n          `\"${selector}\"`,\n          document.querySelector(selector)\n        );\n        window.requestAnimationFrame(() =>\n          document.querySelector(selector)?.focus()\n        );\n        break;\n      case \"scroll_into_view\":\n        var { id, behavior, block, inline } = payload;\n        window.requestAnimationFrame(() =>\n          document\n            .getElementById(id)\n            ?.scrollIntoView({ behavior, block, inline })\n        );\n        break;\n      case \"url_change\":\n        var { url } = payload;\n        console.log(\"<< URL\", payload.command, url);\n        switch (payload.command) {\n          case \"redirect\":\n            boost.HistoryCache.load(url);\n            break;\n          case \"replace\":\n            boost.HistoryCache.replace(url);\n            break;\n          case \"push\":\n            boost.HistoryCache.push(url);\n            break;\n        }\n        break;\n\n      case \"set_query_string\":\n        var { qs } = payload;\n        qs = qs.length ? `?${qs}` : \"\";\n        console.log(\"<< SET URL PARAMS\", qs);\n        boost.HistoryCache.replace(document.location.pathname + qs);\n        break;\n\n      case \"back\":\n        boost.HistoryCache.back();\n        break;\n      default:\n        console.error(`Unknown command \"${command}\"`, payload);\n    }\n  }\n\n  sendQueryString() {\n    // \"?a=x&...\" -> \"a=x&...\"\n    let qs = document.location.search.slice(1);\n    console.log(\"QS\", qs);\n    this._send(\"query_string\", { qs });\n  }\n\n  sendJoin(name, component_id, parent_id, state) {\n    console.log(\">>> JOIN\", name, component_id);\n    this._send(\"join\", { name, parent_id, state });\n  }\n\n  sendLeave(id) {\n    console.log(\">>> LEAVE\", id);\n    this._send(\"leave\", { id });\n  }\n\n  sendUserEvent(id, command, implicit_args, explicit_args) {\n    console.log(\">>> USER_EVENT\", id, command, explicit_args);\n    this._send(\"user_event\", { id, command, implicit_args, explicit_args });\n  }\n\n  _send(command, payload) {\n    if (this.isOpen) {\n      this.socket.send(JSON.stringify({ command, payload }));\n    }\n  }\n}\n\nlet connection = new ServerConnection();\n\nfor ({ dataset } of document.querySelectorAll(\"meta[name=reactor-component]\")) {\n  let baseElement = document.createElement(dataset.extends);\n\n  class ReactorComponent extends baseElement.constructor {\n    constructor(...args) {\n      super(...args);\n      this._lastReceivedHtml = [];\n      this.joinBind = () => this.join();\n      this.wentOffline = () => this.classList.add(\"reactor-disconnected\");\n    }\n\n    connectedCallback() {\n      connection.addEventListener(\"open\", this.joinBind);\n      connection.addEventListener(\"close\", this.wentOffline);\n      this.join();\n    }\n\n    disconnectedCallback() {\n      connection.removeEventListener(\"open\", this.joinBind);\n      connection.removeEventListener(\"close\", this.wentOffline);\n      this.leave();\n    }\n\n    join() {\n      this.classList.remove(\"reactor-disconnected\");\n      connection.sendJoin(\n        this.dataset.name,\n        this.id,\n        this.parentId,\n        this.dataset.state\n      );\n    }\n\n    leave() {\n      connection.sendLeave(this.id);\n    }\n\n    applyDiff(diff) {\n      window.requestAnimationFrame(() => {\n        let html = this.getHtml(diff);\n        boost.morph(this, html);\n      });\n    }\n\n    getHtml(diff) {\n      let fragments = [];\n      let cursor = 0;\n      for (let fragment of diff) {\n        if (typeof fragment === \"string\") {\n          fragments.push(fragment);\n        } else if (fragment < 0) {\n          cursor -= fragment;\n        } else {\n          fragments.push(\n            ...this._lastReceivedHtml.slice(cursor, cursor + fragment)\n          );\n          cursor += fragment;\n        }\n      }\n      this._lastReceivedHtml = fragments;\n      return fragments.join(\" \");\n    }\n\n    /**\n     * Returns the id of the parent component\n     *\n     * @returns {?String}\n     */\n    get parentId() {\n      return this.parentComponent?.id;\n    }\n\n    /**\n     * Returns the high parent reactor component if any is found component\n     *\n     * @returns {?ReactorComponent}\n     */\n    get parentComponent() {\n      return this.parentElement?.closest(\"[reactor-component]\");\n    }\n\n    /**\n     * Dispatches a command to this component and sends it to the backend\n     * @param {String} command\n     * @param {Object} args\n     * @param {?HTMLFormElement} form\n     */\n    dispatch(command, args, formScope) {\n      connection.sendUserEvent(\n        this.id,\n        command,\n        this.serialize(formScope),\n        args\n      );\n    }\n\n    /**\n     * Serialize all elements inside `element` with a [name] attribute into\n     * a an array of `[element[name], element[value]]`\n     * @param {HTMLElement} element\n     */\n    serialize(element) {\n      let result = {};\n      for (let el of element.querySelectorAll(\"[name]\")) {\n        // Avoid serializing data of a nested component\n        if (el.closest(\"[reactor-component]\") !== this) {\n          continue;\n        }\n\n        let value = null;\n        switch (el.type.toLowerCase()) {\n          case \"checkbox\":\n          case \"radio\":\n            value = el.checked ? el.value || true : null;\n            break;\n          case \"select-multiple\":\n            value = el.selectedOptions.map((option) => option.value);\n            break;\n          default:\n            value = el.value;\n            break;\n        }\n\n        if (value !== null) {\n          let key = el.getAttribute(\"name\");\n          let values = result[key] ?? [];\n          values.push(value);\n          result[key] = values;\n        }\n      }\n      return result;\n    }\n  }\n\n  customElements.define(dataset.tagName, ReactorComponent, {\n    extends: dataset.extends,\n  });\n}\n\nconnection.open();\nvar debounceTimeout = undefined;\n\nwindow.reactor = {\n  /**\n   * Forwards a user event to a component\n   * @param {HTMLElement} element\n   * @param {String} name\n   * @param {Object} args\n   */\n  send(element, name, args) {\n    let component = element.closest(\"[reactor-component]\");\n    if (component !== null) {\n      let form = element.closest(\"form\");\n      let formScope = component.contains(form) ? form : component;\n      component.dispatch(name, args, formScope);\n    }\n  },\n\n  /**\n   * Debounce a function call\n   * @param {Number} delay\n   * @returns\n   */\n  debounce(delay) {\n    return (f) => {\n      return (...args) => {\n        clearTimeout(debounceTimeout);\n        debounceTimeout = setTimeout(() => f(...args), delay);\n      };\n    };\n  },\n};\n"
+        "import _load from \"idiomorph\";\n\nfunction morph(oldNode, newNode) {\n  Idiomorph.morph(oldNode, newNode);\n}\n\nconst BOOST_PAGES = JSON.parse(\n  document.querySelector(\"meta[name=reactor-boost]\")?.dataset.enabled || \"false\"\n);\n\nconsole.log(\"BOOST_PAGES\", BOOST_PAGES);\n\nclass NavEvents extends EventTarget {\n  sendNewLocation() {\n    console.log(\"LOAD\", document.location.href);\n    this.dispatchEvent(new Event(\"newLocation\"));\n  }\n\n  sendNewContent() {\n    this.dispatchEvent(new Event(\"newContent\"));\n  }\n}\n\nlet navEvent = new NavEvents();\n\nif (BOOST_PAGES) {\n  document.addEventListener(\"click\", (e) => {\n    let link = e.target;\n    link = link.tagName.toLowerCase() !== \"a\" ? link.closest(\"a\") : link;\n    if (\n      link &&\n      link.href &&\n      (!link.target || link.target === \"_self\") &&\n      link.origin == document.location.origin &&\n      e.button === 0 && // left click only\n      !e.metaKey && // open in new tab (mac)\n      !e.ctrlKey && // open in new tab (win & linux)\n      !e.altKey && // download\n      !e.shiftKey\n    ) {\n      e.preventDefault();\n      HistoryCache.load(link.href);\n    }\n  });\n}\n\nfunction replaceBodyContent(newBody, scrollY = undefined) {\n  window.requestAnimationFrame(() => {\n    morph(document.body, newBody);\n    if (scrollY === undefined) {\n      document.querySelector(\"[autofocus]\")?.focus();\n    } else {\n      window.scrollTo(0, scrollY);\n    }\n    navEvent.sendNewContent();\n  });\n}\n\nfunction hasSameOriginAsDocument(url) {\n  if (url.startsWith(\"http://\") || url.startsWith(\"https://\")) {\n    return new URL(url).origin === document.location.origin;\n  } else {\n    return true;\n  }\n}\n\nclass HistoryCache {\n  static async load(url) {\n    if (BOOST_PAGES) {\n      // this._saveCurrentPage();\n      if (hasSameOriginAsDocument(url)) {\n        this.push(url);\n      } else {\n        document.location.assign(url);\n      }\n    } else {\n      document.location.assign(url);\n    }\n  }\n\n  static back() {\n    window.history.back();\n  }\n\n  static async push(path) {\n    if (document.body == null) debugger;\n    history.replaceState(\n      {\n        content: document.body.outerHTML,\n        scrollY: window.scrollY,\n      },\n      document.title,\n      document.location.href\n    );\n    history.pushState({}, document.title, path);\n    this.replaceContentFromUrl(path);\n  }\n\n  static async replaceContentFromUrl(url) {\n    navEvent.sendNewLocation();\n    let response = await fetch(url);\n    let content = await response.text();\n    let doc = new DOMParser().parseFromString(content, \"text/html\");\n    document.title = doc.querySelector(\"title\")?.text ?? \"\";\n    replaceBodyContent(doc.body);\n  }\n\n  static replace(path) {\n    history.replaceState({}, document.title, path);\n  }\n}\n\nwindow.addEventListener(\"popstate\", (event) => {\n  navEvent.sendNewLocation();\n  if (event.state?.content !== undefined) {\n    replaceBodyContent(event.state.content, event.state.scrollY);\n  }\n  HistoryCache.replaceContentFromUrl(document.location.href);\n});\n\nexport default {\n  HistoryCache: HistoryCache,\n  morph: morph,\n  navEvent: navEvent,\n};\n",
+        "import ReconnectingWebSocket from \"reconnecting-websocket\";\nimport boost from \"./reactor-boost\";\n\n// Connection\n\nconst parser = new DOMParser();\n\nclass ServerConnection {\n  constructor() {\n    this.components = {};\n  }\n\n  open(path = \"__reactor__\") {\n    let protocol = location.protocol.replace(\"http\", \"ws\");\n    this.socket = new ReconnectingWebSocket(\n      `${protocol}//${location.host}/${path}`,\n      [],\n      {\n        maxEnqueuedMessages: 0,\n      }\n    );\n\n    this.socket.addEventListener(\"open\", () => {\n      console.log(\"WS: OPEN\");\n      this.sendQueryString();\n      this.components = {};\n      this.joinAllComponents();\n    });\n\n    this.socket.addEventListener(\"message\", (event) =>\n      this._processMessage(event)\n    );\n\n    this.socket.addEventListener(\"close\", () => {\n      console.log(\"WS: CLOSE\");\n      this.components = {};\n      document.querySelectorAll(\"[reactor-component]\").forEach((element) => {\n        element.classList.add(\"reactor-disconnected\");\n        element.dataset.isLive = \"false\";\n      });\n    });\n\n    boost.navEvent.addEventListener(\"newLocation\", () => {\n      this.sendQueryString();\n    });\n\n    boost.navEvent.addEventListener(\"newContent\", () => {\n      this.joinAllComponents();\n    });\n  }\n\n  get isOpen() {\n    return this.socket?.readyState == ReconnectingWebSocket.OPEN;\n  }\n\n  joinAllComponents() {\n    let registeredIds = new Set(Object.keys(this.components));\n    for (let element of document.querySelectorAll(\"[reactor-component]\")) {\n      if (registeredIds.delete(element.id)) {\n        this.components[element.id].join();\n      } else {\n        let component = new ReactorComponent(element.id);\n        this.components[element.id] = component;\n        component.join();\n      }\n    }\n    for (let id of registeredIds.keys()) {\n      delete this.components[id];\n      this.sendLeave(id);\n    }\n  }\n\n  _processMessage(event) {\n    let { command, payload } = JSON.parse(event.data);\n    switch (command) {\n      case \"render\":\n        var { id, diff } = payload;\n        console.log(\"<<< RENDER\", id);\n        this.components[id]?.applyDiff(diff);\n        break;\n      case \"append\":\n      case \"prepend\":\n      case \"insert_after\":\n      case \"insert_before\":\n      case \"replace_with\":\n        var { id, html } = payload;\n        console.log(`<<< ${command.toUpperCase()}`, id);\n        html = parser.parseFromString(html, \"text/html\").body.firstChild;\n        var element = document.getElementById(id);\n        if (element) {\n          switch (command) {\n            case \"append\":\n              element.append(html);\n              break;\n            case \"prepend\":\n              element.prepend(html);\n              break;\n            case \"insert_after\":\n              element.after(html);\n              break;\n            case \"insert_before\":\n              element.before(html);\n              break;\n            case \"replace_with\":\n              boost.morph(element, html);\n              break;\n          }\n          boost.navEvent.sendNewContent();\n        }\n        break;\n      case \"remove\":\n        var { id } = payload;\n        console.log(\"<<< REMOVE\", id);\n        document.getElementById(id)?.remove();\n        boost.navEvent.sendNewContent();\n        break;\n      case \"focus_on\":\n        var { selector } = payload;\n        console.log(\n          \"<<< FOCUS-ON\",\n          `\"${selector}\"`,\n          document.querySelector(selector)\n        );\n        window.requestAnimationFrame(() =>\n          document.querySelector(selector)?.focus()\n        );\n        break;\n      case \"scroll_into_view\":\n        var { id, behavior, block, inline } = payload;\n        window.requestAnimationFrame(() =>\n          document\n            .getElementById(id)\n            ?.scrollIntoView({ behavior, block, inline })\n        );\n        break;\n      case \"url_change\":\n        var { url } = payload;\n        console.log(\"<< URL\", payload.command, url);\n        switch (payload.command) {\n          case \"redirect\":\n            boost.HistoryCache.load(url);\n            break;\n          case \"replace\":\n            boost.HistoryCache.replace(url);\n            break;\n          case \"push\":\n            boost.HistoryCache.push(url);\n            break;\n        }\n        break;\n\n      case \"set_query_string\":\n        var { qs } = payload;\n        qs = qs.length ? `?${qs}` : \"\";\n        console.log(\"<< SET URL PARAMS\", qs);\n        boost.HistoryCache.replace(document.location.pathname + qs);\n        break;\n\n      case \"back\":\n        boost.HistoryCache.back();\n        break;\n      default:\n        console.error(`Unknown command \"${command}\"`, payload);\n    }\n  }\n\n  sendQueryString() {\n    // \"?a=x&...\" -> \"a=x&...\"\n    let qs = document.location.search.slice(1);\n    console.log(\"QS\", qs);\n    this._send(\"query_string\", { qs });\n  }\n\n  sendJoin(name, component_id, state, children) {\n    console.log(\">>> JOIN\", name, component_id);\n    this._send(\"join\", { name, state, children });\n  }\n\n  sendLeave(id) {\n    console.log(\">>> LEAVE\", id);\n    this._send(\"leave\", { id });\n  }\n\n  sendUserEvent(id, command, implicit_args, explicit_args) {\n    console.log(\">>> USER_EVENT\", id, command, explicit_args);\n    this._send(\"user_event\", { id, command, implicit_args, explicit_args });\n  }\n\n  _send(command, payload) {\n    if (this.isOpen) {\n      this.socket.send(JSON.stringify({ command, payload }));\n    }\n  }\n}\n\nlet connection = new ServerConnection();\n\nclass ReactorComponent {\n  /**\n   * Returns the id of the parent component\n   *\n   * @param {HTMLElement} el\n   */\n  constructor(id) {\n    this.id = id;\n    this.lastReceivedHtml = [];\n  }\n\n  getElemenet() {\n    return document.getElementById(this.id);\n  }\n\n  applyDiff(diff) {\n    window.requestAnimationFrame(() => {\n      let el = this.getElemenet();\n      if (el) {\n        let html = this.getHtml(diff);\n        boost.morph(el, html);\n        boost.navEvent.sendNewContent();\n      }\n    });\n  }\n\n  getHtml(diff) {\n    let fragments = [];\n    let cursor = 0;\n    for (let fragment of diff) {\n      if (typeof fragment === \"string\") {\n        fragments.push(fragment);\n      } else if (fragment < 0) {\n        cursor -= fragment;\n      } else {\n        fragments.push(\n          ...this.lastReceivedHtml.slice(cursor, cursor + fragment)\n        );\n        cursor += fragment;\n      }\n    }\n    this.lastReceivedHtml = fragments;\n    return fragments.join(\" \");\n  }\n\n  join() {\n    let element = this.getElemenet();\n    if (element && element.dataset.isLive === \"false\") {\n      let parent = element?.parentElement?.closest(\"[reactor-component]\");\n      if (!parent || parent.dataset.isLive === \"true\") {\n        element.dataset.isLive = \"true\";\n        let children = Array.from(\n          element.querySelectorAll(\"[reactor-component]\")\n        ).reduce((children, el) => {\n          children[el.id] = [el.dataset.name, el.dataset.state];\n          return children;\n        }, {});\n\n        connection.sendJoin(\n          element.dataset.name,\n          element.id,\n          element.dataset.state,\n          children\n        );\n      }\n    }\n  }\n\n  /**\n   * Dispatches a command to this component and sends it to the backend\n   * @param {String} command\n   * @param {Object} args\n   * @param {?HTMLFormElement} form\n   */\n  dispatch(command, args, formScope) {\n    connection.sendUserEvent(this.id, command, this.serialize(formScope), args);\n  }\n\n  /**\n   * Serialize all elements inside `element` with a [name] attribute into\n   * a an array of `[element[name], element[value]]`\n   * @param {HTMLElement} element\n   */\n  serialize(element) {\n    let result = {};\n    let thisElement = this.getElemenet();\n    for (let el of element.querySelectorAll(\"[name]\")) {\n      // Avoid serializing data of a nested component\n      if (el.closest(\"[reactor-component]\") !== thisElement) {\n        continue;\n      }\n\n      let value = null;\n      switch (el.type.toLowerCase()) {\n        case \"checkbox\":\n        case \"radio\":\n          value = el.checked ? el.value || true : null;\n          break;\n        case \"select-multiple\":\n          value = el.selectedOptions.map((option) => option.value);\n          break;\n        default:\n          value = el.value;\n          break;\n      }\n\n      if (value !== null) {\n        let key = el.getAttribute(\"name\");\n        let values = result[key] ?? [];\n        values.push(value);\n        result[key] = values;\n      }\n    }\n    return result;\n  }\n}\n\nconnection.open();\nvar debounceTimeout = undefined;\n\nwindow.reactor = {\n  /**\n   * Forwards a user event to a component\n   * @param {HTMLElement} element\n   * @param {String} name\n   * @param {Object} args\n   */\n  send(element, name, args) {\n    let component_el = element.closest(\"[reactor-component]\");\n    let component = connection.components[component_el.id];\n    if (component_el !== null && component !== undefined) {\n      let form = element.closest(\"form\");\n      let formScope = component_el.contains(form) ? form : component_el;\n      component.dispatch(name, args, formScope);\n    }\n  },\n\n  /**\n   * Debounce a function call\n   * @param {Number} delay\n   * @returns\n   */\n  debounce(delay) {\n    return (f) => {\n      return (...args) => {\n        clearTimeout(debounceTimeout);\n        debounceTimeout = setTimeout(() => f(...args), delay);\n      };\n    };\n  },\n};\n"
     ],
     "version": 3
 }
```

### Comparing `django-reactor-5.2.0b0/reactor/templatetags/reactor.py` & `django-reactor-5.3.0b0/reactor/templatetags/reactor.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,58 +11,52 @@
 from ..repository import ComponentRepository
 
 register = template.Library()
 
 
 @register.inclusion_tag("reactor_header.html")
 def reactor_header():
-    return {
-        "components": [
-            {"tag_name": component._tag_name, "extends": component._extends}
-            for component in Component._all.values()
-        ],
-        "BOOST_PAGES": settings.BOOST_PAGES,
-    }
+    return {"BOOST_PAGES": settings.BOOST_PAGES}
 
 
 @register.simple_tag(takes_context=True)
 def tag_header(context):
     component: Component = context["this"]
+    repo: ComponentRepository = context["reactor_repository"]
     return format_html(
         (
-            'is="{tag_name}" '
             'id="{id}" '
             'data-name="{name}" '
             'data-state="{state}" '
+            'data-is-live="{is_live}" '
             "reactor-component"
         ),
-        tag_name=component._tag_name,
         id=component.id,
         name=component._name,
+        is_live=str(repo.is_live).lower(),
         state=Signer().sign(component.json(exclude=component._exclude_fields)),
     )
 
 
 @register.simple_tag(takes_context=True)
 def component(context, _name, **kwargs):
-    parent: t.Optional[Component] = context.get("this")
-    parent_id = parent.id if parent else None
-
     if (repo := context.get("reactor_repository")) is None:
         qs = (
             (request := context.get("request"))
             and request.META["QUERY_STRING"]
             or ""
         )
         repo = ComponentRepository(
+            is_live=False,
             user=context.get("user"),
             params=ComponentRepository.extract_params(qs),
         )
+        context["reactor_repository"] = repo
 
-    component, _created = repo.build(_name, state=kwargs, parent_id=parent_id)
+    component = repo.build(_name, state=kwargs)
     return component._render(repo) or ""
 
 
 @register.simple_tag(takes_context=True)
 def on(context, _event_and_modifiers, _command, **kwargs: t.Any):
     component: t.Optional[Component] = context.get("this")
```

### Comparing `django-reactor-5.2.0b0/reactor/utils.py` & `django-reactor-5.3.0b0/reactor/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import inspect
 import logging
 import typing as t
 from collections import defaultdict
 from functools import wraps
 
 from asgiref.sync import async_to_sync
+from channels.db import database_sync_to_async as db
 from channels.layers import get_channel_layer
 from django.utils.datastructures import MultiValueDict
 
 log = logging.getLogger("reactor")
 
+P = t.ParamSpec("P")
 
-def on_commit(f: t.Callable[(...), None]):
+__all__ = (
+    "on_commit",
+    "db",
+    "send_to",
+    "send_notification",
+    "filter_parameters",
+    "parse_request_data",
+)
+
+
+def on_commit(f: t.Callable[P, None]):
     @wraps(f)
-    def wrapper(*args: t.Any, **kwargs: t.Any):
+    def wrapper(*args: P.args, **kwargs: P.kwargs):
         from django.db.transaction import on_commit  # type: ignore
 
         on_commit(lambda: f(*args, **kwargs))
 
     return wrapper
```

### Comparing `django-reactor-5.2.0b0/setup.cfg` & `django-reactor-5.3.0b0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reactor
-version = 5.2.0b0
+version = 5.3.0b0
 description = Brings LiveView from Phoenix framework into Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Framework :: Django
```

