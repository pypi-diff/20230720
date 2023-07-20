# Comparing `tmp/timedctl-3.2.0.tar.gz` & `tmp/timedctl-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-3.2.0.tar", max compression
+gzip compressed data, was "timedctl-3.3.0.tar", max compression
```

## Comparing `timedctl-3.2.0.tar` & `timedctl-3.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-19 23:38:19.094421 timedctl-3.2.0/LICENSE
--rw-r--r--   0        0        0      810 2023-07-19 23:38:19.094421 timedctl-3.2.0/README.md
--rw-r--r--   0        0        0      849 2023-07-19 23:38:19.938450 timedctl-3.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 23:38:19.094421 timedctl-3.2.0/timedctl/__init__.py
--rwxr-xr-x   0        0        0    14568 2023-07-19 23:38:19.094421 timedctl-3.2.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-20 13:18:35.219366 timedctl-3.3.0/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-20 13:18:35.219366 timedctl-3.3.0/README.md
+-rw-r--r--   0        0        0      849 2023-07-20 13:18:36.187407 timedctl-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 13:18:35.219366 timedctl-3.3.0/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    16533 2023-07-20 13:18:35.223366 timedctl-3.3.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.3.0/PKG-INFO
```

### Comparing `timedctl-3.2.0/LICENSE` & `timedctl-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-3.2.0/README.md` & `timedctl-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-3.2.0/pyproject.toml` & `timedctl-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "3.2.0"
+version = "3.3.0"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-3.2.0/timedctl/timedctl.py` & `timedctl-3.3.0/timedctl/timedctl.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     error_handler("ERR_FZF_EXCEPTION")
     return []
 
 
 def time_picker(default=None):
     """Interactively pick a time using either arrow keys or typing."""
     res = ""
-    while not re.match(r"^\d{2}:\d{2}:\d{2}$", res):
+    while not re.match(r"^\d{1,2}:\d{2}:\d{2}$", res):
         rich.print("[bold green]Duration[/bold green] (hh:mm:ss)", end="")
         res = click.prompt("", default=default)
     return res
 
 
 def time_sum(arr):
     """Sum up an array of time strings."""
@@ -228,15 +228,15 @@
 
 
 @get.command("activities", aliases=["a", "ac", "activity"])
 @click.option("--date", default=None)
 def get_activities(date):
     """Get activities."""
     activities = timed.activities.get(
-        {"day": date}, include="task,task.project,task.project.customer"
+        {"day": date}, include="task,task.project,task.project.customer",
     )
     table = [["Activity", "Comment", "Start", "End"]]
     for activity in activities:
         task_obj = activity["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
         project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"])
@@ -306,35 +306,63 @@
 @timedctl.group(cls=ClickAliasedGroup, aliases=["a", "create"])
 def add():
     """Add different things."""
     pass  # pylint: disable=W0107
 
 
 @add.command("report", aliases=["r"])
-def add_report():
+@click.option("--customer", default=None)
+@click.option("--project", default=None)
+@click.option("--task", default=None)
+@click.option("--description", default=None)
+@click.option("--duration", default=None)
+def add_report(customer, project, task, description, duration):
     """Add report(s)."""
     customers = timed.customers.get()
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
-    customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
+    if customer:
+        customer = [c for c in customers if c["attributes"]["name"] == customer]
+        if len(customer) == 0:
+            error_handler("ERR_CUSTOMER_NOT_FOUND")
+        customer = customer[0]
+    else:
+        customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
     projects = timed.projects.get({"customer": customer["id"]})
     # select a project
-    project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
+    if project:
+        project = [p for p in projects if p["attributes"]["name"] == project]
+        if len(project) == 0:
+            error_handler("ERR_PROJECT_NOT_FOUND")
+        project = project[0]
+    else:
+        project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
     tasks = timed.tasks.get({"project": project["id"]})
     # select a task
-    task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
+    if task:
+        task = [t for t in tasks if t["attributes"]["name"] == task]
+        if len(task) == 0:
+            error_handler("ERR_TASK_NOT_FOUND")
+        task = task[0]
+    else:
+        task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
     # ask the user to enter a description
-    msg("Enter a description")
-    # get description
-    description = click.prompt("")
+    if not description:
+        msg("Enter a description")
+        # get description
+        description = click.prompt("")
     # ask the user to enter a duration
-    duration = time_picker()
+    if duration:
+        if re.match(r"^\d{1,2}:\d{2}:\d{2}$", duration) is None:
+            error_handler("ERR_INVALID_DURATION")
+    else:
+        duration = time_picker()
     # create the report
     res = timed.reports.post(
         {"duration": duration, "comment": description},
         {
             "task": task["id"],
         },
     )
@@ -402,29 +430,50 @@
 def activity():
     """Do stuff with activities."""
     pass  # pylint: disable=W0107
 
 
 @activity.command(aliases=["add", "s"])
 @click.argument("comment")
-def start(comment):
+@click.option("--customer", default=None)
+@click.option("--project", default=None)
+@click.option("--task", default=None)
+def start(comment, customer, project, task):
     """Start recording activity."""
     customers = timed.customers.get()
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
-    customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
+    if customer:
+        customer = [c for c in customers if c["attributes"]["name"] == customer]
+        if len(customer) == 0:
+            error_handler("ERR_CUSTOMER_NOT_FOUND")
+        customer = customer[0]
+    else:
+        customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
     projects = timed.projects.get({"customer": customer["id"]})
     # select a project
-    project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
+    if project:
+        project = [p for p in projects if p["attributes"]["name"] == project]
+        if len(project) == 0:
+            error_handler("ERR_PROJECT_NOT_FOUND")
+        project = project[0]
+    else:
+        project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
     tasks = timed.tasks.get({"project": project["id"]})
     # select a task
-    task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
+    if task:
+        task = [t for t in tasks if t["attributes"]["name"] == task]
+        if len(task) == 0:
+            error_handler("ERR_TASK_NOT_FOUND")
+        task = task[0]
+    else:
+        task = fzf_wrapper(tasks, ["attributes", "name"], "Select a task: ")
     # create the activity
     res = timed.activities.start(
         attributes={"comment": comment}, relationships={"task": task["id"]}
     )
 
     if res.status_code == 201:
         msg(f"Activity {comment} started successfully.")
@@ -447,21 +496,23 @@
         msg(
             f"Current activity: {current_activity['attributes']['comment']} (Since {current_activity['attributes']['from-time'].strftime('%H:%M:%S')})"
         )
     else:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
 
 
-@activity.command()
-def generate_timesheet(aliases=["gts", "ts", "timesheet", "generate"]):
+@activity.command(aliases=["gts", "ts"])
+def generate_timesheet():
     """Generate the timesheet of the current activities."""
     activities = timed.activities.get()
     if activities:
         for activity in activities:
             if not activity["attributes"]["transferred"]:
+                if not activity["attributes"]["to-time"]:
+                    activity["attributes"]["to-time"] = datetime.now()
                 from_time = activity["attributes"]["from-time"]
                 to_time = activity["attributes"]["to-time"]
                 duration = to_time - from_time
                 task = activity["relationships"]["task"]["data"]["id"]
                 timed.reports.post(
                     {
                         "duration": duration,
```

### Comparing `timedctl-3.2.0/PKG-INFO` & `timedctl-3.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 3.2.0
+Version: 3.3.0
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

