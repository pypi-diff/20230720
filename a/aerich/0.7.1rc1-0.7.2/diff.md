# Comparing `tmp/aerich-0.7.1rc1.tar.gz` & `tmp/aerich-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerich-0.7.1rc1.tar", max compression
+gzip compressed data, was "aerich-0.7.2.tar", max compression
```

## Comparing `aerich-0.7.1rc1.tar` & `aerich-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     4337 2022-09-23 15:35:02.755230 aerich-0.7.1rc1/CHANGELOG.md
--rw-r--r--   0        0        0    11338 2022-09-23 15:35:02.755230 aerich-0.7.1rc1/LICENSE
--rw-r--r--   0        0        0     7397 2022-09-23 15:35:02.755230 aerich-0.7.1rc1/README.md
--rw-r--r--   0        0        0     5119 2022-09-23 15:35:02.755230 aerich-0.7.1rc1/aerich/__init__.py
--rw-r--r--   0        0        0     7813 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/cli.py
--rw-r--r--   0        0        0      709 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/coder.py
--rw-r--r--   0        0        0    11454 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/ddl/__init__.py
--rw-r--r--   0        0        0     1779 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/ddl/mysql/__init__.py
--rw-r--r--   0        0        0     2140 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/ddl/postgres/__init__.py
--rw-r--r--   0        0        0      960 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/ddl/sqlite/__init__.py
--rw-r--r--   0        0        0      106 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/enums.py
--rw-r--r--   0        0        0      168 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/exceptions.py
--rw-r--r--   0        0        0     5855 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/inspectdb/__init__.py
--rw-r--r--   0        0        0     2579 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/inspectdb/mysql.py
--rw-r--r--   0        0        0     3087 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/inspectdb/postgres.py
--rw-r--r--   0        0        0     2250 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/inspectdb/sqlite.py
--rw-r--r--   0        0        0    26270 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/migrate.py
--rw-r--r--   0        0        0      373 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/models.py
--rw-r--r--   0        0        0     2751 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/utils.py
--rw-r--r--   0        0        0       25 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/aerich/version.py
--rw-r--r--   0        0        0     1427 2022-09-23 15:35:02.759230 aerich-0.7.1rc1/pyproject.toml
--rw-r--r--   0        0        0     8686 1970-01-01 00:00:00.000000 aerich-0.7.1rc1/setup.py
--rw-r--r--   0        0        0     8422 1970-01-01 00:00:00.000000 aerich-0.7.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4672 2023-07-20 09:58:54.850268 aerich-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0    11338 2023-07-20 09:58:54.850268 aerich-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7441 2023-07-20 09:58:54.850268 aerich-0.7.2/README.md
+-rw-r--r--   0        0        0     5466 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/__init__.py
+-rw-r--r--   0        0        0     8060 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/cli.py
+-rw-r--r--   0        0        0      709 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/coder.py
+-rw-r--r--   0        0        0    11488 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/ddl/__init__.py
+-rw-r--r--   0        0        0     1779 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/ddl/mysql/__init__.py
+-rw-r--r--   0        0        0     2140 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/ddl/postgres/__init__.py
+-rw-r--r--   0        0        0      960 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/ddl/sqlite/__init__.py
+-rw-r--r--   0        0        0      106 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/enums.py
+-rw-r--r--   0        0        0      168 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/exceptions.py
+-rw-r--r--   0        0        0     5855 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/inspectdb/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/inspectdb/mysql.py
+-rw-r--r--   0        0        0     3087 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/inspectdb/postgres.py
+-rw-r--r--   0        0        0     2250 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/inspectdb/sqlite.py
+-rw-r--r--   0        0        0    26749 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/migrate.py
+-rw-r--r--   0        0        0      373 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/models.py
+-rw-r--r--   0        0        0     2751 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/utils.py
+-rw-r--r--   0        0        0       22 2023-07-20 09:58:54.850268 aerich-0.7.2/aerich/version.py
+-rw-r--r--   0        0        0     1423 2023-07-20 09:58:54.854268 aerich-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8536 1970-01-01 00:00:00.000000 aerich-0.7.2/PKG-INFO
```

### Comparing `aerich-0.7.1rc1/CHANGELOG.md` & `aerich-0.7.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # ChangeLog
 
 ## 0.7
 
