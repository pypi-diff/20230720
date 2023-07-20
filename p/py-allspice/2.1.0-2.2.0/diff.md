# Comparing `tmp/py-allspice-2.1.0.tar.gz` & `tmp/py-allspice-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-allspice-2.1.0.tar", last modified: Wed Jun 28 17:43:51 2023, max compression
+gzip compressed data, was "py-allspice-2.2.0.tar", last modified: Thu Jul 20 20:07:05 2023, max compression
```

## Comparing `py-allspice-2.1.0.tar` & `py-allspice-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 17:43:51.687418 py-allspice-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-28 17:43:35.000000 py-allspice-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-28 17:43:51.687418 py-allspice-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-28 17:43:35.000000 py-allspice-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 17:43:51.683418 py-allspice-2.1.0/allspice/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/allspice.py
--rw-r--r--   0 runner    (1001) docker     (123)    55853 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/apiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/baseapiobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-28 17:43:35.000000 py-allspice-2.1.0/allspice/ratelimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 17:43:51.687418 py-allspice-2.1.0/py_allspice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-28 17:43:51.000000 py-allspice-2.1.0/py_allspice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-28 17:43:51.000000 py-allspice-2.1.0/py_allspice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 17:43:51.000000 py-allspice-2.1.0/py_allspice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-28 17:43:51.000000 py-allspice-2.1.0/py_allspice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 17:43:51.000000 py-allspice-2.1.0/py_allspice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 17:43:51.687418 py-allspice-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-28 17:43:42.000000 py-allspice-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 17:43:51.687418 py-allspice-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-06-28 17:43:35.000000 py-allspice-2.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-28 17:43:35.000000 py-allspice-2.1.0/tests/test_api_longtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-28 17:43:35.000000 py-allspice-2.1.0/tests/test_api_ratelimiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 20:06:48.000000 py-allspice-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-20 20:07:05.506049 py-allspice-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-20 20:06:48.000000 py-allspice-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.502049 py-allspice-2.2.0/allspice/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/allspice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58771 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/apiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/baseapiobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-20 20:06:48.000000 py-allspice-2.2.0/allspice/ratelimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/py_allspice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 20:07:05.000000 py-allspice-2.2.0/py_allspice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:07:05.506049 py-allspice-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 20:06:54.000000 py-allspice-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:07:05.506049 py-allspice-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api_longtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-20 20:06:48.000000 py-allspice-2.2.0/tests/test_api_ratelimiting.py
```

### Comparing `py-allspice-2.1.0/LICENSE` & `py-allspice-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/PKG-INFO` & `py-allspice-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.1.0
+Version: 2.2.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/Langenfeld/py-gitea
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py-allspice-2.1.0/README.md` & `py-allspice-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/allspice/__init__.py` & `py-allspice-2.2.0/allspice/__init__.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/allspice/allspice.py` & `py-allspice-2.2.0/allspice/allspice.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,17 +127,31 @@
         page = 1
         combined_params = {}
         combined_params.update(params)
         aggregated_result = []
         while True:
             combined_params[page_key] = page
             result = self.requests_get(endpoint, combined_params, sudo)
+
             if not result:
                 return aggregated_result
-            aggregated_result.extend(result)
+
+            if isinstance(result, dict):
+                if "data" in result:
+                    data = result["data"]
+                    if len(data) == 0:
+                        return aggregated_result
+                    aggregated_result.extend(data)
+                else:
+                    raise NotImplementedError(
+                        "requests_get_paginated does not know how to handle responses of this type."
+                    )
+            else:
+                aggregated_result.extend(result)
+            
             page += 1
 
     def requests_put(self, endpoint: str, data: dict = None):
         if not data:
             data = {}
         request = self.requests.put(self.__get_url(endpoint), headers=self.headers, data=json.dumps(data))
         if request.status_code not in [200, 204]:
```

### Comparing `py-allspice-2.1.0/allspice/apiobject.py` & `py-allspice-2.2.0/allspice/apiobject.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,28 +354,30 @@
     def request(cls, allspice_client: 'AllSpice', owner: str, repo: str, branch: str):
         return cls._request(allspice_client, {"owner": owner, "repo": repo, "branch": branch})
 
 
 class Repository(ApiObject):
     API_OBJECT = """/repos/{owner}/{name}"""  # <owner>, <reponame>
     REPO_IS_COLLABORATOR = """/repos/%s/%s/collaborators/%s"""  # <owner>, <reponame>, <username>
