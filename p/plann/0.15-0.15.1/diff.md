# Comparing `tmp/plann-0.15.tar.gz` & `tmp/plann-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plann-0.15.tar", last modified: Wed Jul 19 14:40:21 2023, max compression
+gzip compressed data, was "plann-0.15.1.tar", last modified: Thu Jul 20 12:50:15 2023, max compression
```

## Comparing `plann-0.15.tar` & `plann-0.15.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 14:40:21.660176 plann-0.15/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2023-01-08 16:34:30.000000 plann-0.15/LICENSE.TXT
--rw-r--r--   0 tobias    (7385) tobias    (7385)      657 2023-07-19 14:40:21.660176 plann-0.15/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)    11343 2023-03-22 21:33:20.000000 plann-0.15/README.md
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 14:40:21.656843 plann-0.15/plann/
--rw-r--r--   0 tobias    (7385) tobias    (7385)        5 2023-01-10 11:42:00.000000 plann-0.15/plann/__init__.py
--rwxr-xr-x   0 tobias    (7385) tobias    (7385)    60751 2023-07-18 17:19:36.000000 plann-0.15/plann/cli.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     7221 2023-02-08 14:54:19.000000 plann-0.15/plann/config.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)    15950 2023-07-18 17:30:01.000000 plann-0.15/plann/lib.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)      585 2023-07-19 14:31:09.000000 plann-0.15/plann/metadata.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     5687 2023-07-17 20:36:44.000000 plann-0.15/plann/panic_planning.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1616 2023-03-11 20:25:10.000000 plann-0.15/plann/template.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 14:40:21.656843 plann-0.15/plann.egg-info/
--rw-r--r--   0 tobias    (7385) tobias    (7385)      657 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (7385) tobias    (7385)      469 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       40 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)       66 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/requires.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)        6 2023-07-19 14:40:21.000000 plann-0.15/plann.egg-info/top_level.txt
--rw-r--r--   0 tobias    (7385) tobias    (7385)      409 2023-07-19 14:40:21.660176 plann-0.15/setup.cfg
--rw-r--r--   0 tobias    (7385) tobias    (7385)     1148 2023-07-18 13:57:38.000000 plann-0.15/setup.py
-drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-19 14:40:21.660176 plann-0.15/tests/
--rw-r--r--   0 tobias    (7385) tobias    (7385)    10157 2023-07-17 20:36:50.000000 plann-0.15/tests/test_functional.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3651 2023-07-18 17:35:14.000000 plann-0.15/tests/test_lib.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     3407 2023-05-01 12:19:43.000000 plann-0.15/tests/test_panic.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)       97 2023-01-18 15:49:37.000000 plann-0.15/tests/test_plann_cli.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     2215 2023-04-21 20:11:42.000000 plann-0.15/tests/test_template.py
--rw-r--r--   0 tobias    (7385) tobias    (7385)     5372 2023-07-17 20:36:44.000000 plann-0.15/tests/test_timespec.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-20 12:50:15.871508 plann-0.15.1/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    35147 2023-07-20 12:50:09.000000 plann-0.15.1/LICENSE.TXT
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      659 2023-07-20 12:50:15.871508 plann-0.15.1/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    11343 2023-07-20 12:50:09.000000 plann-0.15.1/README.md
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-20 12:50:15.868174 plann-0.15.1/plann/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        5 2023-07-20 12:50:09.000000 plann-0.15.1/plann/__init__.py
+-rwxr-xr-x   0 tobias    (7385) tobias    (7385)    60893 2023-07-20 12:50:09.000000 plann-0.15.1/plann/cli.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     7221 2023-07-20 12:50:09.000000 plann-0.15.1/plann/config.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    16503 2023-07-20 12:50:09.000000 plann-0.15.1/plann/lib.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      587 2023-07-20 12:50:09.000000 plann-0.15.1/plann/metadata.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     5687 2023-07-20 12:50:09.000000 plann-0.15.1/plann/panic_planning.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1616 2023-07-20 12:50:09.000000 plann-0.15.1/plann/template.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-20 12:50:15.871508 plann-0.15.1/plann.egg-info/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      659 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      469 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        1 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       40 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       66 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/requires.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)        6 2023-07-20 12:50:15.000000 plann-0.15.1/plann.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (7385) tobias    (7385)      409 2023-07-20 12:50:15.871508 plann-0.15.1/setup.cfg
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     1148 2023-07-20 12:50:09.000000 plann-0.15.1/setup.py
+drwxr-xr-x   0 tobias    (7385) tobias    (7385)        0 2023-07-20 12:50:15.871508 plann-0.15.1/tests/
+-rw-r--r--   0 tobias    (7385) tobias    (7385)    10157 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_functional.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3651 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_lib.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     3407 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_panic.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)       97 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_plann_cli.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     2215 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_template.py
+-rw-r--r--   0 tobias    (7385) tobias    (7385)     5372 2023-07-20 12:50:09.000000 plann-0.15.1/tests/test_timespec.py
```

### Comparing `plann-0.15/LICENSE.TXT` & `plann-0.15.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `plann-0.15/PKG-INFO` & `plann-0.15.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plann
-Version: 0.15
+Version: 0.15.1
 Summary: Simple command-line CalDAV client and planning tool, for adding and browsing calendar items, todo list items, etc.
 Home-page: https://plann.no/
 Author: Tobias Brox
 Author-email: t-plann@tobixen.no
 Maintainer: Tobias Brox
 License: GPLv3+
 Classifier: Environment :: Web Environment
```