+### 0.7.2
+
+- Support virtual fields.
+- Fix modify multiple times. (#279)
+- Added `-i` and `--in-transaction` options to `aerich migrate` command. (#296)
+- Fix generates two semicolons in a row. (#301)
+
+### 0.7.1
+
+- Fix syntax error with python3.8.10. (#265)
+- Fix sql generate error. (#263)
+- Fix initialize an empty database. (#267)
+
 ### 0.7.1rc1
 
 - Fix postgres sql error (#263)
 
 ### 0.7.0
 
 **Now aerich use `.py` file to record versions.**
```

### Comparing `aerich-0.7.1rc1/LICENSE` & `aerich-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/README.md` & `aerich-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Aerich
 
 [![image](https://img.shields.io/pypi/v/aerich.svg?style=flat)](https://pypi.python.org/pypi/aerich)
 [![image](https://img.shields.io/github/license/tortoise/aerich)](https://github.com/tortoise/aerich)
 [![image](https://github.com/tortoise/aerich/workflows/pypi/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:pypi)
 [![image](https://github.com/tortoise/aerich/workflows/ci/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:ci)
 
+English | [Русский](./README_RU.md)
+
 ## Introduction
 
 Aerich is a database migrations tool for TortoiseORM, which is like alembic for SQLAlchemy, or like Django ORM with
 it\'s own migration solution.
 
 ## Install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aerich-0.7.1rc1/aerich/__init__.py` & `aerich-0.7.2/aerich/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,34 +32,40 @@
         self.app = app
         self.location = location
         Migrate.app = app
 
     async def init(self):
         await Migrate.init(self.tortoise_config, self.app, self.location)
 
-    async def upgrade(self):
+    async def _upgrade(self, conn, version_file):
+        file_path = Path(Migrate.migrate_location, version_file)
+        m = import_py_file(file_path)
+        upgrade = getattr(m, "upgrade")
+        await conn.execute_script(await upgrade(conn))
+        await Aerich.create(
+            version=version_file,
+            app=self.app,
+            content=get_models_describe(self.app),
+        )
+
+    async def upgrade(self, run_in_transaction: bool):
         migrated = []
         for version_file in Migrate.get_all_version_files():
             try:
                 exists = await Aerich.exists(version=version_file, app=self.app)
             except OperationalError:
                 exists = False
             if not exists:
-                async with in_transaction(
-                    get_app_connection_name(self.tortoise_config, self.app)
-                ) as conn:
-                    file_path = Path(Migrate.migrate_location, version_file)
-                    m = import_py_file(file_path)
-                    upgrade = getattr(m, "upgrade")
-                    await upgrade(conn)
-                    await Aerich.create(
-                        version=version_file,
-                        app=self.app,
-                        content=get_models_describe(self.app),
-                    )
+                app_conn_name = get_app_connection_name(self.tortoise_config, self.app)
+                if run_in_transaction:
+                    async with in_transaction(app_conn_name) as conn:
+                        await self._upgrade(conn, version_file)
+                else:
+                    app_conn = get_app_connection(self.tortoise_config, self.app)
+                    await self._upgrade(app_conn, version_file)
                 migrated.append(version_file)
         return migrated
 
     async def downgrade(self, version: int, delete: bool):
         ret = []
         if version == -1:
             specified_version = await Migrate.get_last_version()
@@ -76,18 +82,19 @@
         for version in versions:
             file = version.version
             async with in_transaction(
                 get_app_connection_name(self.tortoise_config, self.app)
             ) as conn:
                 file_path = Path(Migrate.migrate_location, file)
                 m = import_py_file(file_path)
-                downgrade = getattr(m, "downgrade", None)
-                if not downgrade:
+                downgrade = getattr(m, "downgrade")
+                downgrade_sql = await downgrade(conn)
+                if not downgrade_sql.strip():
                     raise DowngradeError("No downgrade items found")
-                await downgrade(conn)
+                await conn.execute_script(downgrade_sql)
                 await version.delete()
                 if delete:
                     os.unlink(file_path)
                 ret.append(file)
         return ret
 
     async def heads(self):
@@ -134,10 +141,10 @@
         version = await Migrate.generate_version()
         await Aerich.create(
             version=version,
             app=app,
             content=get_models_describe(app),
         )
         version_file = Path(dirname, version)
-        content = MIGRATE_TEMPLATE.format(upgrade_sql=f'"""{schema}"""', downgrade_sql="")
+        content = MIGRATE_TEMPLATE.format(upgrade_sql=schema, downgrade_sql="")
         with open(version_file, "w", encoding="utf-8") as f:
             f.write(content)
```

### Comparing `aerich-0.7.1rc1/aerich/cli.py` & `aerich-0.7.2/aerich/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def wrapper(*args, **kwargs):
         loop = asyncio.get_event_loop()
 
         # Close db connections at the end of all but the cli group function
         try:
             loop.run_until_complete(f(*args, **kwargs))
         finally:
-            if f.__name__ not in ["cli", "init_db", "init"]:
+            if f.__name__ not in ["cli", "init"]:
                 loop.run_until_complete(Tortoise.close_connections())
 
     return wrapper
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(__version__, "-V", "--version")
@@ -86,19 +86,26 @@
     ret = await command.migrate(name)
     if not ret:
         return click.secho("No changes detected", fg=Color.yellow)
     click.secho(f"Success migrate {ret}", fg=Color.green)
 
 
 @cli.command(help="Upgrade to specified version.")
+@click.option(
+    "--in-transaction",
+    "-i",
+    default=True,
+    type=bool,
+    help="Make migrations in transaction or not. Can be helpful for large migrations or creating concurrent indexes.",
+)
 @click.pass_context
 @coro
-async def upgrade(ctx: Context):
+async def upgrade(ctx: Context, in_transaction: bool):
     command = ctx.obj["command"]
-    migrated = await command.upgrade()
+    migrated = await command.upgrade(run_in_transaction=in_transaction)
     if not migrated:
         click.secho("No upgrade items found", fg=Color.yellow)
     else:
         for version_file in migrated:
             click.secho(f"Success upgrade {version_file}", fg=Color.green)
```

### Comparing `aerich-0.7.1rc1/aerich/coder.py` & `aerich-0.7.2/aerich/coder.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/ddl/__init__.py` & `aerich-0.7.2/aerich/ddl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     _RENAME_TABLE_TEMPLATE = 'ALTER TABLE "{old_table_name}" RENAME TO "{new_table_name}"'
 
     def __init__(self, client: "BaseDBAsyncClient"):
         self.client = client
         self.schema_generator = self.schema_generator_cls(client)
 
     def create_table(self, model: "Type[Model]"):
-        return self.schema_generator._get_table_sql(model, True)["table_creation_string"]
+        return self.schema_generator._get_table_sql(model, True)["table_creation_string"].rstrip(
+            ";"
+        )
 
     def drop_table(self, table_name: str):
         return self._DROP_TABLE_TEMPLATE.format(table_name=table_name)
 
     def create_m2m(
         self, model: "Type[Model]", field_describe: dict, reference_table_describe: dict
     ):
```

### Comparing `aerich-0.7.1rc1/aerich/ddl/mysql/__init__.py` & `aerich-0.7.2/aerich/ddl/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/ddl/postgres/__init__.py` & `aerich-0.7.2/aerich/ddl/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/ddl/sqlite/__init__.py` & `aerich-0.7.2/aerich/ddl/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/inspectdb/__init__.py` & `aerich-0.7.2/aerich/inspectdb/__init__.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/inspectdb/mysql.py` & `aerich-0.7.2/aerich/inspectdb/mysql.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/inspectdb/postgres.py` & `aerich-0.7.2/aerich/inspectdb/postgres.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/inspectdb/sqlite.py` & `aerich-0.7.2/aerich/inspectdb/sqlite.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/aerich/migrate.py` & `aerich-0.7.2/aerich/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 from tortoise.exceptions import OperationalError
 from tortoise.indexes import Index
 
 from aerich.ddl import BaseDDL
 from aerich.models import MAX_VERSION_LENGTH, Aerich
 from aerich.utils import get_app_connection, get_models_describe, is_default_function
 
-MIGRATE_TEMPLATE = """from typing import List
+MIGRATE_TEMPLATE = """from tortoise import BaseDBAsyncClient
 
-from tortoise import BaseDBAsyncClient
 
+async def upgrade(db: BaseDBAsyncClient) -> str:
+    return \"\"\"
+        {upgrade_sql}\"\"\"
 
-async def upgrade(db: BaseDBAsyncClient) -> List[str]:
-    return [
-        {upgrade_sql}
-    ]
 
-
-async def downgrade(db: BaseDBAsyncClient) -> List[str]:
-    return [
-        {downgrade_sql}
-    ]
+async def downgrade(db: BaseDBAsyncClient) -> str:
+    return \"\"\"
+        {downgrade_sql}\"\"\"
 """
 
 
 class Migrate:
     upgrade_operators: List[str] = []
     downgrade_operators: List[str] = []
     _upgrade_fk_m2m_index_operators: List[str] = []
@@ -48,15 +44,15 @@
     _last_version_content: Optional[dict] = None
     app: str
     migrate_location: Path
     dialect: str
     _db_version: Optional[str] = None
 
     @classmethod
-    def get_all_version_files(cls) -> list[str]:
+    def get_all_version_files(cls) -> List[str]:
         return sorted(
             filter(lambda x: x.endswith("py"), os.listdir(cls.migrate_location)),
             key=lambda x: int(x.split("_")[0]),
         )
 
     @classmethod
     def _get_model(cls, model: str) -> Type[Model]:
@@ -121,17 +117,18 @@
         # delete if same version exists
         for version_file in cls.get_all_version_files():
             if version_file.startswith(version.split("_")[0]):
                 os.unlink(Path(cls.migrate_location, version_file))
 
         version_file = Path(cls.migrate_location, version)
         content = MIGRATE_TEMPLATE.format(
-            upgrade_sql=",\n        ".join(map(lambda x: f"'{x}'", cls.upgrade_operators)),
-            downgrade_sql=",\n        ".join(map(lambda x: f"'{x}'", cls.downgrade_operators)),
+            upgrade_sql=";\n        ".join(cls.upgrade_operators) + ";",
+            downgrade_sql=";\n        ".join(cls.downgrade_operators) + ";",
         )
+
         with open(version_file, "w", encoding="utf-8") as f:
             f.write(content)
         return version
 
     @classmethod
     async def migrate(cls, name) -> str:
         """
@@ -155,14 +152,15 @@
         """
         add operator,differentiate fk because fk is order limit
         :param operator:
         :param upgrade:
         :param fk_m2m_index:
         :return:
         """
+        operator = operator.rstrip(";")
         if upgrade:
             if fk_m2m_index:
                 cls._upgrade_fk_m2m_index_operators.append(operator)
             else:
                 cls.upgrade_operators.append(operator)
         else:
             if fk_m2m_index:
@@ -280,16 +278,26 @@
                     cls._add_operator(cls._drop_index(model, index, True), upgrade, True)
                 # add indexes
                 for index in new_indexes.difference(old_indexes):
                     cls._add_operator(cls._add_index(model, index, False), upgrade, True)
                 # remove indexes
                 for index in old_indexes.difference(new_indexes):
                     cls._add_operator(cls._drop_index(model, index, False), upgrade, True)
-                old_data_fields = old_model_describe.get("data_fields")
-                new_data_fields = new_model_describe.get("data_fields")
+                old_data_fields = list(
+                    filter(
+                        lambda x: x.get("db_field_types") is not None,
+                        old_model_describe.get("data_fields"),
+                    )
+                )
+                new_data_fields = list(
+                    filter(
+                        lambda x: x.get("db_field_types") is not None,
+                        new_model_describe.get("data_fields"),
+                    )
+                )
 
                 old_data_fields_name = list(map(lambda x: x.get("name"), old_data_fields))
                 new_data_fields_name = list(map(lambda x: x.get("name"), new_data_fields))
 
                 # add fields or rename fields
                 for new_data_field_name in set(new_data_fields_name).difference(
                     set(old_data_fields_name)
@@ -437,14 +445,15 @@
                     old_data_field = next(
                         filter(lambda x: x.get("name") == field_name, old_data_fields)
                     )
                     new_data_field = next(
                         filter(lambda x: x.get("name") == field_name, new_data_fields)
                     )
                     changes = diff(old_data_field, new_data_field)
+                    modified = False
                     for change in changes:
                         _, option, old_new = change
                         if option == "indexed":
                             # change index
                             unique = new_data_field.get("unique")
                             if old_new[0] is False and old_new[1] is True:
                                 cls._add_operator(
@@ -474,19 +483,22 @@
                         elif option == "unique":
                             # because indexed include it
                             continue
                         elif option == "nullable":
                             # change nullable
                             cls._add_operator(cls._alter_null(model, new_data_field), upgrade)
                         else:
+                            if modified:
+                                continue
                             # modify column
                             cls._add_operator(
                                 cls._modify_field(model, new_data_field),
                                 upgrade,
                             )
+                            modified = True
 
         for old_model in old_models:
             if old_model not in new_models.keys():
                 cls._add_operator(cls.drop_model(old_models.get(old_model).get("table")), upgrade)
 
     @classmethod
     def rename_table(cls, model: Type[Model], old_table_name: str, new_table_name: str):
```

### Comparing `aerich-0.7.1rc1/aerich/utils.py` & `aerich-0.7.2/aerich/utils.py`

 * *Files identical despite different names*

### Comparing `aerich-0.7.1rc1/pyproject.toml` & `aerich-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aerich"
-version = "0.7.1rc1"
+version = "0.7.2"
 description = "A database migrations tool for Tortoise ORM."
 authors = ["long2ice <long2ice@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/tortoise/aerich"
 repository = "https://github.com/tortoise/aerich.git"
 documentation = "https://github.com/tortoise/aerich"
@@ -15,30 +15,29 @@
 include = ["CHANGELOG.md", "LICENSE", "README.md"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tortoise-orm = "*"
 click = "*"
 asyncpg = { version = "*", optional = true }
-asyncmy = { version = "*", optional = true }
+asyncmy = { version = "^0.2.8rc1", optional = true, allow-prereleases = true }
 pydantic = "*"
 dictdiffer = "*"
 tomlkit = "*"
 
 [tool.poetry.dev-dependencies]
-flake8 = "*"
+ruff = "*"
 isort = "*"
 black = "*"
 pytest = "*"
 pytest-xdist = "*"
 pytest-asyncio = "*"
 bandit = "*"
 pytest-mock = "*"
 cryptography = "*"
-pyproject-flake8 = "*"
 
 [tool.poetry.extras]
 asyncmy = ["asyncmy"]
 asyncpg = ["asyncpg"]
 
 [tool.aerich]
 tortoise_orm = "conftest.tortoise_orm"
@@ -59,9 +58,9 @@
 [tool.pytest.ini_options]
 asyncio_mode = 'auto'
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 
-[tool.flake8]
-ignore = 'E501,W503,E203'
+[tool.ruff]
+ignore = ['E501']
```

### Comparing `aerich-0.7.1rc1/setup.py` & `aerich-0.7.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,307 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aerich
+Version: 0.7.2
+Summary: A database migrations tool for Tortoise ORM.
+Home-page: https://github.com/tortoise/aerich
+License: Apache-2.0
+Keywords: migrate,Tortoise-ORM,mysql
+Author: long2ice
+Author-email: long2ice@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: asyncmy
+Provides-Extra: asyncpg
+Requires-Dist: asyncmy (>=0.2.8rc1,<0.3.0) ; extra == "asyncmy"
+Requires-Dist: asyncpg ; extra == "asyncpg"
+Requires-Dist: click
+Requires-Dist: dictdiffer
+Requires-Dist: pydantic
+Requires-Dist: tomlkit
+Requires-Dist: tortoise-orm
+Project-URL: Documentation, https://github.com/tortoise/aerich
+Project-URL: Repository, https://github.com/tortoise/aerich.git
+Description-Content-Type: text/markdown
 
-packages = \
-['aerich',
- 'aerich.ddl',
- 'aerich.ddl.mysql',
- 'aerich.ddl.postgres',
- 'aerich.ddl.sqlite',
- 'aerich.inspectdb']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click', 'dictdiffer', 'pydantic', 'tomlkit', 'tortoise-orm']
-
-extras_require = \
-{'asyncmy': ['asyncmy'], 'asyncpg': ['asyncpg']}
-
-entry_points = \
-{'console_scripts': ['aerich = aerich.cli:main']}
-
-setup_kwargs = {
-    'name': 'aerich',
-    'version': '0.7.1rc1',
-    'description': 'A database migrations tool for Tortoise ORM.',
-    'long_description': '# Aerich\n\n[![image](https://img.shields.io/pypi/v/aerich.svg?style=flat)](https://pypi.python.org/pypi/aerich)\n[![image](https://img.shields.io/github/license/tortoise/aerich)](https://github.com/tortoise/aerich)\n[![image](https://github.com/tortoise/aerich/workflows/pypi/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:pypi)\n[![image](https://github.com/tortoise/aerich/workflows/ci/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:ci)\n\n## Introduction\n\nAerich is a database migrations tool for TortoiseORM, which is like alembic for SQLAlchemy, or like Django ORM with\nit\\\'s own migration solution.\n\n## Install\n\nJust install from pypi:\n\n```shell\npip install aerich\n```\n\n## Quick Start\n\n```shell\n> aerich -h\n\nUsage: aerich [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  -V, --version      Show the version and exit.\n  -c, --config TEXT  Config file.  [default: pyproject.toml]\n  --app TEXT         Tortoise-ORM app name.\n  -h, --help         Show this message and exit.\n\nCommands:\n  downgrade  Downgrade to specified version.\n  heads      Show current available heads in migrate location.\n  history    List all migrate items.\n  init       Init config file and generate root migrate location.\n  init-db    Generate schema and generate app migrate location.\n  inspectdb  Introspects the database tables to standard output as...\n  migrate    Generate migrate changes file.\n  upgrade    Upgrade to specified version.\n```\n\n## Usage\n\nYou need add `aerich.models` to your `Tortoise-ORM` config first. Example:\n\n```python\nTORTOISE_ORM = {\n    "connections": {"default": "mysql://root:123456@127.0.0.1:3306/test"},\n    "apps": {\n        "models": {\n            "models": ["tests.models", "aerich.models"],\n            "default_connection": "default",\n        },\n    },\n}\n```\n\n### Initialization\n\n```shell\n> aerich init -h\n\nUsage: aerich init [OPTIONS]\n\n  Init config file and generate root migrate location.\n\nOptions:\n  -t, --tortoise-orm TEXT  Tortoise-ORM config module dict variable, like\n                           settings.TORTOISE_ORM.  [required]\n  --location TEXT          Migrate store location.  [default: ./migrations]\n  -s, --src_folder TEXT    Folder of the source, relative to the project root.\n  -h, --help               Show this message and exit.\n```\n\nInitialize the config file and migrations location:\n\n```shell\n> aerich init -t tests.backends.mysql.TORTOISE_ORM\n\nSuccess create migrate location ./migrations\nSuccess write config to pyproject.toml\n```\n\n### Init db\n\n```shell\n> aerich init-db\n\nSuccess create app migrate location ./migrations/models\nSuccess generate schema for app "models"\n```\n\nIf your Tortoise-ORM app is not the default `models`, you must specify the correct app via `--app`,\ne.g. `aerich --app other_models init-db`.\n\n### Update models and make migrate\n\n```shell\n> aerich migrate --name drop_column\n\nSuccess migrate 1_202029051520102929_drop_column.py\n```\n\nFormat of migrate filename is\n`{version_num}_{datetime}_{name|update}.py`.\n\nIf `aerich` guesses you are renaming a column, it will ask `Rename {old_column} to {new_column} [True]`. You can choose\n`True` to rename column without column drop, or choose `False` to drop the column then create. Note that the latter may\nlose data.\n\n### Upgrade to latest version\n\n```shell\n> aerich upgrade\n\nSuccess upgrade 1_202029051520102929_drop_column.py\n```\n\nNow your db is migrated to latest.\n\n### Downgrade to specified version\n\n```shell\n> aerich downgrade -h\n\nUsage: aerich downgrade [OPTIONS]\n\n  Downgrade to specified version.\n\nOptions:\n  -v, --version INTEGER  Specified version, default to last.  [default: -1]\n  -d, --delete           Delete version files at the same time.  [default:\n                         False]\n\n  --yes                  Confirm the action without prompting.\n  -h, --help             Show this message and exit.\n```\n\n```shell\n> aerich downgrade\n\nSuccess downgrade 1_202029051520102929_drop_column.py\n```\n\nNow your db is rolled back to the specified version.\n\n### Show history\n\n```shell\n> aerich history\n\n1_202029051520102929_drop_column.py\n```\n\n### Show heads to be migrated\n\n```shell\n> aerich heads\n\n1_202029051520102929_drop_column.py\n```\n\n### Inspect db tables to TortoiseORM model\n\nCurrently `inspectdb` support MySQL & Postgres & SQLite.\n\n```shell\nUsage: aerich inspectdb [OPTIONS]\n\n  Introspects the database tables to standard output as TortoiseORM model.\n\nOptions:\n  -t, --table TEXT  Which tables to inspect.\n  -h, --help        Show this message and exit.\n```\n\nInspect all tables and print to console:\n\n```shell\naerich --app models inspectdb\n```\n\nInspect a specified table in the default app and redirect to `models.py`:\n\n```shell\naerich inspectdb -t user > models.py\n```\n\nFor example, you table is:\n\n```sql\nCREATE TABLE `test`\n(\n    `id`       int            NOT NULL AUTO_INCREMENT,\n    `decimal`  decimal(10, 2) NOT NULL,\n    `date`     date                                    DEFAULT NULL,\n    `datetime` datetime       NOT NULL                 DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,\n    `time`     time                                    DEFAULT NULL,\n    `float`    float                                   DEFAULT NULL,\n    `string`   varchar(200) COLLATE utf8mb4_general_ci DEFAULT NULL,\n    `tinyint`  tinyint                                 DEFAULT NULL,\n    PRIMARY KEY (`id`),\n    KEY `asyncmy_string_index` (`string`)\n) ENGINE = InnoDB\n  DEFAULT CHARSET = utf8mb4\n  COLLATE = utf8mb4_general_ci\n```\n\nNow run `aerich inspectdb -t test` to see the generated model:\n\n```python\nfrom tortoise import Model, fields\n\n\nclass Test(Model):\n    date = fields.DateField(null=True, )\n    datetime = fields.DatetimeField(auto_now=True, )\n    decimal = fields.DecimalField(max_digits=10, decimal_places=2, )\n    float = fields.FloatField(null=True, )\n    id = fields.IntField(pk=True, )\n    string = fields.CharField(max_length=200, null=True, )\n    time = fields.TimeField(null=True, )\n    tinyint = fields.BooleanField(null=True, )\n```\n\nNote that this command is limited and can\'t infer some fields, such as `IntEnumField`, `ForeignKeyField`, and others.\n\n### Multiple databases\n\n```python\ntortoise_orm = {\n    "connections": {\n        "default": expand_db_url(db_url, True),\n        "second": expand_db_url(db_url_second, True),\n    },\n    "apps": {\n        "models": {"models": ["tests.models", "aerich.models"], "default_connection": "default"},\n        "models_second": {"models": ["tests.models_second"], "default_connection": "second", },\n    },\n}\n```\n\nYou only need to specify `aerich.models` in one app, and must specify `--app` when running `aerich migrate` and so on.\n\n## Restore `aerich` workflow\n\nIn some cases, such as broken changes from upgrade of `aerich`, you can\'t run `aerich migrate` or `aerich upgrade`, you\ncan make the following steps:\n\n1. drop `aerich` table.\n2. delete `migrations/{app}` directory.\n3. rerun `aerich init-db`.\n\nNote that these actions is safe, also you can do that to reset your migrations if your migration files is too many.\n\n## Use `aerich` in application\n\nYou can use `aerich` out of cli by use `Command` class.\n\n```python\nfrom aerich import Command\n\ncommand = Command(tortoise_config=config, app=\'models\')\nawait command.init()\nawait command.migrate(\'test\')\n```\n\n## License\n\nThis project is licensed under the\n[Apache-2.0](https://github.com/long2ice/aerich/blob/master/LICENSE) License.\n',
-    'author': 'long2ice',
-    'author_email': 'long2ice@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tortoise/aerich',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+# Aerich
+
+[![image](https://img.shields.io/pypi/v/aerich.svg?style=flat)](https://pypi.python.org/pypi/aerich)
+[![image](https://img.shields.io/github/license/tortoise/aerich)](https://github.com/tortoise/aerich)
+[![image](https://github.com/tortoise/aerich/workflows/pypi/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:pypi)
+[![image](https://github.com/tortoise/aerich/workflows/ci/badge.svg)](https://github.com/tortoise/aerich/actions?query=workflow:ci)
+
+English | [Русский](./README_RU.md)
+
+## Introduction
+
+Aerich is a database migrations tool for TortoiseORM, which is like alembic for SQLAlchemy, or like Django ORM with
+it\'s own migration solution.
+
+## Install
+
+Just install from pypi:
+
+```shell
+pip install aerich
+```
+
+## Quick Start
+
+```shell
+> aerich -h
+
+Usage: aerich [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -V, --version      Show the version and exit.
+  -c, --config TEXT  Config file.  [default: pyproject.toml]
+  --app TEXT         Tortoise-ORM app name.
+  -h, --help         Show this message and exit.
+
+Commands:
+  downgrade  Downgrade to specified version.
+  heads      Show current available heads in migrate location.
+  history    List all migrate items.
+  init       Init config file and generate root migrate location.
+  init-db    Generate schema and generate app migrate location.
+  inspectdb  Introspects the database tables to standard output as...
+  migrate    Generate migrate changes file.
+  upgrade    Upgrade to specified version.
+```
+
+## Usage
+
+You need add `aerich.models` to your `Tortoise-ORM` config first. Example:
+
+```python
+TORTOISE_ORM = {
+    "connections": {"default": "mysql://root:123456@127.0.0.1:3306/test"},
+    "apps": {
+        "models": {
+            "models": ["tests.models", "aerich.models"],
+            "default_connection": "default",
+        },
+    },
+}
+```
+
+### Initialization
+
+```shell
+> aerich init -h
+
+Usage: aerich init [OPTIONS]
+
+  Init config file and generate root migrate location.
+
+Options:
+  -t, --tortoise-orm TEXT  Tortoise-ORM config module dict variable, like
+                           settings.TORTOISE_ORM.  [required]
+  --location TEXT          Migrate store location.  [default: ./migrations]
+  -s, --src_folder TEXT    Folder of the source, relative to the project root.
+  -h, --help               Show this message and exit.
+```
+
+Initialize the config file and migrations location:
+
+```shell
+> aerich init -t tests.backends.mysql.TORTOISE_ORM
+
+Success create migrate location ./migrations
+Success write config to pyproject.toml
+```
+
+### Init db
+
+```shell
+> aerich init-db
+
+Success create app migrate location ./migrations/models
+Success generate schema for app "models"
+```
+
+If your Tortoise-ORM app is not the default `models`, you must specify the correct app via `--app`,
+e.g. `aerich --app other_models init-db`.
+
+### Update models and make migrate
+
+```shell
+> aerich migrate --name drop_column
+
+Success migrate 1_202029051520102929_drop_column.py
+```
+
+Format of migrate filename is
+`{version_num}_{datetime}_{name|update}.py`.
+
+If `aerich` guesses you are renaming a column, it will ask `Rename {old_column} to {new_column} [True]`. You can choose
+`True` to rename column without column drop, or choose `False` to drop the column then create. Note that the latter may
+lose data.
+
+### Upgrade to latest version
+
+```shell
+> aerich upgrade
+
+Success upgrade 1_202029051520102929_drop_column.py
+```
+
+Now your db is migrated to latest.
+
+### Downgrade to specified version
+
+```shell
+> aerich downgrade -h
+
+Usage: aerich downgrade [OPTIONS]
+
+  Downgrade to specified version.
+
+Options:
+  -v, --version INTEGER  Specified version, default to last.  [default: -1]
+  -d, --delete           Delete version files at the same time.  [default:
+                         False]
+
+  --yes                  Confirm the action without prompting.
+  -h, --help             Show this message and exit.
+```
+
+```shell
+> aerich downgrade
+
+Success downgrade 1_202029051520102929_drop_column.py
+```
+
+Now your db is rolled back to the specified version.
+
+### Show history
+
+```shell
+> aerich history
+
+1_202029051520102929_drop_column.py
+```
+
+### Show heads to be migrated
+
+```shell
+> aerich heads
+
+1_202029051520102929_drop_column.py
+```
+
+### Inspect db tables to TortoiseORM model
+
+Currently `inspectdb` support MySQL & Postgres & SQLite.
+
+```shell
+Usage: aerich inspectdb [OPTIONS]
+
+  Introspects the database tables to standard output as TortoiseORM model.
+
+Options:
+  -t, --table TEXT  Which tables to inspect.
+  -h, --help        Show this message and exit.
+```
+
+Inspect all tables and print to console:
+
+```shell
+aerich --app models inspectdb
+```
+
+Inspect a specified table in the default app and redirect to `models.py`:
+
+```shell
+aerich inspectdb -t user > models.py
+```
+
+For example, you table is:
+
+```sql
+CREATE TABLE `test`
+(
+    `id`       int            NOT NULL AUTO_INCREMENT,
+    `decimal`  decimal(10, 2) NOT NULL,
+    `date`     date                                    DEFAULT NULL,
+    `datetime` datetime       NOT NULL                 DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
+    `time`     time                                    DEFAULT NULL,
+    `float`    float                                   DEFAULT NULL,
+    `string`   varchar(200) COLLATE utf8mb4_general_ci DEFAULT NULL,
+    `tinyint`  tinyint                                 DEFAULT NULL,
+    PRIMARY KEY (`id`),
+    KEY `asyncmy_string_index` (`string`)
+) ENGINE = InnoDB
+  DEFAULT CHARSET = utf8mb4
+  COLLATE = utf8mb4_general_ci
+```
+
+Now run `aerich inspectdb -t test` to see the generated model:
+
+```python
+from tortoise import Model, fields
+
+
+class Test(Model):
+    date = fields.DateField(null=True, )
+    datetime = fields.DatetimeField(auto_now=True, )
+    decimal = fields.DecimalField(max_digits=10, decimal_places=2, )
+    float = fields.FloatField(null=True, )
+    id = fields.IntField(pk=True, )
+    string = fields.CharField(max_length=200, null=True, )
+    time = fields.TimeField(null=True, )
+    tinyint = fields.BooleanField(null=True, )
+```
+
+Note that this command is limited and can't infer some fields, such as `IntEnumField`, `ForeignKeyField`, and others.
+
+### Multiple databases
+
+```python
+tortoise_orm = {
+    "connections": {
+        "default": expand_db_url(db_url, True),
+        "second": expand_db_url(db_url_second, True),
+    },
+    "apps": {
+        "models": {"models": ["tests.models", "aerich.models"], "default_connection": "default"},
+        "models_second": {"models": ["tests.models_second"], "default_connection": "second", },
+    },
 }
+```
+
+You only need to specify `aerich.models` in one app, and must specify `--app` when running `aerich migrate` and so on.
+
+## Restore `aerich` workflow
+
+In some cases, such as broken changes from upgrade of `aerich`, you can't run `aerich migrate` or `aerich upgrade`, you
+can make the following steps:
+
+1. drop `aerich` table.
+2. delete `migrations/{app}` directory.
+3. rerun `aerich init-db`.
+
+Note that these actions is safe, also you can do that to reset your migrations if your migration files is too many.
+
+## Use `aerich` in application
+
+You can use `aerich` out of cli by use `Command` class.
+
+```python
+from aerich import Command
+
+command = Command(tortoise_config=config, app='models')
+await command.init()
+await command.migrate('test')
+```
+
+## License
 
+This project is licensed under the
+[Apache-2.0](https://github.com/long2ice/aerich/blob/master/LICENSE) License.
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