-    REPO_SEARCH = """/repos/search/%s"""  # <reponame>
+    REPO_SEARCH = """/repos/search/"""
     REPO_BRANCHES = """/repos/%s/%s/branches"""  # <owner>, <reponame>
     REPO_BRANCH = """/repos/{owner}/{repo}/branches/{branch}"""
     REPO_ISSUES = """/repos/{owner}/{repo}/issues"""  # <owner, reponame>
     REPO_DESIGN_REVIEWS = """/repos/{owner}/{repo}/pulls"""
     REPO_DELETE = """/repos/%s/%s"""  # <owner>, <reponame>
     REPO_TIMES = """/repos/%s/%s/times"""  # <owner>, <reponame>
     REPO_USER_TIME = """/repos/%s/%s/times/%s"""  # <owner>, <reponame>, <username>
     REPO_COMMITS = "/repos/%s/%s/commits"  # <owner>, <reponame>
     REPO_TRANSFER = "/repos/{owner}/{repo}/transfer"
     REPO_MILESTONES = """/repos/{owner}/{repo}/milestones"""
     REPO_GET_ARCHIVE = "/repos/{owner}/{repo}/archive/{ref}.{format}"
     REPO_GET_ALLSPICE_JSON = "/repos/{owner}/{repo}/allspice_generated/json/{content}"
     REPO_GET_ALLSPICE_SVG = "/repos/{owner}/{repo}/allspice_generated/svg/{content}"
+    REPO_GET_TOPICS = "/repos/{owner}/{repo}/topics"
+    REPO_ADD_TOPIC = "/repos/{owner}/{repo}/topics/{topic}"
 
     class ArchiveFormat(Enum):
         """
         Archive formats for Repository.get_archive
         """
 
         TAR = "tar.gz"
@@ -395,17 +397,69 @@
         # dont know how to tell apart user and org as owner except form email being empty.
         "owner": lambda allspice_client, r: Organization.parse_response(allspice_client, r)
         if r["email"] == "" else User.parse_response(allspice_client, r),
         "updated_at": lambda allspice_client, t: Util.convert_time(t),
     }
 
     @classmethod
-    def request(cls, allspice_client: 'AllSpice', owner: str, name: str):
+    def request(
+            cls,
+            allspice_client: 'AllSpice',
+            owner: str,
+            name: str,
+    ) -> Repository:
         return cls._request(allspice_client, {"owner": owner, "name": name})
 
+    @classmethod
+    def search(
+        cls, 
+        allspice_client: 'AllSpice',
+        query: Optional[str] = None,
+        topic: bool = False,
+        include_description: bool = False,
+        user: Optional[User] = None,
+        owner_to_prioritize: Union[User, Organization, None] = None,
+    ) -> list[Repository]:
+        """
+        Search for repositories.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoSearch 
+
+        :param query: The query string to search for
+        :param topic: If true, the query string will only be matched against the 
+            repository's topic.
+        :param include_description: If true, the query string will be matched 
+            against the repository's description as well.
+        :param user: If specified, only repositories that this user owns or
+            contributes to will be searched.
+        :param owner_to_prioritize: If specified, repositories owned by the
+            given entity will be prioritized in the search.
+        :returns: All repositories matching the query. If there are many
+            repositories matching this query, this may take some time.
+        """
+
+        params = {}
+
+        if query is not None:
+            params["q"] = query
+        if topic:
+            params["topic"] = topic
+        if include_description:
+            params["include_description"] = include_description
+        if user is not None:
+            params["user"] = user.id
+        if owner_to_prioritize is not None:
+            params["owner_to_prioritize"] = owner_to_prioritize.id
+
+        responses = allspice_client.requests_get_paginated(cls.REPO_SEARCH, params=params)
+
+        return [Repository.parse_response(allspice_client, response) 
+                for response in responses]
+
+
     _patchable_fields = {
         "allow_manual_merge",
         "allow_merge_commits",
         "allow_rebase",
         "allow_rebase_explicit",
         "allow_rebase_update",
         "allow_squash_merge",
@@ -899,14 +953,48 @@
             owner=self.owner.username,
             repo=self.name,
             ref=ref_string,
             format=archive_format.value,
         )
         return self.allspice_client.requests_get_raw(url)
 
+    def get_topics(self) -> list[str]:
+        """
+        Gets the list of topics on this repository.
+
+        See http://localhost:3000/api/swagger#/repository/repoListTopics
+        """
+
+        url = self.REPO_GET_TOPICS.format(
+            owner=self.owner.username,
+            repo=self.name,
+        )
+        return self.allspice_client.requests_get(url)["topics"]
+
+
+    def add_topic(self, topic: str):
+        """
+        Adds a topic to the repository.
+
+        See https://hub.allspice.io/api/swagger#/repository/repoAddTopic 
+
+        :param topic: The topic to add. Topic names must consist only of
+            lowercase letters, numnbers and dashes (-), and cannot start with
+            dashes. Topic names also must be under 35 characters long.
+        """
+
+        url = self.REPO_ADD_TOPIC.format(
+            owner=self.owner.username, 
+            repo=self.name, 
+            topic=topic
+        )
+        self.allspice_client.requests_put(url)
+
+
+
     def delete(self):
         self.allspice_client.requests_delete(
             Repository.REPO_DELETE % (self.owner.username, self.name)
         )
         self.deleted = True
