# Comparing `tmp/vbtex-0.1.4.tar.gz` & `tmp/vbtex-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.4.tar", max compression
+gzip compressed data, was "vbtex-0.1.5.tar", max compression
```

## Comparing `vbtex-0.1.4.tar` & `vbtex-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.4/README.md
--rw-r--r--   0        0        0      368 2023-07-19 12:29:25.059051 vbtex-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-19 12:19:39.103602 vbtex-0.1.4/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.4/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.4/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.4/vbtex/choice_option.py
--rw-r--r--   0        0        0     1547 2023-07-19 12:19:19.372901 vbtex-0.1.4/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.4/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.4/vbtex/padded.py
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vbtex-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.5/README.md
+-rw-r--r--   0        0        0      370 2023-07-20 13:25:13.078644 vbtex-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-20 05:43:48.477861 vbtex-0.1.5/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.5/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.5/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.5/vbtex/choice_option.py
+-rw-r--r--   0        0        0     1812 2023-07-20 13:24:27.451139 vbtex-0.1.5/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.5/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.5/vbtex/padded.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 vbtex-0.1.5/PKG-INFO
```

### Comparing `vbtex-0.1.4/vbtex/.DS_Store` & `vbtex-0.1.5/vbtex/.DS_Store`

 * *Files 16% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 00000240: 0000 0000 000b 005f 005f 006d 0061 0069  ......._._.m.a.i
 00000250: 006e 005f 005f 002e 0070 0079 496c 6f63  .n._._...p.yIloc
 00000260: 626c 6f62 0000 0010 0000 00af 0000 002e  blob............
 00000270: ffff ffff ffff 0000 0000 0010 0063 0068  .............c.h
 00000280: 006f 0069 0063 0065 005f 006f 0070 0074  .o.i.c.e._.o.p.t
 00000290: 0069 006f 006e 002e 0070 0079 496c 6f63  .i.o.n...p.yIloc
 000002a0: 626c 6f62 0000 0010 0000 011d 0000 002e  blob............
-000002b0: ffff ffff ffff 0000 0000 000e 0066 0072  .............f.r
-000002c0: 0061 006d 0065 0064 0020 0063 006f 0070  .a.m.e.d. .c.o.p
-000002d0: 0079 002e 0070 0079 496c 6f63 626c 6f62  .y...p.yIlocblob
-000002e0: 0000 0010 0000 01ab 0000 004e ffff ffff  ...........N....
-000002f0: ffff 0000 0000 0009 0066 0072 0061 006d  .........f.r.a.m
-00000300: 0065 0064 002e 0070 0079 496c 6f63 626c  .e.d...p.yIlocbl
-00000310: 6f62 0000 0010 0000 018b 0000 002e ffff  ob..............
-00000320: ffff ffff 0000 0000 0007 006d 0061 0069  ...........m.a.i
-00000330: 006e 002e 0070 0079 496c 6f63 626c 6f62  .n...p.yIlocblob
-00000340: 0000 0010 0000 01f9 0000 002e ffff ffff  ................
-00000350: ffff 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: ffff ffff ffff 0000 0000 0009 0066 0072  .............f.r
+000002c0: 0061 006d 0065 0064 002e 0070 0079 496c  .a.m.e.d...p.yIl
+000002d0: 6f63 626c 6f62 0000 0010 0000 018b 0000  ocblob..........
+000002e0: 002e ffff ffff ffff 0000 0000 0007 006d  ...............m
+000002f0: 0061 0069 006e 002e 0070 0079 496c 6f63  .a.i.n...p.yIloc
+00000300: 626c 6f62 0000 0010 0000 01f9 0000 002e  blob............
+00000310: ffff ffff ffff 0000 0000 0009 0070 0061  .............p.a
+00000320: 0064 0064 0065 0064 002e 0070 0079 496c  .d.d.e.d...p.yIl
+00000330: 6f63 626c 6f62 0000 0010 0000 0075 0000  ocblob.......u..
+00000340: 010b ffff ffff ffff 0000 0000 0000 0000  ................
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `vbtex-0.1.4/vbtex/choice_option.py` & `vbtex-0.1.5/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.4/vbtex/framed.py` & `vbtex-0.1.5/vbtex/framed.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,38 @@
 
 
 
 @click.command(
     help="Renders tex expressions into pdf"
 )
 @click.option(
+    '-i',
+    '--inputtext',
+    type=click.get_text_stream('stdin'),
+    default=None,
+    show_default=True,
+    help="It takes std inputs and try to render as pdf"
+)
+@click.option(
     '-s',
     '--size',
     prompt='Format',
     type=click.Choice(['SQUARE', 'VRECT', 'HRECT']),
     cls=ChoiceOption,
     default=1,
     show_default=True,
     help="Format of the output"
 )
-def framed(size):
-    tex = click.edit()
+def framed(inputtext, size):
+    
+    if inputtext is None:
+        tex = click.edit()
+    else:
+        tex = inputtext
+
     click.echo(tex)
     
     os.makedirs(f'./vbtex', exist_ok=True)
     path_main = os.path.join(f'./vbtex', 'main.tex')
 
     
     with open(path_main, 'w') as file:
```

### Comparing `vbtex-0.1.4/vbtex/padded.py` & `vbtex-0.1.5/vbtex/padded.py`

 * *Files identical despite different names*

