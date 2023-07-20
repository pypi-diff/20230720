# Comparing `tmp/kathara-3.6.2.tar.gz` & `tmp/kathara-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kathara-3.6.2.tar", last modified: Wed Jun 21 14:21:36 2023, max compression
+gzip compressed data, was "kathara-3.6.3.tar", last modified: Thu Jul 20 15:53:28 2023, max compression
```

## Comparing `kathara-3.6.2.tar` & `kathara-3.6.3.tar`

### file list

```diff
@@ -1,413 +1,413 @@
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/.github/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      527 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      560 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      510 2022-07-26 14:39:39.000000 kathara-3.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1435 2023-05-19 15:22:33.000000 kathara-3.6.2/.gitignore
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3351 2022-07-26 14:39:39.000000 kathara-3.6.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1514 2022-07-26 14:39:39.000000 kathara-3.6.2/CONTRIBUTING.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35141 2022-07-26 14:39:39.000000 kathara-3.6.2/LICENSE
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-06-21 14:21:36.783736 kathara-3.6.2/PKG-INFO
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8365 2023-01-17 11:29:05.000000 kathara-3.6.2/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/docs/
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1413 2022-07-26 14:39:39.000000 kathara-3.6.2/docs/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1161 2022-09-09 09:29:44.000000 kathara-3.6.2/docs/footer.txt
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1307 2022-07-26 14:39:39.000000 kathara-3.6.2/docs/index.txt
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      985 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-check.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-connect.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1622 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-exec.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3267 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab-dirs.7.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4449 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.conf.5.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      658 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.dep.5.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1820 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-lab.ext.5.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1108 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lclean.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2214 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lconfig.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1985 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-linfo.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1417 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-list.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4210 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lrestart.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5303 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-lstart.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5417 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-ltest.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      524 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-settings.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      567 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-vclean.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara-vconfig.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7226 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-vstart.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1163 2023-05-24 09:06:02.000000 kathara-3.6.2/docs/kathara-wipe.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3313 2022-09-09 09:29:44.000000 kathara-3.6.2/docs/kathara.1.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6196 2022-09-02 15:11:08.000000 kathara-3.6.2/docs/kathara.conf.5.ronn
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1986 2023-06-18 15:50:16.000000 kathara-3.6.2/pyproject.toml
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.747736 kathara-3.6.2/scripts/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      841 2023-05-17 13:20:12.000000 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/Dockerfile_template
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      168 2023-05-18 10:29:39.000000 kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/dput.cf
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)     6087 2023-06-21 13:32:12.000000 kathara-3.6.2/scripts/Linux-Deb/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1340 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/debian/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      354 2023-06-21 13:41:59.000000 kathara-3.6.2/scripts/Linux-Deb/debian/changelog
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        3 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/compat
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      871 2023-04-27 14:28:28.000000 kathara-3.6.2/scripts/Linux-Deb/debian/control
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1042 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/copyright
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.dirs
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       40 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.links
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      344 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.lintian-overrides
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      157 2023-05-18 09:09:00.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.postinst
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       88 2023-05-18 09:08:56.000000 kathara-3.6.2/scripts/Linux-Deb/debian/kathara.prerm
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1379 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Linux-Deb/debian/rules
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Deb/debian/source/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       12 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/source/format
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       33 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Deb/debian/source/lintian-overrides
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/Docker-Linux-Build/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      691 2023-05-24 09:06:38.000000 kathara-3.6.2/scripts/Linux-Pkg/Docker-Linux-Build/Dockerfile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2694 2023-06-18 17:19:35.000000 kathara-3.6.2/scripts/Linux-Pkg/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1283 2023-06-18 17:20:44.000000 kathara-3.6.2/scripts/Linux-Pkg/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3067 2023-06-18 17:18:39.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/PKGBUILD
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      262 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/kathara.changelog
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      235 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Linux-Pkg/pkginfo/kathara.install
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/Docker-Linux-Build/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      383 2023-01-04 12:29:14.000000 kathara-3.6.2/scripts/Linux-Rpm/Docker-Linux-Build/Dockerfile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2008 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Rpm/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      538 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Linux-Rpm/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/Linux-Rpm/rpm/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3041 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Linux-Rpm/rpm/kathara.spec
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.755736 kathara-3.6.2/scripts/OSX/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4476 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/OSX/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2429 2022-09-09 09:29:44.000000 kathara-3.6.2/scripts/OSX/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1501 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Distribution
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/Resources/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    59811 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/banner.png
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1926 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/conclusion.html
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1240 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/Resources/welcome.html
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/OSX/darwin/scripts/
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)      393 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/scripts/postinstall
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1527 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/darwin/uninstall.sh
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2836 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/OSX/kathara.spec
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/Windows/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/Windows/Assets/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32988 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/app_icon.ico
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1580 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/environment.iss
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2844 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/Windows/Assets/kathara.spec
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      707 2022-09-09 09:29:44.000000 kathara-3.6.2/scripts/Windows/README.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      761 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/Windows/WindowsBuild.bat
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2288 2023-06-18 15:50:16.000000 kathara-3.6.2/scripts/Windows/installer.iss
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/autocompletion/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3034 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/autocompletion/generate_autocompletion.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      120 2023-05-24 09:06:02.000000 kathara-3.6.2/scripts/autocompletion/requirements.txt
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/pip-package/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      291 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pip-package/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      387 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pip-package/README.md
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/scripts/pydoc/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1142 2022-12-28 11:38:10.000000 kathara-3.6.2/scripts/pydoc/Makefile
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      194 2022-09-26 11:15:29.000000 kathara-3.6.2/scripts/pydoc/README.md
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      706 2022-07-26 14:39:39.000000 kathara-3.6.2/scripts/pydoc/generate_doc.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      723 2023-06-21 14:21:36.783736 kathara-3.6.2/setup.cfg
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1679 2023-06-18 15:50:16.000000 kathara-3.6.2/setup.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/auth/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1650 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/auth/PrivilegeHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/auth/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.759736 kathara-3.6.2/src/Kathara/cli/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/command/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2240 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/CheckCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2521 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ConnectCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3068 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ExecCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1972 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LcleanCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3010 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LconfigCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4632 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LinfoCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2575 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/ListCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4324 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LrestartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8237 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LstartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4512 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/LtestCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      350 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/command/SettingsCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1253 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VcleanCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2698 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VconfigCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6964 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/VstartCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2217 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/command/WipeCommand.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/command/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/event/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1313 2022-11-02 11:57:09.000000 kathara-3.6.2/src/Kathara/cli/ui/event/HandleProgressBar.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      694 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/OpenMachineTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1058 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/UpdateDockerImage.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2402 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/event/register.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/cli/ui/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    21159 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13071 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8908 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1483 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3828 2022-08-26 10:08:06.000000 kathara-3.6.2/src/Kathara/cli/ui/setting/utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5981 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/cli/ui/utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      623 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/decorators.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/event/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2832 2022-09-02 16:43:02.000000 kathara-3.6.2/src/Kathara/event/EventDispatcher.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/event/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3718 2023-05-16 16:24:29.000000 kathara-3.6.2/src/Kathara/exceptions.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      741 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/foundation/cli/CliArgs.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/command/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/Command.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      205 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/CommandFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/command/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/ui/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1023 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      233 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/factory/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1010 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/factory/Factory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/factory/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    17939 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/foundation/manager/IManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      213 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/ManagerFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/ILinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      674 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/IMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.763736 kathara-3.6.2/src/Kathara/foundation/manager/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2095 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/Terminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1178 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/manager/terminal/terminal_utils.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/model/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11374 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/foundation/model/FilesystemMixin.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/foundation/model/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      749 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      228 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddonFactory.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/foundation/test/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1662 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/foundation/test/Test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/foundation/test/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    18970 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/manager/Kathara.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7128 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerImage.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13831 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    36272 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerMachine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    31189 2023-05-09 13:30:55.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3606 2022-09-02 16:24:37.000000 kathara-3.6.2/src/Kathara/manager/docker/DockerPlugin.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3383 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/DockerLinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5220 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/DockerMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/docker/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2205 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1157 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/docker/terminal/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1924 2022-09-02 17:03:11.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfig.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14270 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    34969 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesMachine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    30101 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesManager.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4366 2022-12-22 14:55:44.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesNamespace.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2144 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3444 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/stats/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2418 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/model/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1975 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/model/ExternalLink.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14058 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/model/Lab.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1252 2022-08-26 10:08:06.000000 kathara-3.6.2/src/Kathara/model/Link.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    25351 2023-06-16 09:17:57.000000 kathara-3.6.2/src/Kathara/model/Machine.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-29 14:35:19.000000 kathara-3.6.2/src/Kathara/model/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/os/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5402 2022-09-02 17:03:11.000000 kathara-3.6.2/src/Kathara/os/Networking.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/os/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.767736 kathara-3.6.2/src/Kathara/parser/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/parser/netkit/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2657 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/parser/netkit/DepParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2665 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/parser/netkit/ExtParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1146 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/FolderParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3436 2023-06-16 09:17:54.000000 kathara-3.6.2/src/Kathara/parser/netkit/LabParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      903 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/OptionParser.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/parser/netkit/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/setting/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11573 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/setting/Setting.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/setting/addon/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1116 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/DockerSettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      906 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/KubernetesSettingsAddon.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/setting/addon/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1404 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/strings.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/test/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5449 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/test/BuiltinTest.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4534 2022-09-09 09:29:44.000000 kathara-3.6.2/src/Kathara/test/UserTest.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/test/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      519 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15168 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/console_menu.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      850 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14430 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_borders.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1502 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_margins.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_padding.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3760 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_style.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      385 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1335 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/command_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      803 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/external_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1353 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/function_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/selection_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1596 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/submenu_item.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13445 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_component.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11425 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_formatter.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3281 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/multiselect_menu.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12321 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/prompt_utils.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1805 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/screen.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2772 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/selection_menu.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.771736 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      765 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/base.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1009 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/regex.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      558 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/url.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       22 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/consolemenu/version.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/curses/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/curses/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1352 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/curses/curses.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/depgen/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/depgen/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2992 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/depgen/depgen.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/libtmux/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/trdparty/libtmux/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2738 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/libtmux/tmux.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/trdparty/strtobool/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/strtobool/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      692 2023-05-24 09:06:02.000000 kathara-3.6.2/src/Kathara/trdparty/strtobool/strtobool.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     9659 2023-05-29 14:28:12.000000 kathara-3.6.2/src/Kathara/utils.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/validator/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      599 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/validator/ImageValidator.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      457 2022-09-02 15:11:08.000000 kathara-3.6.2/src/Kathara/validator/TerminalValidator.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/validator/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      308 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/version.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/Kathara/webhooks/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3461 2023-06-18 15:50:16.000000 kathara-3.6.2/src/Kathara/webhooks/DockerHubApi.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      795 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/webhooks/GitHubApi.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/src/Kathara/webhooks/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/src/kathara.egg-info/
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/PKG-INFO
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    11859 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/SOURCES.txt
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)        1 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/dependency_links.txt
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)      463 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/requires.txt
--rw-rw-r--   0 tommaso   (1000) tommaso   (1000)       16 2023-06-21 14:21:36.000000 kathara-3.6.2/src/kathara.egg-info/top_level.txt
--rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     4027 2022-09-09 09:29:44.000000 kathara-3.6.2/src/kathara.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      444 2023-05-24 09:06:02.000000 kathara-3.6.2/src/requirements.txt
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.747736 kathara-3.6.2/tests/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/cli/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4997 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/connect_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7588 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/exec_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3025 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lclean_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7356 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lconfig_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7011 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/linfo_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8275 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/list_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1855 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lrestart_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27515 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/lstart_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      632 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vclean_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1285 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vconfig_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32948 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/vstart_command_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4157 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/cli/wipe_command_test.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/manager/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/__init__.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.775736 kathara-3.6.2/tests/manager/docker/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/docker/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11289 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_image_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13862 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_link_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    36139 2022-12-22 14:55:44.000000 kathara-3.6.2/tests/manager/docker/docker_machine_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    46614 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/manager/docker/docker_manager_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6072 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/docker/docker_plugin_test.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/manager/kubernetes/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/manager/kubernetes/__init__.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    19509 2022-12-22 14:55:44.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_link_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    30115 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_machine_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35405 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/manager/kubernetes/kubernetes_manager_test.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/model/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1422 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/model/external_link_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16555 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/filesystem_mixin_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12130 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/lab_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)    10461 2023-06-16 09:17:54.000000 kathara-3.6.2/tests/model/machine_test.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      779 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/dep_parser_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      881 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/ext_parser_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      669 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/folder_parser_test.py
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2987 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/lab_parser_test.py
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labconf/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/inline_comment/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       43 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/inline_comment/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/inline_comment_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       42 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/inline_comment_error/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      177 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_interface_name_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       76 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_interface_name_error/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_lab_description/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      303 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_lab_description/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_same_collision_domain_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_same_collision_domain_error/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/one_device_shared_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       14 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/one_device_shared_error/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/two_devices_one_cd/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      131 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labconf/two_devices_one_cd/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/unclosed_quotes/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        9 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/unclosed_quotes/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labconf/unmatched_quotes/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       10 2023-05-24 09:06:02.000000 kathara-3.6.2/tests/parser/labconf/unmatched_quotes/lab.conf
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labdep/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/comments_empty_lines/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       66 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/comments_empty_lines/lab.dep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/devices_loop/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       26 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/devices_loop/lab.dep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/syntax_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/syntax_error/lab.dep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labdep/three_devices_dependencies/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labdep/three_devices_dependencies/lab.dep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labext/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/syntax_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/syntax_error/lab.conf
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       23 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/syntax_error/lab.ext
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/two_devices/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labext/two_devices/lab.conf
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       36 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labext/two_devices/lab.ext
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labext/value_error/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/value_error/lab.conf
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)       17 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/labext/value_error/lab.ext
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc1/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc1/.gitkeep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc2/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/pc2/.gitkeep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/shared/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/ignore_shared_folder/shared/.gitkeep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/one_device/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/one_device/pc1/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/one_device/pc1/.gitkeep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.751736 kathara-3.6.2/tests/parser/labfolder/two_devices/
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/two_devices/pc1/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/two_devices/pc1/.gitkeep
-drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-06-21 14:21:36.779736 kathara-3.6.2/tests/parser/labfolder/two_devices/pc2/
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.2/tests/parser/labfolder/two_devices/pc2/.gitkeep
--rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-09-09 09:29:44.000000 kathara-3.6.2/tests/parser/option_parser_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.338121 kathara-3.6.3/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.254120 kathara-3.6.3/.github/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.254120 kathara-3.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      527 2022-07-26 14:39:39.000000 kathara-3.6.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      560 2022-07-26 14:39:39.000000 kathara-3.6.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      510 2022-07-26 14:39:39.000000 kathara-3.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1435 2023-05-19 15:22:33.000000 kathara-3.6.3/.gitignore
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3351 2022-07-26 14:39:39.000000 kathara-3.6.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1514 2022-07-26 14:39:39.000000 kathara-3.6.3/CONTRIBUTING.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35141 2022-07-26 14:39:39.000000 kathara-3.6.3/LICENSE
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-07-20 15:53:28.338121 kathara-3.6.3/PKG-INFO
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8365 2023-07-18 10:03:12.000000 kathara-3.6.3/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.262120 kathara-3.6.3/docs/
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1413 2022-07-26 14:39:39.000000 kathara-3.6.3/docs/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1161 2022-09-09 09:29:44.000000 kathara-3.6.3/docs/footer.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1307 2022-07-26 14:39:39.000000 kathara-3.6.3/docs/index.txt
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      985 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-check.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-connect.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1752 2023-07-20 13:39:26.000000 kathara-3.6.3/docs/kathara-exec.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3267 2022-09-02 15:11:08.000000 kathara-3.6.3/docs/kathara-lab-dirs.7.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4619 2023-07-18 10:05:02.000000 kathara-3.6.3/docs/kathara-lab.conf.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      658 2022-09-02 15:11:08.000000 kathara-3.6.3/docs/kathara-lab.dep.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1820 2022-09-02 15:11:08.000000 kathara-3.6.3/docs/kathara-lab.ext.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1108 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-lclean.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2214 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-lconfig.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1985 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-linfo.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1417 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-list.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4210 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-lrestart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5303 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-lstart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5417 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-ltest.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      524 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-settings.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      567 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-vclean.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1638 2022-09-02 15:11:08.000000 kathara-3.6.3/docs/kathara-vconfig.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7226 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-vstart.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1163 2023-05-24 09:06:02.000000 kathara-3.6.3/docs/kathara-wipe.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3313 2022-09-09 09:29:44.000000 kathara-3.6.3/docs/kathara.1.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6196 2022-09-02 15:11:08.000000 kathara-3.6.3/docs/kathara.conf.5.ronn
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2001 2023-07-20 13:39:26.000000 kathara-3.6.3/pyproject.toml
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.246120 kathara-3.6.3/scripts/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.262120 kathara-3.6.3/scripts/Linux-Deb/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.262120 kathara-3.6.3/scripts/Linux-Deb/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      841 2023-06-24 13:20:35.000000 kathara-3.6.3/scripts/Linux-Deb/Docker-Linux-Build/Dockerfile_template
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      168 2023-05-18 10:29:39.000000 kathara-3.6.3/scripts/Linux-Deb/Docker-Linux-Build/dput.cf
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)     6065 2023-07-20 15:53:11.000000 kathara-3.6.3/scripts/Linux-Deb/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1340 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.266120 kathara-3.6.3/scripts/Linux-Deb/debian/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      770 2023-07-20 14:05:52.000000 kathara-3.6.3/scripts/Linux-Deb/debian/changelog
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        3 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/compat
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      871 2023-06-24 13:20:27.000000 kathara-3.6.3/scripts/Linux-Deb/debian/control
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1042 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/copyright
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/kathara.dirs
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       40 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/kathara.links
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      344 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/kathara.lintian-overrides
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      157 2023-05-18 09:09:00.000000 kathara-3.6.3/scripts/Linux-Deb/debian/kathara.postinst
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       88 2023-05-18 09:08:56.000000 kathara-3.6.3/scripts/Linux-Deb/debian/kathara.prerm
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1379 2023-06-24 13:20:30.000000 kathara-3.6.3/scripts/Linux-Deb/debian/rules
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.266120 kathara-3.6.3/scripts/Linux-Deb/debian/source/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       12 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/source/format
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       33 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Deb/debian/source/lintian-overrides
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.266120 kathara-3.6.3/scripts/Linux-Pkg/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.266120 kathara-3.6.3/scripts/Linux-Pkg/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      691 2023-06-24 13:20:55.000000 kathara-3.6.3/scripts/Linux-Pkg/Docker-Linux-Build/Dockerfile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2743 2023-07-20 14:06:43.000000 kathara-3.6.3/scripts/Linux-Pkg/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1278 2023-06-21 14:47:45.000000 kathara-3.6.3/scripts/Linux-Pkg/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/Linux-Pkg/pkginfo/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3067 2023-06-18 17:18:39.000000 kathara-3.6.3/scripts/Linux-Pkg/pkginfo/PKGBUILD
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      678 2023-07-20 13:39:26.000000 kathara-3.6.3/scripts/Linux-Pkg/pkginfo/kathara.changelog
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      235 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Linux-Pkg/pkginfo/kathara.install
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/Linux-Rpm/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/Linux-Rpm/Docker-Linux-Build/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      383 2023-01-04 12:29:14.000000 kathara-3.6.3/scripts/Linux-Rpm/Docker-Linux-Build/Dockerfile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2008 2023-07-20 13:39:26.000000 kathara-3.6.3/scripts/Linux-Rpm/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      538 2023-05-24 09:06:02.000000 kathara-3.6.3/scripts/Linux-Rpm/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/Linux-Rpm/rpm/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3441 2023-07-20 13:39:26.000000 kathara-3.6.3/scripts/Linux-Rpm/rpm/kathara.spec
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/OSX/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4476 2023-07-20 13:39:26.000000 kathara-3.6.3/scripts/OSX/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2429 2023-06-24 13:21:58.000000 kathara-3.6.3/scripts/OSX/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.270120 kathara-3.6.3/scripts/OSX/darwin/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1501 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/Distribution
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.274120 kathara-3.6.3/scripts/OSX/darwin/Resources/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    59811 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/Resources/banner.png
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1926 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/Resources/conclusion.html
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1240 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/Resources/welcome.html
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.274120 kathara-3.6.3/scripts/OSX/darwin/scripts/
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)      393 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/scripts/postinstall
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     1527 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/darwin/uninstall.sh
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2836 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/OSX/kathara.spec
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.274120 kathara-3.6.3/scripts/Windows/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.278120 kathara-3.6.3/scripts/Windows/Assets/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32988 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Windows/Assets/app_icon.ico
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1580 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Windows/Assets/environment.iss
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2844 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/Windows/Assets/kathara.spec
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      707 2023-06-24 13:22:04.000000 kathara-3.6.3/scripts/Windows/README.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      871 2023-07-18 10:05:02.000000 kathara-3.6.3/scripts/Windows/WindowsBuild.bat
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2288 2023-07-20 13:39:26.000000 kathara-3.6.3/scripts/Windows/installer.iss
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.278120 kathara-3.6.3/scripts/autocompletion/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3034 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/autocompletion/generate_autocompletion.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      120 2023-05-24 09:06:02.000000 kathara-3.6.3/scripts/autocompletion/requirements.txt
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.278120 kathara-3.6.3/scripts/pip-package/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      291 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/pip-package/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      387 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/pip-package/README.md
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.278120 kathara-3.6.3/scripts/pydoc/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1142 2022-12-28 11:38:10.000000 kathara-3.6.3/scripts/pydoc/Makefile
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      194 2022-09-26 11:15:29.000000 kathara-3.6.3/scripts/pydoc/README.md
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      706 2022-07-26 14:39:39.000000 kathara-3.6.3/scripts/pydoc/generate_doc.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      723 2023-07-20 15:53:28.338121 kathara-3.6.3/setup.cfg
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1698 2023-07-20 13:39:26.000000 kathara-3.6.3/setup.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.278120 kathara-3.6.3/src/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.282120 kathara-3.6.3/src/Kathara/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.282120 kathara-3.6.3/src/Kathara/auth/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1650 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/auth/PrivilegeHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/auth/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.282120 kathara-3.6.3/src/Kathara/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.286120 kathara-3.6.3/src/Kathara/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2240 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/CheckCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2521 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/ConnectCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3665 2023-07-18 10:05:12.000000 kathara-3.6.3/src/Kathara/cli/command/ExecCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1972 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3010 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4632 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LinfoCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2575 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/ListCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4324 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LrestartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8237 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4512 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/LtestCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      350 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/command/SettingsCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1253 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/VcleanCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2698 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/VconfigCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6964 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/command/VstartCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2076 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/cli/command/WipeCommand.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.286120 kathara-3.6.3/src/Kathara/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.286120 kathara-3.6.3/src/Kathara/cli/ui/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1204 2023-07-18 10:05:12.000000 kathara-3.6.3/src/Kathara/cli/ui/event/HandleMachineTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1313 2022-11-02 11:57:09.000000 kathara-3.6.3/src/Kathara/cli/ui/event/HandleProgressBar.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1058 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/event/UpdateDockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2703 2023-07-18 10:05:12.000000 kathara-3.6.3/src/Kathara/cli/ui/event/register.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    21159 2023-06-16 09:17:57.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/CommonOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13071 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/DockerOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8908 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1483 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/SettingsMenuFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3828 2022-08-26 10:08:06.000000 kathara-3.6.3/src/Kathara/cli/ui/setting/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5981 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/cli/ui/utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      623 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/decorators.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/event/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2832 2022-09-02 16:43:02.000000 kathara-3.6.3/src/Kathara/event/EventDispatcher.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/event/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3718 2023-05-16 16:24:29.000000 kathara-3.6.3/src/Kathara/exceptions.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/foundation/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/foundation/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      741 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/foundation/cli/CliArgs.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/foundation/cli/command/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/command/Command.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      205 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/command/CommandFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/command/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/foundation/cli/ui/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/ui/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.290120 kathara-3.6.3/src/Kathara/foundation/cli/ui/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1023 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      233 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/ui/setting/OptionsHandlerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/cli/ui/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/factory/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1010 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/factory/Factory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/factory/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    19095 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/foundation/manager/IManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      213 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/ManagerFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/manager/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/stats/ILinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      674 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/stats/IMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/manager/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2095 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/terminal/Terminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/terminal/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1178 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/manager/terminal/terminal_utils.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11374 2023-06-16 09:17:54.000000 kathara-3.6.3/src/Kathara/foundation/model/FilesystemMixin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/foundation/model/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      749 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/setting/SettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      228 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/setting/SettingsAddonFactory.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/foundation/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1929 2023-07-18 10:05:12.000000 kathara-3.6.3/src/Kathara/foundation/test/Test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/foundation/test/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.294120 kathara-3.6.3/src/Kathara/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    20143 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/manager/Kathara.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.298120 kathara-3.6.3/src/Kathara/manager/docker/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7128 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/manager/docker/DockerImage.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13831 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/manager/docker/DockerLink.py
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    42011 2023-07-20 15:45:44.000000 kathara-3.6.3/src/Kathara/manager/docker/DockerMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32472 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/manager/docker/DockerManager.py
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)     3606 2023-07-20 13:39:23.000000 kathara-3.6.3/src/Kathara/manager/docker/DockerPlugin.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.298120 kathara-3.6.3/src/Kathara/manager/docker/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3383 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/stats/DockerLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5220 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/stats/DockerMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.298120 kathara-3.6.3/src/Kathara/manager/docker/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2205 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1157 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/docker/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1924 2022-09-02 17:03:11.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesConfig.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4252 2022-09-09 09:29:44.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesConfigMap.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14270 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    35196 2023-07-18 11:41:30.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesMachine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    31463 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesManager.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4366 2022-12-22 14:55:44.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesNamespace.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/manager/kubernetes/stats/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2144 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3444 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/stats/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/manager/kubernetes/terminal/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2418 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/manager/kubernetes/terminal/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1975 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/model/ExternalLink.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16855 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/model/Lab.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1252 2022-08-26 10:08:06.000000 kathara-3.6.3/src/Kathara/model/Link.py
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    25887 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/model/Machine.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-29 14:35:19.000000 kathara-3.6.3/src/Kathara/model/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/os/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5402 2022-09-02 17:03:11.000000 kathara-3.6.3/src/Kathara/os/Networking.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/os/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.302121 kathara-3.6.3/src/Kathara/parser/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/parser/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.306120 kathara-3.6.3/src/Kathara/parser/netkit/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2657 2022-09-09 09:29:44.000000 kathara-3.6.3/src/Kathara/parser/netkit/DepParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2665 2022-09-09 09:29:44.000000 kathara-3.6.3/src/Kathara/parser/netkit/ExtParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1146 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/parser/netkit/FolderParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3436 2023-06-16 09:17:54.000000 kathara-3.6.3/src/Kathara/parser/netkit/LabParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      903 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/parser/netkit/OptionParser.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/parser/netkit/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.306120 kathara-3.6.3/src/Kathara/setting/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11573 2023-06-18 15:50:16.000000 kathara-3.6.3/src/Kathara/setting/Setting.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/setting/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.306120 kathara-3.6.3/src/Kathara/setting/addon/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1116 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/setting/addon/DockerSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      906 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/setting/addon/KubernetesSettingsAddon.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/setting/addon/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1404 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/strings.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.306120 kathara-3.6.3/src/Kathara/test/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     5449 2022-09-09 09:29:44.000000 kathara-3.6.3/src/Kathara/test/BuiltinTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4534 2022-09-09 09:29:44.000000 kathara-3.6.3/src/Kathara/test/UserTest.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/test/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.306120 kathara-3.6.3/src/Kathara/trdparty/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.310121 kathara-3.6.3/src/Kathara/trdparty/consolemenu/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      519 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15168 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/console_menu.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.310121 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      850 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    14430 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_borders.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1502 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_margins.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1445 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_padding.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3760 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_style.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.310121 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      385 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1335 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/command_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      803 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/external_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1353 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/function_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      595 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/selection_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1596 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/submenu_item.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13445 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/menu_component.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11425 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/menu_formatter.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3281 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/multiselect_menu.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    12321 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/prompt_utils.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1805 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/screen.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2772 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/selection_menu.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.310121 kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      765 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/base.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1009 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/regex.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      558 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/url.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       22 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/consolemenu/version.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/trdparty/curses/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/curses/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1352 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/curses/curses.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/trdparty/depgen/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/depgen/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2992 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/depgen/depgen.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/trdparty/libtmux/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/trdparty/libtmux/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2738 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/trdparty/libtmux/tmux.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/trdparty/strtobool/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/trdparty/strtobool/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      692 2023-05-24 09:06:02.000000 kathara-3.6.3/src/Kathara/trdparty/strtobool/strtobool.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     9322 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/utils.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/validator/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      599 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/validator/ImageValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      457 2022-09-02 15:11:08.000000 kathara-3.6.3/src/Kathara/validator/TerminalValidator.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/validator/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      308 2023-07-20 13:39:26.000000 kathara-3.6.3/src/Kathara/version.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.314121 kathara-3.6.3/src/Kathara/webhooks/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3461 2023-06-18 15:50:16.000000 kathara-3.6.3/src/Kathara/webhooks/DockerHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      795 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/webhooks/GitHubApi.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/src/Kathara/webhooks/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.318121 kathara-3.6.3/src/kathara.egg-info/
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    50225 2023-07-20 15:53:28.000000 kathara-3.6.3/src/kathara.egg-info/PKG-INFO
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    11861 2023-07-20 15:53:28.000000 kathara-3.6.3/src/kathara.egg-info/SOURCES.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)        1 2023-07-20 15:53:28.000000 kathara-3.6.3/src/kathara.egg-info/dependency_links.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)      471 2023-07-20 15:53:28.000000 kathara-3.6.3/src/kathara.egg-info/requires.txt
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)       16 2023-07-20 15:53:28.000000 kathara-3.6.3/src/kathara.egg-info/top_level.txt
+-rwxr-xr-x   0 tommaso   (1000) tommaso   (1000)     4027 2022-09-09 09:29:44.000000 kathara-3.6.3/src/kathara.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      453 2023-07-18 10:05:12.000000 kathara-3.6.3/src/requirements.txt
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.318121 kathara-3.6.3/tests/cli/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     4997 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/connect_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7658 2023-07-18 10:05:12.000000 kathara-3.6.3/tests/cli/exec_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     3025 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/lclean_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7356 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/lconfig_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     7011 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/linfo_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     8275 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/list_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1855 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/lrestart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    27515 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/lstart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      632 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/vclean_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1285 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/vconfig_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    32948 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/cli/vstart_command_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2857 2023-07-20 13:39:26.000000 kathara-3.6.3/tests/cli/wipe_command_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.318121 kathara-3.6.3/tests/manager/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/manager/__init__.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.322121 kathara-3.6.3/tests/manager/docker/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/manager/docker/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    11289 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/manager/docker/docker_image_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    13862 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/manager/docker/docker_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    36730 2023-07-18 10:05:12.000000 kathara-3.6.3/tests/manager/docker/docker_machine_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    55212 2023-07-20 13:39:26.000000 kathara-3.6.3/tests/manager/docker/docker_manager_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     6072 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/manager/docker/docker_plugin_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.322121 kathara-3.6.3/tests/manager/kubernetes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/manager/kubernetes/__init__.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    19509 2022-12-22 14:55:44.000000 kathara-3.6.3/tests/manager/kubernetes/kubernetes_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    30223 2023-07-18 10:05:12.000000 kathara-3.6.3/tests/manager/kubernetes/kubernetes_machine_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    39918 2023-07-18 10:05:12.000000 kathara-3.6.3/tests/manager/kubernetes/kubernetes_manager_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/model/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     1422 2023-07-20 13:39:26.000000 kathara-3.6.3/tests/model/external_link_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    16555 2023-06-16 09:17:54.000000 kathara-3.6.3/tests/model/filesystem_mixin_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)    15807 2023-07-20 13:39:26.000000 kathara-3.6.3/tests/model/lab_test.py
+-rw-rw-r--   0 tommaso   (1000) tommaso   (1000)    12319 2023-07-20 13:39:26.000000 kathara-3.6.3/tests/model/machine_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      779 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/dep_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      881 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/ext_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      669 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/folder_parser_test.py
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)     2987 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/parser/lab_parser_test.py
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labconf/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/inline_comment/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       43 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/parser/labconf/inline_comment/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/inline_comment_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       42 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/parser/labconf/inline_comment_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/one_device/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      177 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/one_device/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/one_device_interface_name_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       76 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/one_device_interface_name_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/one_device_lab_description/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      303 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/one_device_lab_description/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.326121 kathara-3.6.3/tests/parser/labconf/one_device_same_collision_domain_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/one_device_same_collision_domain_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labconf/one_device_shared_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       14 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/one_device_shared_error/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labconf/two_devices_one_cd/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      131 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labconf/two_devices_one_cd/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labconf/unclosed_quotes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        9 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/parser/labconf/unclosed_quotes/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labconf/unmatched_quotes/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       10 2023-05-24 09:06:02.000000 kathara-3.6.3/tests/parser/labconf/unmatched_quotes/lab.conf
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labdep/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labdep/comments_empty_lines/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       66 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labdep/comments_empty_lines/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labdep/devices_loop/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       26 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labdep/devices_loop/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labdep/syntax_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       24 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labdep/syntax_error/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.330121 kathara-3.6.3/tests/parser/labdep/three_devices_dependencies/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       21 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labdep/three_devices_dependencies/lab.dep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labext/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.334121 kathara-3.6.3/tests/parser/labext/syntax_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/labext/syntax_error/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       23 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/labext/syntax_error/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.334121 kathara-3.6.3/tests/parser/labext/two_devices/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labext/two_devices/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       36 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labext/two_devices/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.334121 kathara-3.6.3/tests/parser/labext/value_error/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       65 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/labext/value_error/lab.conf
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)       17 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/labext/value_error/lab.ext
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labfolder/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.334121 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.334121 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/pc2/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/pc2/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.338121 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/shared/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/ignore_shared_folder/shared/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.250120 kathara-3.6.3/tests/parser/labfolder/one_device/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.338121 kathara-3.6.3/tests/parser/labfolder/one_device/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/one_device/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.254120 kathara-3.6.3/tests/parser/labfolder/two_devices/
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.338121 kathara-3.6.3/tests/parser/labfolder/two_devices/pc1/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/two_devices/pc1/.gitkeep
+drwxrwxr-x   0 tommaso   (1000) tommaso   (1000)        0 2023-07-20 15:53:28.338121 kathara-3.6.3/tests/parser/labfolder/two_devices/pc2/
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)        0 2022-07-26 14:39:39.000000 kathara-3.6.3/tests/parser/labfolder/two_devices/pc2/.gitkeep
+-rw-r--r--   0 tommaso   (1000) tommaso   (1000)      681 2022-09-09 09:29:44.000000 kathara-3.6.3/tests/parser/option_parser_test.py
```

### Comparing `kathara-3.6.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kathara-3.6.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/.github/ISSUE_TEMPLATE/feature_request.md` & `kathara-3.6.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/.gitignore` & `kathara-3.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/CODE_OF_CONDUCT.md` & `kathara-3.6.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/CONTRIBUTING.md` & `kathara-3.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/LICENSE` & `kathara-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/PKG-INFO` & `kathara-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.6.2
+Version: 3.6.3
 Summary: A lightweight container-based emulation system.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.3.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `kathara-3.6.2/README.md` & `kathara-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/Makefile` & `kathara-3.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/footer.txt` & `kathara-3.6.3/docs/footer.txt`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/index.txt` & `kathara-3.6.3/docs/index.txt`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-check.1.ronn` & `kathara-3.6.3/docs/kathara-check.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-connect.1.ronn` & `kathara-3.6.3/docs/kathara-connect.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-exec.1.ronn` & `kathara-3.6.3/docs/kathara-exec.1.ronn`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 m4_changequote()
 kathara-exec(1) -- Execute a command in a Kathara device
 =============================================
 
 ## SYNOPSIS
 
 `kathara exec` [`-h`] [`-d` <DIRECTORY> \| `-v`]  