```

### Comparing `py-allspice-2.1.0/allspice/baseapiobject.py` & `py-allspice-2.2.0/allspice/baseapiobject.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/allspice/exceptions.py` & `py-allspice-2.2.0/allspice/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/allspice/ratelimiter.py` & `py-allspice-2.2.0/allspice/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/py_allspice.egg-info/PKG-INFO` & `py-allspice-2.2.0/py_allspice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-allspice
-Version: 2.1.0
+Version: 2.2.0
 Summary: A python wrapper for the AllSpice Hub API
 Home-page: https://github.com/Langenfeld/py-gitea
 Download-URL: https://github.com/AllSpiceIO/py-allspice
 Author: AllSpice, Inc.
 Author-email: maintainers@allspice.io
 License: MIT
 Keywords: AllSpice,AllSpice Hub,api,wrapper
```

### Comparing `py-allspice-2.1.0/setup.py` & `py-allspice-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='py-allspice',
-    version='2.1.0',
+    version='2.2.0',
     description='A python wrapper for the AllSpice Hub API',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='AllSpice, Inc.',
     author_email='maintainers@allspice.io',
```

### Comparing `py-allspice-2.1.0/tests/test_api.py` & `py-allspice-2.2.0/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import base64
 import datetime
+import time
 
 import pytest
 import uuid
 
 from allspice import AllSpice, User, Organization, Team, Repository, Issue, Milestone, \
     DesignReview, Branch, Comment
 from allspice import NotFoundException
 from allspice.apiobject import Util
+from allspice.exceptions import NotYetGeneratedException
 
 
 # put a ".token" file into your directory containg only the token for AllSpice Hub
 @pytest.fixture
 def instance(scope="module"):
     try:
         g = AllSpice("http://localhost:3000", open(".token", "r").read().strip(), ratelimiting=None)
@@ -27,14 +29,16 @@
                     ?"
 
 # make up some fresh names for the tests run
 test_org = "org_" + uuid.uuid4().hex[:8]
 test_user = "user_" + uuid.uuid4().hex[:8]
 test_team = "team_" + uuid.uuid4().hex[:8]  # team names seem to have a rather low max lenght
 test_repo = "repo_" + uuid.uuid4().hex[:8]
+# Topic names can't have underscores.
+test_topic = "topic-" + uuid.uuid4().hex[:8]
 
 
 def test_token_owner(instance):
     user = instance.get_user()
     assert user.username == "test", "Token user not 'tests'."
     assert user.is_admin, "Testuser is not Admin - Tests may fail"
 
@@ -133,19 +137,93 @@
 
 def test_get_repository(instance):
     repo = instance.get_repository(test_org, test_repo)
     assert repo is not None
     assert repo.name == test_repo
     assert repo.owner.username == test_org
 
+def test_add_content_to_repo(instance):
+    repo = Repository.request(instance, test_org, test_repo)
+    file_content = open("tests/data/test.pcbdoc", "rb").read()
+    file_content = base64.b64encode(file_content).decode("utf-8")
+    repo.create_file("test.pcbdoc", file_content)
+    assert len(repo.get_commits()) == 2
+    assert [content.name for content in repo.get_git_content()] == ["README.md", "test.pcbdoc"]
+
+
+def test_get_json_before_generated(instance):
+    repo = Repository.request(instance, test_org, test_repo)
+    with pytest.raises(NotYetGeneratedException) as e:
+        repo.get_generated_json("test.pcbdoc")
+
+
+def test_get_svg_before_generated(instance):
+    repo = Repository.request(instance, test_org, test_repo)
+    with pytest.raises(NotYetGeneratedException) as e:
+        repo.get_generated_svg("test.pcbdoc")
+
+
+def test_get_generated_json(instance):
+    repo = Repository.request(instance, test_org, test_repo)
+    branch = repo.get_branches()[0]
+    # This is scuffed but not much better we can do :(
+    while True:
+        try:
+            json = repo.get_generated_json("test.pcbdoc", branch)
+            break
+        except NotYetGeneratedException:
+            time.sleep(1)
+            pass
+    assert json is not None
+    assert json["type"] == "Pcb"
+
+
+def test_get_generated_svg(instance):
+    repo = Repository.request(instance, test_org, test_repo)
+    branch = repo.get_branches()[0]
+    while True:
+        try:
+            svg = repo.get_generated_svg("test.pcbdoc", branch)
+            break
+        except NotYetGeneratedException:
+            time.sleep(1)
+            pass
+    assert svg is not None
+    assert svg.startswith(b"<svg")
+
+
 def test_get_repository_non_existent(instance):
     with pytest.raises(NotFoundException) as e:
         instance.get_repository("doesnotexist", "doesnotexist")
 
 