### Comparing `plann-0.15/README.md` & `plann-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `plann-0.15/plann/cli.py` & `plann-0.15.1/plann/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,15 @@
         if cancel:
             comp.status='CANCELLED'
         elif cancel is False:
             comp.status='NEEDS-ACTION'
         if postpone:
             for attrib in ('DTSTART', 'DTEND', 'DUE'):
                 if comp.get(attrib):
-                    comp[attrib].dt = parse_add_dur(comp[attrib].dt, postpone).astimezone(tz.store_timezone)
+                    comp[attrib].dt = parse_add_dur(comp[attrib].dt, postpone, for_storage=True)
         obj.save()
 
 
 @select.command()
 @click.pass_context
 @click.option('--recurrence-mode', default='safe', help="Completion of recurrent tasks, mode to use - can be 'safe', 'thisandfuture' or '' (see caldav library for details)")
 def complete(ctx, **kwargs):
@@ -913,14 +913,16 @@
             c.save_event(ical)
 
 def _process_set_args(ctx, kwargs):
     ctx.obj['set_args'] = {}
     for x in kwargs:
         if kwargs[x] is None or kwargs[x]==():
             continue
+        if x in ('set_due', 'set_dtend', 'set_dtstart', 'set_completed'):
+            kwargs[x] = parse_dt(kwargs[x], for_storage=True)
         if x == 'set_rrule':
             rrule = {}
             for split1 in kwargs[x].split(';'):
                 k,v = split1.split('=')
                 rrule[k] = v
             ctx.obj['set_args']['rrule'] = rrule
         elif x == 'set_category':
@@ -982,15 +984,15 @@
     kal add event "release party" 2004-11-30T19:00+2h
     """
     _add_event(ctx, timespec, **kwargs)
 
 def _add_event(ctx, timespec, **kwargs):
     _process_set_args(ctx, kwargs)
     for cal in ctx.obj['calendars']:
-        (dtstart, dtend) = parse_timespec(timespec)
+        (dtstart, dtend) = parse_timespec(timespec, for_storage=True)
         event = cal.save_event(dtstart=dtstart, dtend=dtend, **ctx.obj['set_args'], no_overwrite=True)
         click.echo(f"uid={event.id}")
 
 def journal():
     click.echo("soon you should be able to add journal entries to your calendar")
     raise NotImplementedError("foo")
```

### Comparing `plann-0.15/plann/config.py` & `plann-0.15.1/plann/config.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/plann/lib.py` & `plann-0.15.1/plann/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,21 @@
     if isinstance(dt, datetime.datetime):
         if not dt.tzinfo:
             return dt.replace(tzinfo=tz.implicit_timezone).astimezone(tz.implicit_timezone)
         else:
             return dt
     return datetime.datetime(dt.year, dt.month, dt.day, tzinfo=tz.implicit_timezone).astimezone(tz.implicit_timezone)
 
-def parse_dt(input, return_type=None):
+def parse_dt(input, return_type=None, for_storage=False):
+    ret = _parse_dt(input, return_type)
+    if for_storage:
+        ret = ret.astimezone(tz.store_timezone)
+    return ret
+    
+def _parse_dt(input, return_type=None):
     """
     Convenience-method, it is very liberal in what it accepts as input:
 
     * Date string or datetime string (uses dateutil.parser)
     * datetime or date
     * VDDDTypes from the icalendar library
     * strings like "+2h" means "two hours in the future"
@@ -102,15 +108,15 @@
     elif return_type is datetime.date:
         return ret.date()
     elif ret.time() == datetime.time(0,0) and len(input)<12 and not '00:00' in input and not '0000' in input:
         return ret.date()
     else:
         return _ensure_ts(ret)
 