-[`--no-stdout`] [`--no-stderr`]  
+[`--no-stdout`] [`--no-stderr`] [`--wait`]  
 <DEVICE_NAME> <COMMAND> [<COMMAND> ...]
 
 ## DESCRIPTION
 
 Execute a command in the Kathara device DEVICE_NAME.
 
 ## OPTIONS
@@ -31,14 +31,19 @@
 
 * `--no-stdout`:
     Disable stdout of the executed command.
 
 * `--no-stderr`:
     Disable stderr of the executed command.
 
+* `--wait`:
+    Wait until startup commands execution finishes.
+
+    You can override the wait by pressing `[ENTER]`.
+
 * `<DEVICE_NAME>:
     Name of the device to execute the command into.
 
 * `<COMMAND>:
     Shell command that will be executed inside the device.
 
 ## EXAMPLES
```

### Comparing `kathara-3.6.2/docs/kathara-lab-dirs.7.ronn` & `kathara-3.6.3/docs/kathara-lab-dirs.7.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lab.conf.5.ronn` & `kathara-3.6.3/docs/kathara-lab.conf.5.ronn`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     Set the amount of available RAM inside the device. If you set this option, the minimum allowed value is 4m (4 megabyte).
 
     This option takes a positive integer, followed by a suffix of "b", "k", "m", "g", to indicate bytes, kilobytes, megabytes, or gigabytes.
 
 * `cpus` (float):
     Limit the amount of CPU available for this device.
 
-    This option takes a positive float, ranging from 0 to max number of host logical CPUs. For instance, if the host device has two CPUs and you set `device[cpus]=1.5`, the container is guaranteed at most one and a half of the CPUs.
+    This option takes a positive float, ranging from 0 to max number of host logical CPUs. For instance, if the host device has two CPUs and you set `device[cpus]=1.5`, the device is guaranteed at most one and a half of the CPUs.
 
 * `port` (string):
-    Map localhost port HOST to the internal port GUEST of the device for the specified PROTOCOL.
+    Map localhost port HOST to the internal port GUEST of the device for the specified PROTOCOL. The syntax is [HOST:]GUEST[/PROTOCOL].
 
     If HOST port is not specified, default is 3000. If PROTOCOL is not specified, default is `tcp`. Supported PROTOCOL values are: tcp, udp, or sctp.
+    For instance, with this command you can map host's port 8080 to device's port 80 with TCP protocol: `device[port]="8080:80/tcp"`.
 
 * `bridged` (boolean):
     Connect the device to the host network by adding an additional network interface. This interface will be connected to the host network through a NAT connection.
 
 * `ipv6` (boolean):
     Enable or disable IPv6 on this device.
```