+def test_repo_topics(instance):
+    # Since topics aren't part of the Repository object directly, we
+    # have to test both get and add at the same time.
+    repo = Repository.request(instance, test_org, test_repo)
+    topics = repo.get_topics()
+    assert len(topics) == 0
+
+    repo.add_topic(test_topic)
+    topics = repo.get_topics()
+    assert len(topics) == 1
+    assert topics[0] == test_topic
+
+
+def test_search_repos(instance):
+    repos = Repository.search(instance, test_repo)
+    # Two repos have been made with this name so far!
+    assert len(repos) == 2
+    assert repos[0].name == test_repo
+
+    repos = Repository.search(instance, test_topic, topic=True)
+    assert len(repos) == 1
+    assert repos[0].name == test_repo
+
+
 def test_patch_repo(instance):
     fields = {
         "allow_rebase": False,
         "description": "new description",
         "has_projects": True,
         "private": True,
     }
@@ -464,17 +542,17 @@
 
     assert review.state == DesignReview.OPEN
     assert review.title == "TestDesignReview"
     assert review.base == "master"
     assert review.head == "test_branch"
     assert review.body == "This is a test review"
     assert review.assignees[0].username == "test"
-    assert Util.format_time(Util.convert_time(review.due_date)) == Util.format_time(
-        due_date)
 
+    review_due_date = Util.convert_time(review.due_date)
+    assert review_due_date.date() == due_date.date()
 
 def test_get_design_reviews(instance):
     org = Organization.request(instance, test_org)
     repo = Repository.request(instance, org.username, test_repo)
     dr = repo.get_design_reviews()[0]
 
     assert dr.title == "TestDesignReview"
@@ -517,32 +595,37 @@
     comments = dr.get_comments()
     assert len(comments) > 0
     assert comments[0].body == "This is a test comment"
 
 
 def test_get_repo_archive(instance):
     # This requires a repo with actual files in it, so we use the test repo
-    repo = Repository.request(instance, "test", "test")
-    archive = repo.get_archive()
+    repo = Repository.request(instance, test_org, test_repo)
+    branch = repo.get_branches()[0]
+    archive = repo.get_archive(branch)
     assert archive is not None
 
 
+
+
 def test_team_get_org(instance):
     org = Organization.request(instance, test_org)
     user = instance.get_user_by_name(test_user)
     teams = user.get_teams()
     assert org.username == teams[0].organization.name
 
+
 def test_delete_repo_userowned(instance):
     user = User.request(instance, test_user)
     repo = Repository.request(instance, user.username, test_repo)
     repo.delete()
     with pytest.raises(NotFoundException) as e:
         Repository.request(instance, test_user, test_repo)
 
+
 def test_secundary_email(instance):
     SECONDARYMAIL = "secondarytest@test.org"  # set up with real email
     sec_user = instance.get_user_by_email(SECONDARYMAIL)
     assert SECONDARYMAIL in sec_user.emails
     assert sec_user.username == "test"
 
 
@@ -605,22 +688,7 @@
     user_name = test_user + "delte_test"
     email = user_name + "@example.org"
     user = instance.create_user(user_name, email, "abcdefg1.23AB", send_notify=False)
     assert user.username == user_name
     user.delete()
     with pytest.raises(NotFoundException) as e:
         User.request(instance, user_name)
-
-def test_get_generated_json(instance):
-    # Note: this expects the test repo to have a file called test.pcbdoc,
-    # which will have json and svg generated from it.
-    repo = instance.get_repository("test", "test")
-    json = repo.get_generated_json("test.pcbdoc")
-    assert json is not None
-    assert json["type"] == "Pcb"
-
-
-def test_get_generated_svg(instance):
-    repo = instance.get_repository("test", "test")
-    svg = repo.get_generated_svg("test.pcbdoc")
-    assert svg is not None
-    assert svg.startswith(b"<svg")
```

### Comparing `py-allspice-2.1.0/tests/test_api_longtests.py` & `py-allspice-2.2.0/tests/test_api_longtests.py`

 * *Files identical despite different names*

### Comparing `py-allspice-2.1.0/tests/test_api_ratelimiting.py` & `py-allspice-2.2.0/tests/test_api_ratelimiting.py`

 * *Files identical despite different names*

