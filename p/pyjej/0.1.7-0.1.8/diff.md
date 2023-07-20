# Comparing `tmp/pyjej-0.1.7.tar.gz` & `tmp/pyjej-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.7.tar", max compression
+gzip compressed data, was "pyjej-0.1.8.tar", max compression
```

## Comparing `pyjej-0.1.7.tar` & `pyjej-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10796 2023-05-26 15:26:43.521571 pyjej-0.1.7/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.7/pyjej/__main__.py
--rw-r--r--   0        0        0      142 2023-05-26 14:31:45.812687 pyjej-0.1.7/pyjej/groovy/export_plugins.txt
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.7/pyjej/selflib.py
--rw-r--r--   0        0        0     4213 2023-05-26 14:45:01.866921 pyjej-0.1.7/pyjej/tasks.py
--rw-r--r--   0        0        0      400 2023-05-26 14:49:43.698251 pyjej-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    11427 1970-01-01 00:00:00.000000 pyjej-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10796 2023-07-20 11:38:25.750723 pyjej-0.1.8/README.md
+-rw-r--r--   0        0        0      171 2023-07-20 11:38:25.750723 pyjej-0.1.8/pyjej/__main__.py
+-rw-r--r--   0        0        0      142 2023-07-20 11:38:25.750723 pyjej-0.1.8/pyjej/groovy/export_plugins.txt
+-rw-r--r--   0        0        0     1956 2023-07-20 11:38:25.750723 pyjej-0.1.8/pyjej/selflib.py
+-rw-r--r--   0        0        0     4657 2023-07-20 11:59:58.554996 pyjej-0.1.8/pyjej/tasks.py
+-rw-r--r--   0        0        0      400 2023-07-20 12:01:51.699108 pyjej-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    11427 1970-01-01 00:00:00.000000 pyjej-0.1.8/PKG-INFO
```

### Comparing `pyjej-0.1.7/README.md` & `pyjej-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.7/pyjej/selflib.py` & `pyjej-0.1.8/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.7/pyjej/tasks.py` & `pyjej-0.1.8/pyjej/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,45 @@
 
 def get_base_command_cli(server):
     return INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
 
 @task
 def export_all_jobs(ctx: Runner, server: str):
-    """Экспортировать указанную Job из Jenkins"""
+    """Экспортировать все Job из Jenkins"""
+    dir_server = pathlib.Path("data", server, "jobs")
     base_command_cli = get_base_command_cli(server)
     pathlib.Path("data", server, "jobs").mkdir(parents=True, exist_ok=True)
     # Получить список всех Job
-    jobs: Result = ctx.run(f"{base_command_cli} list-jobs", hide=True).stdout.split(
-        "\n"
-    )
+    jobs_jenkins: Result = ctx.run(
+        f"{base_command_cli} list-jobs", hide=True
+    ).stdout.split("\n")
+    # Удаляем задачи которых нет в Jenkins
+    job_in_dir = set(map(lambda x: x.stem, dir_server.glob("*")))
+    # Файлы которые есть локально, но которых нет на сервере Jenkins
+    file_no_jenkins = set(job_in_dir).difference(jobs_jenkins)
+    for p in file_no_jenkins:
+        os.remove(dir_server / f"{p}.xml")
     # Перебрать в цикле все job и скачать их в XML
-    commands = [(f'{base_command_cli} get-job "{job}"', job) for job in jobs if job]
+    commands = [
+        (f'{base_command_cli} get-job "{job}"', job) for job in jobs_jenkins if job
+    ]
     print("count jobs: ", len(commands))
     # Выполнить команды асинхронно
     os_exe_async(
         commands,
-        handle=lambda label, stdout, stderr, cod, cmd: pathlib.Path(
-            "data", server, "jobs", f"{label}.xml"
+        handle=lambda label, stdout, stderr, cod, cmd: (
+            dir_server / f"{label}.xml"
         ).write_text(stdout),
     )
 
 
 @task
 def export_job(ctx: Runner, server: str, jobname: str):
-    """Экспортировать все Job из Jenkins"""
+    """Экспортировать указанную Job из Jenkins"""
     pathlib.Path("data", server, "jobs").mkdir(parents=True, exist_ok=True)
     res: Result = ctx.run(
         f"{get_base_command_cli(server)} get-job {jobname}", hide=True
     )
     if not res.stderr:
         pathlib.Path("data", server, "jobs", f"{jobname}.xml").write_text(res.stdout)
```

### Comparing `pyjej-0.1.7/PKG-INFO` & `pyjej-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.7
+Version: 0.1.8
 Summary: Проект для взаимодействия с Jenkins через CLI
 Author: Кустов Денис
 Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