### Comparing `kathara-3.6.2/docs/kathara-lab.dep.5.ronn` & `kathara-3.6.3/docs/kathara-lab.dep.5.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lab.ext.5.ronn` & `kathara-3.6.3/docs/kathara-lab.ext.5.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lclean.1.ronn` & `kathara-3.6.3/docs/kathara-lclean.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lconfig.1.ronn` & `kathara-3.6.3/docs/kathara-lconfig.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-linfo.1.ronn` & `kathara-3.6.3/docs/kathara-linfo.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-list.1.ronn` & `kathara-3.6.3/docs/kathara-list.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lrestart.1.ronn` & `kathara-3.6.3/docs/kathara-lrestart.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-lstart.1.ronn` & `kathara-3.6.3/docs/kathara-lstart.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-ltest.1.ronn` & `kathara-3.6.3/docs/kathara-ltest.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-settings.1.ronn` & `kathara-3.6.3/docs/kathara-settings.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-vclean.1.ronn` & `kathara-3.6.3/docs/kathara-vclean.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-vconfig.1.ronn` & `kathara-3.6.3/docs/kathara-vconfig.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-vstart.1.ronn` & `kathara-3.6.3/docs/kathara-vstart.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara-wipe.1.ronn` & `kathara-3.6.3/docs/kathara-wipe.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara.1.ronn` & `kathara-3.6.3/docs/kathara.1.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/docs/kathara.conf.5.ronn` & `kathara-3.6.3/docs/kathara.conf.5.ronn`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/pyproject.toml` & `kathara-3.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kathara"
-version = "3.6.2"
+version = "3.6.3"
 description = "A lightweight container-based emulation system."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = ["NETWORK-EMULATION", "CONTAINERS", "NFV"]
 authors = [
     { name = "Kathara Framework", email = "contact@kathara.org" } # Optional
@@ -36,14 +36,15 @@
     "coloredlogs>=10.0",
     "terminaltables>=3.1.0",
     "slug>=2.0",
     "deepdiff==6.2.2",
     "pyroute2>=0.5.19",
     "progressbar2>=1.14.0",
     "fs>=2.4.16",
+    "chardet",
     "libtmux>=0.8.2; platform_system == 'darwin' or platform_system == 'linux'",
     "appscript>=1.1.0; platform_system == 'darwin'",
     "pypiwin32>=223; platform_system == 'win32'",
     "windows-curses>=2.1.0; platform_system == 'win32'"
 ]
 
 [project.optional-dependencies]
```

### Comparing `kathara-3.6.2/scripts/Linux-Deb/Docker-Linux-Build/Dockerfile_template` & `kathara-3.6.3/scripts/Linux-Deb/Docker-Linux-Build/Dockerfile_template`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Deb/Makefile` & `kathara-3.6.3/scripts/Linux-Deb/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/make -f
 
-VERSION=3.6.2
+VERSION=3.6.3
 DEBIAN_PACKAGE_VERSION=1
 LAUNCHPAD_NAME=tcaiazzi
 NO_BINARY_PACKAGES=pyroute2|pyuv|deepdiff
 
 .PHONY: allSigned docker-build-image prepare-deb-source unpack-deb-source clean-output-folder copy-debian-folder download-pip build-man build-deb-unsigned build-deb-signed ppa clean venv autocompletion
 
-allSigned: clean prepare-deb-source docker-signed_focal docker-signed_jammy docker-signed_kinetic
+allSigned: clean prepare-deb-source docker-signed_focal docker-signed_jammy
 
 docker-unsigned_%: clean prepare-deb-source docker-build-image_%
 	docker run -ti --rm -v `pwd`/../../:/opt/kathara kathara/linux-build-deb:$* /bin/bash -c \
 	 	"make build-deb-unsigned distro=$* && chown -R $(shell id -u):$(shell id -g) Output"
 
 docker-signed_%: docker-build-image_%
 	docker run -ti --rm -v $(HOME)/.gnupg:/root/gnupg-host -v `pwd`/../../:/opt/kathara kathara/linux-build-deb:$* /bin/bash -c \
```

### Comparing `kathara-3.6.2/scripts/Linux-Deb/README.md` & `kathara-3.6.3/scripts/Linux-Deb/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Deb/debian/control` & `kathara-3.6.3/scripts/Linux-Deb/debian/control`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Deb/debian/copyright` & `kathara-3.6.3/scripts/Linux-Deb/debian/copyright`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Deb/debian/rules` & `kathara-3.6.3/scripts/Linux-Deb/debian/rules`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Pkg/Docker-Linux-Build/Dockerfile` & `kathara-3.6.3/scripts/Linux-Pkg/Docker-Linux-Build/Dockerfile`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Pkg/Makefile` & `kathara-3.6.3/scripts/Linux-Pkg/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/make -f
 
-VERSION=3.6.2
+VERSION=3.6.3
 PACKAGE_VERSION=1
-AUR_NAME=user
-AUR_MAIL=contact@kathara.org
+AUR_NAME=tcaiazzi
+AUR_MAIL=tommasocaiazzi@gmail.com
 
 .PHONY: all allRemote clean docker-build-image docker-build-local docker-build-remote build-local build-remote
 
-allLocal: clean docker-build-image docker-build-local
+all: clean docker-build-image docker-build-local
 
 allRemote: clean docker-build-image docker-build-remote
 
 docker-build-local: docker-build-image
 	mkdir -p Output
 	docker run -ti -v `pwd`:/home/builduser/kathara:ro -v `pwd`/Output:/home/builduser/output -v `pwd`/../..:/home/builduser/kathara-source/Kathara-$(VERSION):ro  kathara/linux-build-pkg /usr/bin/su -c \
 		"make -f /home/builduser/kathara/Makefile build-local" builduser
@@ -37,18 +37,19 @@
 	sed -i -e 's/__PYTHON_DEP__//g' /home/builduser/build/PKGBUILD
 	sed -i -e 's/__SOURCE__/"kathara-$(VERSION).tar.gz"/g' /home/builduser/build/PKGBUILD
 	makepkg
 	mv kathara*.pkg.tar.zst /home/builduser/output/
 
 build-remote: prepare-files
 	sed -i -e "s/__PYTHON_DEP__/'python310'/g" /home/builduser/build/PKGBUILD
-	sed -i -e 's/__SOURCE__/"https:\/\/github.com\/KatharaFramework\/Kathara\/archive\/refs\/tags\/$pkgver.tar.gz"/g' /home/builduser/build/PKGBUILD
+	sed -i -e 's/__SOURCE__/"https:\/\/github.com\/KatharaFramework\/Kathara\/archive\/refs\/tags\/\$$\pkgver.tar.gz"/g' /home/builduser/build/PKGBUILD
 	cp -r /home/builduser/ssh/ /home/builduser/.ssh/ && chmod 600 /home/builduser/.ssh/id_rsa
 	ssh-keyscan aur.archlinux.org > /home/builduser/.ssh/known_hosts
 	cd .. && git clone ssh://aur@aur.archlinux.org/kathara kathara-aur