-def parse_add_dur(dt, dur):
+def parse_add_dur(dt, dur, for_storage=False):
     """
     duration may be something like this:
       * 1s (one second)
       * 3m (three minutes, not months
       * 3.5h
       * 1y1w
     
@@ -140,20 +146,26 @@
         if u=='y' and dt:
             dt = datetime.datetime.combine(datetime.date(dt.year+int(i), dt.month, dt.day), dt.time(), tzinfo=dt.tzinfo)
         else:
             diff = datetime.timedelta(0, i*time_units[u])
             if dt:
                 dt = dt + diff
     if dt:
-        return dt
+        return dt.astimezone(tz.store_timezone) if for_storage else dt
     else:
         return diff
    
 
-def parse_timespec(timespec):
+def parse_timespec(timespec, for_storage=False):
+    ret = _parse_timespec(timespec)
+    if for_storage:
+        ret = (x and x.astimezone(tz.store_timezone) for x in ret)
+    return ret
+
+def _parse_timespec(timespec):
     """parses a timespec and return two timestamps
 
     The ISO8601 interval format, format 1, 2 or 3 as described at
     https://en.wikipedia.org/wiki/ISO_8601#Time_intervals should be
     accepted, though it may be dependent on
     https://github.com/gweis/isodate/issues/77 or perhaps
     https://github.com/dateutil/dateutil/issues/1184 
@@ -271,20 +283,21 @@
 
 def _procrastinate(objs, delay, check_dependent="error", with_children=False, with_family=False, with_parent=False, err_callback=print, confirm_callback=lambda x: False, recursivity=0):
     assert recursivity<16 ## TODO: better error message.  Probably we have some kind of relationship loop here.
     for x in objs:
         if x.icalendar_component.get('RELATED-TO'):
             if with_family == 'interactive':
                 with_family = confirm_callback("There are relations - postpone the whole family tree?")
-            if not with_family and with_parent == 'interactive' and _hasreltype(x, parentlike):
+            if not with_family and with_parent == 'interactive' and x.get_relatives(parentlike, fetch_objs=False):
                 with_parent = confirm_callback("There exists (a) parent(s) - postpone the parent?")
-            if not with_family and with_children == 'interactive' and _hasreltype(x, childlike):
+            if not with_family and with_children == 'interactive' and x.get_telatives(childlike, fetch_objs=False):
                 with_children = confirm_callback("There exists children - postpone the children?")
         if with_family:
             parents = x.get_relatives(reltypes=parentlike)
+            parents = sum([x.values() for x in parents], start=[])
             if parents:
                 _procrastinate(parents, delay, check_dependent, with_children, with_family, with_parent, err_callback, confirm_callback, recursivity=recursivity+1)
                 continue
             else:
                 _procrastinate([x], delay, check_dependent, with_children=True, with_family=False, with_parent=False, err_callback=err_callback, confirm_callback=confirm_callback, recursivity=recursivity+1)
                 continue
         if with_parent:
```

### Comparing `plann-0.15/plann/metadata.py` & `plann-0.15.1/plann/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 metadata = {
-    "version": "0.15",
+    "version": "0.15.1",
     "author": "Tobias Brox",
     "author_short": "tobixen",
     "copyright": "Copyright 2013-2023, Tobias Brox and contributors",
     "license": "GPLv3+",
     "license_url": "http://www.gnu.org/licenses/gpl-3.0-standalone.html",
     "maintainer": "Tobias Brox",
     "author_email": "t-plann@tobixen.no",
```

### Comparing `plann-0.15/plann/panic_planning.py` & `plann-0.15.1/plann/panic_planning.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/plann/template.py` & `plann-0.15.1/plann/template.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/plann.egg-info/PKG-INFO` & `plann-0.15.1/plann.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plann
-Version: 0.15
+Version: 0.15.1
 Summary: Simple command-line CalDAV client and planning tool, for adding and browsing calendar items, todo list items, etc.
 Home-page: https://plann.no/
 Author: Tobias Brox
 Author-email: t-plann@tobixen.no
 Maintainer: Tobias Brox
 License: GPLv3+
 Classifier: Environment :: Web Environment
```

### Comparing `plann-0.15/setup.py` & `plann-0.15.1/setup.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/tests/test_functional.py` & `plann-0.15.1/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/tests/test_lib.py` & `plann-0.15.1/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/tests/test_panic.py` & `plann-0.15.1/tests/test_panic.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/tests/test_template.py` & `plann-0.15.1/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `plann-0.15/tests/test_timespec.py` & `plann-0.15.1/tests/test_timespec.py`

 * *Files identical despite different names*