+	cd ../kathara-aur && git checkout master
 	git config --global user.name "$(AUR_NAME)"
 	git config --global user.email "$(AUR_MAIL)"
 	cp -r /home/builduser/build/* ../kathara-aur/
 	cd ../kathara-aur && makepkg --printsrcinfo > .SRCINFO
 	cd ../kathara-aur && git add .
 	cd ../kathara-aur && git commit -m "Bump to v$(VERSION)-$(PACKAGE_VERSION)"
 	cd ../kathara-aur && git push
```

### Comparing `kathara-3.6.2/scripts/Linux-Pkg/README.md` & `kathara-3.6.3/scripts/Linux-Pkg/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 # Compiling Kathara for Linux (PKG) locally
 
 1. Change the Kathara version number in the following files:
     1. `src/Kathara/version.py`
     2. `Makefile`
 2. Write a proper `changelog` section in `pkginfo/kathara.changelog` file. 
-3. Run `make allLocal`. This will:
+3. Run `make all`. This will:
     1. Create a proper Docker image for the build environment
     2. Run a Docker container with the image built above.
     3. Compile Kathara into a binary.
     4. Create a `.pkg` package.
     5. Automatically remove the Docker container.
 4. Output file is located in the `Output` directory
```

### Comparing `kathara-3.6.2/scripts/Linux-Pkg/pkginfo/PKGBUILD` & `kathara-3.6.3/scripts/Linux-Pkg/pkginfo/PKGBUILD`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Linux-Rpm/Makefile` & `kathara-3.6.3/scripts/Linux-Rpm/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/make -f
 
-VERSION=3.6.2
+VERSION=3.6.3
 PACKAGE_VERSION=1
 
 .PHONY: all clean docker-build-image prepare-source prepare-man-pages prepare-bash-completion pack-source build
 
 all: clean docker-build-image docker-build
 
 docker-build: docker-build-image
```

### Comparing `kathara-3.6.2/scripts/Linux-Rpm/README.md` & `kathara-3.6.3/scripts/Linux-Rpm/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/Makefile` & `kathara-3.6.3/scripts/OSX/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/make -s
 
 PRODUCT=Kathara
-VERSION=3.6.2
+VERSION=3.6.3
 TARGET_DIRECTORY=Output
 APPLE_DEVELOPER_CERTIFICATE_ID=FakeID
 ROFF_DIR=../../docs/Roff
 VENV_DIR:=${CURDIR}/venv
 
 .PHONY: all_x86 allSigned_x86 all_arm64 allSigned_arm64 test deps manpages cleanall cleanman cleanbinary cleanenv
 all: all_x86 all_arm64
```

### Comparing `kathara-3.6.2/scripts/OSX/README.md` & `kathara-3.6.3/scripts/OSX/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/darwin/Distribution` & `kathara-3.6.3/scripts/OSX/darwin/Distribution`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/darwin/Resources/banner.png` & `kathara-3.6.3/scripts/OSX/darwin/Resources/banner.png`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/darwin/Resources/conclusion.html` & `kathara-3.6.3/scripts/OSX/darwin/Resources/conclusion.html`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/darwin/Resources/welcome.html` & `kathara-3.6.3/scripts/OSX/darwin/Resources/welcome.html`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/darwin/uninstall.sh` & `kathara-3.6.3/scripts/OSX/darwin/uninstall.sh`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/OSX/kathara.spec` & `kathara-3.6.3/scripts/OSX/kathara.spec`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Windows/Assets/app_icon.ico` & `kathara-3.6.3/scripts/Windows/Assets/app_icon.ico`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Windows/Assets/environment.iss` & `kathara-3.6.3/scripts/Windows/Assets/environment.iss`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Windows/Assets/kathara.spec` & `kathara-3.6.3/scripts/Windows/Assets/kathara.spec`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Windows/README.md` & `kathara-3.6.3/scripts/Windows/README.md`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/Windows/installer.iss` & `kathara-3.6.3/scripts/Windows/installer.iss`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Kathara"
-#define MyAppVersion "3.6.2"
+#define MyAppVersion "3.6.3"
 #define MyAppPublisher "Kathara Team"
 #define MyAppURL "https://www.kathara.org"
 #define MyAppExeName "kathara.exe"
 
 #include "Assets\environment.iss"
 
 [Setup]
```

### Comparing `kathara-3.6.2/scripts/autocompletion/generate_autocompletion.py` & `kathara-3.6.3/scripts/autocompletion/generate_autocompletion.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/pydoc/Makefile` & `kathara-3.6.3/scripts/pydoc/Makefile`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/scripts/pydoc/generate_doc.py` & `kathara-3.6.3/scripts/pydoc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/setup.cfg` & `kathara-3.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kathara
-version = 3.6.2
+version = 3.6.3
 author = Kathara Framework
 author_email = contact@kathara.org
 description = A lightweight container based emulation system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = www.kathara.org
 project_urls =
```

### Comparing `kathara-3.6.2/setup.py` & `kathara-3.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 from setuptools import find_packages
 
 setup(
     name='kathara',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     py_modules=['kathara'],
-    version='3.6.2',
+    version='3.6.3',
     license='gpl-3.0',
     description='A lightweight container based emulation system.',
     author='Kathara Framework',
     author_email='contact@kathara.org',
     url='https://www.kathara.org',
-    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz',
+    download_url='https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.3.tar.gz',
     keywords=['NETWORK-EMULATION', 'CONTAINERS', 'NFV'],
     install_requires=[
         "binaryornot>=0.4.4",
         "docker>=6.0.1",
         "kubernetes>=23.3.0",
         "requests>=2.22.0",
         "coloredlogs>=10.0",
         "terminaltables>=3.1.0",
         "slug>=2.0",
         "deepdiff==6.2.2",
         "pyroute2>=0.5.19",
         "progressbar2>=1.14.0",
         "fs>=2.4.16",
+        "chardet",
         "libtmux>=0.8.2; platform_system == 'darwin' or platform_system == 'linux'",
         "appscript>=1.1.0; platform_system == 'darwin'",
         "pypiwin32>=223; platform_system == 'win32'",
         "windows-curses>=2.1.0; platform_system == 'win32'"
     ],
     extras_require={
         'pyuv': ["pyuv @ https://api.github.com/repos/saghul/pyuv/tarball/master"],
```

### Comparing `kathara-3.6.2/src/Kathara/auth/PrivilegeHandler.py` & `kathara-3.6.3/src/Kathara/auth/PrivilegeHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/CheckCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/CheckCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/ConnectCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/ConnectCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/ExecCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/ListCommand.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,80 @@
 import argparse
-import sys
-from typing import List
+from typing import List, Optional
 
+from ..ui.utils import create_table
 from ... import utils
+from ...exceptions import PrivilegeError
 from ...foundation.cli.command.Command import Command
 from ...manager.Kathara import Kathara
-from ...model.Lab import Lab
-from ...parser.netkit.LabParser import LabParser
 from ...strings import strings, wiki_description
+from ...trdparty.curses.curses import Curses
 
 
-class ExecCommand(Command):
+class ListCommand(Command):
     def __init__(self) -> None:
         Command.__init__(self)
 
         self.parser: argparse.ArgumentParser = argparse.ArgumentParser(
-            prog='kathara exec',
-            description=strings['exec'],
+            prog='kathara list',
+            description=strings['list'],
             epilog=wiki_description,
             add_help=False
         )
 
         self.parser.add_argument(
             '-h', '--help',
             action='help',
             default=argparse.SUPPRESS,
             help='Show a help message and exit.'
         )
 
-        group = self.parser.add_mutually_exclusive_group(required=False)
-
-        group.add_argument(
-            '-d', '--directory',
-            help='Specify the folder containing the network scenario.',
-        )
-        group.add_argument(
-            '-v', '--vmachine',
-            dest="vmachine",
-            action="store_true",
-            help='The device has been started with vstart command.',
-        )
         self.parser.add_argument(
-            '--no-stdout',
-            dest="no_stdout",
-            action="store_true",
-            help='Disable stdout of the executed command.',
+            '-a', '--all',
+            required=False,
+            action='store_true',
+            help='Show all running Kathara devices of all users. MUST BE ROOT FOR THIS OPTION.'
         )
+
         self.parser.add_argument(
-            '--no-stderr',
-            dest="no_stderr",
-            action="store_true",
-            help='Disable stderr of the executed command.',
+            '-w', '-l', '--watch', '--live',
+            required=False,
+            action='store_true',
+            help='Watch mode.'
         )
+
         self.parser.add_argument(
-            'machine_name',
+            '-n', '--name',
             metavar='DEVICE_NAME',
-            help='Name of the device to execute the command into.'
-        )
-        self.parser.add_argument(
-            'command',
-            metavar='COMMAND',
-            nargs='+',
-            help='Shell command that will be executed inside the device.'
+            required=False,
+            help='Show only information about a specified device.'
         )
 
     def run(self, current_path: str, argv: List[str]) -> None:
         self.parse_args(argv)
         args = self.get_args()
 
-        if args['vmachine']:
-            lab = Lab("kathara_vlab")
+        if args['all'] and not utils.is_admin():
+            raise PrivilegeError("You must be root in order to show all Kathara devices of all users.")
+
+        all_users = bool(args['all'])
+
+        if args['watch']:
+            self._get_live_info(machine_name=args['name'], all_users=all_users)
         else:
-            lab_path = args['directory'].replace('"', '').replace("'", '') if args['directory'] else current_path
-            lab_path = utils.get_absolute_path(lab_path)
-            try:
-                lab = LabParser.parse(lab_path)
-            except (Exception, IOError):
-                lab = Lab(None, path=lab_path)
+            machines_stats = Kathara.get_instance().get_machines_stats(machine_name=args['name'], all_users=all_users)
+            print(next(create_table(machines_stats)))
+
+    @staticmethod
+    def _get_live_info(machine_name: Optional[str], all_users: bool) -> None:
+        machines_stats = Kathara.get_instance().get_machines_stats(machine_name=machine_name, all_users=all_users)
+        table = create_table(machines_stats)
 
-        exec_output = Kathara.get_instance().exec(args['machine_name'], args['command'], lab_hash=lab.hash)
+        Curses.get_instance().init_window()
 
         try:
             while True:
-                (stdout, stderr) = next(exec_output)
-                stdout = stdout.decode('utf-8') if stdout else ""
-                stderr = stderr.decode('utf-8') if stderr else ""
-
-                if not args['no_stdout']:
-                    sys.stdout.write(stdout)
-                if stderr and not args['no_stderr']:
-                    sys.stderr.write(stderr)
+                Curses.get_instance().print_string(next(table))
         except StopIteration:
             pass
+        finally:
+            Curses.get_instance().close()
```

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LcleanCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LconfigCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LinfoCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LinfoCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LrestartCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LrestartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LstartCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/LtestCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/LtestCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/VcleanCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/VcleanCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/VconfigCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/VconfigCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/VstartCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/VstartCommand.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/command/WipeCommand.py` & `kathara-3.6.3/src/Kathara/cli/command/WipeCommand.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import shutil
 import sys
 from typing import List
 
 from ..ui.utils import confirmation_prompt
 from ... import utils
 from ...exceptions import PrivilegeError
 from ...foundation.cli.command.Command import Command
@@ -63,10 +62,7 @@
         if args['settings']:
             Setting.wipe_from_disk()
         else:
             if args['all'] and not utils.is_admin():
                 raise PrivilegeError("You must be root in order to wipe all Kathara devices of all users.")
 
             Kathara.get_instance().wipe(all_users=bool(args['all']))
-
-            vlab_dir = utils.get_vlab_temp_path(force_creation=False)
-            shutil.rmtree(vlab_dir, ignore_errors=True)
```

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/event/HandleProgressBar.py` & `kathara-3.6.3/src/Kathara/cli/ui/event/HandleProgressBar.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/event/UpdateDockerImage.py` & `kathara-3.6.3/src/Kathara/cli/ui/event/UpdateDockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/event/register.py` & `kathara-3.6.3/src/Kathara/cli/ui/event/register.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .UpdateDockerImage import UpdateDockerImage
-from .OpenMachineTerminal import OpenMachineTerminal
+from .HandleMachineTerminal import HandleMachineTerminal
 from .HandleProgressBar import HandleProgressBar
+from .UpdateDockerImage import UpdateDockerImage
 from ....event.EventDispatcher import EventDispatcher
 
 
 def register_cli_events() -> None:
     """Register events to handle UI from CLI.
 
     Returns:
@@ -35,8 +35,11 @@
     EventDispatcher.get_instance().register("machines_deploy_ended", machine_deploy_progress_bar_handler, "finish")
 
     machine_undeploy_progress_bar_handler = HandleProgressBar('Deleting devices...')
     EventDispatcher.get_instance().register("machines_undeploy_started", machine_undeploy_progress_bar_handler, "init")
     EventDispatcher.get_instance().register("machine_undeployed", machine_undeploy_progress_bar_handler, "update")
     EventDispatcher.get_instance().register("machines_undeploy_ended", machine_undeploy_progress_bar_handler, "finish")
 
-    EventDispatcher.get_instance().register("machine_deployed", OpenMachineTerminal())
+    machine_terminal_handler = HandleMachineTerminal()
+    EventDispatcher.get_instance().register("machine_deployed", machine_terminal_handler, "run")
+    EventDispatcher.get_instance().register("machine_startup_wait_started", machine_terminal_handler, "print_wait_msg")
+    EventDispatcher.get_instance().register("machine_startup_wait_ended", machine_terminal_handler, "flush")
```

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/setting/CommonOptionsHandler.py` & `kathara-3.6.3/src/Kathara/cli/ui/setting/CommonOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/setting/DockerOptionsHandler.py` & `kathara-3.6.3/src/Kathara/cli/ui/setting/DockerOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py` & `kathara-3.6.3/src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/setting/SettingsMenuFactory.py` & `kathara-3.6.3/src/Kathara/cli/ui/setting/SettingsMenuFactory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/setting/utils.py` & `kathara-3.6.3/src/Kathara/cli/ui/setting/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/cli/ui/utils.py` & `kathara-3.6.3/src/Kathara/cli/ui/utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/decorators.py` & `kathara-3.6.3/src/Kathara/decorators.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/event/EventDispatcher.py` & `kathara-3.6.3/src/Kathara/event/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/exceptions.py` & `kathara-3.6.3/src/Kathara/exceptions.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/cli/CliArgs.py` & `kathara-3.6.3/src/Kathara/foundation/cli/CliArgs.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/cli/command/Command.py` & `kathara-3.6.3/src/Kathara/foundation/cli/command/Command.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py` & `kathara-3.6.3/src/Kathara/foundation/cli/ui/setting/OptionsHandler.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/factory/Factory.py` & `kathara-3.6.3/src/Kathara/foundation/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/manager/IManager.py` & `kathara-3.6.3/src/Kathara/foundation/manager/IManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 from abc import ABC, abstractmethod
-from typing import Dict, Set, Any, Generator, Tuple, List, Optional
+from typing import Dict, Set, Any, Generator, Tuple, List, Optional, Union
 
 from .stats.ILinkStats import ILinkStats
 from .stats.IMachineStats import IMachineStats
 from ...model.Lab import Lab
 from ...model.Link import Link
 from ...model.Machine import Machine
 
@@ -117,23 +117,25 @@
 
         Raises:
             LabNotFoundError: If the collision domain is not associated to any network scenario.
         """
         raise NotImplementedError("You must implement `undeploy_link` method.")
 
     @abstractmethod
-    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
+    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None, lab: Optional[Lab] = None,
                      selected_machines: Optional[Set[str]] = None) -> None:
         """Undeploy a Kathara network scenario.
 
         Args:
-            lab_hash (Optional[str]): The hash of the network scenario. Can be used as an alternative to lab_name.
-                If None, lab_name should be set.
-            lab_name (Optional[str]): The name of the network scenario. Can be used as an alternative to lab_hash.
-                If None, lab_hash should be set.
+            lab_hash (Optional[str]): The hash of the network scenario.
+                Can be used as an alternative to lab_name and lab. If None, lab_name or lab should be set.
+            lab_name (Optional[str]): The name of the network scenario.
+                Can be used as an alternative to lab_hash and lab. If None, lab_hash or lab should be set.
+            lab (Optional[Kathara.model.Lab]): The network scenario object.
+                Can be used as an alternative to lab_hash and lab_name. If None, lab_hash or lab_name should be set.
             selected_machines (Optional[Set[str]]): If not None, undeploy only the specified devices.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
@@ -151,42 +153,51 @@
         Returns:
             None
         """
         raise NotImplementedError("You must implement `wipe` method.")
 
     @abstractmethod
     def connect_tty(self, machine_name: str, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
-                    shell: str = None, logs: bool = False) -> None:
+                    shell: str = None, logs: bool = False, wait: Union[bool, Tuple[int, float]] = True) -> None:
         """Connect to a device in a running network scenario, using the specified shell.
 
         Args:
             machine_name (str): The name of the device to connect.
             lab_hash (str): The hash of the network scenario where the device is deployed.
             lab_name (str): The name of the network scenario where the device is deployed.
             shell (str): The name of the shell to use for connecting.
             logs (bool): If True, print startup logs on stdout.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before connecting. If a tuple is provided, the first value indicates the number of retries
+                before stopping waiting and the second value indicates the time interval to wait for each retry.
+                Default is True.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
         raise NotImplementedError("You must implement `connect_tty` method.")
 
     @abstractmethod
-    def exec(self, machine_name: str, command: List[str], lab_hash: Optional[str] = None,
-             lab_name: Optional[str] = None) -> Generator[Tuple[bytes, bytes], None, None]:
+    def exec(self, machine_name: str, command: Union[List[str], str], lab_hash: Optional[str] = None,
+             lab_name: Optional[str] = None, wait: Union[bool, Tuple[int, float]] = False) \
+            -> Generator[Tuple[bytes, bytes], None, None]:
         """Exec a command on a device in a running network scenario.
 
         Args:
             machine_name (str): The name of the device to connect.
-            command (List[str]): The command to exec on the device.
+            command (Union[List[str], str]): The command to exec on the device.
             lab_hash (Optional[str]): The hash of the network scenario where the device is deployed.
             lab_name (Optional[str]): The name of the network scenario where the device is deployed.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before executing the command. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to wait
+                for each retry. Default is False.
 
         Returns:
             Generator[Tuple[bytes, bytes]]: A generator of tuples containing the stdout and stderr in bytes.
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
```

### Comparing `kathara-3.6.2/src/Kathara/foundation/manager/stats/ILinkStats.py` & `kathara-3.6.3/src/Kathara/foundation/manager/stats/ILinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/manager/stats/IMachineStats.py` & `kathara-3.6.3/src/Kathara/foundation/manager/stats/IMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/manager/terminal/Terminal.py` & `kathara-3.6.3/src/Kathara/foundation/manager/terminal/Terminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/manager/terminal/terminal_utils.py` & `kathara-3.6.3/src/Kathara/foundation/manager/terminal/terminal_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/model/FilesystemMixin.py` & `kathara-3.6.3/src/Kathara/foundation/model/FilesystemMixin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/setting/SettingsAddon.py` & `kathara-3.6.3/src/Kathara/foundation/setting/SettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/foundation/test/Test.py` & `kathara-3.6.3/src/Kathara/foundation/test/Test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from abc import ABC, abstractmethod
 from typing import Dict, Union, List
 
+import chardet
 from deepdiff import DeepDiff
 
 from ...manager.Kathara import Kathara
 from ...model.Lab import Lab
 
 
 class Test(ABC):
@@ -38,13 +39,17 @@
             'stdout': '',
             'stderr': ''
         }
 
         try:
             while True:
                 (stdout, stderr) = next(exec_output)
+
+                stdout_char_encoding = chardet.detect(stdout) if stdout else None
+                stderr_char_encoding = chardet.detect(stderr) if stderr else None
+
                 if stdout:
-                    result['stdout'] += stdout.decode('utf-8')
+                    result['stdout'] += stdout.decode(stdout_char_encoding['encoding']) if stdout else ""
                 if stderr:
-                    result['stderr'] += stderr.decode('utf-8')
+                    result['stderr'] += stderr.decode(stderr_char_encoding['encoding']) if stderr else ""
         except StopIteration:
             return result['stdout'], result['stderr']
```

### Comparing `kathara-3.6.2/src/Kathara/manager/Kathara.py` & `kathara-3.6.3/src/Kathara/manager/Kathara.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import io
-from typing import Set, Dict, Generator, Any, Tuple, List, Optional
+from typing import Set, Dict, Generator, Any, Tuple, List, Optional, Union
 
 from ..exceptions import InstantiationError
 from ..foundation.manager.IManager import IManager
 from ..foundation.manager.ManagerFactory import ManagerFactory
 from ..foundation.manager.stats.ILinkStats import ILinkStats
 from ..foundation.manager.stats.IMachineStats import IMachineStats
 from ..model.Lab import Lab
@@ -145,81 +145,92 @@
             None
 
         Raises:
             LabNotFoundError: If the collision domain is not associated to any network scenario.
         """
         self.manager.undeploy_link(link)
 
-    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
+    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None, lab: Optional[Lab] = None,
                      selected_machines: Optional[Set[str]] = None) -> None:
         """Undeploy a Kathara network scenario.
 
         Args:
-            lab_hash (Optional[str]): The hash of the network scenario. Can be used as an alternative to lab_name.
-                If None, lab_name should be set.
-            lab_name (Optional[str]): The name of the network scenario. Can be used as an alternative to lab_hash.
-                If None, lab_hash should be set.
+            lab_hash (Optional[str]): The hash of the network scenario.
+                Can be used as an alternative to lab_name and lab. If None, lab_name or lab should be set.
+            lab_name (Optional[str]): The name of the network scenario.
+                Can be used as an alternative to lab_hash and lab. If None, lab_hash or lab should be set.
+            lab (Optional[Kathara.model.Lab]): The network scenario object.
+                Can be used as an alternative to lab_hash and lab_name. If None, lab_hash or lab_name should be set.
             selected_machines (Optional[Set[str]]): If not None, undeploy only the specified devices.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
-        self.manager.undeploy_lab(lab_hash, lab_name, selected_machines)
+        self.manager.undeploy_lab(lab_hash, lab_name, lab, selected_machines)
 
     def wipe(self, all_users: bool = False) -> None:
         """Undeploy all the running network scenarios.
 
         Args:
             all_users (bool): If false, undeploy only the current user network scenarios. If true, undeploy the
                 running network scenarios of all users.
 
         Returns:
             None
         """
         self.manager.wipe(all_users)
 
     def connect_tty(self, machine_name: str, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
-                    shell: str = None, logs: bool = False) -> None:
+                    shell: str = None, logs: bool = False, wait: Union[bool, Tuple[int, float]] = True) -> None:
         """Connect to a device in a running network scenario, using the specified shell.
 
         Args:
             machine_name (str): The name of the device to connect.
             lab_hash (str): The hash of the network scenario where the device is deployed.
             lab_name (str): The name of the network scenario where the device is deployed.
             shell (str): The name of the shell to use for connecting.
             logs (bool): If True, print startup logs on stdout.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before connecting. If a tuple is provided, the first value indicates the number of retries
+                before stopping waiting and the second value indicates the time interval to wait for each retry.
+                Default is True.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
-        self.manager.connect_tty(machine_name, lab_hash, lab_name, shell, logs)
+        self.manager.connect_tty(machine_name, lab_hash, lab_name, shell, logs, wait)
 
-    def exec(self, machine_name: str, command: List[str], lab_hash: Optional[str] = None,
-             lab_name: Optional[str] = None) -> Generator[Tuple[bytes, bytes], None, None]:
+    def exec(self, machine_name: str, command: Union[List[str], str], lab_hash: Optional[str] = None,
+             lab_name: Optional[str] = None, wait: Union[bool, Tuple[int, float]] = False) \
+            -> Generator[Tuple[bytes, bytes], None, None]:
         """Exec a command on a device in a running network scenario.
 
         Args:
             machine_name (str): The name of the device to connect.
-            command (List[str]): The command to exec on the device.
+            command (Union[List[str], str]): The command to exec on the device.
             lab_hash (Optional[str]): The hash of the network scenario where the device is deployed.
             lab_name (Optional[str]): The name of the network scenario where the device is deployed.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before executing the command. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to wait
+                for each retry. Default is False.
 
         Returns:
             Generator[Tuple[bytes, bytes]]: A generator of tuples containing the stdout and stderr in bytes.
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
-        return self.manager.exec(machine_name, command, lab_hash, lab_name)
+        return self.manager.exec(machine_name, command, lab_hash, lab_name, wait)
 
     def copy_files(self, machine: Machine, guest_to_host: Dict[str, io.IOBase]) -> None:
         """Copy files on a running device in the specified paths.
 
         Args:
             machine (Kathara.model.Machine): A running device object. It must have the api_object field populated.
             guest_to_host (Dict[str, io.IOBase]): A dict containing the device path as key and
```

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/DockerImage.py` & `kathara-3.6.3/src/Kathara/manager/docker/DockerImage.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/DockerLink.py` & `kathara-3.6.3/src/Kathara/manager/docker/DockerLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/DockerMachine.py` & `kathara-3.6.3/src/Kathara/manager/docker/DockerMachine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import re
 import shlex
+import sys
+import time
 from itertools import islice
 from multiprocessing.dummy import Pool
 from typing import List, Dict, Generator, Optional, Set, Tuple, Union, Any
 
+import chardet
 import docker.models.containers
 from docker import DockerClient
 from docker.errors import APIError
 
 from .DockerImage import DockerImage
 from .stats.DockerMachineStats import DockerMachineStats
 from ... import utils
@@ -22,44 +25,44 @@
 
 RP_FILTER_NAMESPACE = "net.ipv4.conf.%s.rp_filter"
 OCI_RUNTIME_RE = re.compile(
     r"OCI runtime exec failed(.*?)(stat (.*): no such file or directory|exec: \"(.*)\": executable file not found)"
 )
 
 # Known commands that each container should execute
-# Run order: shared.startup, machine.startup and machine.meta['startup_commands']
+# Run order: shared.startup, machine.startup and machine.meta['exec_commands']
 STARTUP_COMMANDS = [
     # Unmount the /etc/resolv.conf and /etc/hosts files, automatically mounted by Docker inside the container.
     # In this way, they can be overwritten by custom user files.
     "umount /etc/resolv.conf",
     "umount /etc/hosts",
 
     # Copy the machine folder (if present) from the hostlab directory into the root folder of the container
     # In this way, files are all replaced in the container root folder
     "if [ -d \"/hostlab/{machine_name}\" ]; then "
-    "(cd /hostlab/{machine_name} && tar c .) | (cd / && tar xhf -); fi",
+    "(cd /hostlab/{machine_name} && tar c .) | (cd / && tar xhf - --no-same-owner --no-same-permissions); fi",
 
     # If /etc/hosts is not configured by the user, add the localhost mapping
     "if [ ! -s \"/etc/hosts\" ]; then "
     "echo '127.0.0.1 localhost' > /etc/hosts",
     "echo '::1 localhost' >> /etc/hosts",
     "fi",
 
     # Give proper permissions to /var/www
     "if [ -d \"/var/www\" ]; then "
     "chmod -R 777 /var/www/*; fi",
 
     # Give proper permissions to Quagga files (if present)
     "if [ -d \"/etc/quagga\" ]; then "
-    "chown --recursive quagga:quagga /etc/quagga/",
+    "chown -R quagga:quagga /etc/quagga/",
     "chmod 640 /etc/quagga/*; fi",
 
     # Give proper permissions to FRR files (if present)
     "if [ -d \"/etc/frr\" ]; then "
-    "chown frr:frr /etc/frr/*",
+    "chown -R frr:frr /etc/frr/",
     "chmod 640 /etc/frr/*; fi",
 
     # If shared.startup file is present
     "if [ -f \"/hostlab/shared.startup\" ]; then "
     # Give execute permissions to the file and execute it
     # We redirect the output "&>" to a debugging file
     "chmod u+x /hostlab/shared.startup",
@@ -73,15 +76,17 @@
     # We redirect the output "&>" to a debugging file
     "chmod u+x /hostlab/{machine_name}.startup",
     # Adds a line to enable command output
     "sed -i \"1s;^;set -x\\n\\n;\" /hostlab/{machine_name}.startup",
     "/hostlab/{machine_name}.startup &> /var/log/startup.log; fi",
 
     # Placeholder for user commands
-    "{machine_commands}"
+    "{machine_commands}",
+
+    "touch /tmp/EOS"
 ]
 
 SHUTDOWN_COMMANDS = [
     # If machine.shutdown file is present
     "if [ -f \"/hostlab/{machine_name}.shutdown\" ]; then "
     # Give execute permissions to the file and execute it
     "chmod u+x /hostlab/{machine_name}.shutdown; /hostlab/{machine_name}.shutdown; fi",
@@ -230,14 +235,15 @@
             sysctl_parameters[RP_FILTER_NAMESPACE % "eth0"] = 0
 
         sysctl_parameters["net.ipv4.ip_forward"] = 1
         sysctl_parameters["net.ipv4.icmp_ratelimit"] = 0
 
         if machine.is_ipv6_enabled():
             sysctl_parameters["net.ipv6.conf.all.forwarding"] = 1
+            sysctl_parameters["net.ipv6.conf.all.accept_ra"] = 0
             sysctl_parameters["net.ipv6.icmp.ratelimit"] = 0
             sysctl_parameters["net.ipv6.conf.default.disable_ipv6"] = 0
             sysctl_parameters["net.ipv6.conf.all.disable_ipv6"] = 0
 
         # Merge machine sysctls
         sysctl_parameters = {**sysctl_parameters, **machine.meta['sysctls']}
 
@@ -392,25 +398,25 @@
 
         # Bridged connection required but not added in `deploy` method.
         if "bridge_connected" not in machine.meta and machine.is_bridged():
             bridge_link = machine.lab.get_or_new_link(BRIDGE_LINK_NAME).api_object
             bridge_link.connect(machine.api_object)
 
         # Append executed machine startup commands inside the /var/log/startup.log file
-        if machine.meta['startup_commands']:
+        if machine.meta['exec_commands']:
             new_commands = []
-            for command in machine.meta['startup_commands']:
+            for command in machine.meta['exec_commands']:
                 new_commands.append("echo \"++ %s\" &>> /var/log/startup.log" % command)
                 new_commands.append(command)
-            machine.meta['startup_commands'] = new_commands
+            machine.meta['exec_commands'] = new_commands
 
         # Build the final startup commands string
         startup_commands_string = "; ".join(STARTUP_COMMANDS).format(
             machine_name=machine.name,
-            machine_commands="; ".join(machine.meta['startup_commands'])
+            machine_commands="; ".join(machine.meta['exec_commands']) if machine.meta['exec_commands'] else ":"
         )
 
         logging.debug(f"Executing startup command on `{machine.name}`: {startup_commands_string}")
 
         try:
             # Execute the startup commands inside the container (without privileged flag so basic permissions are used)
             self._exec_run(machine.api_object,
@@ -488,59 +494,90 @@
             None
         """
         self._delete_machine(machine_api_object)
 
         EventDispatcher.get_instance().dispatch("machine_undeployed", item=machine_api_object)
 
     def connect(self, lab_hash: str, machine_name: str, user: str = None, shell: str = None,
-                logs: bool = False) -> None:
+                logs: bool = False, wait: Union[bool, Tuple[int, float]] = True) -> None:
         """Open a stream to the Docker container specified by machine_name using the specified shell.
 
         Args:
             lab_hash (str): The hash of the network scenario containing the device.
             machine_name (str): The name of the device to connect.
             user (str): The name of a current user on the host.
             shell (str): The path to the desired shell.
             logs (bool): If True, print the logs of the startup command.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before giving control to the user. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to wait
+                for each retry. Default is True.
 
         Returns:
             None
 
         Raises:
             MachineNotFoundError: If the specified device is not running.
+            ValueError: If the wait values is neither a boolean nor a tuple, or an invalid tuple.
         """
         containers = self.get_machines_api_objects_by_filters(lab_hash=lab_hash, machine_name=machine_name, user=user)
         if not containers:
             raise MachineNotFoundError("The specified device `%s` is not running." % machine_name)
         container = containers.pop()
 
         if not shell:
             shell = shlex.split(container.labels['shell'])
         else:
             shell = shlex.split(shell)
 
         logging.debug("Connect to device `%s` with shell: %s" % (machine_name, shell))
 
-        # Get the logs, if the command fails it means that the shell is not found.
-        cat_logs_cmd = "cat /var/log/shared.log /var/log/startup.log"
-        startup_command = [item for item in shell]
-        startup_command.extend(['-c', cat_logs_cmd])
-        exec_result = self._exec_run(container,
-                                     cmd=startup_command,
-                                     stdout=True,
-                                     stderr=False,
-                                     privileged=False,
-                                     detach=False
-                                     )
-        startup_output = exec_result['output'].decode('utf-8')
+        if isinstance(wait, tuple):
+            if len(wait) != 2:
+                raise ValueError("Invalid `wait` value.")
+
+            n_retries, retry_interval = wait
+            should_wait = True
+        elif isinstance(wait, bool):
+            n_retries = None
+            retry_interval = 1
+            should_wait = wait
+        else:
+            raise ValueError("Invalid `wait` value.")
+
+        startup_waited = False
+        if should_wait:
+            startup_waited = self._wait_startup_execution(container, n_retries=n_retries, retry_interval=retry_interval)
+
+            EventDispatcher.get_instance().dispatch("machine_startup_wait_ended")
+
+        if logs and Setting.get_instance().print_startup_log:
+            # Get the logs, if the command fails it means that the shell is not found.
+            cat_logs_cmd = "cat /var/log/shared.log /var/log/startup.log"
+            startup_command = [item for item in shell]
+            startup_command.extend(['-c', cat_logs_cmd])
+            exec_result = self._exec_run(container,
+                                         cmd=startup_command,
+                                         stdout=True,
+                                         stderr=False,
+                                         privileged=False,
+                                         detach=False
+                                         )
+            char_encoding = chardet.detect(exec_result['output']) if exec_result['output'] else None
+            startup_output = exec_result['output'].decode(char_encoding['encoding']) if exec_result['output'] else None
+
+            if startup_output:
+                sys.stdout.write("--- Startup Commands Log\n")
+                sys.stdout.write(startup_output)
+                sys.stdout.write("--- End Startup Commands Log\n")
+
+                if not startup_waited:
+                    sys.stdout.write("!!! Executing other commands in background !!!\n")
 
-        if startup_output and logs and Setting.get_instance().print_startup_log:
-            print("--- Startup Commands Log\n")
-            print(startup_output)
-            print("--- End Startup Commands Log\n")
+                sys.stdout.flush()
 
         resp = self.client.api.exec_create(container.id,
                                            shell,
                                            stdout=True,
                                            stderr=True,
                                            stdin=True,
                                            tty=True,
@@ -559,37 +596,59 @@
         def cmd_connect():
             from .terminal.DockerNPipeTerminal import DockerNPipeTerminal
             DockerNPipeTerminal(exec_output, self.client, resp['Id']).start()
 
         utils.exec_by_platform(tty_connect, cmd_connect, tty_connect)
 
     def exec(self, lab_hash: str, machine_name: str, command: Union[str, List], user: str = None,
-             tty: bool = True) -> Generator[Tuple[bytes, bytes], None, None]:
+             tty: bool = True, wait: Union[bool, Tuple[int, float]] = False) \
+            -> Generator[Tuple[bytes, bytes], None, None]:
         """Execute the command on the Docker container specified by the lab_hash and the machine_name.
 
         Args:
             lab_hash (str): The hash of the network scenario containing the device.
             machine_name (str): The name of the device.
             user (str): The name of a current user on the host.
             command (Union[str, List]): The command to execute.
             tty (bool): If True, open a new tty.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before executing the command. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to
+                wait for each retry. Default is False.
 
         Returns:
             Generator[Tuple[bytes, bytes]]: A generator of tuples containing the stdout and stderr in bytes.
 
         Raises:
             MachineNotFoundError: If the specified device is not running.
+            ValueError: If the wait values is neither a boolean nor a tuple, or an invalid tuple.
         """
         logging.debug("Executing command `%s` to device with name: %s" % (command, machine_name))
 
         containers = self.get_machines_api_objects_by_filters(lab_hash=lab_hash, machine_name=machine_name, user=user)
         if not containers:
             raise MachineNotFoundError("The specified device `%s` is not running." % machine_name)
         container = containers.pop()
 
+        if isinstance(wait, tuple):
+            if len(wait) != 2:
+                raise ValueError("Invalid `wait` value.")
+
+            n_retries, retry_interval = wait
+            should_wait = True
+        elif isinstance(wait, bool):
+            n_retries = None
+            retry_interval = 1
+            should_wait = wait
+        else:
+            raise ValueError("Invalid `wait` value.")
+
+        if should_wait:
+            self._wait_startup_execution(container, n_retries=n_retries, retry_interval=retry_interval)
+
         command = shlex.split(command) if type(command) == str else command
         exec_result = self._exec_run(container,
                                      cmd=command,
                                      stdout=True,
                                      stderr=True,
                                      tty=tty,
                                      privileged=False,
@@ -655,24 +714,86 @@
                 raise MachineBinaryError(matches.group(3) or matches.group(4), container.labels['name'])
 
             raise e
 
         exit_code = self.client.api.exec_inspect(resp['Id'])['ExitCode']
         if not socket and not stream and (exit_code is not None and exit_code != 0):
             (stdout_out, _) = exec_output if demux else (exec_output, None)
-            exec_stdout = (stdout_out.decode('utf-8') if type(stdout_out) == bytes else stdout_out) if stdout else ""
+            exec_stdout = ""
+            if stdout_out:
+                if type(stdout_out) == bytes:
+                    char_encoding = chardet.detect(stdout_out)
+                    exec_stdout = stdout_out.decode(char_encoding['encoding'])
+                else:
+                    exec_stdout = stdout_out
             matches = OCI_RUNTIME_RE.search(exec_stdout)
             if matches:
                 raise MachineBinaryError(matches.group(3) or matches.group(4), container.labels['name'])
 
         if socket or stream:
             return {'exit_code': None, 'output': exec_output}
 
         return {'exit_code': int(exit_code) if exit_code is not None else None, 'output': exec_output}
 
+    def _wait_startup_execution(self, container: docker.models.containers.Container,
+                                n_retries: Optional[int] = None, retry_interval: float = 1) -> bool:
+        """Wait until the startup commands are executed or until the user requests the control over the device.
+
+        Args:
+            container (docker.models.containers.Container): The Docker container to wait.
+            n_retries (Optional[int]): Number of retries before stopping waiting. Default is None, waits indefinitely.
+            retry_interval (float): The time interval in seconds to wait for each retry. Default is 1.
+
+        Returns:
+            bool: False if the user requests the control before the ending of the startup. Else, True.
+        """
+        logging.debug(f"Waiting startup commands execution for device {container.labels['name']}...")
+
+        n_retries = n_retries if n_retries is None or n_retries >= 0 else abs(n_retries)
+        retry_interval = retry_interval if retry_interval >= 0 else 1
+
+        retries = 0
+        is_cmd_success = False
+        startup_waited = True
+        printed = False
+        while not is_cmd_success:
+            try:
+                exec_result = self._exec_run(container,
+                                             cmd="cat /tmp/EOS",
+                                             stdout=True,
+                                             stderr=False,
+                                             privileged=False,
+                                             detach=False
+                                             )
+                is_cmd_success = exec_result['exit_code'] == 0
+
+                if not printed and not is_cmd_success:
+                    EventDispatcher.get_instance().dispatch("machine_startup_wait_started")
+                    printed = True
+
+                # If the user requests the control, break the while loop
+                if utils.exec_by_platform(utils.wait_user_input_linux,
+                                          utils.wait_user_input_windows,
+                                          utils.wait_user_input_linux):
+                    startup_waited = False or is_cmd_success
+                    break
+
+                if not is_cmd_success:
+                    if n_retries is not None:
+                        if retries == n_retries:
+                            break
+                        retries += 1
+
+                    time.sleep(retry_interval)
+            except KeyboardInterrupt:
+                # Disable the CTRL+C interrupt while waiting for startup, otherwise terminal will close.
+                pass
+
+        return startup_waited
+
     @staticmethod
     def copy_files(machine_api_object: docker.models.containers.Container, path: str, tar_data: bytes) -> None:
         """Copy the files contained in tar_data in the Docker container path specified by the machine_api_object.
 
         Args:
             machine_api_object (docker.models.containers.Container): A Docker container.
             path (str): The path of the container where copy the tar_data.
@@ -791,8 +912,8 @@
                                )
             except MachineBinaryError as e:
                 logging.warning(f"Shell `{e.binary}` not found in "
                                 f"image `{container.image.tags[0]}` of device `{container.labels['name']}`. "
                                 f"Shutdown commands will not be executed."
                                 )
 
-        container.remove(force=True)
+        container.remove(v=True, force=True)
```

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/DockerManager.py` & `kathara-3.6.3/src/Kathara/manager/docker/DockerManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 import logging
-from typing import Set, Dict, Generator, Tuple, List, Optional
+from typing import Set, Dict, Generator, Tuple, List, Optional, Union
 
 import docker
 import docker.models.containers
 import docker.models.networks
 from requests.exceptions import ConnectionError as RequestsConnectionError
 
 from .DockerImage import DockerImage
@@ -120,15 +120,15 @@
 
         Returns:
             None
 
         Raises:
             MachineNotFoundError: If the specified devices are not in the network scenario.
         """
-        if selected_machines and not lab.find_machines(selected_machines):
+        if selected_machines and not lab.has_machines(selected_machines):
             machines_not_in_lab = selected_machines - set(lab.machines.keys())
             raise MachineNotFoundError(f"The following devices are not in the network scenario: {machines_not_in_lab}.")
 
         selected_links = None
         if selected_machines:
             selected_links = lab.get_links_from_machines(selected_machines)
 
@@ -236,35 +236,39 @@
         """
         if not link.lab:
             raise LabNotFoundError(f"Collision domain `{link.name}` is not associated to a network scenario.")
 
         self.docker_link.undeploy(link.lab.hash, selected_links={link.name})
 
     @privileged
-    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
+    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None, lab: Optional[Lab] = None,
                      selected_machines: Optional[Set[str]] = None) -> None:
         """Undeploy a Kathara network scenario.
 
         Args:
-            lab_hash (Optional[str]): The hash of the network scenario. Can be used as an alternative to lab_name.
-                If None, lab_name should be set.
-            lab_name (Optional[str]): The name of the network scenario. Can be used as an alternative to lab_hash.
-                If None, lab_hash should be set.
+            lab_hash (Optional[str]): The hash of the network scenario.
+                Can be used as an alternative to lab_name and lab. If None, lab_name or lab should be set.
+            lab_name (Optional[str]): The name of the network scenario.
+                Can be used as an alternative to lab_hash and lab. If None, lab_hash or lab should be set.
+            lab (Optional[Kathara.model.Lab]): The network scenario object.
+                Can be used as an alternative to lab_hash and lab_name. If None, lab_hash or lab_name should be set.
             selected_machines (Optional[Set[str]]): If not None, undeploy only the specified devices.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
-        if not lab_hash and not lab_name:
-            raise InvocationError("You must specify a running network scenario hash or name.")
+        if not lab_hash and not lab_name and not lab:
+            raise InvocationError("You must specify a running network scenario hash, name or object.")
 
-        if lab_name:
+        if lab:
+            lab_hash = lab.hash
+        elif lab_name:
             lab_hash = utils.generate_urlsafe_hash(lab_name)
 
         self.docker_machine.undeploy(lab_hash, selected_machines=selected_machines)
 
         self.docker_link.undeploy(lab_hash)
 
     @privileged
@@ -287,23 +291,27 @@
         user_name = utils.get_current_user_name() if not all_users else None
 
         self.docker_machine.wipe(user=user_name)
         self.docker_link.wipe(user=user_name)
 
     @privileged
     def connect_tty(self, machine_name: str, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
-                    shell: str = None, logs: bool = False) -> None:
+                    shell: str = None, logs: bool = False, wait: Union[bool, Tuple[int, float]] = True) -> None:
         """Connect to a device in a running network scenario, using the specified shell.
 
         Args:
             machine_name (str): The name of the device to connect.
             lab_hash (str): The hash of the network scenario where the device is deployed.
             lab_name (str): The name of the network scenario where the device is deployed.
             shell (str): The name of the shell to use for connecting.
             logs (bool): If True, print startup logs on stdout.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before connecting. If a tuple is provided, the first value indicates the number of retries
+                before stopping waiting and the second value indicates the time interval to wait for each retry.
+                Default is True.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
@@ -315,42 +323,48 @@
 
         user_name = utils.get_current_user_name()
 
         self.docker_machine.connect(lab_hash=lab_hash,
                                     machine_name=machine_name,
                                     user=user_name,
                                     shell=shell,
-                                    logs=logs
+                                    logs=logs,
+                                    wait=wait
                                     )
 
     @privileged
-    def exec(self, machine_name: str, command: List[str], lab_hash: Optional[str] = None,
-             lab_name: Optional[str] = None) -> Generator[Tuple[bytes, bytes], None, None]:
+    def exec(self, machine_name: str, command: Union[List[str], str], lab_hash: Optional[str] = None,
+             lab_name: Optional[str] = None, wait: Union[bool, Tuple[int, float]] = False) \
+            -> Generator[Tuple[bytes, bytes], None, None]:
         """Exec a command on a device in a running network scenario.
 
         Args:
             machine_name (str): The name of the device to connect.
-            command (List[str]): The command to exec on the device.
+            command (Union[List[str], str]): The command to exec on the device.
             lab_hash (Optional[str]): The hash of the network scenario where the device is deployed.
             lab_name (Optional[str]): The name of the network scenario where the device is deployed.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before executing the command. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to wait
+                for each retry. Default is False.
 
         Returns:
             Generator[Tuple[bytes, bytes]]: A generator of tuples containing the stdout and stderr in bytes.
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
         if not lab_hash and not lab_name:
             raise InvocationError("You must specify a running network scenario hash or name.")
 
         user_name = utils.get_current_user_name()
         if lab_name:
             lab_hash = utils.generate_urlsafe_hash(lab_name)
 
-        return self.docker_machine.exec(lab_hash, machine_name, command, user=user_name, tty=False)
+        return self.docker_machine.exec(lab_hash, machine_name, command, user=user_name, tty=False, wait=wait)
 
     @privileged
     def copy_files(self, machine: Machine, guest_to_host: Dict[str, io.IOBase]) -> None:
         """Copy files on a running device in the specified paths.
 
         Args:
             machine (Kathara.model.Machine): A running device object. It must have the api_object field populated.
```

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/DockerPlugin.py` & `kathara-3.6.3/src/Kathara/manager/docker/DockerPlugin.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/stats/DockerLinkStats.py` & `kathara-3.6.3/src/Kathara/manager/docker/stats/DockerLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/stats/DockerMachineStats.py` & `kathara-3.6.3/src/Kathara/manager/docker/stats/DockerMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py` & `kathara-3.6.3/src/Kathara/manager/docker/terminal/DockerNPipeTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py` & `kathara-3.6.3/src/Kathara/manager/docker/terminal/DockerTTYTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfig.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesConfig.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesConfigMap.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesConfigMap.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesLink.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesMachine.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesMachine.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import shlex
 import sys
 import uuid
 from multiprocessing.dummy import Pool
 from typing import Optional, Set, List, Union, Generator, Tuple, Dict
 
+import chardet
 from kubernetes import client
 from kubernetes.client.api import apps_v1_api
 from kubernetes.client.api import core_v1_api
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import stream
 from kubernetes.watch import watch
 
@@ -25,15 +26,15 @@
 from ...model.Machine import Machine
 from ...setting.Setting import Setting
 
 RP_FILTER_NAMESPACE = "net.ipv4.conf.%s.rp_filter"
 MAX_RESTART_COUNT = 3
 
 # Known commands that each container should execute
-# Run order: shared.startup, machine.startup and machine.meta['startup_commands']
+# Run order: shared.startup, machine.startup and machine.meta['exec_commands']
 STARTUP_COMMANDS = [
     # If execution flag file is found, abort (this means that postStart has been called again)
     # If not flag the startup execution with a file
     "if [ -f \"/tmp/post_start\" ]; then exit; else touch /tmp/post_start; fi",
 
     "{sysctl_commands}",
 
@@ -49,34 +50,34 @@
     "base64 -d /tmp/kathara/hostlab.b64 > /hostlab.tar.gz",
     # Extract hostlab.tar.gz data into /
     "tar xmfz /hostlab.tar.gz -C /; rm -f hostlab.tar.gz",
 
     # Copy the machine folder (if present) from the hostlab directory into the root folder of the container
     # In this way, files are all replaced in the container root folder
     "if [ -d \"/hostlab/{machine_name}\" ]; then "
-    "(cd /hostlab/{machine_name} && tar c .) | (cd / && tar xhf -); fi",
+    "(cd /hostlab/{machine_name} && tar c .) | (cd / && tar xhf - --no-same-owner --no-same-permissions); fi",
 
     # If /etc/hosts is not configured by the user, add the localhost mapping
     "if [ ! -s \"/etc/hosts\" ]; then "
     "echo '127.0.0.1 localhost' > /etc/hosts",
     "echo '::1 localhost' >> /etc/hosts",
     "fi",
 
     # Give proper permissions to /var/www
     "if [ -d \"/var/www\" ]; then "
     "chmod -R 777 /var/www/*; fi",
 
     # Give proper permissions to Quagga files (if present)
     "if [ -d \"/etc/quagga\" ]; then "
-    "chown --recursive quagga:quagga /etc/quagga/",
+    "chown -R quagga:quagga /etc/quagga/",
     "chmod 640 /etc/quagga/*; fi",
 
     # Give proper permissions to FRR files (if present)
     "if [ -d \"/etc/frr\" ]; then "
-    "chown frr:frr /etc/frr/*",
+    "chown -R frr:frr /etc/frr/",
     "chmod 640 /etc/frr/*; fi",
 
     # If shared.startup file is present
     "if [ -f \"/hostlab/shared.startup\" ]; then "
     # Give execute permissions to the file and execute it
     # We redirect the output "&>" to a debugging file
     "chmod u+x /hostlab/shared.startup",
@@ -93,15 +94,17 @@
     "sed -i \"1s;^;set -x\\n\\n;\" /hostlab/{machine_name}.startup",
     "/hostlab/{machine_name}.startup &> /var/log/startup.log; fi",
 
     # Remove the Kubernetes' default gateway which points to the eth0 interface and causes problems sometimes.
     "route del default dev eth0 || true",
 
     # Placeholder for user commands
-    "{machine_commands}"
+    "{machine_commands}",
+
+    "touch /tmp/EOS"
 ]
 
 SHUTDOWN_COMMANDS = [
     # If machine.shutdown file is present
     "if [ -f \"/hostlab/{machine_name}.shutdown\" ]; then "
     # Give execute permissions to the file and execute it
     "chmod u+x /hostlab/{machine_name}.shutdown; /hostlab/{machine_name}.shutdown; fi",
@@ -258,14 +261,15 @@
         sysctl_parameters = {RP_FILTER_NAMESPACE % x: 0 for x in ["all", "default", "lo"]}
 
         sysctl_parameters["net.ipv4.ip_forward"] = 1
         sysctl_parameters["net.ipv4.icmp_ratelimit"] = 0
 
         if machine.is_ipv6_enabled():
             sysctl_parameters["net.ipv6.conf.all.forwarding"] = 1
+            sysctl_parameters["net.ipv6.conf.all.accept_ra"] = 0
             sysctl_parameters["net.ipv6.icmp.ratelimit"] = 0
             sysctl_parameters["net.ipv6.conf.default.disable_ipv6"] = 0
             sysctl_parameters["net.ipv6.conf.all.disable_ipv6"] = 0
 
         # Merge machine sysctls
         machine.meta['sysctls'] = {**sysctl_parameters, **machine.meta['sysctls']}
 
@@ -337,15 +341,15 @@
         # On Ready state, the pod has volumes and network interfaces up, so this hook is used
         # to execute custom commands coming from .startup file and "exec" option
         # Build the final startup commands string
         sysctl_commands = "; ".join(["sysctl -w -q %s=%d" % item for item in machine.meta["sysctls"].items()])
         startup_commands_string = "; ".join(STARTUP_COMMANDS) \
             .format(machine_name=machine.name,
                     sysctl_commands=sysctl_commands,
-                    machine_commands="; ".join(machine.meta['startup_commands'])
+                    machine_commands="; ".join(machine.meta['exec_commands'])
                     )
 
         post_start = client.V1LifecycleHandler(
             _exec=client.V1ExecAction(
                 command=[shell, "-c", startup_commands_string]
             )
         )
@@ -597,15 +601,18 @@
                                     machine_name,
                                     command="/bin/cat /var/log/shared.log /var/log/startup.log"
                                     )
             try:
                 print("--- Startup Commands Log\n")
                 while True:
                     (stdout, _) = next(exec_output)
-                    stdout = stdout.decode('utf-8') if stdout else ""
+
+                    char_encoding = chardet.detect(stdout) if stdout else None
+
+                    stdout = stdout.decode(char_encoding['encoding']) if stdout else ""
                     sys.stdout.write(stdout)
             except StopIteration:
                 print("\n--- End Startup Commands Log\n")
                 pass
 
         resp = stream(self.core_client.connect_get_namespaced_pod_exec,
                       name=deployment.metadata.name,
```

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesManager.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import json
 import logging
-from typing import Set, Dict, Generator, Any, List, Tuple, Optional
+from typing import Set, Dict, Generator, Any, List, Tuple, Optional, Union
 
 from kubernetes import client
 from kubernetes.client.rest import ApiException
 
 from .KubernetesConfig import KubernetesConfig
 from .KubernetesLink import KubernetesLink
 from .KubernetesMachine import KubernetesMachine
@@ -86,15 +86,15 @@
             None
 
         Raises:
             MachineNotFoundError: If the specified devices are not in the network scenario specified.
             LabAlreadyExistsError: If a network scenario is deployed while it is terminating its execution.
             ApiError: If the Kubernetes APIs throw an exception.
         """
-        if selected_machines and not lab.find_machines(selected_machines):
+        if selected_machines and not lab.has_machines(selected_machines):
             machines_not_in_lab = selected_machines - set(lab.machines.keys())
             raise MachineNotFoundError(f"The following devices are not in the network scenario: {machines_not_in_lab}.")
 
         # Kubernetes needs only lowercase letters for resources.
         # We force the hash to be lowercase
         lab.hash = lab.hash.lower()
 
@@ -213,35 +213,39 @@
             network_annotation = json.loads(running_machine.metadata.annotations["k8s.v1.cni.cncf.io/networks"])
             # If the collision domain to undeploy is still used, do nothing
             if network_name in [net['name'] for net in network_annotation]:
                 return
 
         self.k8s_link.undeploy(link.lab.hash, selected_links={network_name})
 
-    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
+    def undeploy_lab(self, lab_hash: Optional[str] = None, lab_name: Optional[str] = None, lab: Optional[Lab] = None,
                      selected_machines: Optional[Set[str]] = None) -> None:
         """Undeploy a Kathara network scenario.
 
         Args:
-            lab_hash (Optional[str]): The hash of the network scenario. Can be used as an alternative to lab_name.
-                If None, lab_name should be set.
-            lab_name (Optional[str]): The name of the network scenario. Can be used as an alternative to lab_hash.
-                If None, lab_hash should be set.
+            lab_hash (Optional[str]): The hash of the network scenario.
+                Can be used as an alternative to lab_name and lab. If None, lab_name or lab should be set.
+            lab_name (Optional[str]): The name of the network scenario.
+                Can be used as an alternative to lab_hash and lab. If None, lab_hash or lab should be set.
+            lab (Optional[Kathara.model.Lab]): The network scenario object.
+                Can be used as an alternative to lab_hash and lab_name. If None, lab_hash or lab_name should be set.
             selected_machines (Optional[Set[str]]): If not None, undeploy only the specified devices.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
-        if not lab_hash and not lab_name:
-            raise InvocationError("You must specify a running network scenario hash or name.")
+        if not lab_hash and not lab_name and not lab:
+            raise InvocationError("You must specify a running network scenario hash, name or object.")
 
-        if lab_name:
+        if lab:
+            lab_hash = lab.hash
+        elif lab_name:
             lab_hash = utils.generate_urlsafe_hash(lab_name)
 
         lab_hash = lab_hash.lower()
 
         # When only some machines should be undeployed, special checks are required.
         if selected_machines:
             # Get all current deployed networks and save only their name
@@ -293,23 +297,27 @@
         """
         if all_users:
             logging.warning("User-specific options have no effect on Megalos.")
 
         self.k8s_namespace.wipe()
 
     def connect_tty(self, machine_name: str, lab_hash: Optional[str] = None, lab_name: Optional[str] = None,
-                    shell: str = None, logs: bool = False) -> None:
+                    shell: str = None, logs: bool = False, wait: Union[bool, Tuple[int, float]] = True) -> None:
         """Connect to a device in a running network scenario, using the specified shell.
 
         Args:
             machine_name (str): The name of the device to connect.
             lab_hash (str): The hash of the network scenario where the device is deployed.
             lab_name (str): The name of the network scenario where the device is deployed.
             shell (str): The name of the shell to use for connecting.
             logs (bool): If True, print startup logs on stdout.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before connecting. If a tuple is provided, the first value indicates the number of retries
+                before stopping waiting and the second value indicates the time interval to wait for each retry.
+                Default is True. No effect on Kubernetes.
 
         Returns:
             None
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
@@ -323,33 +331,41 @@
 
         self.k8s_machine.connect(lab_hash=lab_hash,
                                  machine_name=machine_name,
                                  shell=shell,
                                  logs=logs
                                  )
 
-    def exec(self, machine_name: str, command: List[str], lab_hash: Optional[str] = None,
-             lab_name: Optional[str] = None) -> Generator[Tuple[bytes, bytes], None, None]:
+    def exec(self, machine_name: str, command: Union[List[str], str], lab_hash: Optional[str] = None,
+             lab_name: Optional[str] = None, wait: Union[bool, Tuple[int, float]] = False) \
+            -> Generator[Tuple[bytes, bytes], None, None]:
         """Exec a command on a device in a running network scenario.
 
         Args:
             machine_name (str): The name of the device to connect.
-            command (List[str]): The command to exec on the device.
+            command (Union[List[str], str]): The command to exec on the device.
             lab_hash (Optional[str]): The hash of the network scenario where the device is deployed.
             lab_name (Optional[str]): The name of the network scenario where the device is deployed.
+            wait (Union[bool, Tuple[int, float]]): If True, wait indefinitely until the end of the startup commands
+                execution before executing the command. If a tuple is provided, the first value indicates the
+                number of retries before stopping waiting and the second value indicates the time interval to wait
+                for each retry. Default is False. No effect on Kubernetes.
 
         Returns:
             Generator[Tuple[bytes, bytes]]: A generator of tuples containing the stdout and stderr in bytes.
 
         Raises:
             InvocationError: If a running network scenario hash or name is not specified.
         """
         if not lab_hash and not lab_name:
             raise InvocationError("You must specify a running network scenario hash or name.")
 
+        if wait:
+            logging.warning("Wait option has no effect on Megalos.")
+
         if lab_name:
             lab_hash = utils.generate_urlsafe_hash(lab_name)
 
         lab_hash = lab_hash.lower()
 
         return self.k8s_machine.exec(lab_hash, machine_name, command, stderr=True, tty=False, is_stream=True)
```

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/KubernetesNamespace.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/KubernetesNamespace.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/stats/KubernetesLinkStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/stats/KubernetesMachineStats.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py` & `kathara-3.6.3/src/Kathara/manager/kubernetes/terminal/KubernetesWSTerminal.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/model/ExternalLink.py` & `kathara-3.6.3/src/Kathara/model/ExternalLink.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/model/Lab.py` & `kathara-3.6.3/src/Kathara/model/Lab.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,14 +102,37 @@
         machine = self.get_or_new_machine(machine_name)
         link = self.get_or_new_link(link_name)
 
         machine.add_interface(link, number=machine_iface_number)
 
         return machine, link
 
+    def connect_machine_obj_to_link(self, machine: 'MachinePackage.Machine',
+                                    link_name: str, machine_iface_number: int = None) -> Tuple[Link, Optional[int]]:
+        """Connect the specified device object to the specified collision domain.
+
+        Args:
+            machine (Kathara.model.Machine): The device object.
+            link_name (str): The collision domain name.
+            machine_iface_number (int): The number of the device interface to connect. If it is None, the first free
+                number is used.
+
+        Returns:
+            Tuple[Kathara.model.Link, Optional[int]]: A tuple containing the collision domain and
+                the assigned interface number (if machine_iface_number is None).
+
+        Raises:
+            Exception: If an already used interface number is specified.
+        """
+        link = self.get_or_new_link(link_name)
+
+        machine_iface_number = machine.add_interface(link, number=machine_iface_number)
+
+        return link, machine_iface_number
+
     def assign_meta_to_machine(self, machine_name: str, meta_name: str, meta_value: str) -> Optional[Any]:
         """Assign meta information to the specified device.
 
         Args:
             machine_name (str): The name of the device.
             meta_name (str): The name of the meta property.
             meta_value (str): The value of the meta property.
@@ -149,27 +172,49 @@
 
         Returns:
             None
         """
         for machine in self.machines:
             self.machines[machine].check()
 
-    def get_links_from_machines(self, selected_machines: Union[List[str], Set[str]]) -> Set[str]:
-        """Return the name of the collision domains connected to the selected devices.
+    def get_links_from_machines(self, machines: Union[List[str], Set[str]]) -> Set[str]:
+        """Return the name of the collision domains connected to the devices.
 
         Args:
-            selected_machines (Set[str]): A set with selected devices names.
+            machines (Union[List[str], Set[str]]): A set or a list with selected devices names.
 
         Returns:
-            Set[str]: A set of names of collision domains to deploy.
+            Set[str]: A set of names of collision domains.
         """
         # Intersect selected machines names with self.machines keys
-        selected_machines = set(self.machines.keys()) & set(selected_machines)
+        machines = set(self.machines.keys()) & set(machines)
         # Apply filtering
-        machines = [v for (k, v) in self.machines.items() if k in selected_machines]
+        machines = [v for (k, v) in self.machines.items() if k in machines]
+
+        # Get only selected machines Link objects.
+        selected_links = set(chain.from_iterable([machine.interfaces.values() for machine in machines]))
+        selected_links = {link.name for link in selected_links}
+
+        return selected_links
+
+    def get_links_from_machine_objs(self,
+                                    machines: Union[List['MachinePackage.Machine'], Set['MachinePackage.Machine']]) -> \
+            Set[str]:
+        """Return the name of the collision domains connected to the devices.
+
+        Args:
+            machines (Union[List[str], Set[str]]): A set or a list with selected devices names.
+
+        Returns:
+            Set[str]: A set of names of collision domains.
+        """
+        # Intersect selected machines names with self.machines keys
+        machines = set(self.machines.keys()) & set(map(lambda x: x.name, machines))
+        # Apply filtering
+        machines = [v for (k, v) in self.machines.items() if k in machines]
 
         # Get only selected machines Link objects.
         selected_links = set(chain.from_iterable([machine.interfaces.values() for machine in machines]))
         selected_links = {link.name for link in selected_links}
 
         return selected_links
 
@@ -334,35 +379,57 @@
 
         Returns:
             None
         """
         if value is not None:
             self.general_options[name] = value
 
-    def find_machine(self, machine_name: str) -> bool:
+    def has_machine(self, machine_name: str) -> bool:
         """Check if the specified device is in the network scenario.
 
         Args:
             machine_name (str): The name of the device to search.
 
         Returns:
             bool: True if the device is in the network scenario, else False.
         """
         return machine_name in self.machines.keys()
 
-    def find_machines(self, machine_names: Set[str]) -> bool:
+    def has_machines(self, machine_names: Set[str]) -> bool:
         """Check if the specified devices are in the network scenario.
 
         Args:
             machine_names (Set[str]): A set of strings containing the names of the devices to search.
 
         Returns:
             bool: True if the devices are all in the network scenario, else False.
         """
-        return all(map(lambda x: self.find_machine(x), machine_names))
+        return all(map(lambda x: self.has_machine(x), machine_names))
+
+    def has_link(self, link_name: str) -> bool:
+        """Check if the specified collision domain is in the network scenario.
+
+        Args:
+            link_name (str): The name of the collision domain to search.
+
+        Returns:
+            bool: True if the collision domain is in the network scenario, else False.
+        """
+        return link_name in self.links.keys()
+
+    def has_links(self, link_names: Set[str]) -> bool:
+        """Check if the specified collision domains are in the network scenario.
+
+        Args:
+            link_names (Set[str]): A set of strings containing the names of the collision domains to search.
+
+        Returns:
+            bool: True if the collision domains are all in the network scenario, else False.
+        """
+        return all(map(lambda x: self.has_link(x), link_names))
 
     def __repr__(self) -> str:
         return "Lab(%s, %s, %s, %s)" % (self.fs, self.hash, self.machines, self.links)
 
     def __str__(self) -> str:
         lab_info = ""
```

### Comparing `kathara-3.6.2/src/Kathara/model/Link.py` & `kathara-3.6.3/src/Kathara/model/Link.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/model/Machine.py` & `kathara-3.6.3/src/Kathara/model/Machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,55 +60,59 @@
 
         self.lab: LabPackage.Lab = lab
         self.name: str = name
 
         self.interfaces: OrderedDict[int, Link] = collections.OrderedDict()
 
         self.meta: Dict[str, Any] = {
-            'startup_commands': [],
+            'exec_commands': [],
             'sysctls': {},
             'envs': {},
             'ports': {},
         }
 
         self.api_object: Any = None
 
         self.fs: FS = self.lab.fs.opendir(self.name) \
             if self.lab.fs.exists(self.name) and self.lab.fs.isdir(self.name) else None
 
         self.update_meta(kwargs)
 
-    def add_interface(self, link: 'LinkPackage.Link', number: int = None) -> None:
+    def add_interface(self, link: 'LinkPackage.Link', number: int = None) -> Optional[int]:
         """Add an interface to the device attached to the specified collision domain.
 
         Args:
             link (Kathara.model.Link): The Kathara collision domain to attach.
             number (int): The number of the new interface. If it is None, the first free number is selected.
 
         Returns:
-            None
+            Optional[int]: The number of the assigned interface if not passed, else None.
 
         Raises:
             MachineCollisionDomainConflictError: If the interface number specified is already used on the device.
             MachineCollisionDomainConflictError: If the device is already connected to the collision domain.
         """
+        had_number = True
         if number is None:
             number = len(self.interfaces.keys())
+            had_number = False
 
         if number in self.interfaces:
             raise MachineCollisionDomainError(f"Interface {number} already set on device `{self.name}`.")
 
         if self.name in link.machines:
             raise MachineCollisionDomainError(
                 f"Device `{self.name}` is already connected to collision domain `{link.name}`."
             )
 
         self.interfaces[number] = link
         link.machines[self.name] = self
 
+        return number if not had_number else None
+
     def remove_interface(self, link: 'LinkPackage.Link') -> None:
         """Disconnect the device from the specified collision domain.
 
         Args:
             link (Kathara.model.Link): The Kathara collision domain to disconnect.
 
         Returns:
@@ -137,34 +141,34 @@
         Returns:
             Optional[Any]: Previous value if meta was already assigned, None otherwise.
 
         Raises:
             MachineOptionError: If the specified value is not valid for the specified property.
         """
         if name == "exec":
-            self.meta['startup_commands'].append(value)
+            self.meta['exec_commands'].append(value)
             return None
 
         if name == "bridged":
             old_value = self.meta[name] if name in self.meta else None
             self.meta[name] = strtobool(str(value))
             return old_value
 
         if name == "sysctl":
-            matches = re.search(r"^(?P<key>net\.([\w-]+\.)+[\w-]+)=(?P<value>\w+)$", value)
+            matches = re.search(r"^(?P<key>net\.([\w-]+\.)+[\w-]+)=(?P<value>-?\w+)$", value)
 
             # Check for valid kv-pair
             if matches:
                 key = matches.group("key").strip()
                 val = matches.group("value").strip()
 
                 old_value = self.meta['sysctls'][key] if key in self.meta['sysctls'] else None
 
                 # Convert to int if possible
-                self.meta['sysctls'][key] = int(val) if val.isdigit() else val
+                self.meta['sysctls'][key] = int(val) if val.strip('-').isnumeric() else val
             else:
                 raise MachineOptionError(
                     "Invalid sysctl value (`%s`) on `%s`, missing `=` or value not in `net.` namespace."
                     % (value, self.name)
                 )
             return old_value
 
@@ -248,14 +252,20 @@
             for sysctl in args['sysctls']:
                 self.add_meta("sysctl", sysctl)
 
         if 'envs' in args and args['envs'] is not None:
             for envs in args['envs']:
                 self.add_meta("env", envs)
 
+        if 'ipv6' in args and args['ipv6'] is not None:
+            self.add_meta("ipv6", args['ipv6'])
+
+        if 'shell' in args and args['shell'] is not None:
+            self.add_meta("shell", args['shell'])
+
     def check(self) -> None:
         """Sort interfaces and check if there are missing interface numbers.
 
         Returns:
             None
 
         Raises:
@@ -306,21 +316,21 @@
         if not is_empty:
             file.seek(0)
             return file.read()
 
         # If no machine files are found, return None.
         return None
 
-    def get_startup_commands(self) -> List[str]:
-        """Get the additional device startup commands.
+    def get_exec_commands(self) -> List[str]:
+        """Get the device exec commands.
 
         Returns:
             List[str]: The list containing the additional commands.
         """
-        return self.meta['startup_commands']
+        return self.meta['exec_commands']
 
     def is_bridged(self) -> bool:
         """Return True if the device is bridged, else return False.
 
         Returns:
             bool: True if the device is bridged, else False.
         """
@@ -456,17 +466,23 @@
 
         Returns:
             bool: True if it is enabled, else False.
 
         Raises:
             MachineOptionError: If the IPv6 value specified is not valid.
         """
+        is_v6_enabled = Setting.get_instance().enable_ipv6
+
         try:
-            return strtobool(self.lab.general_options["ipv6"]) if "ipv6" in self.lab.general_options else \
-                strtobool(self.meta["ipv6"]) if "ipv6" in self.meta else Setting.get_instance().enable_ipv6
+            if "ipv6" in self.lab.general_options:
+                is_v6_enabled = self.lab.general_options["ipv6"]
+            elif "ipv6" in self.meta:
+                is_v6_enabled = self.meta["ipv6"]
+
+            return is_v6_enabled if type(is_v6_enabled) == bool else strtobool(is_v6_enabled)
         except ValueError:
             raise MachineOptionError("IPv6 value not valid on `%s`." % self.name)
 
     # Override FilesystemMixin methods to handle the condition if we want to add a file but self.fs is not set
     # In this case, we create the machine directory and assign it to self.fs before calling the actual method
     def create_file_from_string(self, content: str, dst_path: str) -> None:
         """Create a file from a string in the device fs. If fs is None, create it in the network scenario.
```

### Comparing `kathara-3.6.2/src/Kathara/os/Networking.py` & `kathara-3.6.3/src/Kathara/os/Networking.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/parser/netkit/DepParser.py` & `kathara-3.6.3/src/Kathara/parser/netkit/DepParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/parser/netkit/ExtParser.py` & `kathara-3.6.3/src/Kathara/parser/netkit/ExtParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/parser/netkit/FolderParser.py` & `kathara-3.6.3/src/Kathara/parser/netkit/FolderParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/parser/netkit/LabParser.py` & `kathara-3.6.3/src/Kathara/parser/netkit/LabParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/parser/netkit/OptionParser.py` & `kathara-3.6.3/src/Kathara/parser/netkit/OptionParser.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/setting/Setting.py` & `kathara-3.6.3/src/Kathara/setting/Setting.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/setting/addon/DockerSettingsAddon.py` & `kathara-3.6.3/src/Kathara/setting/addon/DockerSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/setting/addon/KubernetesSettingsAddon.py` & `kathara-3.6.3/src/Kathara/setting/addon/KubernetesSettingsAddon.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/strings.py` & `kathara-3.6.3/src/Kathara/strings.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/test/BuiltinTest.py` & `kathara-3.6.3/src/Kathara/test/BuiltinTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/test/UserTest.py` & `kathara-3.6.3/src/Kathara/test/UserTest.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/__init__.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/console_menu.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/console_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/__init__.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/__init__.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_borders.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_borders.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_margins.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_margins.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_padding.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_padding.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/format/menu_style.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/format/menu_style.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/command_item.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/command_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/external_item.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/external_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/function_item.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/function_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/selection_item.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/selection_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/items/submenu_item.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/items/submenu_item.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_component.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/menu_component.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/menu_formatter.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/menu_formatter.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/multiselect_menu.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/multiselect_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/prompt_utils.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/screen.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/screen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/selection_menu.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/selection_menu.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/base.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/base.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/regex.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/regex.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/consolemenu/validators/url.py` & `kathara-3.6.3/src/Kathara/trdparty/consolemenu/validators/url.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/curses/curses.py` & `kathara-3.6.3/src/Kathara/trdparty/curses/curses.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/depgen/depgen.py` & `kathara-3.6.3/src/Kathara/trdparty/depgen/depgen.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/libtmux/tmux.py` & `kathara-3.6.3/src/Kathara/trdparty/libtmux/tmux.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/trdparty/strtobool/strtobool.py` & `kathara-3.6.3/src/Kathara/trdparty/strtobool/strtobool.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/utils.py` & `kathara-3.6.3/src/Kathara/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import tarfile
 import tempfile
 from io import BytesIO
 from itertools import islice
 from multiprocessing import cpu_count
 from platform import node, machine
 from sys import platform as _platform
-from typing import Any, Optional, Match, Generator, List, Callable, Union, Dict, Iterable
 from types import ModuleType
+from typing import Any, Optional, Match, Generator, List, Callable, Union, Dict, Iterable
 
 from binaryornot.check import is_binary
 from slug import slug
 
 from .exceptions import HostArchitectureError
 
 # Platforms constants definition.
@@ -137,14 +137,27 @@
     return pywintypes
 
 
 def import_pywintypes() -> ModuleType:
     return exec_by_platform(pywintypes_import_stub, pywintypes_import_win, pywintypes_import_stub)
 
 
+def wait_user_input_linux() -> list:
+    """Non-blocking input function for Linux and macOS."""
+    import select
+    to_break, _, _ = select.select([sys.stdin], [], [], 0.1)
+    return to_break
+
+
+def wait_user_input_windows() -> bool:
+    """Return True if an Enter keypress is waiting to be read. Only for Windows."""
+    import msvcrt
+    return b'\r' in msvcrt.getch() if msvcrt.kbhit() else False
+
+
 # Architecture Test
 def get_architecture() -> str:
     architecture = machine().lower()
 
     logging.debug("Machine architecture is `%s`." % architecture)
 
     if architecture in ["x86_64", "amd64"]:
@@ -257,34 +270,14 @@
     p = math.pow(1024, i)
     s = round(size_bytes / p, 2)
 
     return "%s %s" % (s, size_name[i])
 
 
 # Lab Functions
-def get_lab_temp_path(lab_name: str, force_creation: bool = True) -> str:
-    def windows_path():
-        import win32file
-        return win32file.GetLongPathName(tempfile.gettempdir())
-
-    tempdir = exec_by_platform(tempfile.gettempdir,
-                               windows_path,
-                               lambda: re.sub(r"/+", "/", "/%s" % get_absolute_path("/tmp"))
-                               )
-    lab_temp_directory = os.path.join(tempdir, lab_name)
-    if not os.path.isdir(lab_temp_directory) and force_creation:
-        os.mkdir(lab_temp_directory)
-
-    return lab_temp_directory
-
-
-def get_vlab_temp_path(force_creation: bool = True) -> str:
-    return get_lab_temp_path("kathara_vlab", force_creation=force_creation)
-
-
 def pack_file_for_tar(file_obj: Union[str, io.IOBase], arc_name: str) -> (tarfile.TarInfo, bytes):
     if isinstance(file_obj, str):
         file_content_patched = convert_win_2_linux(file_obj)
         file_content = BytesIO(file_content_patched)
         filesize = len(file_content_patched)
     elif isinstance(file_obj, io.IOBase):
         file_content = file_obj.read()
```

### Comparing `kathara-3.6.2/src/Kathara/validator/ImageValidator.py` & `kathara-3.6.3/src/Kathara/validator/ImageValidator.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/webhooks/DockerHubApi.py` & `kathara-3.6.3/src/Kathara/webhooks/DockerHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/Kathara/webhooks/GitHubApi.py` & `kathara-3.6.3/src/Kathara/webhooks/GitHubApi.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/src/kathara.egg-info/PKG-INFO` & `kathara-3.6.3/src/kathara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kathara
-Version: 3.6.2
+Version: 3.6.3
 Summary: A lightweight container-based emulation system.
 Home-page: https://www.kathara.org
-Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.2.tar.gz
+Download-URL: https://github.com/KatharaFramework/Kathara/archive/refs/tags/3.6.3.tar.gz
 Author: Kathara Framework
 Author-email: Kathara Framework <contact@kathara.org>
 Maintainer-email: Tommaso Caiazzi <contact@kathara.org>, Mariano Scazzariello <contact@kathara.org>, Lorenzo Ariemma <contact@kathara.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `kathara-3.6.2/src/kathara.egg-info/SOURCES.txt` & `kathara-3.6.3/src/kathara.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 src/Kathara/cli/command/VcleanCommand.py
 src/Kathara/cli/command/VconfigCommand.py
 src/Kathara/cli/command/VstartCommand.py
 src/Kathara/cli/command/WipeCommand.py
 src/Kathara/cli/command/__init__.py
 src/Kathara/cli/ui/__init__.py
 src/Kathara/cli/ui/utils.py
+src/Kathara/cli/ui/event/HandleMachineTerminal.py
 src/Kathara/cli/ui/event/HandleProgressBar.py
-src/Kathara/cli/ui/event/OpenMachineTerminal.py
 src/Kathara/cli/ui/event/UpdateDockerImage.py
 src/Kathara/cli/ui/event/__init__.py
 src/Kathara/cli/ui/event/register.py
 src/Kathara/cli/ui/setting/CommonOptionsHandler.py
 src/Kathara/cli/ui/setting/DockerOptionsHandler.py
 src/Kathara/cli/ui/setting/KubernetesOptionsHandler.py
 src/Kathara/cli/ui/setting/SettingsMenuFactory.py
```

### Comparing `kathara-3.6.2/src/kathara.py` & `kathara-3.6.3/src/kathara.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/connect_command_test.py` & `kathara-3.6.3/tests/cli/connect_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/exec_command_test.py` & `kathara-3.6.3/tests/cli/exec_command_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                        mock_manager_get_instance, exec_output):
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.getcwd())
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     mock_stdout_write.assert_called_once_with('stdout')
     mock_stderr_write.assert_called_once_with('stderr')
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -49,15 +49,15 @@
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['-d', os.path.join('/test', 'path'), 'pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.path.abspath(os.path.join('/test', 'path')))
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     mock_stdout_write.assert_called_once_with('stdout')
     mock_stderr_write.assert_called_once_with('stderr')
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -69,15 +69,15 @@
                                           exec_output):
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['-d', os.path.join('test', 'path'), 'pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.path.join(os.getcwd(), 'test', 'path'))
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     mock_stdout_write.assert_called_once_with('stdout')
     mock_stderr_write.assert_called_once_with('stderr')
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -87,15 +87,15 @@
                            mock_manager_get_instance, exec_output):
     mock_manager_get_instance.return_value = mock_docker_manager
     lab = Lab('kathara_vlab')
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['-v', 'pc1', 'test command'])
     assert not mock_parse_lab.called
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=lab.hash, wait=False)
     mock_stdout_write.assert_called_once_with('stdout')
     mock_stderr_write.assert_called_once_with('stderr')
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -106,15 +106,15 @@
                        mock_manager_get_instance, exec_output):
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['--no-stdout', 'pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.getcwd())
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     assert not mock_stdout_write.called
     mock_stderr_write.assert_called_once_with('stderr')
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -125,15 +125,15 @@
                        mock_manager_get_instance, exec_output):
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['--no-stderr', 'pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.getcwd())
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     mock_stdout_write.assert_called_once_with('stdout')
     assert not mock_stderr_write.called
 
 
 @mock.patch("src.Kathara.manager.Kathara.Kathara.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerManager.DockerManager")
 @mock.patch("src.Kathara.parser.netkit.LabParser.LabParser.parse")
@@ -145,10 +145,10 @@
                                  exec_output):
     mock_parse_lab.return_value = mock_lab
     mock_manager_get_instance.return_value = mock_docker_manager
     mock_docker_manager.exec.return_value = exec_output
     command = ExecCommand()
     command.run('.', ['--no-stdout', '--no-stderr', 'pc1', 'test command'])
     mock_parse_lab.assert_called_once_with(os.getcwd())
-    mock_docker_manager.exec.assert_called_once_with("pc1", ['test command'], lab_hash=mock_lab.hash)
+    mock_docker_manager.exec.assert_called_once_with("pc1", 'test command', lab_hash=mock_lab.hash, wait=False)
     assert not mock_stdout_write.called
     assert not mock_stderr_write.called
```

### Comparing `kathara-3.6.2/tests/cli/lclean_command_test.py` & `kathara-3.6.3/tests/cli/lclean_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/lconfig_command_test.py` & `kathara-3.6.3/tests/cli/lconfig_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/linfo_command_test.py` & `kathara-3.6.3/tests/cli/linfo_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/list_command_test.py` & `kathara-3.6.3/tests/cli/list_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/lrestart_command_test.py` & `kathara-3.6.3/tests/cli/lrestart_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/lstart_command_test.py` & `kathara-3.6.3/tests/cli/lstart_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/vclean_command_test.py` & `kathara-3.6.3/tests/cli/vclean_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/vconfig_command_test.py` & `kathara-3.6.3/tests/cli/vconfig_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/cli/vstart_command_test.py` & `kathara-3.6.3/tests/cli/vstart_command_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/manager/docker/docker_image_test.py` & `kathara-3.6.3/tests/manager/docker/docker_image_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/manager/docker/docker_link_test.py` & `kathara-3.6.3/tests/manager/docker/docker_link_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/manager/docker/docker_machine_test.py` & `kathara-3.6.3/tests/manager/docker/docker_machine_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         network_mode='none',
         sysctls={'net.ipv4.conf.all.rp_filter': 0,
                  'net.ipv4.conf.default.rp_filter': 0,
                  'net.ipv4.conf.lo.rp_filter': 0,
                  'net.ipv4.ip_forward': 1,
                  'net.ipv4.icmp_ratelimit': 0,
                  'net.ipv6.conf.all.forwarding': 1,
+                 'net.ipv6.conf.all.accept_ra': 0,
                  'net.ipv6.icmp.ratelimit': 0,
                  'net.ipv6.conf.default.disable_ipv6': 0,
                  'net.ipv6.conf.all.disable_ipv6': 0
                  },
         environment={},
         mem_limit='64m',
         nano_cpus=2000000000,
@@ -173,14 +174,15 @@
     default_device.lab.add_option("privileged_machines", True)
     mock_get_current_user_name.return_value = "test-user"
     setting_mock = Mock()
     setting_mock.configure_mock(**{
         'shared_cd': False,
         'device_prefix': 'dev_prefix',
         "device_shell": '/bin/bash',
+        'enable_ipv6': True,
         "hosthome_mount": False,
         "shared_mount": False,
         'remote_url': None
     })
     mock_setting_get_instance.return_value = setting_mock
     docker_machine.create(default_device)
     docker_machine.client.containers.create.assert_called_once_with(
@@ -193,14 +195,15 @@
         network_mode='none',
         sysctls={'net.ipv4.conf.all.rp_filter': 0,
                  'net.ipv4.conf.default.rp_filter': 0,
                  'net.ipv4.conf.lo.rp_filter': 0,
                  'net.ipv4.ip_forward': 1,
                  'net.ipv4.icmp_ratelimit': 0,
                  'net.ipv6.conf.all.forwarding': 1,
+                 'net.ipv6.conf.all.accept_ra': 0,
                  'net.ipv6.icmp.ratelimit': 0,
                  'net.ipv6.conf.default.disable_ipv6': 0,
                  'net.ipv6.conf.all.disable_ipv6': 0},
         environment={},
         mem_limit='64m',
         nano_cpus=2000000000,
         ports=None,
@@ -277,16 +280,29 @@
     mock_create.assert_called_once()
     mock_start.assert_called_once()
 
 
 #
 # TEST: deploy_machines
 #
+@mock.patch("src.Kathara.setting.Setting.Setting.get_instance")
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine._deploy_and_start_machine")
-def test_deploy_machines(mock_deploy_and_start, docker_machine):
+def test_deploy_machines(mock_deploy_and_start, mock_setting_get_instance, docker_machine):
+    setting_mock = Mock()
+    setting_mock.configure_mock(**{
+        'shared_cd': False,
+        'device_prefix': 'dev_prefix',
+        "device_shell": '/bin/bash',
+        'enable_ipv6': False,
+        "hosthome_mount": False,
+        "shared_mount": False,
+        'remote_url': None
+    })
+    mock_setting_get_instance.return_value = setting_mock
+
     lab = Lab("Default scenario")
     lab.get_or_new_machine("pc1", **{'image': 'kathara/test1'})
     lab.get_or_new_machine("pc2", **{'image': 'kathara/test2'})
     docker_machine.docker_image.check_from_list.return_value = None
     mock_deploy_and_start.return_value = None
     docker_machine.deploy_machines(lab)
     docker_machine.docker_image.check_from_list.assert_called_once_with({'kathara/test1', 'kathara/test2'})
@@ -737,25 +753,25 @@
     default_device.api_object.remove.return_value = None
     default_device.api_object.status = "running"
 
     docker_machine._delete_machine(default_device.api_object)
     docker_machine.client.api.exec_create.assert_called_once()
     docker_machine.client.api.exec_start.assert_called_once()
     docker_machine.client.api.exec_inspect.assert_called_once()
-    default_device.api_object.remove.assert_called_once_with(force=True)
+    default_device.api_object.remove.assert_called_once_with(v=True, force=True)
 
 
 def test_delete_machine_not_running(docker_machine, default_device):
     default_device.api_object.exec_run.return_value = None
     default_device.api_object.remove.return_value = None
     default_device.api_object.status = "stop"
 
     docker_machine._delete_machine(default_device.api_object)
     assert not default_device.api_object.exec_run.called
-    default_device.api_object.remove.assert_called_once_with(force=True)
+    default_device.api_object.remove.assert_called_once_with(v=True, force=True)
 
 
 #
 # TEST: get_machines_stats
 #
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.get_machines_api_objects_by_filters")
 def test_get_machines_stats_lab_hash(mock_get_machines_api_objects_by_filters, docker_machine, default_device):
```

### Comparing `kathara-3.6.2/tests/manager/docker/docker_manager_test.py` & `kathara-3.6.3/tests/manager/docker/docker_manager_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -397,27 +397,73 @@
 
 #
 # TEST: undeploy_lab
 #
 @mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
 def test_undeploy_lab(mock_undeploy_machine, mock_undeploy_link, docker_manager):
-    docker_manager.undeploy_lab('lab_hash')
+    docker_manager.undeploy_lab(lab_hash='lab_hash')
     mock_undeploy_machine.assert_called_once_with('lab_hash', selected_machines=None)
     mock_undeploy_link.assert_called_once_with('lab_hash')
 
 
 @mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
 def test_undeploy_lab_selected_machines(mock_undeploy_machine, mock_undeploy_link, docker_manager):
-    docker_manager.undeploy_lab('lab_hash', selected_machines={'pc1', 'pc2'})
+    docker_manager.undeploy_lab(lab_hash='lab_hash', selected_machines={'pc1', 'pc2'})
     mock_undeploy_machine.assert_called_once_with('lab_hash', selected_machines={'pc1', 'pc2'})
     mock_undeploy_link.assert_called_once_with('lab_hash')
 
 
+@mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
+@mock.patch("src.Kathara.utils.generate_urlsafe_hash")
+def test_undeploy_lab_lab_name(mock_generate_urlsafe_hash, mock_undeploy_machine, mock_undeploy_link, docker_manager):
+    mock_generate_urlsafe_hash.return_value = "lab_hash"
+
+    docker_manager.undeploy_lab(lab_name='lab_name')
+    mock_undeploy_machine.assert_called_once_with('lab_hash', selected_machines=None)
+    mock_undeploy_link.assert_called_once_with('lab_hash')
+    mock_generate_urlsafe_hash.assert_called_once_with("lab_name")
+
+
+@mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
+@mock.patch("src.Kathara.utils.generate_urlsafe_hash")
+def test_undeploy_lab_lab_name_selected_machines(mock_generate_urlsafe_hash,
+                                                 mock_undeploy_machine, mock_undeploy_link, docker_manager):
+    mock_generate_urlsafe_hash.return_value = "lab_hash"
+
+    docker_manager.undeploy_lab(lab_name='lab_name', selected_machines={'pc1', 'pc2'})
+    mock_undeploy_machine.assert_called_once_with('lab_hash', selected_machines={'pc1', 'pc2'})
+    mock_undeploy_link.assert_called_once_with('lab_hash')
+    mock_generate_urlsafe_hash.assert_called_once_with("lab_name")
+
+
+@mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
+def test_undeploy_lab_lab_obj(mock_undeploy_machine, mock_undeploy_link, docker_manager, two_device_scenario):
+    expected_hash = two_device_scenario.hash
+
+    docker_manager.undeploy_lab(lab=two_device_scenario)
+    mock_undeploy_machine.assert_called_once_with(expected_hash, selected_machines=None)
+    mock_undeploy_link.assert_called_once_with(expected_hash)
+
+
+@mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.undeploy")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.undeploy")
+def test_undeploy_lab_lab_obj_selected_machines(mock_undeploy_machine, mock_undeploy_link, docker_manager,
+                                                two_device_scenario):
+    expected_hash = two_device_scenario.hash
+
+    docker_manager.undeploy_lab(lab=two_device_scenario, selected_machines={'pc1', 'pc2'})
+    mock_undeploy_machine.assert_called_once_with(expected_hash, selected_machines={'pc1', 'pc2'})
+    mock_undeploy_link.assert_called_once_with(expected_hash)
+
+
 #
 # TEST: wipe
 #
 @mock.patch("src.Kathara.manager.docker.DockerLink.DockerLink.wipe")
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.wipe")
 @mock.patch("src.Kathara.utils.get_current_user_name")
 def test_wipe(mock_get_current_user_name, mock_wipe_machines, mock_wipe_links, docker_manager):
@@ -464,14 +510,159 @@
     docker_manager.wipe(all_users=True)
     assert not mock_get_current_user_name.called
     mock_wipe_machines.assert_called_once_with(user=None)
     mock_wipe_links.assert_called_once_with(user=None)
 
 
 #
+# TEST: connect_tty
+#
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.connect")
+def test_connect_tty_lab_hash(mock_connect, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.connect_tty(default_device.name,
+                               lab_hash=default_device.lab.hash)
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash,
+                                         machine_name=default_device.name,
+                                         user="kathara_user",
+                                         shell=None,
+                                         logs=False,
+                                         wait=True)
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.connect")
+def test_connect_tty_lab_name(mock_connect, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.connect_tty(default_device.name,
+                               lab_name=default_device.lab.name)
+
+    mock_connect.assert_called_once_with(lab_hash=generate_urlsafe_hash(default_device.lab.name),
+                                         machine_name=default_device.name,
+                                         user="kathara_user",
+                                         shell=None,
+                                         logs=False,
+                                         wait=True)
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.connect")
+def test_connect_tty_with_custom_shell(mock_connect, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.connect_tty(default_device.name,
+                               lab_hash=default_device.lab.hash,
+                               shell="/usr/bin/zsh")
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash,
+                                         machine_name=default_device.name,
+                                         user="kathara_user",
+                                         shell="/usr/bin/zsh",
+                                         logs=False,
+                                         wait=True)
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.connect")
+def test_connect_tty_with_logs(mock_connect, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.connect_tty(default_device.name,
+                               lab_hash=default_device.lab.hash,
+                               logs=True)
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash,
+                                         machine_name=default_device.name,
+                                         user="kathara_user",
+                                         shell=None,
+                                         logs=True,
+                                         wait=True)
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.connect")
+def test_connect_tty_error(mock_connect, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    with pytest.raises(InvocationError):
+        docker_manager.connect_tty(default_device.name)
+
+    assert not mock_connect.called
+
+
+#
+# TEST: exec
+#
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.exec")
+def test_exec_lab_hash(mock_exec, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.exec(default_device.name, ["test", "command"], lab_hash=default_device.lab.hash)
+
+    mock_exec.assert_called_once_with(
+        default_device.lab.hash,
+        default_device.name,
+        ["test", "command"],
+        user="kathara_user",
+        tty=False,
+        wait=False
+    )
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.exec")
+def test_exec_lab_name(mock_exec, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.exec(default_device.name, ["test", "command"], lab_name=default_device.lab.name)
+
+    mock_exec.assert_called_once_with(
+        generate_urlsafe_hash(default_device.lab.name),
+        default_device.name,
+        ["test", "command"],
+        user="kathara_user",
+        tty=False,
+        wait=False
+    )
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.exec")
+def test_exec_wait(mock_exec, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    docker_manager.exec(default_device.name, ["test", "command"], lab_hash=default_device.lab.hash, wait=True)
+
+    mock_exec.assert_called_once_with(
+        default_device.lab.hash,
+        default_device.name,
+        ["test", "command"],
+        user="kathara_user",
+        tty=False,
+        wait=True
+    )
+
+
+@mock.patch("src.Kathara.utils.get_current_user_name")
+@mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.exec")
+def test_exec_invocation_error(mock_exec, mock_get_current_user_name, docker_manager, default_device):
+    mock_get_current_user_name.return_value = "kathara_user"
+
+    with pytest.raises(InvocationError):
+        docker_manager.exec(default_device.name, ["test", "command"])
+
+    assert not mock_exec.called
+
+
+#
 # TEST: get_machine_api_object
 #
 @mock.patch("src.Kathara.utils.get_current_user_name")
 @mock.patch("src.Kathara.manager.docker.DockerMachine.DockerMachine.get_machines_api_objects_by_filters")
 def test_get_machine_api_object_lab_hash_user(mock_get_machines_api_objects, mock_get_current_user_name,
                                               docker_manager, default_device):
     mock_get_machines_api_objects.return_value = [default_device.api_object]
```

### Comparing `kathara-3.6.2/tests/manager/docker/docker_plugin_test.py` & `kathara-3.6.3/tests/manager/docker/docker_plugin_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/manager/kubernetes/kubernetes_link_test.py` & `kathara-3.6.3/tests/manager/kubernetes/kubernetes_link_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/manager/kubernetes/kubernetes_machine_test.py` & `kathara-3.6.3/tests/manager/kubernetes/kubernetes_machine_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,14 +347,15 @@
 
     sysctl_commands = "; ".join(["sysctl -w -q %s=%d" % item for item in {'net.ipv4.conf.all.rp_filter': 0,
                                                                           'net.ipv4.conf.default.rp_filter': 0,
                                                                           'net.ipv4.conf.lo.rp_filter': 0,
                                                                           'net.ipv4.ip_forward': 1,
                                                                           'net.ipv4.icmp_ratelimit': 0,
                                                                           'net.ipv6.conf.all.forwarding': 1,
+                                                                          'net.ipv6.conf.all.accept_ra': 0,
                                                                           'net.ipv6.icmp.ratelimit': 0,
                                                                           'net.ipv6.conf.default.disable_ipv6': 0,
                                                                           'net.ipv6.conf.all.disable_ipv6': 0
                                                                           }.items()])
     startup_commands_string = "; ".join(STARTUP_COMMANDS) \
         .format(machine_name="test_device", sysctl_commands=sysctl_commands, machine_commands="ls")
```

### Comparing `kathara-3.6.2/tests/manager/kubernetes/kubernetes_manager_test.py` & `kathara-3.6.3/tests/manager/kubernetes/kubernetes_manager_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -449,14 +449,124 @@
     mock_get_machines_api_objects.assert_called_once_with(lab_hash='lab_hash')
     mock_undeploy_machine.assert_called_once_with('lab_hash', selected_machines={'pc1'})
     mock_undeploy_link.assert_called_once_with('lab_hash', selected_links={'netprefix-b'})
     assert not mock_namespace_undeploy.called
 
 
 #
+# TEST: connect_tty
+#
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.connect")
+def test_connect_tty_lab_hash(mock_connect, kubernetes_manager, default_device):
+    kubernetes_manager.connect_tty(default_device.name,
+                                   lab_hash=default_device.lab.hash)
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash.lower(),
+                                         machine_name=default_device.name,
+                                         shell=None,
+                                         logs=False)
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.connect")
+def test_connect_tty_lab_name(mock_connect, kubernetes_manager, default_device):
+    kubernetes_manager.connect_tty(default_device.name,
+                                   lab_name=default_device.lab.name)
+
+    mock_connect.assert_called_once_with(lab_hash=generate_urlsafe_hash(default_device.lab.name).lower(),
+                                         machine_name=default_device.name,
+                                         shell=None,
+                                         logs=False)
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.connect")
+def test_connect_tty_custom_shell(mock_connect, kubernetes_manager, default_device):
+    kubernetes_manager.connect_tty(default_device.name,
+                                   lab_hash=default_device.lab.hash,
+                                   shell='/usr/bin/zsh')
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash.lower(),
+                                         machine_name=default_device.name,
+                                         shell='/usr/bin/zsh',
+                                         logs=False)
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.connect")
+def test_connect_tty_with_logs(mock_connect, kubernetes_manager, default_device):
+    kubernetes_manager.connect_tty(default_device.name,
+                                   lab_hash=default_device.lab.hash,
+                                   logs=True)
+
+    mock_connect.assert_called_once_with(lab_hash=default_device.lab.hash.lower(),
+                                         machine_name=default_device.name,
+                                         shell=None,
+                                         logs=True)
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.connect")
+def test_connect_tty_invocation_error(mock_connect, kubernetes_manager, default_device):
+    with pytest.raises(InvocationError):
+        kubernetes_manager.connect_tty(default_device.name)
+
+    assert not mock_connect.called
+
+
+#
+# TEST: exec
+#
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.exec")
+def test_exec_lab_hash(mock_exec, kubernetes_manager, default_device):
+    kubernetes_manager.exec(default_device.name, ["test", "command"], lab_hash=default_device.lab.hash)
+
+    mock_exec.assert_called_once_with(
+        default_device.lab.hash.lower(),
+        default_device.name,
+        ["test", "command"],
+        stderr=True,
+        tty=False,
+        is_stream=True
+    )
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.exec")
+def test_exec_lab_name(mock_exec, kubernetes_manager, default_device):
+    kubernetes_manager.exec(default_device.name, ["test", "command"], lab_name=default_device.lab.name)
+
+    mock_exec.assert_called_once_with(
+        generate_urlsafe_hash(default_device.lab.name).lower(),
+        default_device.name,
+        ["test", "command"],
+        stderr=True,
+        tty=False,
+        is_stream=True
+    )
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.exec")
+def test_exec_wait(mock_exec, kubernetes_manager, default_device):
+    kubernetes_manager.exec(default_device.name, ["test", "command"], lab_hash=default_device.lab.hash, wait=True)
+
+    mock_exec.assert_called_once_with(
+        default_device.lab.hash.lower(),
+        default_device.name,
+        ["test", "command"],
+        stderr=True,
+        tty=False,
+        is_stream=True
+    )
+
+
+@mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.exec")
+def test_exec_invocation_error(mock_exec, kubernetes_manager, default_device):
+    with pytest.raises(InvocationError):
+        kubernetes_manager.exec(default_device.name, ["test", "command"])
+
+    assert not mock_exec.called
+
+
+#
 # TEST: get_machine_api_objects
 #
 @mock.patch("src.Kathara.manager.kubernetes.KubernetesMachine.KubernetesMachine.get_machines_api_objects_by_filters")
 def test_get_machine_api_object_lab_hash(mock_get_machines_api_objects, kubernetes_manager, default_device):
     default_device.api_object.name = "default_device"
     mock_get_machines_api_objects.return_value = [default_device.api_object]
     kubernetes_manager.get_machine_api_object(machine_name="default_device", lab_hash="lab_hash_value")
```

### Comparing `kathara-3.6.2/tests/model/external_link_test.py` & `kathara-3.6.3/tests/model/external_link_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     assert external_link_vlan.interface == "eth0"
     assert external_link_vlan.vlan == 1
 
 
 def test_get_name_and_vlan(external_link_vlan):
     interface, vlan = external_link_vlan.get_name_and_vlan()
     assert interface == "eth0"
-    assert vlan is 1
+    assert vlan == 1
 
 
 def test_get_name_and_vlan_no_vlan(external_link_no_vlan):
     interface, vlan = external_link_no_vlan.get_name_and_vlan()
     assert interface == "eth0"
     assert vlan is None
 
 
 def test_get_name_and_vlan_long_name():
     external_link = ExternalLink("long-interface-name", 1)
     interface, vlan = external_link.get_name_and_vlan()
     # If the length of interface name + vlan tag is more than 15 chars, we truncate the interface name to
     # 15 - VLAN_NAME_LENGTH in order to fit the whole string in 15 chars
     assert interface == "long-interfac"
-    assert vlan is 1
+    assert vlan == 1
 
 
 def test_full_name(external_link_vlan):
     full_name = external_link_vlan.get_full_name()
     assert full_name == "eth0.1"
```

### Comparing `kathara-3.6.2/tests/model/filesystem_mixin_test.py` & `kathara-3.6.3/tests/model/filesystem_mixin_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/model/lab_test.py` & `kathara-3.6.3/tests/model/lab_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -195,14 +195,80 @@
     assert default_scenario.links['B']
     assert default_scenario.machines['pc1'].interfaces[0].name == 'A'
     assert default_scenario.machines['pc1'].interfaces[1].name == 'B'
     assert result_1 == (default_scenario.machines['pc1'], default_scenario.links['A'])
     assert result_2 == (default_scenario.machines['pc1'], default_scenario.links['B'])
 
 
+def test_connect_machine_to_link_iface_numbers(default_scenario: Lab):
+    result_1 = default_scenario.connect_machine_to_link("pc1", "A", machine_iface_number=2)
+    assert len(default_scenario.machines) == 1
+    assert default_scenario.machines['pc1']
+    assert len(default_scenario.links) == 1
+    assert default_scenario.links['A']
+    assert default_scenario.machines['pc1'].interfaces[2].name == 'A'
+    assert result_1 == (default_scenario.machines['pc1'], default_scenario.links['A'])
+
+
+def test_connect_one_machine_obj_to_link(default_scenario: Lab):
+    pc1 = default_scenario.new_machine("pc1")
+    result_1 = default_scenario.connect_machine_obj_to_link(pc1, "A")
+    assert len(default_scenario.machines) == 1
+    assert default_scenario.machines['pc1']
+    assert len(default_scenario.links) == 1
+    assert default_scenario.links['A']
+    assert default_scenario.machines['pc1'].interfaces[0].name == 'A'
+    assert result_1 == (default_scenario.links['A'], 0)
+
+
+def test_connect_two_machine_obj_to_link(default_scenario: Lab):
+    pc1 = default_scenario.new_machine("pc1")
+    result_1 = default_scenario.connect_machine_obj_to_link(pc1, "A")
+    assert len(default_scenario.machines) == 1
+    assert default_scenario.machines['pc1']
+    assert len(default_scenario.links) == 1
+    assert default_scenario.links['A']
+    pc2 = default_scenario.new_machine("pc2")
+    result_2 = default_scenario.connect_machine_obj_to_link(pc2, "A")
+    assert len(default_scenario.machines) == 2
+    assert default_scenario.machines['pc2']
+    assert len(default_scenario.links) == 1
+    assert default_scenario.links['A']
+    assert default_scenario.machines['pc1'].interfaces[0].name == 'A'
+    assert default_scenario.machines['pc2'].interfaces[0].name == 'A'
+    assert result_1 == (default_scenario.links['A'], 0)
+    assert result_2 == (default_scenario.links['A'], 0)
+
+
+def test_connect_machine_obj_to_two_links(default_scenario: Lab):
+    pc1 = default_scenario.new_machine("pc1")
+    result_1 = default_scenario.connect_machine_obj_to_link(pc1, "A")
+    result_2 = default_scenario.connect_machine_obj_to_link(pc1, "B")
+    assert len(default_scenario.machines) == 1
+    assert default_scenario.machines['pc1']
+    assert len(default_scenario.links) == 2
+    assert default_scenario.links['A']
+    assert default_scenario.links['B']
+    assert default_scenario.machines['pc1'].interfaces[0].name == 'A'
+    assert default_scenario.machines['pc1'].interfaces[1].name == 'B'
+    assert result_1 == (default_scenario.links['A'], 0)
+    assert result_2 == (default_scenario.links['B'], 1)
+
+
+def test_connect_machine_obj_to_link_iface_numbers(default_scenario: Lab):
+    pc1 = default_scenario.new_machine("pc1")
+    result_1 = default_scenario.connect_machine_obj_to_link(pc1, "A", machine_iface_number=2)
+    assert len(default_scenario.machines) == 1
+    assert default_scenario.machines['pc1']
+    assert len(default_scenario.links) == 1
+    assert default_scenario.links['A']
+    assert default_scenario.machines['pc1'].interfaces[2].name == 'A'
+    assert result_1 == (default_scenario.links['A'], None)
+
+
 def test_assign_meta_to_machine(default_scenario: Lab):
     default_scenario.get_or_new_machine("pc1")
     result = default_scenario.assign_meta_to_machine("pc1", "test_meta", "test_value")
     assert "test_meta" in default_scenario.machines['pc1'].meta
     assert default_scenario.machines['pc1'].meta["test_meta"] == "test_value"
     assert result is None
 
@@ -256,15 +322,28 @@
 
 
 def test_intersect_machines(default_scenario: Lab):
     default_scenario.connect_machine_to_link("pc1", "A")
     default_scenario.connect_machine_to_link("pc2", "A")
     default_scenario.connect_machine_to_link("pc2", "B")
     assert len(default_scenario.machines) == 2
-    links = default_scenario.get_links_from_machines(selected_machines=["pc1"])
+    links = default_scenario.get_links_from_machines(machines=["pc1"])
+    assert len(default_scenario.machines) == 2
+    assert 'pc1' in default_scenario.machines
+    assert 'pc2' in default_scenario.machines
+    assert 'A' in links
+    assert 'B' not in links
+
+
+def test_intersect_machines_objs(default_scenario: Lab):
+    default_scenario.connect_machine_to_link("pc1", "A")
+    default_scenario.connect_machine_to_link("pc2", "A")
+    default_scenario.connect_machine_to_link("pc2", "B")
+    assert len(default_scenario.machines) == 2
+    links = default_scenario.get_links_from_machine_objs(machines=[default_scenario.get_machine("pc1")])
     assert len(default_scenario.machines) == 2
     assert 'pc1' in default_scenario.machines
     assert 'pc2' in default_scenario.machines
     assert 'A' in links
     assert 'B' not in links
 
 
@@ -288,29 +367,29 @@
     assert default_scenario.machines.popitem()[0] == "pc1"
     assert default_scenario.machines.popitem()[0] == "pc3"
 
 
 def test_find_machine_true(default_scenario: Lab):
     default_scenario.get_or_new_machine("pc1")
 
-    assert default_scenario.find_machine("pc1")
+    assert default_scenario.has_machine("pc1")
 
 
 def test_find_machine_false(default_scenario: Lab):
     default_scenario.get_or_new_machine("pc1")
 
-    assert not default_scenario.find_machine("pc2")
+    assert not default_scenario.has_machine("pc2")
 
 
 def test_find_machines_true(default_scenario: Lab):
     default_scenario.get_or_new_machine("pc1")
     default_scenario.get_or_new_machine("pc2")
     default_scenario.get_or_new_machine("pc3")
 
-    assert default_scenario.find_machines({"pc1", "pc2", "pc3"})
+    assert default_scenario.has_machines({"pc1", "pc2", "pc3"})
 
 
 def test_find_machines_false(default_scenario: Lab):
     default_scenario.get_or_new_machine("pc1")
     default_scenario.get_or_new_machine("pc2")
 
-    assert not default_scenario.find_machines({"pc1", "pc2", "pc3"})
+    assert not default_scenario.has_machines({"pc1", "pc2", "pc3"})
```

### Comparing `kathara-3.6.2/tests/model/machine_test.py` & `kathara-3.6.3/tests/model/machine_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,31 +21,39 @@
     return Machine(Lab("test_lab"), "test_machine")
 
 
 def test_default_device_parameters(default_device: Machine):
     assert default_device.name == "test_machine"
     assert len(default_device.interfaces) == 0
     assert default_device.meta == {
-        'startup_commands': [],
+        'exec_commands': [],
         'sysctls': {},
         'envs': {},
         'ports': {},
     }
     assert default_device.api_object is None
     assert default_device.fs is None
     assert not default_device.lab.has_host_path()
 
 
 #
 # TEST: add_interface
 #
 def test_add_interface(default_device: Machine):
-    default_device.add_interface(Link(default_device.lab, "A"))
+    result = default_device.add_interface(Link(default_device.lab, "A"))
     assert len(default_device.interfaces) == 1
     assert default_device.interfaces[0].name == "A"
+    assert result == 0
+
+
+def test_add_interface_with_number(default_device: Machine):
+    result = default_device.add_interface(Link(default_device.lab, "A"), number=2)
+    assert len(default_device.interfaces) == 1
+    assert default_device.interfaces[2].name == "A"
+    assert result is None
 
 
 def test_add_interface_exception(default_device: Machine):
     default_device.add_interface(Link(default_device.lab, "A"))
     with pytest.raises(MachineCollisionDomainError):
         default_device.add_interface(Link(default_device.lab, "B"), number=0)
 
@@ -136,14 +144,29 @@
 
 
 def test_add_meta_sysctl_not_format_exception(default_device: Machine):
     with pytest.raises(MachineOptionError):
         default_device.add_meta("sysctl", "kernel.shm_rmid_forced")
 
 
+def test_add_meta_sysctl_non_numeric(default_device: Machine):
+    default_device.add_meta("sysctl", "net.test_sysctl.text=test")
+    assert default_device.meta['sysctls']['net.test_sysctl.text'] == "test"
+
+
+def test_add_meta_sysctl_negative_number(default_device: Machine):
+    default_device.add_meta("sysctl", "net.test_sysctl.negative=-1")
+    assert default_device.meta['sysctls']['net.test_sysctl.negative'] == -1
+
+
+def test_add_meta_sysctl_negative_number_not_format(default_device: Machine):
+    with pytest.raises(MachineOptionError):
+        default_device.add_meta("sysctl", "net.test_sysctl.negative=-1-")
+
+
 def test_add_meta_env(default_device: Machine):
     default_device.add_meta("env", "MY_ENV_VAR=test")
     assert default_device.meta['envs']['MY_ENV_VAR'] == "test"
 
 
 def test_add_meta_env_number(default_device: Machine):
     default_device.add_meta("env", "MY_ENV_VAR=1")
@@ -324,7 +347,40 @@
     lab = Lab('mem_test')
     lab.add_option("num_terms", "2")
     kwargs = {"num_terms": "1"}
     device1 = Machine(lab, "test_machine1", **kwargs)
     device2 = Machine(lab, "test_machine2")
     assert device1.get_num_terms() == 2
     assert device2.get_num_terms() == 2
+
+
+#
+# TEST: is_ipv6_enabled
+#
+def test_is_ipv6_enabled_from_lab_options():
+    lab = Lab('mem_test')
+    lab.add_option("ipv6", True)
+    device = Machine(lab, "test_machine")
+    assert device.is_ipv6_enabled()
+
+
+def test_is_ipv6_enabled_from_device_meta_bool():
+    kwargs = {"ipv6": True}
+    device = Machine(Lab("test_lab"), "test_machine", **kwargs)
+    assert device.is_ipv6_enabled()
+
+
+def test_is_ipv6_enabled_from_device_meta_str():
+    kwargs = {"ipv6": "True"}
+    device = Machine(Lab("test_lab"), "test_machine", **kwargs)
+    assert device.is_ipv6_enabled()
+
+
+def test_is_ipv6_enabled_mix():
+    # Lab options have a greater priority than machine options
+    lab = Lab('mem_test')
+    lab.add_option("ipv6", False)
+    kwargs = {"ipv6": True}
+    device1 = Machine(lab, "test_machine1", **kwargs)
+    device2 = Machine(lab, "test_machine2")
+    assert not device1.is_ipv6_enabled()
+    assert not device2.is_ipv6_enabled()
```

### Comparing `kathara-3.6.2/tests/parser/dep_parser_test.py` & `kathara-3.6.3/tests/parser/dep_parser_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/parser/ext_parser_test.py` & `kathara-3.6.3/tests/parser/ext_parser_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/parser/folder_parser_test.py` & `kathara-3.6.3/tests/parser/folder_parser_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/parser/lab_parser_test.py` & `kathara-3.6.3/tests/parser/lab_parser_test.py`

 * *Files identical despite different names*

### Comparing `kathara-3.6.2/tests/parser/option_parser_test.py` & `kathara-3.6.3/tests/parser/option_parser_test.py`

 * *Files identical despite different names*

