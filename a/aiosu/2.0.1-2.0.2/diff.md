# Comparing `tmp/aiosu-2.0.1.tar.gz` & `tmp/aiosu-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosu-2.0.1.tar", max compression
+gzip compressed data, was "aiosu-2.0.2.tar", max compression
```

## Comparing `aiosu-2.0.1.tar` & `aiosu-2.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    35149 2023-07-18 23:59:54.919847 aiosu-2.0.1/LICENSE
--rw-r--r--   0        0        0     3860 2023-07-18 23:59:54.919847 aiosu-2.0.1/README.rst
--rw-r--r--   0        0        0      675 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/__init__.py
--rw-r--r--   0        0        0     2318 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/events.py
--rw-r--r--   0        0        0      736 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/exceptions.py
--rw-r--r--   0        0        0     1790 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/helpers.py
--rw-r--r--   0        0        0      664 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/__init__.py
--rw-r--r--   0        0        0     1149 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/artist.py
--rw-r--r--   0        0        0      406 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/backgrounds.py
--rw-r--r--   0        0        0      889 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/base.py
--rw-r--r--   0        0        0    14988 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/beatmap.py
--rw-r--r--   0        0        0     2175 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/changelog.py
--rw-r--r--   0        0        0     1746 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/chat.py
--rw-r--r--   0        0        0     1652 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/comment.py
--rw-r--r--   0        0        0     2545 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/common.py
--rw-r--r--   0        0        0     1715 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/event.py
--rw-r--r--   0        0        0     1696 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/forum.py
--rw-r--r--   0        0        0     1976 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/gamemode.py
--rw-r--r--   0        0        0      763 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/kudosu.py
--rw-r--r--   0        0        0     5638 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/lazer.py
--rw-r--r--   0        0        0       79 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/legacy/__init__.py
--rw-r--r--   0        0        0     3358 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/legacy/match.py
--rw-r--r--   0        0        0      272 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/legacy/replay.py
--rw-r--r--   0        0        0     6536 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/mods.py
--rw-r--r--   0        0        0     4610 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/multiplayer.py
--rw-r--r--   0        0        0     1074 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/news.py
--rw-r--r--   0        0        0     1941 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/oauthtoken.py
--rw-r--r--   0        0        0      843 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/performance.py
--rw-r--r--   0        0        0      693 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/rankings.py
--rw-r--r--   0        0        0     2855 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/replay.py
--rw-r--r--   0        0        0     1241 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/scopes.py
--rw-r--r--   0        0        0     7800 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/score.py
--rw-r--r--   0        0        0      494 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/search.py
--rw-r--r--   0        0        0      394 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/spotlight.py
--rw-r--r--   0        0        0    10151 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/user.py
--rw-r--r--   0        0        0      386 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/models/wiki.py
--rw-r--r--   0        0        0      241 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/__init__.py
--rw-r--r--   0        0        0     8815 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/accuracy.py
--rw-r--r--   0        0        0     2941 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/auth.py
--rw-r--r--   0        0        0     7905 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/binary.py
--rw-r--r--   0        0        0    22091 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/performance.py
--rw-r--r--   0        0        0     6182 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/utils/replay.py
--rw-r--r--   0        0        0      106 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v1/__init__.py
--rw-r--r--   0        0        0    17958 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v1/client.py
--rw-r--r--   0        0        0      154 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v2/__init__.py
--rw-r--r--   0        0        0    90367 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v2/client.py
--rw-r--r--   0        0        0     7691 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v2/clientstorage.py
--rw-r--r--   0        0        0      103 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v2/repository/__init__.py
--rw-r--r--   0        0        0     1905 2023-07-18 23:59:54.919847 aiosu-2.0.1/aiosu/v2/repository/oauthtoken.py
--rw-r--r--   0        0        0        0 2023-07-18 23:59:54.923847 aiosu-2.0.1/py.typed
--rw-r--r--   0        0        0     1816 2023-07-18 23:59:54.923847 aiosu-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 aiosu-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-04-17 12:28:56.829150 aiosu-2.0.2/aiosu/__init__.py
+-rw-r--r--   0        0        0     2410 2023-04-17 12:28:56.829150 aiosu-2.0.2/aiosu/events.py
+-rw-r--r--   0        0        0      767 2023-04-17 12:28:56.829150 aiosu-2.0.2/aiosu/exceptions.py
+-rw-r--r--   0        0        0     1856 2023-04-17 12:28:56.829150 aiosu-2.0.2/aiosu/helpers.py
+-rw-r--r--   0        0        0      695 2023-04-17 12:28:56.829150 aiosu-2.0.2/aiosu/models/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-18 22:52:49.245173 aiosu-2.0.2/aiosu/models/artist.py
+-rw-r--r--   0        0        0      430 2023-04-17 12:28:56.830150 aiosu-2.0.2/aiosu/models/backgrounds.py
+-rw-r--r--   0        0        0      926 2023-07-18 23:59:07.561529 aiosu-2.0.2/aiosu/models/base.py
+-rw-r--r--   0        0        0    16229 2023-07-20 07:34:35.921907 aiosu-2.0.2/aiosu/models/beatmap.py
+-rw-r--r--   0        0        0     2271 2023-07-18 22:52:49.246249 aiosu-2.0.2/aiosu/models/changelog.py
+-rw-r--r--   0        0        0     1832 2023-07-18 22:52:49.246249 aiosu-2.0.2/aiosu/models/chat.py
+-rw-r--r--   0        0        0     1718 2023-07-18 22:52:49.246773 aiosu-2.0.2/aiosu/models/comment.py
+-rw-r--r--   0        0        0     3184 2023-07-20 07:30:19.222005 aiosu-2.0.2/aiosu/models/common.py
+-rw-r--r--   0        0        0     1791 2023-07-18 22:52:49.247301 aiosu-2.0.2/aiosu/models/event.py
+-rw-r--r--   0        0        0     1780 2023-07-18 22:52:49.247301 aiosu-2.0.2/aiosu/models/forum.py
+-rw-r--r--   0        0        0     2068 2023-04-17 12:28:56.832151 aiosu-2.0.2/aiosu/models/gamemode.py
+-rw-r--r--   0        0        0      809 2023-07-18 22:52:49.247301 aiosu-2.0.2/aiosu/models/kudosu.py
+-rw-r--r--   0        0        0     5861 2023-07-18 22:52:49.248287 aiosu-2.0.2/aiosu/models/lazer.py
+-rw-r--r--   0        0        0       83 2023-04-17 12:28:56.832151 aiosu-2.0.2/aiosu/models/legacy/__init__.py
+-rw-r--r--   0        0        0     3503 2023-07-18 22:52:49.248287 aiosu-2.0.2/aiosu/models/legacy/match.py
+-rw-r--r--   0        0        0      286 2023-04-17 12:28:56.833149 aiosu-2.0.2/aiosu/models/legacy/replay.py
+-rw-r--r--   0        0        0     6799 2023-07-18 22:52:49.248287 aiosu-2.0.2/aiosu/models/mods.py
+-rw-r--r--   0        0        0     4793 2023-07-18 22:52:49.249288 aiosu-2.0.2/aiosu/models/multiplayer.py
+-rw-r--r--   0        0        0     1132 2023-07-18 22:52:49.249288 aiosu-2.0.2/aiosu/models/news.py
+-rw-r--r--   0        0        0     2011 2023-07-20 08:01:30.051968 aiosu-2.0.2/aiosu/models/oauthtoken.py
+-rw-r--r--   0        0        0      885 2023-04-17 12:28:56.834150 aiosu-2.0.2/aiosu/models/performance.py
+-rw-r--r--   0        0        0      724 2023-07-18 22:52:49.250288 aiosu-2.0.2/aiosu/models/rankings.py
+-rw-r--r--   0        0        0     2982 2023-07-18 22:52:49.250288 aiosu-2.0.2/aiosu/models/replay.py
+-rw-r--r--   0        0        0     1292 2023-04-17 12:46:45.065824 aiosu-2.0.2/aiosu/models/scopes.py
+-rw-r--r--   0        0        0     8060 2023-07-18 22:52:49.251288 aiosu-2.0.2/aiosu/models/score.py
+-rw-r--r--   0        0        0      520 2023-07-18 22:52:49.251288 aiosu-2.0.2/aiosu/models/search.py
+-rw-r--r--   0        0        0      415 2023-07-18 22:52:49.251288 aiosu-2.0.2/aiosu/models/spotlight.py
+-rw-r--r--   0        0        0    10500 2023-07-18 22:52:49.251288 aiosu-2.0.2/aiosu/models/user.py
+-rw-r--r--   0        0        0      408 2023-07-18 22:52:49.252287 aiosu-2.0.2/aiosu/models/wiki.py
+-rw-r--r--   0        0        0      253 2023-04-17 12:28:56.836150 aiosu-2.0.2/aiosu/utils/__init__.py
+-rw-r--r--   0        0        0     9105 2023-04-17 12:28:56.836150 aiosu-2.0.2/aiosu/utils/accuracy.py
+-rw-r--r--   0        0        0     3038 2023-07-18 22:52:49.252287 aiosu-2.0.2/aiosu/utils/auth.py
+-rw-r--r--   0        0        0     8250 2023-04-17 12:28:56.836150 aiosu-2.0.2/aiosu/utils/binary.py
+-rw-r--r--   0        0        0    22765 2023-04-17 12:28:56.837151 aiosu-2.0.2/aiosu/utils/performance.py
+-rw-r--r--   0        0        0     6372 2023-07-18 22:52:49.252287 aiosu-2.0.2/aiosu/utils/replay.py
+-rw-r--r--   0        0        0      112 2023-04-17 12:28:56.837151 aiosu-2.0.2/aiosu/v1/__init__.py
+-rw-r--r--   0        0        0    18438 2023-07-18 22:52:49.253288 aiosu-2.0.2/aiosu/v1/client.py
+-rw-r--r--   0        0        0      161 2023-04-17 12:28:56.838151 aiosu-2.0.2/aiosu/v2/__init__.py
+-rw-r--r--   0        0        0    92758 2023-07-20 08:01:57.239180 aiosu-2.0.2/aiosu/v2/client.py
+-rw-r--r--   0        0        0     7929 2023-04-17 12:28:56.839148 aiosu-2.0.2/aiosu/v2/clientstorage.py
+-rw-r--r--   0        0        0      107 2023-04-17 12:28:56.839148 aiosu-2.0.2/aiosu/v2/repository/__init__.py
+-rw-r--r--   0        0        0     1974 2023-04-17 12:28:56.839148 aiosu-2.0.2/aiosu/v2/repository/oauthtoken.py
+-rw-r--r--   0        0        0    35823 2023-04-17 12:28:56.828148 aiosu-2.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 12:28:56.843686 aiosu-2.0.2/py.typed
+-rw-r--r--   0        0        0     1881 2023-07-20 08:06:55.343982 aiosu-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4003 2023-07-18 22:52:49.244140 aiosu-2.0.2/README.rst
+-rw-r--r--   0        0        0     5427 1970-01-01 00:00:00.000000 aiosu-2.0.2/PKG-INFO
```

### Comparing `aiosu-2.0.1/LICENSE` & `aiosu-2.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `aiosu-2.0.1/README.rst` & `aiosu-2.0.2/README.rst`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-aiosu
-=====
-
-|Python| |pypi| |pre-commit.ci status| |rtd| |pytest| |mypy| |codacy|
-
-Simple and fast asynchronous osu! API v1 and v2 library with various utilities.
-
-
-Features
---------
-
-- Support for modern async syntax (async with)
-- Support for API v1 and API v2
-- Rate limit handling
-- Utilities for osu! related calculations
-- Easy to use
-
-
-Installing
-----------
-
-**Python 3.9 or higher is required**
-
-To install the library, simply run the following commands
-
-.. code:: sh
-
-    # Linux/macOS
-    python3 -m pip install -U aiosu
-
-    # Windows
-    py -3 -m pip install -U aiosu
-
-To install the development version, do the following:
-
-.. code:: sh
-
-    $ git clone https://github.com/NiceAesth/aiosu
-    $ cd aiosu
-    $ python3 -m pip install -U .
-
-
-API v1 Example
---------------
-
-.. code:: py
-
-   import aiosu
-   import asyncio
-
-
-   async def main():
-       # async with syntax
-       async with aiosu.v1.Client("osu api token") as client:
-           user = await client.get_user(7782553)
-
-       # regular syntax
-       client = aiosu.v1.Client("osu api token")
-       user = await client.get_user(7782553)
-       await client.close()
-
-
-   if __name__ == "__main__":
-       asyncio.run(main())
-
-
-API v2 Example
---------------
-
-.. code:: py
-
-    import aiosu
-    import asyncio
-    import datetime
-
-
-    async def main():
-        token = aiosu.models.OAuthToken.model_validate(json_token_from_api)
-
-        # or
-
-        token = aiosu.models.OAuthToken(
-            access_token="access token",
-            refresh_token="refresh token",
-            expires_on=datetime.datetime.utcnow()
-            + datetime.timedelta(days=1),  # can also be string
-        )
-
-        # async with syntax
-        async with aiosu.v2.Client(
-            client_secret="secret", client_id=1000, token=token
-        ) as client:
-            user = await client.get_me()
-
-        # regular syntax
-        client = aiosu.v2.Client(client_secret="secret", client_id=1000, token=token)
-        user = await client.get_me()
-        await client.close()
-
-
-    if __name__ == "__main__":
-        asyncio.run(main())
-
-
-You can find more examples in the examples directory.
-
-
-Contributing
-------------
-
-Please read the `CONTRIBUTING.rst <.github/CONTRIBUTING.rst>`__ to learn how to contribute to aiosu!
-
-
-Acknowledgments
----------------
-
--  `discord.py <https://github.com/Rapptz/discord.py>`__
-   for README formatting
--  `osu!Akatsuki <https://github.com/osuAkatsuki/performance-calculator>`__
-   for performance and accuracy utils
-
-
-.. |Python| image:: https://img.shields.io/pypi/pyversions/aiosu.svg
-    :target: https://pypi.python.org/pypi/aiosu
-    :alt: Python version info
-.. |pypi| image:: https://img.shields.io/pypi/v/aiosu.svg
-    :target: https://pypi.python.org/pypi/aiosu
-    :alt: PyPI version info
-.. |pre-commit.ci status| image:: https://results.pre-commit.ci/badge/github/NiceAesth/aiosu/master.svg
-    :target: https://results.pre-commit.ci/latest/github/NiceAesth/aiosu/master
-    :alt: pre-commit.ci status
-.. |pytest| image:: https://github.com/NiceAesth/aiosu/actions/workflows/pytest.yml/badge.svg
-    :target: https://github.com/NiceAesth/aiosu/actions/workflows/pytest.yml
-    :alt: pytest Status
-.. |mypy| image:: https://github.com/NiceAesth/aiosu/actions/workflows/mypy.yml/badge.svg
-    :target: https://github.com/NiceAesth/aiosu/actions/workflows/mypy.yml
-    :alt: mypy Status
-.. |rtd| image:: https://readthedocs.org/projects/aiosu/badge/?version=latest
-    :target: https://aiosu.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-.. |codacy| image:: https://app.codacy.com/project/badge/Grade/9bf211d7e29546dc99cc0b1a3d89b291
-    :target: https://www.codacy.com/gh/NiceAesth/aiosu/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NiceAesth/aiosu&amp;utm_campaign=Badge_Grade
-    :alt: Codacy Status
+aiosu
+=====
+
+|Python| |pypi| |pre-commit.ci status| |rtd| |pytest| |mypy| |codacy|
+
+Simple and fast asynchronous osu! API v1 and v2 library with various utilities.
+
+
+Features
+--------
+
+- Support for modern async syntax (async with)
+- Support for API v1 and API v2
+- Rate limit handling
+- Utilities for osu! related calculations
+- Easy to use
+
+
+Installing
+----------
+
+**Python 3.9 or higher is required**
+
+To install the library, simply run the following commands
+
+.. code:: sh
+
+    # Linux/macOS
+    python3 -m pip install -U aiosu
+
+    # Windows
+    py -3 -m pip install -U aiosu
+
+To install the development version, do the following:
+
+.. code:: sh
+
+    $ git clone https://github.com/NiceAesth/aiosu
+    $ cd aiosu
+    $ python3 -m pip install -U .
+
+
+API v1 Example
+--------------
+
+.. code:: py
+
+   import aiosu
+   import asyncio
+
+
+   async def main():
+       # async with syntax
+       async with aiosu.v1.Client("osu api token") as client:
+           user = await client.get_user(7782553)
+
+       # regular syntax
+       client = aiosu.v1.Client("osu api token")
+       user = await client.get_user(7782553)
+       await client.close()
+
+
+   if __name__ == "__main__":
+       asyncio.run(main())
+
+
+API v2 Example
+--------------
+
+.. code:: py
+
+    import aiosu
+    import asyncio
+    import datetime
+
+
+    async def main():
+        token = aiosu.models.OAuthToken.model_validate(json_token_from_api)
+
+        # or
+
+        token = aiosu.models.OAuthToken(
+            access_token="access token",
+            refresh_token="refresh token",
+            expires_on=datetime.datetime.utcnow()
+            + datetime.timedelta(days=1),  # can also be string
+        )
+
+        # async with syntax
+        async with aiosu.v2.Client(
+            client_secret="secret", client_id=1000, token=token
+        ) as client:
+            user = await client.get_me()
+
+        # regular syntax
+        client = aiosu.v2.Client(client_secret="secret", client_id=1000, token=token)
+        user = await client.get_me()
+        await client.close()
+
+
+    if __name__ == "__main__":
+        asyncio.run(main())
+
+
+You can find more examples in the examples directory.
+
+
+Contributing
+------------
+
+Please read the `CONTRIBUTING.rst <.github/CONTRIBUTING.rst>`__ to learn how to contribute to aiosu!
+
+
+Acknowledgments
+---------------
+
+-  `discord.py <https://github.com/Rapptz/discord.py>`__
+   for README formatting
+-  `osu!Akatsuki <https://github.com/osuAkatsuki/performance-calculator>`__
+   for performance and accuracy utils
+
+
+.. |Python| image:: https://img.shields.io/pypi/pyversions/aiosu.svg
+    :target: https://pypi.python.org/pypi/aiosu
+    :alt: Python version info
+.. |pypi| image:: https://img.shields.io/pypi/v/aiosu.svg
+    :target: https://pypi.python.org/pypi/aiosu
+    :alt: PyPI version info
+.. |pre-commit.ci status| image:: https://results.pre-commit.ci/badge/github/NiceAesth/aiosu/master.svg
+    :target: https://results.pre-commit.ci/latest/github/NiceAesth/aiosu/master
+    :alt: pre-commit.ci status
+.. |pytest| image:: https://github.com/NiceAesth/aiosu/actions/workflows/pytest.yml/badge.svg
+    :target: https://github.com/NiceAesth/aiosu/actions/workflows/pytest.yml
+    :alt: pytest Status
+.. |mypy| image:: https://github.com/NiceAesth/aiosu/actions/workflows/mypy.yml/badge.svg
+    :target: https://github.com/NiceAesth/aiosu/actions/workflows/mypy.yml
+    :alt: mypy Status
+.. |rtd| image:: https://readthedocs.org/projects/aiosu/badge/?version=latest
+    :target: https://aiosu.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+.. |codacy| image:: https://app.codacy.com/project/badge/Grade/9bf211d7e29546dc99cc0b1a3d89b291
+    :target: https://www.codacy.com/gh/NiceAesth/aiosu/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=NiceAesth/aiosu&amp;utm_campaign=Badge_Grade
+    :alt: Codacy Status
```

### Comparing `aiosu-2.0.1/aiosu/__init__.py` & `aiosu-2.0.2/aiosu/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from __future__ import annotations
-
-from datetime import date
-from importlib import metadata
-
-__title__ = "aiosu"
-__author__ = "Nice Aesthetics"
-__license__ = "GPLv3+"
-__copyright__ = f"Copyright {date.today().year} {__author__}"
-
-from . import events
-from . import exceptions
-from . import helpers
-from . import utils
-from . import models
-from . import v1
-from . import v2
-
-__all__ = (
-    "events",
-    "exceptions",
-    "helpers",
-    "utils",
-    "models",
-    "v1",
-    "v2",
-)
-
-try:
-    __version__ = metadata.version(__package__)
-except metadata.PackageNotFoundError:
-    import toml
-
-    __version__ = toml.load("pyproject.toml")["tool"]["poetry"]["version"] + "dev"
+from __future__ import annotations
+
+from datetime import date
+from importlib import metadata
+
+__title__ = "aiosu"
+__author__ = "Nice Aesthetics"
+__license__ = "GPLv3+"
+__copyright__ = f"Copyright {date.today().year} {__author__}"
+
+from . import events
+from . import exceptions
+from . import helpers
+from . import utils
+from . import models
+from . import v1
+from . import v2
+
+__all__ = (
+    "events",
+    "exceptions",
+    "helpers",
+    "utils",
+    "models",
+    "v1",
+    "v2",
+)
+
+try:
+    __version__ = metadata.version(__package__)
+except metadata.PackageNotFoundError:
+    import toml
+
+    __version__ = toml.load("pyproject.toml")["tool"]["poetry"]["version"] + "dev"
```

### Comparing `aiosu-2.0.1/aiosu/helpers.py` & `aiosu-2.0.2/aiosu/helpers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""
-This module contains miscellaneous helper functions.
-"""
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Any
-    from typing import Callable
-    from typing import Optional
-    from typing import TypeVar
-
-    T = TypeVar("T")
-
-__all__ = (
-    "from_list",
-    "add_param",
-)
-
-
-def from_list(f: Callable[[Any], T], x: Any) -> list[T]:
-    r"""Applies a function to all elements in a list.
-
-    :param f: Function to apply on list elements
-    :type f: Callable[[Any], T]
-    :param x: List of objects
-    :type x: Any
-    :raises TypeError: If x is not a list
-    :return: New list
-    :rtype: list[T]
-    """
-    if not isinstance(x, list):
-        raise TypeError("Wrong type received. Expected list.")
-    return [f(y) for y in x]
-
-
-def add_param(
-    params: dict[str, Any],
-    kwargs: dict[str, Any],
-    key: str,
-    param_name: Optional[str] = None,
-    converter: Optional[Callable[[Any], T]] = None,
-) -> bool:
-    r"""Adds a parameter to a dictionary if it exists in kwargs.
-
-    :param params: Dictionary to add parameter to
-    :type params: dict[str, Any]
-    :param kwargs: Dictionary to get parameter from
-    :type kwargs: dict[str, Any]
-    :param key: Key to get parameter from
-    :type key: str
-    :param param_name: Name of parameter to add to dictionary, defaults to None
-    :type param_name: Optional[str]
-    :param converter: Function to convert parameter, defaults to None
-    :type converter: Optional[Callable[[Any], T]]
-    :return: True if parameter was added, False otherwise
-    :rtype: bool
-    """
-    if key in kwargs:
-        value = kwargs[key]
-        if converter:
-            value = converter(value)
-        params[param_name or key] = value
-        return True
-    return False
+"""
+This module contains miscellaneous helper functions.
+"""
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any
+    from typing import Callable
+    from typing import Optional
+    from typing import TypeVar
+
+    T = TypeVar("T")
+
+__all__ = (
+    "from_list",
+    "add_param",
+)
+
+
+def from_list(f: Callable[[Any], T], x: Any) -> list[T]:
+    r"""Applies a function to all elements in a list.
+
+    :param f: Function to apply on list elements
+    :type f: Callable[[Any], T]
+    :param x: List of objects
+    :type x: Any
+    :raises TypeError: If x is not a list
+    :return: New list
+    :rtype: list[T]
+    """
+    if not isinstance(x, list):
+        raise TypeError("Wrong type received. Expected list.")
+    return [f(y) for y in x]
+
+
+def add_param(
+    params: dict[str, Any],
+    kwargs: dict[str, Any],
+    key: str,
+    param_name: Optional[str] = None,
+    converter: Optional[Callable[[Any], T]] = None,
+) -> bool:
+    r"""Adds a parameter to a dictionary if it exists in kwargs.
+
+    :param params: Dictionary to add parameter to
+    :type params: dict[str, Any]
+    :param kwargs: Dictionary to get parameter from
+    :type kwargs: dict[str, Any]
+    :param key: Key to get parameter from
+    :type key: str
+    :param param_name: Name of parameter to add to dictionary, defaults to None
+    :type param_name: Optional[str]
+    :param converter: Function to convert parameter, defaults to None
+    :type converter: Optional[Callable[[Any], T]]
+    :return: True if parameter was added, False otherwise
+    :rtype: bool
+    """
+    if key in kwargs:
+        value = kwargs[key]
+        if converter:
+            value = converter(value)
+        params[param_name or key] = value
+        return True
+    return False
```

### Comparing `aiosu-2.0.1/aiosu/models/base.py` & `aiosu-2.0.2/aiosu/models/base.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-This module contains base models for objects.
-"""
-from __future__ import annotations
-
-import pydantic
-from pydantic import ConfigDict
-
-__all__ = (
-    "BaseModel",
-    "FrozenModel",
-)
-
-
-class BaseModel(pydantic.BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    @classmethod
-    def model_validate_file(cls, path: str) -> BaseModel:
-        """Validates a model from a file.
-
-        :param path: The path to the file
-        :type path: str
-        :raises TypeError: If the file is not a JSON file
-        :return: The validated model
-        :rtype: aiosu.models.base.BaseModel
-        """
-        with open(path) as f:
-            return cls.model_validate_json(f.read())
-
-
-class FrozenModel(BaseModel):
-    model_config = ConfigDict(
-        arbitrary_types_allowed=True,
-        populate_by_name=True,
-        frozen=True,
-    )
+"""
+This module contains base models for objects.
+"""
+from __future__ import annotations
+
+import pydantic
+from pydantic import ConfigDict
+
+__all__ = (
+    "BaseModel",
+    "FrozenModel",
+)
+
+
+class BaseModel(pydantic.BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    @classmethod
+    def model_validate_file(cls, path: str) -> BaseModel:
+        """Validates a model from a file.
+
+        :param path: The path to the file
+        :type path: str
+        :raises TypeError: If the file is not a JSON file
+        :return: The validated model
+        :rtype: aiosu.models.base.BaseModel
+        """
+        with open(path) as f:
+            return cls.model_validate_json(f.read())
+
+
+class FrozenModel(BaseModel):
+    model_config = ConfigDict(
+        arbitrary_types_allowed=True,
+        populate_by_name=True,
+        frozen=True,
+    )
```

### Comparing `aiosu-2.0.1/aiosu/models/changelog.py` & `aiosu-2.0.2/aiosu/models/changelog.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-"""
-This module contains models for changelog objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Literal
-from typing import Optional
-
-from pydantic import Field
-
-from .base import BaseModel
-from .common import CursorModel
-
-
-__all__ = (
-    "Build",
-    "ChangelogEntry",
-    "GithubUser",
-    "UpdateStream",
-    "Version",
-    "ChangelogListing",
-    "ChangelogSearch",
-    "ChangelogMessageFormats",
-)
-
-ChangelogMessageFormats = Literal["markdown", "html"]
-
-
-class GithubUser(BaseModel):
-    display_name: str
-    github_url: Optional[str] = None
-    id: Optional[int] = None
-    osu_username: Optional[str] = None
-    user_id: Optional[int] = None
-    user_url: Optional[str] = None
-
-
-class ChangelogEntry(BaseModel):
-    type: str
-    category: str
-    major: bool
-    id: Optional[int] = None
-    title: Optional[str] = None
-    created_at: Optional[datetime] = None
-    url: Optional[str] = None
-    github_url: Optional[str] = None
-    github_pull_request_id: Optional[int] = None
-    repository: Optional[str] = None
-    message: Optional[str] = None
-    message_html: Optional[str] = None
-    github_user: Optional[GithubUser] = None
-
-
-class Version(BaseModel):
-    next: Optional[Build] = None
-    previous: Optional[Build] = None
-
-
-class UpdateStream(BaseModel):
-    id: int
-    is_featured: bool
-    name: str
-    display_name: Optional[str] = None
-    user_count: Optional[int] = None
-    latest_build: Optional[Build] = None
-
-
-class Build(BaseModel):
-    id: int
-    created_at: datetime
-    display_version: str
-    users: int
-    version: str
-    youtube_id: Optional[str] = None
-    update_stream: Optional[UpdateStream] = None
-    changelog_entries: Optional[list[ChangelogEntry]] = None
-    versions: Optional[Version] = None
-
-
-class ChangelogSearch(BaseModel):
-    limit: int
-    fro: Optional[str] = Field(default=None, alias="from")
-    to: Optional[str] = None
-    max_id: Optional[int] = None
-    stream: Optional[str] = None
-
-
-class ChangelogListing(CursorModel):
-    builds: list[Build]
-    search: ChangelogSearch
-    streams: list[UpdateStream]
-
-
-Version.model_rebuild()
-UpdateStream.model_rebuild()
+"""
+This module contains models for changelog objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Literal
+from typing import Optional
+
+from pydantic import Field
+
+from .base import BaseModel
+from .common import CursorModel
+
+
+__all__ = (
+    "Build",
+    "ChangelogEntry",
+    "GithubUser",
+    "UpdateStream",
+    "Version",
+    "ChangelogListing",
+    "ChangelogSearch",
+    "ChangelogMessageFormats",
+)
+
+ChangelogMessageFormats = Literal["markdown", "html"]
+
+
+class GithubUser(BaseModel):
+    display_name: str
+    github_url: Optional[str] = None
+    id: Optional[int] = None
+    osu_username: Optional[str] = None
+    user_id: Optional[int] = None
+    user_url: Optional[str] = None
+
+
+class ChangelogEntry(BaseModel):
+    type: str
+    category: str
+    major: bool
+    id: Optional[int] = None
+    title: Optional[str] = None
+    created_at: Optional[datetime] = None
+    url: Optional[str] = None
+    github_url: Optional[str] = None
+    github_pull_request_id: Optional[int] = None
+    repository: Optional[str] = None
+    message: Optional[str] = None
+    message_html: Optional[str] = None
+    github_user: Optional[GithubUser] = None
+
+
+class Version(BaseModel):
+    next: Optional[Build] = None
+    previous: Optional[Build] = None
+
+
+class UpdateStream(BaseModel):
+    id: int
+    is_featured: bool
+    name: str
+    display_name: Optional[str] = None
+    user_count: Optional[int] = None
+    latest_build: Optional[Build] = None
+
+
+class Build(BaseModel):
+    id: int
+    created_at: datetime
+    display_version: str
+    users: int
+    version: str
+    youtube_id: Optional[str] = None
+    update_stream: Optional[UpdateStream] = None
+    changelog_entries: Optional[list[ChangelogEntry]] = None
+    versions: Optional[Version] = None
+
+
+class ChangelogSearch(BaseModel):
+    limit: int
+    fro: Optional[str] = Field(default=None, alias="from")
+    to: Optional[str] = None
+    max_id: Optional[int] = None
+    stream: Optional[str] = None
+
+
+class ChangelogListing(CursorModel):
+    builds: list[Build]
+    search: ChangelogSearch
+    streams: list[UpdateStream]
+
+
+Version.model_rebuild()
+UpdateStream.model_rebuild()
```

### Comparing `aiosu-2.0.1/aiosu/models/chat.py` & `aiosu-2.0.2/aiosu/models/chat.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-This module contains models for chat.
-"""
-from __future__ import annotations
-
-from typing import Literal
-from typing import Optional
-
-from pydantic import Field
-
-from .base import BaseModel
-from .common import CurrentUserAttributes
-from .user import User
-
-__all__ = (
-    "ChatChannel",
-    "ChatMessage",
-    "ChatMessageCreateResponse",
-    "ChatChannelTypes",
-    "ChatIncludeTypes",
-    "ChatUpdateResponse",
-    "ChatUserSilence",
-    "ChatChannelResponse",
-)
-
-ChatChannelTypes = Literal[
-    "PM",
-    "PUBLIC",
-    "PRIVATE",
-    "MULTIPLAYER",
-    "SPECTATOR",
-    "TEMPORARY",
-    "GROUP",
-    "ANNOUNCE",
-]
-
-ChatIncludeTypes = Literal[
-    "messages",
-    "presence",
-    "silences",
-]
-
-
-class ChatUserSilence(BaseModel):
-    id: int
-    user_id: int
-
-
-class ChatChannel(BaseModel):
-    id: int = Field(alias="channel_id")
-    type: ChatChannelTypes
-    name: str
-    moderated: bool
-    message_length_limit: int
-    icon: Optional[str] = None
-    description: Optional[str] = None
-    last_message_id: Optional[int] = None
-    user_ids: Optional[list[int]] = Field(default=None, alias="users")
-    current_user_attributes: Optional[CurrentUserAttributes] = None
-
-
-class ChatMessage(BaseModel):
-    message_id: int
-    sender_id: int
-    channel_id: int
-    timestamp: str
-    content: str
-    is_action: bool
-    uuid: Optional[str] = None
-    sender: Optional[User] = None
-
-
-class ChatMessageCreateResponse(BaseModel):
-    channel: ChatChannel
-    message: ChatMessage
-
-
-class ChatUpdateResponse(BaseModel):
-    messages: Optional[list[ChatMessage]] = None
-    presence: Optional[list[ChatChannel]] = None
-    silences: list
-
-
-class ChatChannelResponse(BaseModel):
-    channel: ChatChannel
-    users: Optional[list[User]] = None
+"""
+This module contains models for chat.
+"""
+from __future__ import annotations
+
+from typing import Literal
+from typing import Optional
+
+from pydantic import Field
+
+from .base import BaseModel
+from .common import CurrentUserAttributes
+from .user import User
+
+__all__ = (
+    "ChatChannel",
+    "ChatMessage",
+    "ChatMessageCreateResponse",
+    "ChatChannelTypes",
+    "ChatIncludeTypes",
+    "ChatUpdateResponse",
+    "ChatUserSilence",
+    "ChatChannelResponse",
+)
+
+ChatChannelTypes = Literal[
+    "PM",
+    "PUBLIC",
+    "PRIVATE",
+    "MULTIPLAYER",
+    "SPECTATOR",
+    "TEMPORARY",
+    "GROUP",
+    "ANNOUNCE",
+]
+
+ChatIncludeTypes = Literal[
+    "messages",
+    "presence",
+    "silences",
+]
+
+
+class ChatUserSilence(BaseModel):
+    id: int
+    user_id: int
+
+
+class ChatChannel(BaseModel):
+    id: int = Field(alias="channel_id")
+    type: ChatChannelTypes
+    name: str
+    moderated: bool
+    message_length_limit: int
+    icon: Optional[str] = None
+    description: Optional[str] = None
+    last_message_id: Optional[int] = None
+    user_ids: Optional[list[int]] = Field(default=None, alias="users")
+    current_user_attributes: Optional[CurrentUserAttributes] = None
+
+
+class ChatMessage(BaseModel):
+    message_id: int
+    sender_id: int
+    channel_id: int
+    timestamp: str
+    content: str
+    is_action: bool
+    uuid: Optional[str] = None
+    sender: Optional[User] = None
+
+
+class ChatMessageCreateResponse(BaseModel):
+    channel: ChatChannel
+    message: ChatMessage
+
+
+class ChatUpdateResponse(BaseModel):
+    messages: Optional[list[ChatMessage]] = None
+    presence: Optional[list[ChatChannel]] = None
+    silences: list
+
+
+class ChatChannelResponse(BaseModel):
+    channel: ChatChannel
+    users: Optional[list[User]] = None
```

### Comparing `aiosu-2.0.1/aiosu/models/comment.py` & `aiosu-2.0.2/aiosu/models/comment.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""
-This module contains models for comment objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Literal
-from typing import Optional
-
-from .base import BaseModel
-from .common import CurrentUserAttributes
-from .common import CursorModel
-from .user import User
-
-__all__ = (
-    "Commentable",
-    "Comment",
-    "CommentBundle",
-    "CommentSortType",
-)
-
-CommentSortType = Literal["new", "old", "top"]
-
-
-class Commentable(BaseModel):
-    id: Optional[int] = None
-    title: Optional[str] = None
-    url: Optional[str] = None
-    type: Optional[str] = None
-    owner_id: Optional[int] = None
-    owner_title: Optional[str] = None
-    current_user_attributes: Optional[CurrentUserAttributes] = None
-
-
-class Comment(BaseModel):
-    id: int
-    commentable_id: int
-    commentable_type: str
-    created_at: datetime
-    updated_at: datetime
-    pinned: bool
-    votes_count: int
-    replies_count: int
-    message: Optional[str] = None
-    message_html: Optional[str] = None
-    deleted_at: Optional[datetime] = None
-    edited_at: Optional[datetime] = None
-    edited_by_id: Optional[int] = None
-    parent_id: Optional[int] = None
-    legacy_name: Optional[str] = None
-    user_id: Optional[int] = None
-
-
-class CommentBundle(CursorModel):
-    commentable_meta: list[Commentable]
-    comments: list[Comment]
-    has_more: bool
-    included_comments: list[Comment]
-    sort: str
-    user_follow: bool
-    user_votes: list[int]
-    users: list[User]
-    pinned_comments: Optional[list[Comment]] = None
-    total: Optional[int] = None
-    top_level_count: Optional[int] = None
-    has_more_id: Optional[int] = None
+"""
+This module contains models for comment objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Literal
+from typing import Optional
+
+from .base import BaseModel
+from .common import CurrentUserAttributes
+from .common import CursorModel
+from .user import User
+
+__all__ = (
+    "Commentable",
+    "Comment",
+    "CommentBundle",
+    "CommentSortType",
+)
+
+CommentSortType = Literal["new", "old", "top"]
+
+
+class Commentable(BaseModel):
+    id: Optional[int] = None
+    title: Optional[str] = None
+    url: Optional[str] = None
+    type: Optional[str] = None
+    owner_id: Optional[int] = None
+    owner_title: Optional[str] = None
+    current_user_attributes: Optional[CurrentUserAttributes] = None
+
+
+class Comment(BaseModel):
+    id: int
+    commentable_id: int
+    commentable_type: str
+    created_at: datetime
+    updated_at: datetime
+    pinned: bool
+    votes_count: int
+    replies_count: int
+    message: Optional[str] = None
+    message_html: Optional[str] = None
+    deleted_at: Optional[datetime] = None
+    edited_at: Optional[datetime] = None
+    edited_by_id: Optional[int] = None
+    parent_id: Optional[int] = None
+    legacy_name: Optional[str] = None
+    user_id: Optional[int] = None
+
+
+class CommentBundle(CursorModel):
+    commentable_meta: list[Commentable]
+    comments: list[Comment]
+    has_more: bool
+    included_comments: list[Comment]
+    sort: str
+    user_follow: bool
+    user_votes: list[int]
+    users: list[User]
+    pinned_comments: Optional[list[Comment]] = None
+    total: Optional[int] = None
+    top_level_count: Optional[int] = None
+    has_more_id: Optional[int] = None
```

### Comparing `aiosu-2.0.1/aiosu/models/forum.py` & `aiosu-2.0.2/aiosu/models/forum.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""
-This module contains the Forum model.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Literal
-from typing import Optional
-
-from .base import BaseModel
-from .common import CursorModel
-from .common import HTMLBody
-
-__all__ = [
-    "ForumPost",
-    "ForumTopic",
-    "ForumTopicResponse",
-    "ForumTopicType",
-    "ForumPoll",
-    "ForumPollOption",
-    "ForumCreateTopicResponse",
-]
-
-ForumTopicType = Literal[
-    "normal",
-    "sticky",
-    "announcement",
-]
-
-
-class ForumPollOption(BaseModel):
-    id: int
-    text: HTMLBody
-    vote_count: Optional[int] = None
-
-
-class ForumPoll(BaseModel):
-    allow_vote_change: bool
-    hide_incomplete_results: bool
-    max_votes: int
-    total_vote_count: int
-    options: list[ForumPollOption]
-    started_at: datetime
-    title: HTMLBody
-    ended_at: Optional[datetime] = None
-    last_vote_at: Optional[datetime] = None
-
-
-class ForumTopic(BaseModel):
-    id: int
-    title: str
-    created_at: datetime
-    first_post_id: int
-    last_post_id: int
-    forum_id: int
-    is_locked: bool
-    post_count: int
-    type: ForumTopicType
-    updated_at: datetime
-    user_id: int
-    deleted_at: Optional[datetime] = None
-    poll: Optional[ForumPoll] = None
-
-
-class ForumPost(BaseModel):
-    id: int
-    created_at: datetime
-    forum_id: int
-    topic_id: int
-    user_id: int
-    edited_by_id: Optional[int] = None
-    edited_at: Optional[datetime] = None
-    deleted_at: Optional[datetime] = None
-    body: Optional[HTMLBody] = None
-
-
-class ForumTopicResponse(CursorModel):
-    topic: ForumTopic
-    posts: list[ForumPost]
-
-
-class ForumCreateTopicResponse(BaseModel):
-    topic: ForumTopic
-    post: ForumPost
+"""
+This module contains the Forum model.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Literal
+from typing import Optional
+
+from .base import BaseModel
+from .common import CursorModel
+from .common import HTMLBody
+
+__all__ = [
+    "ForumPost",
+    "ForumTopic",
+    "ForumTopicResponse",
+    "ForumTopicType",
+    "ForumPoll",
+    "ForumPollOption",
+    "ForumCreateTopicResponse",
+]
+
+ForumTopicType = Literal[
+    "normal",
+    "sticky",
+    "announcement",
+]
+
+
+class ForumPollOption(BaseModel):
+    id: int
+    text: HTMLBody
+    vote_count: Optional[int] = None
+
+
+class ForumPoll(BaseModel):
+    allow_vote_change: bool
+    hide_incomplete_results: bool
+    max_votes: int
+    total_vote_count: int
+    options: list[ForumPollOption]
+    started_at: datetime
+    title: HTMLBody
+    ended_at: Optional[datetime] = None
+    last_vote_at: Optional[datetime] = None
+
+
+class ForumTopic(BaseModel):
+    id: int
+    title: str
+    created_at: datetime
+    first_post_id: int
+    last_post_id: int
+    forum_id: int
+    is_locked: bool
+    post_count: int
+    type: ForumTopicType
+    updated_at: datetime
+    user_id: int
+    deleted_at: Optional[datetime] = None
+    poll: Optional[ForumPoll] = None
+
+
+class ForumPost(BaseModel):
+    id: int
+    created_at: datetime
+    forum_id: int
+    topic_id: int
+    user_id: int
+    edited_by_id: Optional[int] = None
+    edited_at: Optional[datetime] = None
+    deleted_at: Optional[datetime] = None
+    body: Optional[HTMLBody] = None
+
+
+class ForumTopicResponse(CursorModel):
+    topic: ForumTopic
+    posts: list[ForumPost]
+
+
+class ForumCreateTopicResponse(BaseModel):
+    topic: ForumTopic
+    post: ForumPost
```

### Comparing `aiosu-2.0.1/aiosu/models/gamemode.py` & `aiosu-2.0.2/aiosu/models/gamemode.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-"""
-This module contains models for Gamemode objects.
-"""
-from __future__ import annotations
-
-from enum import Enum
-from enum import unique
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Any
-
-__all__ = ("Gamemode",)
-
-GAMEMODE_NAMES = {
-    0: "Standard",
-    1: "Taiko",
-    2: "Catch the Beat",
-    3: "Mania",
-}
-
-GAMEMODE_SHORT_NAMES = {
-    0: "STD",
-    1: "Taiko",
-    2: "CTB",
-    3: "Mania",
-}
-
-GAMEMODE_API_NAMES = {
-    0: "osu",
-    1: "taiko",
-    2: "fruits",
-    3: "mania",
-}
-
-
-@unique
-class Gamemode(Enum):
-    STANDARD = 0
-    TAIKO = 1
-    CTB = 2
-    MANIA = 3
-
-    @property
-    def id(self) -> int:
-        return self.value
-
-    @property
-    def name_full(self) -> str:
-        return GAMEMODE_NAMES[self.id]
-
-    @property
-    def name_short(self) -> str:
-        return GAMEMODE_SHORT_NAMES[self.id]
-
-    @property
-    def name_api(self) -> str:
-        return GAMEMODE_API_NAMES[self.id]
-
-    def __int__(self) -> int:
-        return self.id
-
-    def __str__(self) -> str:
-        return self.name_api
-
-    def __format__(self, spec: str) -> str:
-        if spec == "f":
-            return self.name_full
-        if spec == "s":
-            return self.name_short
-        return self.name_api
-
-    @classmethod
-    def from_type(cls, __o: object) -> Gamemode:
-        """Gets a gamemode.
-
-        :param __o: Object to search for
-        :type __o: object
-        :raises ValueError: If object cannot be converted to Gamemode
-        :return: A Gamemode object. Will search by name_api, name_short, id
-        :rtype: aiosu.models.gamemode.Gamemode
-        """
-        if isinstance(__o, cls):
-            return __o
-        for mode in list(Gamemode):
-            if __o in (mode.name_api, mode.name_short, mode.name_full, mode.id):
-                return mode
-        raise ValueError(f"Gamemode {__o} does not exist.")
-
-    @classmethod
-    def _missing_(cls, query: object) -> Any:
-        return cls.from_type(query)
+"""
+This module contains models for Gamemode objects.
+"""
+from __future__ import annotations
+
+from enum import Enum
+from enum import unique
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Any
+
+__all__ = ("Gamemode",)
+
+GAMEMODE_NAMES = {
+    0: "Standard",
+    1: "Taiko",
+    2: "Catch the Beat",
+    3: "Mania",
+}
+
+GAMEMODE_SHORT_NAMES = {
+    0: "STD",
+    1: "Taiko",
+    2: "CTB",
+    3: "Mania",
+}
+
+GAMEMODE_API_NAMES = {
+    0: "osu",
+    1: "taiko",
+    2: "fruits",
+    3: "mania",
+}
+
+
+@unique
+class Gamemode(Enum):
+    STANDARD = 0
+    TAIKO = 1
+    CTB = 2
+    MANIA = 3
+
+    @property
+    def id(self) -> int:
+        return self.value
+
+    @property
+    def name_full(self) -> str:
+        return GAMEMODE_NAMES[self.id]
+
+    @property
+    def name_short(self) -> str:
+        return GAMEMODE_SHORT_NAMES[self.id]
+
+    @property
+    def name_api(self) -> str:
+        return GAMEMODE_API_NAMES[self.id]
+
+    def __int__(self) -> int:
+        return self.id
+
+    def __str__(self) -> str:
+        return self.name_api
+
+    def __format__(self, spec: str) -> str:
+        if spec == "f":
+            return self.name_full
+        if spec == "s":
+            return self.name_short
+        return self.name_api
+
+    @classmethod
+    def from_type(cls, __o: object) -> Gamemode:
+        """Gets a gamemode.
+
+        :param __o: Object to search for
+        :type __o: object
+        :raises ValueError: If object cannot be converted to Gamemode
+        :return: A Gamemode object. Will search by name_api, name_short, id
+        :rtype: aiosu.models.gamemode.Gamemode
+        """
+        if isinstance(__o, cls):
+            return __o
+        for mode in list(Gamemode):
+            if __o in (mode.name_api, mode.name_short, mode.name_full, mode.id):
+                return mode
+        raise ValueError(f"Gamemode {__o} does not exist.")
+
+    @classmethod
+    def _missing_(cls, query: object) -> Any:
+        return cls.from_type(query)
```

### Comparing `aiosu-2.0.1/aiosu/models/kudosu.py` & `aiosu-2.0.2/aiosu/models/kudosu.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""
-This module contains models for kudosu objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Literal
-from typing import Optional
-
-from .base import BaseModel
-
-__all__ = (
-    "KudosuAction",
-    "KudosuGiver",
-    "KudosuPost",
-    "KudosuHistory",
-)
-
-KudosuAction = Literal[
-    "give",
-    "vote.give",
-    "reset",
-    "vote.reset",
-    "revoke",
-    "vote.revoke",
-]
-
-
-class KudosuGiver(BaseModel):
-    url: str
-    username: str
-
-
-class KudosuPost(BaseModel):
-    title: str
-    url: Optional[str] = None
-
-
-class KudosuHistory(BaseModel):
-    id: int
-    action: KudosuAction
-    created_at: datetime
-    amount: int
-    model: str
-    giver: Optional[KudosuGiver] = None
-    post: Optional[KudosuPost] = None
+"""
+This module contains models for kudosu objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Literal
+from typing import Optional
+
+from .base import BaseModel
+
+__all__ = (
+    "KudosuAction",
+    "KudosuGiver",
+    "KudosuPost",
+    "KudosuHistory",
+)
+
+KudosuAction = Literal[
+    "give",
+    "vote.give",
+    "reset",
+    "vote.reset",
+    "revoke",
+    "vote.revoke",
+]
+
+
+class KudosuGiver(BaseModel):
+    url: str
+    username: str
+
+
+class KudosuPost(BaseModel):
+    title: str
+    url: Optional[str] = None
+
+
+class KudosuHistory(BaseModel):
+    id: int
+    action: KudosuAction
+    created_at: datetime
+    amount: int
+    model: str
+    giver: Optional[KudosuGiver] = None
+    post: Optional[KudosuPost] = None
```

### Comparing `aiosu-2.0.1/aiosu/models/lazer.py` & `aiosu-2.0.2/aiosu/models/lazer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-"""
-This module contains models for lazer specific data.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Any
-from typing import Optional
-
-from pydantic import computed_field
-from pydantic import Field
-from pydantic import model_validator
-
-from .base import BaseModel
-from .beatmap import Beatmap
-from .beatmap import Beatmapset
-from .common import CurrentUserAttributes
-from .gamemode import Gamemode
-from .score import ScoreWeight
-from .user import User
-
-__all__ = (
-    "LazerMod",
-    "LazerScoreStatistics",
-    "LazerReplayData",
-    "LazerScore",
-)
-
-
-def calculate_score_completion(
-    statistics: LazerScoreStatistics,
-    beatmap: Beatmap,
-) -> float:
-    """Calculates completion for a score.
-
-    :param statistics: The statistics of the score
-    :type statistics: aiosu.models.lazer.LazerScoreStatistics
-    :param beatmap: The beatmap of the score
-    :type beatmap: aiosu.models.beatmap.Beatmap
-    :raises ValueError: If the gamemode is unknown
-    :return: Completion for the given score
-    :rtype: float
-    """
-    return (
-        (
-            statistics.perfect
-            + statistics.good
-            + statistics.great
-            + statistics.ok
-            + statistics.meh
-            + statistics.miss
-        )
-        / beatmap.count_objects
-    ) * 100
-
-
-class LazerMod(BaseModel):
-    """Temporary model for lazer mods."""
-
-    acronym: str
-    settings: dict[str, Any] = Field(default_factory=dict)
-
-    def __str__(self) -> str:
-        return self.acronym
-
-
-class LazerScoreStatistics(BaseModel):
-    ok: int = 0
-    meh: int = 0
-    miss: int = 0
-    great: int = 0
-    ignore_hit: int = 0
-    ignore_miss: int = 0
-    large_bonus: int = 0
-    large_tick_hit: int = 0
-    large_tick_miss: int = 0
-    small_bonus: int = 0
-    small_tick_hit: int = 0
-    small_tick_miss: int = 0
-    good: int = 0
-    perfect: int = 0
-    legacy_combo_increase: int = 0
-
-    @computed_field  # type: ignore
-    @property
-    def count_300(self) -> int:
-        return self.great
-
-    @computed_field  # type: ignore
-    @property
-    def count_100(self) -> int:
-        return self.ok
-
-    @computed_field  # type: ignore
-    @property
-    def count_50(self) -> int:
-        return self.meh
-
-    @computed_field  # type: ignore
-    @property
-    def count_miss(self) -> int:
-        return self.miss
-
-    @computed_field  # type: ignore
-    @property
-    def count_geki(self) -> int:
-        return self.perfect
-
-    @computed_field  # type: ignore
-    @property
-    def count_katu(self) -> int:
-        return self.good
-
-
-class LazerReplayData(BaseModel):
-    mods: list[LazerMod]
-    statistics: LazerScoreStatistics
-    maximum_statistics: LazerScoreStatistics
-
-
-class LazerScore(BaseModel):
-    id: int
-    accuracy: float
-    beatmap_id: int
-    max_combo: int
-    maximum_statistics: LazerScoreStatistics
-    mods: list[LazerMod]
-    passed: bool
-    rank: str
-    ruleset_id: int
-    ended_at: datetime
-    statistics: LazerScoreStatistics
-    total_score: int
-    user_id: int
-    replay: bool
-    type: str
-    current_user_attributes: CurrentUserAttributes
-    beatmap: Beatmap
-    beatmapset: Beatmapset
-    user: User
-    build_id: Optional[int] = None
-    started_at: Optional[datetime] = None
-    best_id: Optional[int] = None
-    legacy_perfect: Optional[bool] = None
-    pp: Optional[float] = None
-    weight: Optional[ScoreWeight] = None
-
-    @computed_field  # type: ignore
-    @property
-    def mods_str(self) -> str:
-        return "".join(str(mod) for mod in self.mods)
-
-    @computed_field  # type: ignore
-    @property
-    def created_at(self) -> datetime:
-        return self.ended_at
-
-    @computed_field  # type: ignore
-    @property
-    def completion(self) -> float:
-        """Beatmap completion.
-
-        :raises ValueError: If beatmap is None
-        :raises ValueError: If mode is unknown
-        :return: Beatmap completion of a score (%). 100% for passes
-        :rtype: float
-        """
-        if self.beatmap is None:
-            raise ValueError("Beatmap object is not set.")
-
-        if self.passed:
-            return 100.0
-
-        return calculate_score_completion(self.statistics, self.beatmap)
-
-    @computed_field  # type: ignore
-    @property
-    def mode(self) -> Gamemode:
-        return Gamemode(self.ruleset_id)
-
-    @computed_field  # type: ignore
-    @property
-    def score(self) -> int:
-        return self.total_score
-
-    @computed_field  # type: ignore
-    @property
-    def score_url(self) -> Optional[str]:
-        r"""Link to the score.
-
-        :return: Link to the score on the osu! website
-        :rtype: Optional[str]
-        """
-        if (not self.id and not self.best_id) or not self.passed:
-            return None
-        return (
-            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
-            if self.best_id
-            else f"https://osu.ppy.sh/scores/{self.id}"
-        )
-
-    @computed_field  # type: ignore
-    @property
-    def replay_url(self) -> Optional[str]:
-        r"""Link to the replay.
-
-        :return: Link to download the replay on the osu! website
-        :rtype: Optional[str]
-        """
-        if not self.replay:
-            return None
-        return (
-            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
-            if self.best_id
-            else f"https://osu.ppy.sh/scores/{self.id}/download"
-        )
-
-    @model_validator(mode="before")
-    @classmethod
-    def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if not values["passed"]:
-            values["rank"] = "F"
-        return values
+"""
+This module contains models for lazer specific data.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Any
+from typing import Optional
+
+from pydantic import computed_field
+from pydantic import Field
+from pydantic import model_validator
+
+from .base import BaseModel
+from .beatmap import Beatmap
+from .beatmap import Beatmapset
+from .common import CurrentUserAttributes
+from .gamemode import Gamemode
+from .score import ScoreWeight
+from .user import User
+
+__all__ = (
+    "LazerMod",
+    "LazerScoreStatistics",
+    "LazerReplayData",
+    "LazerScore",
+)
+
+
+def calculate_score_completion(
+    statistics: LazerScoreStatistics,
+    beatmap: Beatmap,
+) -> float:
+    """Calculates completion for a score.
+
+    :param statistics: The statistics of the score
+    :type statistics: aiosu.models.lazer.LazerScoreStatistics
+    :param beatmap: The beatmap of the score
+    :type beatmap: aiosu.models.beatmap.Beatmap
+    :raises ValueError: If the gamemode is unknown
+    :return: Completion for the given score
+    :rtype: float
+    """
+    return (
+        (
+            statistics.perfect
+            + statistics.good
+            + statistics.great
+            + statistics.ok
+            + statistics.meh
+            + statistics.miss
+        )
+        / beatmap.count_objects
+    ) * 100
+
+
+class LazerMod(BaseModel):
+    """Temporary model for lazer mods."""
+
+    acronym: str
+    settings: dict[str, Any] = Field(default_factory=dict)
+
+    def __str__(self) -> str:
+        return self.acronym
+
+
+class LazerScoreStatistics(BaseModel):
+    ok: int = 0
+    meh: int = 0
+    miss: int = 0
+    great: int = 0
+    ignore_hit: int = 0
+    ignore_miss: int = 0
+    large_bonus: int = 0
+    large_tick_hit: int = 0
+    large_tick_miss: int = 0
+    small_bonus: int = 0
+    small_tick_hit: int = 0
+    small_tick_miss: int = 0
+    good: int = 0
+    perfect: int = 0
+    legacy_combo_increase: int = 0
+
+    @computed_field  # type: ignore
+    @property
+    def count_300(self) -> int:
+        return self.great
+
+    @computed_field  # type: ignore
+    @property
+    def count_100(self) -> int:
+        return self.ok
+
+    @computed_field  # type: ignore
+    @property
+    def count_50(self) -> int:
+        return self.meh
+
+    @computed_field  # type: ignore
+    @property
+    def count_miss(self) -> int:
+        return self.miss
+
+    @computed_field  # type: ignore
+    @property
+    def count_geki(self) -> int:
+        return self.perfect
+
+    @computed_field  # type: ignore
+    @property
+    def count_katu(self) -> int:
+        return self.good
+
+
+class LazerReplayData(BaseModel):
+    mods: list[LazerMod]
+    statistics: LazerScoreStatistics
+    maximum_statistics: LazerScoreStatistics
+
+
+class LazerScore(BaseModel):
+    id: int
+    accuracy: float
+    beatmap_id: int
+    max_combo: int
+    maximum_statistics: LazerScoreStatistics
+    mods: list[LazerMod]
+    passed: bool
+    rank: str
+    ruleset_id: int
+    ended_at: datetime
+    statistics: LazerScoreStatistics
+    total_score: int
+    user_id: int
+    replay: bool
+    type: str
+    current_user_attributes: CurrentUserAttributes
+    beatmap: Beatmap
+    beatmapset: Beatmapset
+    user: User
+    build_id: Optional[int] = None
+    started_at: Optional[datetime] = None
+    best_id: Optional[int] = None
+    legacy_perfect: Optional[bool] = None
+    pp: Optional[float] = None
+    weight: Optional[ScoreWeight] = None
+
+    @computed_field  # type: ignore
+    @property
+    def mods_str(self) -> str:
+        return "".join(str(mod) for mod in self.mods)
+
+    @computed_field  # type: ignore
+    @property
+    def created_at(self) -> datetime:
+        return self.ended_at
+
+    @computed_field  # type: ignore
+    @property
+    def completion(self) -> float:
+        """Beatmap completion.
+
+        :raises ValueError: If beatmap is None
+        :raises ValueError: If mode is unknown
+        :return: Beatmap completion of a score (%). 100% for passes
+        :rtype: float
+        """
+        if self.beatmap is None:
+            raise ValueError("Beatmap object is not set.")
+
+        if self.passed:
+            return 100.0
+
+        return calculate_score_completion(self.statistics, self.beatmap)
+
+    @computed_field  # type: ignore
+    @property
+    def mode(self) -> Gamemode:
+        return Gamemode(self.ruleset_id)
+
+    @computed_field  # type: ignore
+    @property
+    def score(self) -> int:
+        return self.total_score
+
+    @computed_field  # type: ignore
+    @property
+    def score_url(self) -> Optional[str]:
+        r"""Link to the score.
+
+        :return: Link to the score on the osu! website
+        :rtype: Optional[str]
+        """
+        if (not self.id and not self.best_id) or not self.passed:
+            return None
+        return (
+            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
+            if self.best_id
+            else f"https://osu.ppy.sh/scores/{self.id}"
+        )
+
+    @computed_field  # type: ignore
+    @property
+    def replay_url(self) -> Optional[str]:
+        r"""Link to the replay.
+
+        :return: Link to download the replay on the osu! website
+        :rtype: Optional[str]
+        """
+        if not self.replay:
+            return None
+        return (
+            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
+            if self.best_id
+            else f"https://osu.ppy.sh/scores/{self.id}/download"
+        )
+
+    @model_validator(mode="before")
+    @classmethod
+    def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if not values["passed"]:
+            values["rank"] = "F"
+        return values
```

### Comparing `aiosu-2.0.1/aiosu/models/legacy/match.py` & `aiosu-2.0.2/aiosu/models/legacy/match.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from __future__ import annotations
-
-from datetime import datetime
-from enum import IntEnum
-from enum import unique
-from typing import Optional
-from typing import TYPE_CHECKING
-
-from pydantic import Field
-from pydantic import field_validator
-from pydantic import model_validator
-
-from ..base import BaseModel
-from ..gamemode import Gamemode
-from ..mods import Mods
-from ..score import ScoreStatistics
-
-if TYPE_CHECKING:
-    from typing import Any
-
-__all__ = (
-    "MatchTeam",
-    "MatchScoringType",
-    "MatchTeamType",
-    "MatchScore",
-    "MatchGame",
-    "Match",
-)
-
-
-@unique
-class MatchTeam(IntEnum):
-    NONE = 0
-    BLUE = 1
-    RED = 2
-
-
-@unique
-class MatchScoringType(IntEnum):
-    SCORE = 0
-    ACCURACY = 1
-    COMBO = 2
-    SCOREV2 = 3
-
-
-@unique
-class MatchTeamType(IntEnum):
-    HEADTOHEAD = 0
-    COOP = 1
-    TEAMVS = 2
-    TAGTEAMVS = 3
-
-
-class MatchScore(BaseModel):
-    slot: int
-    team: MatchTeam
-    user_id: int
-    score: int
-    max_combo: int = Field(alias="maxcombo")
-    passed: bool = Field(alias="pass")
-    perfect: bool
-    enabled_mods: Mods
-    statistics: ScoreStatistics
-
-    def get_full_mods(self, game: MatchGame) -> Mods:
-        r"""Get the mods including globals from the match.
-
-        :param game: The match the score took place in
-        :type game: MatchGame
-        :return: Mods list of Mod objects
-        :rtype: Mods
-        """
-        return Mods(self.enabled_mods | game.mods)
-
-    @model_validator(mode="before")
-    @classmethod
-    def _set_statistics(cls, values: dict[str, Any]) -> dict[str, Any]:
-        values["statistics"] = ScoreStatistics._from_api_v1(values)
-        return values
-
-    @field_validator("enabled_mods", mode="before")
-    @classmethod
-    def _set_enabled_mods(cls, v: Any) -> int:
-        if v is not None:
-            return int(v)
-        return 0
-
-    @field_validator("team", mode="before")
-    @classmethod
-    def _set_team(cls, v: Any) -> int:
-        return int(v)
-
-
-class MatchGame(BaseModel):
-    """Multiplayer game API object."""
-
-    id: int = Field(alias="game_id")
-    start_time: datetime
-    beatmap_id: int
-    mode: Gamemode = Field(alias="play_mode")
-    match_type: int
-    scoring_type: MatchScoringType
-    team_type: MatchTeamType
-    scores: list[MatchScore]
-    mods: Mods
-    end_time: Optional[datetime] = None
-    """None if game was aborted."""
-
-    @field_validator("mode", mode="before")
-    @classmethod
-    def _set_mode(cls, v: Any) -> int:
-        return int(v)
-
-    @field_validator("mods", mode="before")
-    @classmethod
-    def _set_mods(cls, v: Any) -> int:
-        if v is not None:
-            return int(v)
-        return 0
-
-    @field_validator("scoring_type", mode="before")
-    @classmethod
-    def _set_scoring_type(cls, v: Any) -> int:
-        return int(v)
-
-    @field_validator("team_type", mode="before")
-    @classmethod
-    def _set_team_type(cls, v: Any) -> int:
-        return int(v)
-
-
-class Match(BaseModel):
-    """Multiplayer match API object."""
-
-    id: int = Field(alias="match_id")
-    name: str
-    start_time: datetime
-    games: list[MatchGame]
-    end_time: Optional[datetime] = None
-    """None if game is ongoing."""
-
-    @model_validator(mode="before")
-    @classmethod
-    def _format_values(cls, values: dict[str, Any]) -> dict[str, Any]:
-        return {**values["match"], "games": values["games"]}
+from __future__ import annotations
+
+from datetime import datetime
+from enum import IntEnum
+from enum import unique
+from typing import Optional
+from typing import TYPE_CHECKING
+
+from pydantic import Field
+from pydantic import field_validator
+from pydantic import model_validator
+
+from ..base import BaseModel
+from ..gamemode import Gamemode
+from ..mods import Mods
+from ..score import ScoreStatistics
+
+if TYPE_CHECKING:
+    from typing import Any
+
+__all__ = (
+    "MatchTeam",
+    "MatchScoringType",
+    "MatchTeamType",
+    "MatchScore",
+    "MatchGame",
+    "Match",
+)
+
+
+@unique
+class MatchTeam(IntEnum):
+    NONE = 0
+    BLUE = 1
+    RED = 2
+
+
+@unique
+class MatchScoringType(IntEnum):
+    SCORE = 0
+    ACCURACY = 1
+    COMBO = 2
+    SCOREV2 = 3
+
+
+@unique
+class MatchTeamType(IntEnum):
+    HEADTOHEAD = 0
+    COOP = 1
+    TEAMVS = 2
+    TAGTEAMVS = 3
+
+
+class MatchScore(BaseModel):
+    slot: int
+    team: MatchTeam
+    user_id: int
+    score: int
+    max_combo: int = Field(alias="maxcombo")
+    passed: bool = Field(alias="pass")
+    perfect: bool
+    enabled_mods: Mods
+    statistics: ScoreStatistics
+
+    def get_full_mods(self, game: MatchGame) -> Mods:
+        r"""Get the mods including globals from the match.
+
+        :param game: The match the score took place in
+        :type game: MatchGame
+        :return: Mods list of Mod objects
+        :rtype: Mods
+        """
+        return Mods(self.enabled_mods | game.mods)
+
+    @model_validator(mode="before")
+    @classmethod
+    def _set_statistics(cls, values: dict[str, Any]) -> dict[str, Any]:
+        values["statistics"] = ScoreStatistics._from_api_v1(values)
+        return values
+
+    @field_validator("enabled_mods", mode="before")
+    @classmethod
+    def _set_enabled_mods(cls, v: Any) -> int:
+        if v is not None:
+            return int(v)
+        return 0
+
+    @field_validator("team", mode="before")
+    @classmethod
+    def _set_team(cls, v: Any) -> int:
+        return int(v)
+
+
+class MatchGame(BaseModel):
+    """Multiplayer game API object."""
+
+    id: int = Field(alias="game_id")
+    start_time: datetime
+    beatmap_id: int
+    mode: Gamemode = Field(alias="play_mode")
+    match_type: int
+    scoring_type: MatchScoringType
+    team_type: MatchTeamType
+    scores: list[MatchScore]
+    mods: Mods
+    end_time: Optional[datetime] = None
+    """None if game was aborted."""
+
+    @field_validator("mode", mode="before")
+    @classmethod
+    def _set_mode(cls, v: Any) -> int:
+        return int(v)
+
+    @field_validator("mods", mode="before")
+    @classmethod
+    def _set_mods(cls, v: Any) -> int:
+        if v is not None:
+            return int(v)
+        return 0
+
+    @field_validator("scoring_type", mode="before")
+    @classmethod
+    def _set_scoring_type(cls, v: Any) -> int:
+        return int(v)
+
+    @field_validator("team_type", mode="before")
+    @classmethod
+    def _set_team_type(cls, v: Any) -> int:
+        return int(v)
+
+
+class Match(BaseModel):
+    """Multiplayer match API object."""
+
+    id: int = Field(alias="match_id")
+    name: str
+    start_time: datetime
+    games: list[MatchGame]
+    end_time: Optional[datetime] = None
+    """None if game is ongoing."""
+
+    @model_validator(mode="before")
+    @classmethod
+    def _format_values(cls, values: dict[str, Any]) -> dict[str, Any]:
+        return {**values["match"], "games": values["games"]}
```

### Comparing `aiosu-2.0.1/aiosu/models/news.py` & `aiosu-2.0.2/aiosu/models/news.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-This module contains models for news post objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Literal
-from typing import Optional
-
-from .base import BaseModel
-from .common import CursorModel
-
-
-__all__ = (
-    "NewsPost",
-    "Navigation",
-    "NewsListing",
-    "NewsSearch",
-)
-
-
-class NewsSearch(BaseModel):
-    limit: int
-    sort: Literal["published_desc"]
-
-
-class Navigation(BaseModel):
-    newer: Optional[NewsPost] = None
-    older: Optional[NewsPost] = None
-
-
-class NewsPost(BaseModel):
-    id: int
-    title: str
-    slug: str
-    author: str
-    edit_url: str
-    published_at: datetime
-    updated_at: datetime
-    first_image: Optional[str] = None
-    content: Optional[str] = None
-    preview: Optional[str] = None
-    navigation: Optional[Navigation] = None
-
-
-class NewsSidebar(BaseModel):
-    current_year: int
-    years: list[int]
-    news_posts: list[NewsPost]
-
-
-class NewsListing(CursorModel):
-    news_posts: list[NewsPost]
-    search: NewsSearch
-    news_sidebar: NewsSidebar
-
-
-Navigation.model_rebuild()
+"""
+This module contains models for news post objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Literal
+from typing import Optional
+
+from .base import BaseModel
+from .common import CursorModel
+
+
+__all__ = (
+    "NewsPost",
+    "Navigation",
+    "NewsListing",
+    "NewsSearch",
+)
+
+
+class NewsSearch(BaseModel):
+    limit: int
+    sort: Literal["published_desc"]
+
+
+class Navigation(BaseModel):
+    newer: Optional[NewsPost] = None
+    older: Optional[NewsPost] = None
+
+
+class NewsPost(BaseModel):
+    id: int
+    title: str
+    slug: str
+    author: str
+    edit_url: str
+    published_at: datetime
+    updated_at: datetime
+    first_image: Optional[str] = None
+    content: Optional[str] = None
+    preview: Optional[str] = None
+    navigation: Optional[Navigation] = None
+
+
+class NewsSidebar(BaseModel):
+    current_year: int
+    years: list[int]
+    news_posts: list[NewsPost]
+
+
+class NewsListing(CursorModel):
+    news_posts: list[NewsPost]
+    search: NewsSearch
+    news_sidebar: NewsSidebar
+
+
+Navigation.model_rebuild()
```

### Comparing `aiosu-2.0.1/aiosu/models/oauthtoken.py` & `aiosu-2.0.2/aiosu/models/oauthtoken.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""
-This module contains models for API v2 token objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from datetime import timedelta
-from functools import cached_property
-from typing import TYPE_CHECKING
-
-import jwt
-from pydantic import computed_field
-from pydantic import model_validator
-
-from .base import FrozenModel
-from .scopes import Scopes
-
-if TYPE_CHECKING:
-    from typing import Any
-
-__all__ = ("OAuthToken",)
-
-
-class OAuthToken(FrozenModel):
-    token_type: str = "Bearer"
-    """Defaults to 'Bearer'"""
-    access_token: str = ""
-    refresh_token: str = ""
-    expires_on: datetime = datetime.utcfromtimestamp(0)
-    """Can be a datetime.datetime object or a string. Alternatively, expires_in may be passed representing the number of seconds the token will be valid for."""
-
-    @computed_field  # type: ignore
-    @cached_property
-    def owner_id(self) -> int:
-        if not self.access_token:
-            return 0
-        decoded = jwt.decode(self.access_token, options={"verify_signature": False})
-        if decoded["sub"]:
-            return int(decoded["sub"])
-        return 0
-
-    @computed_field  # type: ignore
-    @cached_property
-    def scopes(self) -> Scopes:
-        if not self.access_token:
-            return Scopes.PUBLIC
-        decoded = jwt.decode(self.access_token, options={"verify_signature": False})
-        return Scopes.from_api_list(decoded["scopes"])
-
-    @computed_field  # type: ignore
-    @cached_property
-    def can_refresh(self) -> bool:
-        """Returns True if the token can be refreshed."""
-        return bool(self.refresh_token)
-
-    @model_validator(mode="before")
-    @classmethod
-    def _set_expires_on(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if isinstance(values.get("expires_in"), int):
-            values["expires_on"] = datetime.utcnow() + timedelta(
-                seconds=values["expires_in"],
-            )
-        return values
+"""
+This module contains models for API v2 token objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from datetime import timedelta
+from functools import cached_property
+from typing import TYPE_CHECKING
+
+import jwt
+from pydantic import computed_field
+from pydantic import model_validator
+
+from .base import FrozenModel
+from .scopes import Scopes
+
+if TYPE_CHECKING:
+    from typing import Any
+
+__all__ = ("OAuthToken",)
+
+
+class OAuthToken(FrozenModel):
+    token_type: str = "Bearer"
+    """Defaults to 'Bearer'"""
+    access_token: str = ""
+    refresh_token: str = ""
+    expires_on: datetime = datetime.utcfromtimestamp(31536000)
+    """Can be a datetime.datetime object or a string. Alternatively, expires_in may be passed representing the number of seconds the token will be valid for."""
+
+    @computed_field  # type: ignore
+    @cached_property
+    def owner_id(self) -> int:
+        if not self.access_token:
+            return 0
+        decoded = jwt.decode(self.access_token, options={"verify_signature": False})
+        if decoded["sub"]:
+            return int(decoded["sub"])
+        return 0
+
+    @computed_field  # type: ignore
+    @cached_property
+    def scopes(self) -> Scopes:
+        if not self.access_token:
+            return Scopes.PUBLIC
+        decoded = jwt.decode(self.access_token, options={"verify_signature": False})
+        return Scopes.from_api_list(decoded["scopes"])
+
+    @computed_field  # type: ignore
+    @cached_property
+    def can_refresh(self) -> bool:
+        """Returns True if the token can be refreshed."""
+        return bool(self.refresh_token)
+
+    @model_validator(mode="before")
+    @classmethod
+    def _set_expires_on(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if isinstance(values.get("expires_in"), int):
+            values["expires_on"] = datetime.utcnow() + timedelta(
+                seconds=values["expires_in"],
+            )
+        return values
```

### Comparing `aiosu-2.0.1/aiosu/models/performance.py` & `aiosu-2.0.2/aiosu/models/performance.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-This module contains models for API v2 difficulty attribute objects.
-"""
-from __future__ import annotations
-
-import abc
-
-from .base import BaseModel
-
-__all__ = (
-    "PerformanceAttributes",
-    "OsuPerformanceAttributes",
-    "TaikoPerformanceAttributes",
-    "ManiaPerformanceAttributes",
-    "CatchPerformanceAttributes",
-)
-
-
-class PerformanceAttributes(BaseModel, abc.ABC):
-    total: float
-
-
-class OsuPerformanceAttributes(PerformanceAttributes):
-    aim: float
-    speed: float
-    accuracy: float
-    flashlight: float
-    effective_miss_count: float
-
-
-class TaikoPerformanceAttributes(PerformanceAttributes):
-    difficulty: float
-    accuracy: float
-    effective_miss_count: float
-
-
-class ManiaPerformanceAttributes(PerformanceAttributes):
-    difficulty: float
-
-
-class CatchPerformanceAttributes(PerformanceAttributes):
-    ...
+"""
+This module contains models for API v2 difficulty attribute objects.
+"""
+from __future__ import annotations
+
+import abc
+
+from .base import BaseModel
+
+__all__ = (
+    "PerformanceAttributes",
+    "OsuPerformanceAttributes",
+    "TaikoPerformanceAttributes",
+    "ManiaPerformanceAttributes",
+    "CatchPerformanceAttributes",
+)
+
+
+class PerformanceAttributes(BaseModel, abc.ABC):
+    total: float
+
+
+class OsuPerformanceAttributes(PerformanceAttributes):
+    aim: float
+    speed: float
+    accuracy: float
+    flashlight: float
+    effective_miss_count: float
+
+
+class TaikoPerformanceAttributes(PerformanceAttributes):
+    difficulty: float
+    accuracy: float
+    effective_miss_count: float
+
+
+class ManiaPerformanceAttributes(PerformanceAttributes):
+    difficulty: float
+
+
+class CatchPerformanceAttributes(PerformanceAttributes):
+    ...
```

### Comparing `aiosu-2.0.1/aiosu/models/rankings.py` & `aiosu-2.0.2/aiosu/models/rankings.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-This module contains models for rankings.
-"""
-from __future__ import annotations
-
-from typing import Literal
-from typing import Optional
-
-from .beatmap import Beatmapset
-from .common import CursorModel
-from .spotlight import Spotlight
-from .user import UserStats
-
-
-__all__ = (
-    "RankingFilter",
-    "RankingVariant",
-    "RankingType",
-    "Rankings",
-)
-
-RankingFilter = Literal["all", "friends"]
-RankingType = Literal["performance", "score", "country", "charts"]
-RankingVariant = Literal["4k", "7k"]
-
-
-class Rankings(CursorModel):
-    ranking: list[UserStats]
-    total: Optional[int] = None
-    spotlight: Optional[Spotlight] = None
-    beatmapsets: Optional[list[Beatmapset]] = None
+"""
+This module contains models for rankings.
+"""
+from __future__ import annotations
+
+from typing import Literal
+from typing import Optional
+
+from .beatmap import Beatmapset
+from .common import CursorModel
+from .spotlight import Spotlight
+from .user import UserStats
+
+
+__all__ = (
+    "RankingFilter",
+    "RankingVariant",
+    "RankingType",
+    "Rankings",
+)
+
+RankingFilter = Literal["all", "friends"]
+RankingType = Literal["performance", "score", "country", "charts"]
+RankingVariant = Literal["4k", "7k"]
+
+
+class Rankings(CursorModel):
+    ranking: list[UserStats]
+    total: Optional[int] = None
+    spotlight: Optional[Spotlight] = None
+    beatmapsets: Optional[list[Beatmapset]] = None
```

### Comparing `aiosu-2.0.1/aiosu/models/scopes.py` & `aiosu-2.0.2/aiosu/models/scopes.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-This module contains models for API v2 scopes.
-"""
-from __future__ import annotations
-
-from enum import IntFlag
-from enum import unique
-
-__all__ = (
-    "Scopes",
-    "VALID_CLIENT_SCOPES",
-)
-
-
-@unique
-class Scopes(IntFlag):
-    NONE = 0
-    PUBLIC = 1 << 0
-    IDENTIFY = 1 << 1
-    FRIENDS_READ = 1 << 2
-    FORUM_WRITE = 1 << 3
-    DELEGATE = 1 << 4
-    CHAT_WRITE = 1 << 5
-    LAZER = 1 << 6  # unused, lazer endpoints are not planned for support
-
-    def __flags__(self) -> list[Scopes]:
-        scopes_list = [scope for scope in Scopes if self & scope]
-        return scopes_list
-
-    def __str__(self) -> str:
-        return " ".join(
-            scope_name
-            for scope_name, scope in API_SCOPE_NAMES.items()
-            if scope in self.__flags__()
-        )
-
-    @classmethod
-    def from_api_list(cls, scopes: list[str]) -> Scopes:
-        return cls(sum(API_SCOPE_NAMES[scope] for scope in scopes))
-
-
-API_SCOPE_NAMES = {
-    "public": Scopes.PUBLIC,
-    "identify": Scopes.IDENTIFY,
-    "friends.read": Scopes.FRIENDS_READ,
-    "forum.write": Scopes.FORUM_WRITE,
-    "delegate": Scopes.DELEGATE,
-    "chat.write": Scopes.CHAT_WRITE,
-    "lazer": Scopes.LAZER,
-}
-VALID_CLIENT_SCOPES = Scopes.PUBLIC | Scopes.DELEGATE
+"""
+This module contains models for API v2 scopes.
+"""
+from __future__ import annotations
+
+from enum import IntFlag
+from enum import unique
+
+__all__ = (
+    "Scopes",
+    "VALID_CLIENT_SCOPES",
+)
+
+
+@unique
+class Scopes(IntFlag):
+    NONE = 0
+    PUBLIC = 1 << 0
+    IDENTIFY = 1 << 1
+    FRIENDS_READ = 1 << 2
+    FORUM_WRITE = 1 << 3
+    DELEGATE = 1 << 4
+    CHAT_WRITE = 1 << 5
+    LAZER = 1 << 6  # unused, lazer endpoints are not planned for support
+
+    def __flags__(self) -> list[Scopes]:
+        scopes_list = [scope for scope in Scopes if self & scope]
+        return scopes_list
+
+    def __str__(self) -> str:
+        return " ".join(
+            scope_name
+            for scope_name, scope in API_SCOPE_NAMES.items()
+            if scope in self.__flags__()
+        )
+
+    @classmethod
+    def from_api_list(cls, scopes: list[str]) -> Scopes:
+        return cls(sum(API_SCOPE_NAMES[scope] for scope in scopes))
+
+
+API_SCOPE_NAMES = {
+    "public": Scopes.PUBLIC,
+    "identify": Scopes.IDENTIFY,
+    "friends.read": Scopes.FRIENDS_READ,
+    "forum.write": Scopes.FORUM_WRITE,
+    "delegate": Scopes.DELEGATE,
+    "chat.write": Scopes.CHAT_WRITE,
+    "lazer": Scopes.LAZER,
+}
+VALID_CLIENT_SCOPES = Scopes.PUBLIC | Scopes.DELEGATE
```

### Comparing `aiosu-2.0.1/aiosu/models/score.py` & `aiosu-2.0.2/aiosu/models/score.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-"""
-This module contains models for Score objects.
-"""
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Optional
-from typing import TYPE_CHECKING
-
-from pydantic import computed_field
-from pydantic import model_validator
-
-from ..utils.accuracy import CatchAccuracyCalculator
-from ..utils.accuracy import ManiaAccuracyCalculator
-from ..utils.accuracy import OsuAccuracyCalculator
-from ..utils.accuracy import TaikoAccuracyCalculator
-from .base import BaseModel
-from .beatmap import Beatmap
-from .beatmap import Beatmapset
-from .common import CurrentUserAttributes
-from .gamemode import Gamemode
-from .mods import Mods
-from .user import User
-
-if TYPE_CHECKING:
-    from typing import Any
-    from .. import v1
-
-__all__ = (
-    "Score",
-    "ScoreStatistics",
-    "ScoreWeight",
-    "calculate_score_completion",
-)
-
-accuracy_calculators = {
-    "osu": OsuAccuracyCalculator(),
-    "mania": ManiaAccuracyCalculator(),
-    "taiko": TaikoAccuracyCalculator(),
-    "fruits": CatchAccuracyCalculator(),
-}
-
-
-def calculate_score_completion(
-    mode: Gamemode,
-    statistics: ScoreStatistics,
-    beatmap: Beatmap,
-) -> float:
-    """Calculates completion for a score.
-
-    :param mode: The gamemode of the score
-    :type mode: aiosu.models.gamemode.Gamemode
-    :param statistics: The statistics of the score
-    :type statistics: aiosu.models.score.ScoreStatistics
-    :param beatmap: The beatmap of the score
-    :type beatmap: aiosu.models.beatmap.Beatmap
-    :raises ValueError: If the gamemode is unknown
-    :return: Completion for the given score
-    :rtype: float
-    """
-    if mode == Gamemode.STANDARD:
-        return (
-            (
-                statistics.count_300
-                + statistics.count_100
-                + statistics.count_50
-                + statistics.count_miss
-            )
-            / beatmap.count_objects
-        ) * 100
-    elif mode == Gamemode.TAIKO:
-        return (
-            (statistics.count_300 + statistics.count_100 + statistics.count_miss)
-            / beatmap.count_objects
-        ) * 100
-    elif mode == Gamemode.CTB:
-        return (
-            (statistics.count_300 + statistics.count_100 + +statistics.count_miss)
-            / beatmap.count_objects
-        ) * 100
-    elif mode == Gamemode.MANIA:
-        return (
-            (
-                statistics.count_300
-                + statistics.count_100
-                + statistics.count_50
-                + statistics.count_miss
-                + statistics.count_geki
-                + statistics.count_katu
-            )
-            / beatmap.count_objects
-        ) * 100
-    raise ValueError("Unknown mode specified.")
-
-
-class ScoreWeight(BaseModel):
-    percentage: float
-    pp: float
-
-
-class ScoreStatistics(BaseModel):
-    count_50: int
-    count_100: int
-    count_300: int
-    count_miss: int
-    count_geki: int
-    count_katu: int
-
-    @model_validator(mode="before")
-    @classmethod
-    def _convert_none_to_zero(cls, values: dict[str, Any]) -> dict[str, Any]:
-        # Lazer API returns null for some statistics
-        for key in values:
-            if values[key] is None:
-                values[key] = 0
-        return values
-
-    @classmethod
-    def _from_api_v1(cls, data: Any) -> ScoreStatistics:
-        return cls.model_validate(
-            {
-                "count_50": data["count50"],
-                "count_100": data["count100"],
-                "count_300": data["count300"],
-                "count_geki": data["countgeki"],
-                "count_katu": data["countkatu"],
-                "count_miss": data["countmiss"],
-            },
-        )
-
-
-class Score(BaseModel):
-    user_id: int
-    accuracy: float
-    mods: Mods
-    score: int
-    max_combo: int
-    passed: bool
-    perfect: bool
-    statistics: ScoreStatistics
-    rank: str
-    created_at: datetime
-    mode: Gamemode
-    replay: bool
-    id: Optional[int] = None
-    """Always present except for API v1 recent scores."""
-    pp: Optional[float] = 0
-    best_id: Optional[int] = None
-    beatmap: Optional[Beatmap] = None
-    beatmapset: Optional[Beatmapset] = None
-    weight: Optional[ScoreWeight] = None
-    user: Optional[User] = None
-    rank_global: Optional[int] = None
-    rank_country: Optional[int] = None
-    type: Optional[str] = None
-    current_user_attributes: Optional[CurrentUserAttributes] = None
-    beatmap_id: Optional[int] = None
-    """Only present on API v1"""
-
-    @computed_field  # type: ignore
-    @property
-    def completion(self) -> float:
-        """Beatmap completion.
-
-        :raises ValueError: If beatmap is None
-        :raises ValueError: If mode is unknown
-        :return: Beatmap completion of a score (%). 100% for passes
-        :rtype: float
-        """
-        if not self.beatmap:
-            raise ValueError("Beatmap object is not set.")
-
-        if self.passed:
-            return 100.0
-
-        return calculate_score_completion(self.mode, self.statistics, self.beatmap)
-
-    @computed_field  # type: ignore
-    @property
-    def score_url(self) -> Optional[str]:
-        r"""Link to the score.
-
-        :return: Link to the score on the osu! website
-        :rtype: Optional[str]
-        """
-        if (not self.id and not self.best_id) or not self.passed:
-            return None
-        return (
-            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
-            if self.best_id
-            else f"https://osu.ppy.sh/scores/{self.id}"
-        )
-
-    @computed_field  # type: ignore
-    @property
-    def replay_url(self) -> Optional[str]:
-        r"""Link to the replay.
-
-        :return: Link to download the replay on the osu! website
-        :rtype: Optional[str]
-        """
-        if not self.replay:
-            return None
-        return (
-            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
-            if self.best_id
-            else f"https://osu.ppy.sh/scores/{self.id}/download"
-        )
-
-    @model_validator(mode="before")
-    @classmethod
-    def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if not values["passed"]:
-            values["rank"] = "F"
-        return values
-
-    async def request_beatmap(self, client: v1.Client) -> None:
-        r"""For v1 Scores: requests the beatmap from the API and sets it.
-
-        :param client: An API v1 Client
-        :type client: aiosu.v1.client.Client
-        """
-        if self.beatmap_id is None:
-            raise ValueError("Score has unknown beatmap ID")
-        if self.beatmap is None and self.beatmapset is None:
-            sets = await client.get_beatmap(
-                mode=self.mode,
-                beatmap_id=self.beatmap_id,
-            )
-            self.beatmapset = sets[0]
-            self.beatmap = sets[0].beatmaps[0]  # type: ignore
-
-    @classmethod
-    def _from_api_v1(
-        cls,
-        data: Any,
-        mode: Gamemode,
-    ) -> Score:
-        statistics = ScoreStatistics._from_api_v1(data)
-        score = cls.model_validate(
-            {
-                "id": data["score_id"],
-                "user_id": data["user_id"],
-                "accuracy": 0.0,
-                "mods": int(data["enabled_mods"]),
-                "score": data["score"],
-                "pp": data.get("pp", 0.0),
-                "max_combo": data["maxcombo"],
-                "passed": data["rank"] != "F",
-                "perfect": data["perfect"],
-                "statistics": statistics,
-                "rank": data["rank"],
-                "created_at": data["date"],
-                "mode": mode,
-                "beatmap_id": data.get("beatmap_id"),
-                "replay": data.get("replay_available", False),
-            },
-        )
-        score.accuracy = accuracy_calculators[str(mode)].calculate(score)
-        return score
+"""
+This module contains models for Score objects.
+"""
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Optional
+from typing import TYPE_CHECKING
+
+from pydantic import computed_field
+from pydantic import model_validator
+
+from ..utils.accuracy import CatchAccuracyCalculator
+from ..utils.accuracy import ManiaAccuracyCalculator
+from ..utils.accuracy import OsuAccuracyCalculator
+from ..utils.accuracy import TaikoAccuracyCalculator
+from .base import BaseModel
+from .beatmap import Beatmap
+from .beatmap import Beatmapset
+from .common import CurrentUserAttributes
+from .gamemode import Gamemode
+from .mods import Mods
+from .user import User
+
+if TYPE_CHECKING:
+    from typing import Any
+    from .. import v1
+
+__all__ = (
+    "Score",
+    "ScoreStatistics",
+    "ScoreWeight",
+    "calculate_score_completion",
+)
+
+accuracy_calculators = {
+    "osu": OsuAccuracyCalculator(),
+    "mania": ManiaAccuracyCalculator(),
+    "taiko": TaikoAccuracyCalculator(),
+    "fruits": CatchAccuracyCalculator(),
+}
+
+
+def calculate_score_completion(
+    mode: Gamemode,
+    statistics: ScoreStatistics,
+    beatmap: Beatmap,
+) -> float:
+    """Calculates completion for a score.
+
+    :param mode: The gamemode of the score
+    :type mode: aiosu.models.gamemode.Gamemode
+    :param statistics: The statistics of the score
+    :type statistics: aiosu.models.score.ScoreStatistics
+    :param beatmap: The beatmap of the score
+    :type beatmap: aiosu.models.beatmap.Beatmap
+    :raises ValueError: If the gamemode is unknown
+    :return: Completion for the given score
+    :rtype: float
+    """
+    if mode == Gamemode.STANDARD:
+        return (
+            (
+                statistics.count_300
+                + statistics.count_100
+                + statistics.count_50
+                + statistics.count_miss
+            )
+            / beatmap.count_objects
+        ) * 100
+    elif mode == Gamemode.TAIKO:
+        return (
+            (statistics.count_300 + statistics.count_100 + statistics.count_miss)
+            / beatmap.count_objects
+        ) * 100
+    elif mode == Gamemode.CTB:
+        return (
+            (statistics.count_300 + statistics.count_100 + +statistics.count_miss)
+            / beatmap.count_objects
+        ) * 100
+    elif mode == Gamemode.MANIA:
+        return (
+            (
+                statistics.count_300
+                + statistics.count_100
+                + statistics.count_50
+                + statistics.count_miss
+                + statistics.count_geki
+                + statistics.count_katu
+            )
+            / beatmap.count_objects
+        ) * 100
+    raise ValueError("Unknown mode specified.")
+
+
+class ScoreWeight(BaseModel):
+    percentage: float
+    pp: float
+
+
+class ScoreStatistics(BaseModel):
+    count_50: int
+    count_100: int
+    count_300: int
+    count_miss: int
+    count_geki: int
+    count_katu: int
+
+    @model_validator(mode="before")
+    @classmethod
+    def _convert_none_to_zero(cls, values: dict[str, Any]) -> dict[str, Any]:
+        # Lazer API returns null for some statistics
+        for key in values:
+            if values[key] is None:
+                values[key] = 0
+        return values
+
+    @classmethod
+    def _from_api_v1(cls, data: Any) -> ScoreStatistics:
+        return cls.model_validate(
+            {
+                "count_50": data["count50"],
+                "count_100": data["count100"],
+                "count_300": data["count300"],
+                "count_geki": data["countgeki"],
+                "count_katu": data["countkatu"],
+                "count_miss": data["countmiss"],
+            },
+        )
+
+
+class Score(BaseModel):
+    user_id: int
+    accuracy: float
+    mods: Mods
+    score: int
+    max_combo: int
+    passed: bool
+    perfect: bool
+    statistics: ScoreStatistics
+    rank: str
+    created_at: datetime
+    mode: Gamemode
+    replay: bool
+    id: Optional[int] = None
+    """Always present except for API v1 recent scores."""
+    pp: Optional[float] = 0
+    best_id: Optional[int] = None
+    beatmap: Optional[Beatmap] = None
+    beatmapset: Optional[Beatmapset] = None
+    weight: Optional[ScoreWeight] = None
+    user: Optional[User] = None
+    rank_global: Optional[int] = None
+    rank_country: Optional[int] = None
+    type: Optional[str] = None
+    current_user_attributes: Optional[CurrentUserAttributes] = None
+    beatmap_id: Optional[int] = None
+    """Only present on API v1"""
+
+    @computed_field  # type: ignore
+    @property
+    def completion(self) -> float:
+        """Beatmap completion.
+
+        :raises ValueError: If beatmap is None
+        :raises ValueError: If mode is unknown
+        :return: Beatmap completion of a score (%). 100% for passes
+        :rtype: float
+        """
+        if not self.beatmap:
+            raise ValueError("Beatmap object is not set.")
+
+        if self.passed:
+            return 100.0
+
+        return calculate_score_completion(self.mode, self.statistics, self.beatmap)
+
+    @computed_field  # type: ignore
+    @property
+    def score_url(self) -> Optional[str]:
+        r"""Link to the score.
+
+        :return: Link to the score on the osu! website
+        :rtype: Optional[str]
+        """
+        if (not self.id and not self.best_id) or not self.passed:
+            return None
+        return (
+            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}"
+            if self.best_id
+            else f"https://osu.ppy.sh/scores/{self.id}"
+        )
+
+    @computed_field  # type: ignore
+    @property
+    def replay_url(self) -> Optional[str]:
+        r"""Link to the replay.
+
+        :return: Link to download the replay on the osu! website
+        :rtype: Optional[str]
+        """
+        if not self.replay:
+            return None
+        return (
+            f"https://osu.ppy.sh/scores/{self.mode.name_api}/{self.best_id}/download"
+            if self.best_id
+            else f"https://osu.ppy.sh/scores/{self.id}/download"
+        )
+
+    @model_validator(mode="before")
+    @classmethod
+    def _fail_rank(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if not values["passed"]:
+            values["rank"] = "F"
+        return values
+
+    async def request_beatmap(self, client: v1.Client) -> None:
+        r"""For v1 Scores: requests the beatmap from the API and sets it.
+
+        :param client: An API v1 Client
+        :type client: aiosu.v1.client.Client
+        """
+        if self.beatmap_id is None:
+            raise ValueError("Score has unknown beatmap ID")
+        if self.beatmap is None and self.beatmapset is None:
+            sets = await client.get_beatmap(
+                mode=self.mode,
+                beatmap_id=self.beatmap_id,
+            )
+            self.beatmapset = sets[0]
+            self.beatmap = sets[0].beatmaps[0]  # type: ignore
+
+    @classmethod
+    def _from_api_v1(
+        cls,
+        data: Any,
+        mode: Gamemode,
+    ) -> Score:
+        statistics = ScoreStatistics._from_api_v1(data)
+        score = cls.model_validate(
+            {
+                "id": data["score_id"],
+                "user_id": data["user_id"],
+                "accuracy": 0.0,
+                "mods": int(data["enabled_mods"]),
+                "score": data["score"],
+                "pp": data.get("pp", 0.0),
+                "max_combo": data["maxcombo"],
+                "passed": data["rank"] != "F",
+                "perfect": data["perfect"],
+                "statistics": statistics,
+                "rank": data["rank"],
+                "created_at": data["date"],
+                "mode": mode,
+                "beatmap_id": data.get("beatmap_id"),
+                "replay": data.get("replay_available", False),
+            },
+        )
+        score.accuracy = accuracy_calculators[str(mode)].calculate(score)
+        return score
```

### Comparing `aiosu-2.0.1/aiosu/utils/accuracy.py` & `aiosu-2.0.2/aiosu/utils/accuracy.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-"""
-This module contains accuracy calculators for osu! gamemodes.
-"""
-from __future__ import annotations
-
-import abc
-from typing import TYPE_CHECKING
-
-from ..models.gamemode import Gamemode
-from ..models.mods import Mod
-
-if TYPE_CHECKING:
-    from typing import Type
-    from typing import Callable
-    from ..models.score import Score
-
-__all__ = [
-    "OsuAccuracyCalculator",
-    "TaikoAccuracyCalculator",
-    "ManiaAccuracyCalculator",
-    "CatchAccuracyCalculator",
-]
-
-cast_int: Callable[..., int] = lambda x: int(x or 0)
-
-
-def get_calculator(mode: Gamemode) -> Type[AbstractAccuracyCalculator]:
-    r"""Returns the accuracy calculator for the given gamemode.
-
-    :param mode: The gamemode to get the calculator for
-    :type mode: aiosu.models.gamemode.Gamemode
-    :raises ValueError: If the gamemode is unknown
-    :return: The accuracy calculator type for the given gamemode
-    :rtype: Type[AbstractAccuracyCalculator]
-    """
-    if mode == Gamemode.STANDARD:
-        return OsuAccuracyCalculator
-    elif mode == Gamemode.TAIKO:
-        return TaikoAccuracyCalculator
-    elif mode == Gamemode.MANIA:
-        return ManiaAccuracyCalculator
-    elif mode == Gamemode.CTB:
-        return CatchAccuracyCalculator
-    else:
-        raise ValueError(f"Unknown gamemode: {mode}")
-
-
-class AbstractAccuracyCalculator(abc.ABC):
-    @staticmethod
-    @abc.abstractmethod
-    def calculate(score: Score) -> float:
-        ...
-
-    @staticmethod
-    @abc.abstractmethod
-    def calculate_weighted(score: Score) -> float:
-        ...
-
-
-class OsuAccuracyCalculator(AbstractAccuracyCalculator):
-    @staticmethod
-    def calculate(score: Score) -> float:
-        r"""Calculates accuracy for an osu!std score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Accuracy for the given score
-        :rtype: float
-        """
-        total_hits = (
-            score.statistics.count_300
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        if total_hits <= 0:
-            return 0.0
-
-        return max(
-            (
-                score.statistics.count_300 * 6.0
-                + score.statistics.count_100 * 2.0
-                + score.statistics.count_50
-            )
-            / (total_hits * 6.0),
-            0.0,
-        )
-
-    @staticmethod
-    def calculate_weighted(score: Score) -> float:
-        r"""Calculates weighted accuracy for an osu!std score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :raises ValueError: If score does not have an associated beatmap
-        :return: Weighted accuracy to be used in pp calculation
-        :rtype: float
-        """
-        if score.beatmap is None:
-            raise ValueError("Given score does not have a beatmap.")
-
-        total_hits = (
-            score.statistics.count_300
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        amount_hit_objects_with_accuracy = cast_int(score.beatmap.count_circles)
-
-        if Mod.ScoreV2 in score.mods:  # TODO: Check for lazer classic mod
-            amount_hit_objects_with_accuracy += cast_int(score.beatmap.count_sliders)
-
-        if amount_hit_objects_with_accuracy <= 0:
-            return 0.0
-
-        return max(
-            (
-                (
-                    score.statistics.count_300
-                    - (total_hits - amount_hit_objects_with_accuracy)
-                )
-                * 6.0
-                + score.statistics.count_100 * 2.0
-                + score.statistics.count_50
-            )
-            / (amount_hit_objects_with_accuracy * 6.0),
-            0.0,
-        )
-
-
-class TaikoAccuracyCalculator(AbstractAccuracyCalculator):
-    @staticmethod
-    def calculate(score: Score) -> float:
-        r"""Calculates accuracy for an osu!taiko score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Accuracy for the given score
-        :rtype: float
-        """
-        total_hits = (
-            score.statistics.count_300
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        if total_hits <= 0:
-            return 0.0
-
-        return max(
-            (score.statistics.count_300 * 2.0 + score.statistics.count_100)
-            / (total_hits * 2.0),
-            0.0,
-        )
-
-    @classmethod
-    def calculate_weighted(cls, score: Score) -> float:
-        r"""Calculates weighted accuracy for an osu!taiko score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Weighted accuracy to be used in pp calculation
-        :rtype: float
-        """
-        return cls.calculate(score)
-
-
-class ManiaAccuracyCalculator(AbstractAccuracyCalculator):
-    @staticmethod
-    def calculate(score: Score) -> float:
-        r"""Calculates accuracy for an osu!mania score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Accuracy for the given score
-        :rtype: float
-        """
-        count_perfect = score.statistics.count_geki
-        count_great = score.statistics.count_300
-        count_good = score.statistics.count_katu
-        count_ok = score.statistics.count_100
-        count_meh = score.statistics.count_50
-        count_miss = score.statistics.count_miss
-
-        total_hits = (
-            count_perfect + count_ok + count_great + count_good + count_meh + count_miss
-        )
-
-        if total_hits <= 0:
-            return 0.0
-
-        if Mod.ScoreV2 in score.mods:
-            return max(
-                (
-                    +(count_perfect * 305)
-                    + (count_great * 300)
-                    + (count_good * 200)
-                    + (count_ok * 100)
-                    + (count_meh * 50)
-                )
-                / (total_hits * 305),
-                0.0,
-            )
-
-        return max(
-            (
-                +((count_perfect + count_great) * 6.0)
-                + (count_good * 4.0)
-                + (count_ok * 2.0)
-                + count_meh
-            )
-            / (total_hits * 6.0),
-            0.0,
-        )
-
-    @staticmethod
-    def calculate_weighted(score: Score) -> float:
-        r"""Calculates weighted accuracy for an osu!mania score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Weighted accuracy to be used in pp calculation
-        :rtype: float
-        """
-        count_perfect = score.statistics.count_geki
-        count_great = score.statistics.count_300
-        count_good = score.statistics.count_katu
-        count_ok = score.statistics.count_100
-        count_meh = score.statistics.count_50
-        count_miss = score.statistics.count_miss
-
-        total_hits = (
-            count_perfect + count_ok + count_great + count_good + count_meh + count_miss
-        )
-
-        if total_hits <= 0:
-            return 0.0
-
-        return max(
-            (
-                +(count_perfect * 320)
-                + (count_great * 300)
-                + (count_good * 200)
-                + (count_ok * 100)
-                + (count_meh * 50)
-            )
-            / (total_hits * 320),
-            0.0,
-        )
-
-
-class CatchAccuracyCalculator(AbstractAccuracyCalculator):
-    @staticmethod
-    def calculate(score: Score) -> float:
-        r"""Calculates accuracy for an osu!catch score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Accuracy for the given score
-        :rtype: float
-        """
-        fruits_hit = score.statistics.count_300
-        ticks_hit = score.statistics.count_100
-        tiny_ticks_hit = score.statistics.count_50
-        tiny_ticks_missed = score.statistics.count_katu
-        misses = score.statistics.count_miss
-
-        total_hits = (
-            tiny_ticks_hit + ticks_hit + fruits_hit + misses + tiny_ticks_missed
-        )
-        successful_hits = tiny_ticks_hit + ticks_hit + fruits_hit
-
-        if total_hits <= 0:
-            return 0.0
-
-        return max(float(successful_hits) / total_hits, 0.0)
-
-    @classmethod
-    def calculate_weighted(cls, score: Score) -> float:
-        r"""Calculates weighted accuracy for an osu!catch score.
-
-        :param score: The score to calculate accuracy for
-        :type score: aiosu.models.score.Score
-        :return: Weighted accuracy to be used in pp calculation
-        :rtype: float
-        """
-        return cls.calculate(score)
+"""
+This module contains accuracy calculators for osu! gamemodes.
+"""
+from __future__ import annotations
+
+import abc
+from typing import TYPE_CHECKING
+
+from ..models.gamemode import Gamemode
+from ..models.mods import Mod
+
+if TYPE_CHECKING:
+    from typing import Type
+    from typing import Callable
+    from ..models.score import Score
+
+__all__ = [
+    "OsuAccuracyCalculator",
+    "TaikoAccuracyCalculator",
+    "ManiaAccuracyCalculator",
+    "CatchAccuracyCalculator",
+]
+
+cast_int: Callable[..., int] = lambda x: int(x or 0)
+
+
+def get_calculator(mode: Gamemode) -> Type[AbstractAccuracyCalculator]:
+    r"""Returns the accuracy calculator for the given gamemode.
+
+    :param mode: The gamemode to get the calculator for
+    :type mode: aiosu.models.gamemode.Gamemode
+    :raises ValueError: If the gamemode is unknown
+    :return: The accuracy calculator type for the given gamemode
+    :rtype: Type[AbstractAccuracyCalculator]
+    """
+    if mode == Gamemode.STANDARD:
+        return OsuAccuracyCalculator
+    elif mode == Gamemode.TAIKO:
+        return TaikoAccuracyCalculator
+    elif mode == Gamemode.MANIA:
+        return ManiaAccuracyCalculator
+    elif mode == Gamemode.CTB:
+        return CatchAccuracyCalculator
+    else:
+        raise ValueError(f"Unknown gamemode: {mode}")
+
+
+class AbstractAccuracyCalculator(abc.ABC):
+    @staticmethod
+    @abc.abstractmethod
+    def calculate(score: Score) -> float:
+        ...
+
+    @staticmethod
+    @abc.abstractmethod
+    def calculate_weighted(score: Score) -> float:
+        ...
+
+
+class OsuAccuracyCalculator(AbstractAccuracyCalculator):
+    @staticmethod
+    def calculate(score: Score) -> float:
+        r"""Calculates accuracy for an osu!std score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Accuracy for the given score
+        :rtype: float
+        """
+        total_hits = (
+            score.statistics.count_300
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        if total_hits <= 0:
+            return 0.0
+
+        return max(
+            (
+                score.statistics.count_300 * 6.0
+                + score.statistics.count_100 * 2.0
+                + score.statistics.count_50
+            )
+            / (total_hits * 6.0),
+            0.0,
+        )
+
+    @staticmethod
+    def calculate_weighted(score: Score) -> float:
+        r"""Calculates weighted accuracy for an osu!std score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :raises ValueError: If score does not have an associated beatmap
+        :return: Weighted accuracy to be used in pp calculation
+        :rtype: float
+        """
+        if score.beatmap is None:
+            raise ValueError("Given score does not have a beatmap.")
+
+        total_hits = (
+            score.statistics.count_300
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        amount_hit_objects_with_accuracy = cast_int(score.beatmap.count_circles)
+
+        if Mod.ScoreV2 in score.mods:  # TODO: Check for lazer classic mod
+            amount_hit_objects_with_accuracy += cast_int(score.beatmap.count_sliders)
+
+        if amount_hit_objects_with_accuracy <= 0:
+            return 0.0
+
+        return max(
+            (
+                (
+                    score.statistics.count_300
+                    - (total_hits - amount_hit_objects_with_accuracy)
+                )
+                * 6.0
+                + score.statistics.count_100 * 2.0
+                + score.statistics.count_50
+            )
+            / (amount_hit_objects_with_accuracy * 6.0),
+            0.0,
+        )
+
+
+class TaikoAccuracyCalculator(AbstractAccuracyCalculator):
+    @staticmethod
+    def calculate(score: Score) -> float:
+        r"""Calculates accuracy for an osu!taiko score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Accuracy for the given score
+        :rtype: float
+        """
+        total_hits = (
+            score.statistics.count_300
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        if total_hits <= 0:
+            return 0.0
+
+        return max(
+            (score.statistics.count_300 * 2.0 + score.statistics.count_100)
+            / (total_hits * 2.0),
+            0.0,
+        )
+
+    @classmethod
+    def calculate_weighted(cls, score: Score) -> float:
+        r"""Calculates weighted accuracy for an osu!taiko score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Weighted accuracy to be used in pp calculation
+        :rtype: float
+        """
+        return cls.calculate(score)
+
+
+class ManiaAccuracyCalculator(AbstractAccuracyCalculator):
+    @staticmethod
+    def calculate(score: Score) -> float:
+        r"""Calculates accuracy for an osu!mania score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Accuracy for the given score
+        :rtype: float
+        """
+        count_perfect = score.statistics.count_geki
+        count_great = score.statistics.count_300
+        count_good = score.statistics.count_katu
+        count_ok = score.statistics.count_100
+        count_meh = score.statistics.count_50
+        count_miss = score.statistics.count_miss
+
+        total_hits = (
+            count_perfect + count_ok + count_great + count_good + count_meh + count_miss
+        )
+
+        if total_hits <= 0:
+            return 0.0
+
+        if Mod.ScoreV2 in score.mods:
+            return max(
+                (
+                    +(count_perfect * 305)
+                    + (count_great * 300)
+                    + (count_good * 200)
+                    + (count_ok * 100)
+                    + (count_meh * 50)
+                )
+                / (total_hits * 305),
+                0.0,
+            )
+
+        return max(
+            (
+                +((count_perfect + count_great) * 6.0)
+                + (count_good * 4.0)
+                + (count_ok * 2.0)
+                + count_meh
+            )
+            / (total_hits * 6.0),
+            0.0,
+        )
+
+    @staticmethod
+    def calculate_weighted(score: Score) -> float:
+        r"""Calculates weighted accuracy for an osu!mania score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Weighted accuracy to be used in pp calculation
+        :rtype: float
+        """
+        count_perfect = score.statistics.count_geki
+        count_great = score.statistics.count_300
+        count_good = score.statistics.count_katu
+        count_ok = score.statistics.count_100
+        count_meh = score.statistics.count_50
+        count_miss = score.statistics.count_miss
+
+        total_hits = (
+            count_perfect + count_ok + count_great + count_good + count_meh + count_miss
+        )
+
+        if total_hits <= 0:
+            return 0.0
+
+        return max(
+            (
+                +(count_perfect * 320)
+                + (count_great * 300)
+                + (count_good * 200)
+                + (count_ok * 100)
+                + (count_meh * 50)
+            )
+            / (total_hits * 320),
+            0.0,
+        )
+
+
+class CatchAccuracyCalculator(AbstractAccuracyCalculator):
+    @staticmethod
+    def calculate(score: Score) -> float:
+        r"""Calculates accuracy for an osu!catch score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Accuracy for the given score
+        :rtype: float
+        """
+        fruits_hit = score.statistics.count_300
+        ticks_hit = score.statistics.count_100
+        tiny_ticks_hit = score.statistics.count_50
+        tiny_ticks_missed = score.statistics.count_katu
+        misses = score.statistics.count_miss
+
+        total_hits = (
+            tiny_ticks_hit + ticks_hit + fruits_hit + misses + tiny_ticks_missed
+        )
+        successful_hits = tiny_ticks_hit + ticks_hit + fruits_hit
+
+        if total_hits <= 0:
+            return 0.0
+
+        return max(float(successful_hits) / total_hits, 0.0)
+
+    @classmethod
+    def calculate_weighted(cls, score: Score) -> float:
+        r"""Calculates weighted accuracy for an osu!catch score.
+
+        :param score: The score to calculate accuracy for
+        :type score: aiosu.models.score.Score
+        :return: Weighted accuracy to be used in pp calculation
+        :rtype: float
+        """
+        return cls.calculate(score)
```

### Comparing `aiosu-2.0.1/aiosu/utils/auth.py` & `aiosu-2.0.2/aiosu/utils/auth.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-"""
-This module contains authorization functions.
-"""
-from __future__ import annotations
-
-import urllib.parse
-from typing import Optional
-
-import aiohttp
-import orjson
-
-from ..exceptions import APIException
-from ..models.oauthtoken import OAuthToken
-from ..models.scopes import Scopes
-
-__all__ = (
-    "generate_url",
-    "process_code",
-)
-
-
-async def process_code(
-    client_id: int,
-    client_secret: str,
-    redirect_uri: str,
-    code: str,
-    base_url: str = "https://osu.ppy.sh",
-) -> OAuthToken:
-    r"""Creates an OAuth Token from an authorization code.
-
-    :param client_id: The ID of the client
-    :type client_id: int
-    :param client_secret: The client secret
-    :type client_secret: str
-    :param redirect_uri: The URL to redirect to
-    :type redirect_uri: str
-    :param code: Code returned from the API
-    :type code: str
-    :param base_url: The base URL of the API, defaults to "https://osu.ppy.sh"
-    :type base_url: Optional[str]
-    :return: The OAuth token
-    :rtype: aiosu.models.oauthtoken.OAuthToken
-    """
-    url = f"{base_url}/oauth/token"
-    headers = {"Content-Type": "application/x-www-form-urlencoded"}
-    data = {
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "code": code,
-        "redirect_uri": redirect_uri,
-        "grant_type": "authorization_code",
-    }
-
-    async with aiohttp.ClientSession(headers=headers) as temp_session:
-        async with temp_session.post(url, data=data) as resp:
-            try:
-                body = await resp.read()
-                json = orjson.loads(body)
-                if resp.status != 200:
-                    raise APIException(resp.status, json.get("error", ""))
-                token = OAuthToken.model_validate(json)
-                return token
-            except aiohttp.client_exceptions.ContentTypeError:
-                raise APIException(403, "Invalid code specified.")
-
-
-def generate_url(
-    client_id: int,
-    redirect_uri: str,
-    base_url: str = "https://osu.ppy.sh",
-    scopes: Scopes = Scopes.PUBLIC | Scopes.IDENTIFY,
-    state: Optional[str] = None,
-) -> str:
-    r"""Generates an OAuth URL.
-
-    :param client_id: The ID of the client
-    :type client_id: int
-    :param redirect_uri: The URL to redirect to
-    :type redirect_uri: str
-    :param base_url: The base URL of the API, defaults to "https://osu.ppy.sh"
-    :type base_url: Optional[str]
-    :param scopes: The scopes to request, defaults to Scopes.PUBLIC | Scopes.IDENTIFY
-    :type scopes: Optional[Scopes]
-    :param state: The state to pass to the API, defaults to None
-    :type state: Optional[str]
-    :return: The OAuth URL
-    :rtype: str
-    """
-    params = {
-        "client_id": client_id,
-        "redirect_uri": redirect_uri,
-        "response_type": "code",
-        "scope": str(scopes),
-    }
-    if state:
-        params["state"] = state
-    return f"{base_url}/oauth/authorize?{urllib.parse.urlencode(params)}"
+"""
+This module contains authorization functions.
+"""
+from __future__ import annotations
+
+import urllib.parse
+from typing import Optional
+
+import aiohttp
+import orjson
+
+from ..exceptions import APIException
+from ..models.oauthtoken import OAuthToken
+from ..models.scopes import Scopes
+
+__all__ = (
+    "generate_url",
+    "process_code",
+)
+
+
+async def process_code(
+    client_id: int,
+    client_secret: str,
+    redirect_uri: str,
+    code: str,
+    base_url: str = "https://osu.ppy.sh",
+) -> OAuthToken:
+    r"""Creates an OAuth Token from an authorization code.
+
+    :param client_id: The ID of the client
+    :type client_id: int
+    :param client_secret: The client secret
+    :type client_secret: str
+    :param redirect_uri: The URL to redirect to
+    :type redirect_uri: str
+    :param code: Code returned from the API
+    :type code: str
+    :param base_url: The base URL of the API, defaults to "https://osu.ppy.sh"
+    :type base_url: Optional[str]
+    :return: The OAuth token
+    :rtype: aiosu.models.oauthtoken.OAuthToken
+    """
+    url = f"{base_url}/oauth/token"
+    headers = {"Content-Type": "application/x-www-form-urlencoded"}
+    data = {
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "code": code,
+        "redirect_uri": redirect_uri,
+        "grant_type": "authorization_code",
+    }
+
+    async with aiohttp.ClientSession(headers=headers) as temp_session:
+        async with temp_session.post(url, data=data) as resp:
+            try:
+                body = await resp.read()
+                json = orjson.loads(body)
+                if resp.status != 200:
+                    raise APIException(resp.status, json.get("error", ""))
+                token = OAuthToken.model_validate(json)
+                return token
+            except aiohttp.client_exceptions.ContentTypeError:
+                raise APIException(403, "Invalid code specified.")
+
+
+def generate_url(
+    client_id: int,
+    redirect_uri: str,
+    base_url: str = "https://osu.ppy.sh",
+    scopes: Scopes = Scopes.PUBLIC | Scopes.IDENTIFY,
+    state: Optional[str] = None,
+) -> str:
+    r"""Generates an OAuth URL.
+
+    :param client_id: The ID of the client
+    :type client_id: int
+    :param redirect_uri: The URL to redirect to
+    :type redirect_uri: str
+    :param base_url: The base URL of the API, defaults to "https://osu.ppy.sh"
+    :type base_url: Optional[str]
+    :param scopes: The scopes to request, defaults to Scopes.PUBLIC | Scopes.IDENTIFY
+    :type scopes: Optional[Scopes]
+    :param state: The state to pass to the API, defaults to None
+    :type state: Optional[str]
+    :return: The OAuth URL
+    :rtype: str
+    """
+    params = {
+        "client_id": client_id,
+        "redirect_uri": redirect_uri,
+        "response_type": "code",
+        "scope": str(scopes),
+    }
+    if state:
+        params["state"] = state
+    return f"{base_url}/oauth/authorize?{urllib.parse.urlencode(params)}"
```

### Comparing `aiosu-2.0.1/aiosu/utils/performance.py` & `aiosu-2.0.2/aiosu/utils/performance.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-"""
-This module contains performance point calculators for osu! gamemodes.
-"""
-from __future__ import annotations
-
-import abc
-import math
-from typing import Callable
-from typing import TYPE_CHECKING
-
-from ..models import CatchPerformanceAttributes
-from ..models import Gamemode
-from ..models import ManiaPerformanceAttributes
-from ..models import Mod
-from ..models import OsuPerformanceAttributes
-from ..models import TaikoPerformanceAttributes
-from .accuracy import CatchAccuracyCalculator
-from .accuracy import ManiaAccuracyCalculator
-from .accuracy import OsuAccuracyCalculator
-from .accuracy import TaikoAccuracyCalculator
-
-if TYPE_CHECKING:
-    from typing import Type
-    from ..models.score import Score
-    from ..models.beatmap import BeatmapDifficultyAttributes
-    from ..models.performance import PerformanceAttributes
-
-
-__all__ = [
-    "OsuPerformanceCalculator",
-    "TaikoPerformanceCalculator",
-    "ManiaPerformanceCalculator",
-    "CatchPerformanceCalculator",
-]
-
-OSU_BASE_MULTIPLIER = 1.14
-TAIKO_BASE_MULTIPLIER = 1.13
-MANIA_BASE_MULTIPLIER = 8.0
-CATCH_BASE_MULTIPLIER = 1.0
-
-clamp: Callable[[float, float, float], float] = (
-    lambda x, l, u: l if x < l else u if x > u else x
-)
-
-
-class AbstractPerformanceCalculator(abc.ABC):
-    __slots__ = ("difficulty_attributes",)
-
-    def __init__(self, difficulty_attributes: BeatmapDifficultyAttributes):
-        self.difficulty_attributes = difficulty_attributes
-
-    @abc.abstractmethod
-    def calculate(self, score: Score) -> PerformanceAttributes:
-        ...
-
-
-def get_calculator(mode: Gamemode) -> Type[AbstractPerformanceCalculator]:
-    r"""Returns the performance calculator for the given gamemode.
-
-    :param mode: The gamemode to get the calculator for
-    :type mode: aiosu.models.gamemode.Gamemode
-    :raises ValueError: If the gamemode is unknown
-    :return: The performance calculator type for the given gamemode
-    :rtype: Type[AbstractPerformanceCalculator]
-    """
-    if mode == Gamemode.STANDARD:
-        return OsuPerformanceCalculator
-    elif mode == Gamemode.TAIKO:
-        return TaikoPerformanceCalculator
-    elif mode == Gamemode.MANIA:
-        return ManiaPerformanceCalculator
-    elif mode == Gamemode.CTB:
-        return CatchPerformanceCalculator
-    else:
-        raise ValueError(f"Unknown gamemode: {mode}")
-
-
-class OsuPerformanceCalculator(AbstractPerformanceCalculator):
-    r"""osu!std performance point calculator. Only compatible with scores from API v2.
-
-    :param difficulty_attributes: API difficulty attributes for a beatmap
-    :type difficulty_attributes: BeatmapDifficultyAttributes
-    """
-
-    def calculate(self, score: Score) -> OsuPerformanceAttributes:
-        r"""Calculates performance points for a score.
-
-        :param score: The score to calculate pp for
-        :type score: aiosu.models.score.Score
-        :raises ValueError: If score does not have an associated beatmap
-        :return: Performance attributes for the score
-        :rtype: aiosu.models.performance.OsuPerformanceAttributes
-        """
-        if score.beatmap is None:
-            raise ValueError("Given score does not have a beatmap.")
-
-        effective_miss_count = self._calculate_effective_miss_count(score)
-        total_hits = (
-            score.statistics.count_300
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        multiplier = OSU_BASE_MULTIPLIER
-
-        if Mod.NoFail in score.mods:
-            multiplier *= max(0.9, 1.0 - 0.02 * effective_miss_count)
-
-        if Mod.SpunOut in score.mods and total_hits > 0:
-            multiplier *= 1.0 - math.pow(
-                (score.beatmap.count_spinners / total_hits),  # type: ignore
-                0.85,
-            )
-
-        aim_value = self._compute_aim_value(score, effective_miss_count, total_hits)
-        speed_value = self._compute_speed_value(score, effective_miss_count, total_hits)
-        accuracy_value = self._compute_accuracy_value(score, total_hits)
-        flashlight_value = self._compute_flashlight_value(
-            score,
-            effective_miss_count,
-            total_hits,
-        )
-
-        total_value = (
-            math.pow(
-                math.pow(aim_value, 1.1)
-                + math.pow(speed_value, 1.1)
-                + math.pow(accuracy_value, 1.1)
-                + math.pow(flashlight_value, 1.1),
-                1.0 / 1.1,
-            )
-            * multiplier
-        )
-
-        return OsuPerformanceAttributes(
-            total=total_value,
-            aim=aim_value,
-            speed=speed_value,
-            accuracy=accuracy_value,
-            flashlight=flashlight_value,
-            effective_miss_count=effective_miss_count,
-        )
-
-    def _compute_aim_value(
-        self,
-        score: Score,
-        effective_miss_count: float,
-        total_hits: int,
-    ) -> float:
-        aim_value = (
-            math.pow(
-                5.0 * max(1.0, self.difficulty_attributes.aim_difficulty / 0.0675)  # type: ignore
-                - 4.0,
-                3.0,
-            )
-            / 100000.0
-        )
-
-        length_bonus = (
-            0.95
-            + 0.4 * min(1.0, total_hits / 2000.0)
-            + ((math.log10(total_hits / 2000.0) * 0.5) * int(total_hits > 2000))
-        )
-        aim_value *= length_bonus
-
-        if effective_miss_count > 0:
-            aim_value *= 0.97 * math.pow(
-                1 - math.pow(effective_miss_count / total_hits, 0.775),
-                effective_miss_count,
-            )
-
-        aim_value *= self._get_combo_scaling_factor(score)
-
-        approach_rate_factor = 0.0
-        if self.difficulty_attributes.approach_rate > 10.33:  # type: ignore
-            approach_rate_factor = 0.3 * (
-                self.difficulty_attributes.approach_rate - 10.33  # type: ignore
-            )
-        elif self.difficulty_attributes.approach_rate < 8.0:  # type: ignore
-            approach_rate_factor = 0.05 * (
-                8.0 - self.difficulty_attributes.approach_rate  # type: ignore
-            )
-
-        aim_value *= 1.0 + approach_rate_factor * length_bonus
-
-        if Mod.Hidden in score.mods:
-            aim_value *= 1.0 + 0.04 * (12.0 - self.difficulty_attributes.approach_rate)  # type: ignore
-
-        if score.beatmap.count_sliders > 0:  # type: ignore
-            estimate_difficult_sliders = score.beatmap.count_sliders * 0.15  # type: ignore
-
-            estimate_slider_ends_dropped = clamp(
-                min(
-                    score.statistics.count_100
-                    + score.statistics.count_50
-                    + score.statistics.count_miss,
-                    self.difficulty_attributes.max_combo - score.max_combo,
-                ),
-                0,
-                estimate_difficult_sliders,
-            )
-
-            slider_nerf_factor = (  # type: ignore
-                1 - self.difficulty_attributes.slider_factor  # type: ignore
-            ) * math.pow(
-                1 - estimate_slider_ends_dropped / estimate_difficult_sliders,
-                3,
-            ) + self.difficulty_attributes.slider_factor
-
-            aim_value *= slider_nerf_factor
-
-        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
-        aim_value *= accuracy
-        aim_value *= (
-            0.98 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 2500  # type: ignore
-        )
-
-        return aim_value
-
-    def _compute_speed_value(
-        self,
-        score: Score,
-        effective_miss_count: float,
-        total_hits: int,
-    ) -> float:
-        speed_value = (
-            math.pow(
-                5.0 * max(1.0, self.difficulty_attributes.speed_difficulty / 0.0675)  # type: ignore
-                - 4.0,
-                3.0,
-            )
-            / 100000.0
-        )
-
-        length_bonus = (
-            0.95
-            + 0.4 * min(1.0, total_hits / 2000.0)
-            + ((math.log10(total_hits / 2000.0) * 0.5) * int(total_hits > 2000))
-        )
-        speed_value *= length_bonus
-
-        if effective_miss_count > 0:
-            speed_value *= 0.97 * math.pow(
-                1 - math.pow(effective_miss_count / total_hits, 0.775),
-                math.pow(effective_miss_count, 0.875),
-            )
-
-        speed_value *= self._get_combo_scaling_factor(score)
-
-        approach_rate_factor = 0.0
-        if self.difficulty_attributes.approach_rate > 10.33:  # type: ignore
-            approach_rate_factor = 0.3 * (
-                self.difficulty_attributes.approach_rate - 10.33  # type: ignore
-            )
-
-        speed_value *= 1.0 + approach_rate_factor * length_bonus
-
-        if Mod.Hidden in score.mods:
-            speed_value *= 1.0 + 0.04 * (
-                12.0 - self.difficulty_attributes.approach_rate  # type: ignore
-            )
-
-        relevant_total_diff = total_hits - self.difficulty_attributes.speed_note_count  # type: ignore
-        relevant_count_great = max(0, score.statistics.count_300 - relevant_total_diff)
-        relevant_count_ok = max(
-            0,
-            score.statistics.count_100
-            - max(0, relevant_total_diff - score.statistics.count_300),
-        )
-        relevant_count_meh = max(
-            0,
-            score.statistics.count_50
-            - max(
-                0,
-                relevant_total_diff
-                - score.statistics.count_300
-                - score.statistics.count_100,
-            ),
-        )
-
-        relevant_accuracy = 0
-        if self.difficulty_attributes.speed_note_count > 0:  # type: ignore
-            relevant_accuracy = (
-                relevant_count_great * 6.0
-                + relevant_count_ok * 2.0
-                + relevant_count_meh
-            ) / (
-                self.difficulty_attributes.speed_note_count * 6.0  # type: ignore
-            )
-
-        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
-
-        speed_value *= (
-            0.95 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 750  # type: ignore
-        ) * math.pow(
-            (accuracy + relevant_accuracy) / 2.0,
-            (14.5 - max(self.difficulty_attributes.overall_difficulty, 8)) / 2,  # type: ignore
-        )
-
-        speed_value *= math.pow(
-            0.99,
-            (score.statistics.count_50 - total_hits / 500.0)
-            * int(score.statistics.count_50 > total_hits / 500.0),
-        )
-
-        return speed_value
-
-    def _compute_accuracy_value(
-        self,
-        score: Score,
-        total_hits: int,
-    ) -> float:
-        accuracy_calculator = OsuAccuracyCalculator()
-        better_accuracy_percentage = accuracy_calculator.calculate_weighted(score)
-
-        accuracy_value = (
-            math.pow(1.52163, self.difficulty_attributes.overall_difficulty)  # type: ignore
-            * math.pow(better_accuracy_percentage, 24)
-            * 2.83
-        )
-
-        accuracy_value *= min(
-            1.15,
-            math.pow(score.beatmap.count_circles / 1000.0, 0.3),  # type: ignore
-        )
-
-        if Mod.Hidden in score.mods:
-            accuracy_value *= 1.08
-
-        if Mod.Flashlight in score.mods:
-            accuracy_value *= 1.02
-
-        return accuracy_value
-
-    def _compute_flashlight_value(
-        self,
-        score: Score,
-        effective_miss_count: float,
-        total_hits: int,
-    ) -> float:
-        if Mod.Flashlight not in score.mods:
-            return 0.0
-
-        flashlight_value = (
-            math.pow(self.difficulty_attributes.flashlight_difficulty, 2.0) * 25.0  # type: ignore
-        )
-
-        if effective_miss_count > 0:
-            flashlight_value *= 0.97 * math.pow(
-                1 - math.pow(effective_miss_count / total_hits, 0.775),
-                math.pow(effective_miss_count, 0.875),
-            )
-
-        flashlight_value *= self._get_combo_scaling_factor(score)
-
-        flashlight_value *= (
-            0.7
-            + 0.1 * min(1.0, total_hits / 200.0)
-            + 0.2 * (min(1.0, (total_hits - 200) / 200.0) * int(total_hits > 200))
-        )
-
-        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
-        flashlight_value *= 0.5 + accuracy / 2.0
-        flashlight_value *= (
-            0.98 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 2500.0  # type: ignore
-        )
-
-        return flashlight_value
-
-    def _calculate_effective_miss_count(self, score: Score) -> float:
-        combo_based_miss_count = 0.0
-
-        if score.beatmap.count_sliders > 0:  # type: ignore
-            full_combo_threshold = (
-                self.difficulty_attributes.max_combo - 0.1 * score.beatmap.count_sliders  # type: ignore
-            )
-
-            if score.max_combo < full_combo_threshold:
-                combo_based_miss_count = full_combo_threshold / max(
-                    1.0,
-                    score.max_combo,
-                )
-
-        combo_based_miss_count = min(
-            combo_based_miss_count,
-            score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss,
-        )
-
-        return max(score.statistics.count_miss, combo_based_miss_count)
-
-    def _get_combo_scaling_factor(self, score: Score) -> float:
-        if self.difficulty_attributes.max_combo <= 0:
-            return 1.0
-
-        return min(
-            math.pow(score.max_combo, 0.8)
-            / math.pow(self.difficulty_attributes.max_combo, 0.8),
-            1.0,
-        )
-
-
-class TaikoPerformanceCalculator(AbstractPerformanceCalculator):
-    r"""osu!taiko performance point calculator.
-
-    :param difficulty_attributes: API difficulty attributes for a beatmap
-    :type difficulty_attributes: BeatmapDifficultyAttributes
-    """
-
-    def calculate(self, score: Score) -> TaikoPerformanceAttributes:
-        r"""Calculates performance points for a score
-
-        :param score: The score to calculate pp for
-        :type score: aiosu.models.score.Score
-        :return: Performance attributes for the score
-        :rtype: aiosu.models.performance.TaikoPerformanceAttributes
-        """
-        accuracy_calculator = TaikoAccuracyCalculator()
-        accuracy = accuracy_calculator.calculate_weighted(score)
-
-        effective_miss_count = self._calculate_effective_miss_count(score)
-        total_hits = (
-            score.statistics.count_300
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        multiplier = TAIKO_BASE_MULTIPLIER
-
-        if Mod.Hidden in score.mods:
-            multiplier *= 1.075
-
-        if Mod.Easy in score.mods:
-            multiplier *= 0.975
-
-        difficulty_value = self._compute_difficulty_value(
-            score,
-            total_hits,
-            effective_miss_count,
-            accuracy,
-        )
-        accuracy_value = self._compute_accuracy_value(
-            score,
-            total_hits,
-            accuracy,
-        )
-        total_value = (
-            math.pow(
-                math.pow(difficulty_value, 1.1) + math.pow(accuracy_value, 1.1),
-                1.0 / 1.1,
-            )
-            * multiplier
-        )
-
-        return TaikoPerformanceAttributes(
-            total=total_value,
-            difficulty=difficulty_value,
-            accuracy=accuracy_value,
-            effective_miss_count=effective_miss_count,
-        )
-
-    def _compute_difficulty_value(
-        self,
-        score: Score,
-        total_hits: int,
-        effective_miss_count: float,
-        accuracy: float,
-    ) -> float:
-        difficulty_value = (
-            math.pow(
-                5 * max(1.0, self.difficulty_attributes.star_rating / 0.115) - 4.0,
-                2.25,
-            )
-            / 1150.0
-        )
-
-        length_bonus = 1 + 0.1 * min(1.0, total_hits / 1500.0)
-        difficulty_value *= length_bonus
-
-        difficulty_value *= math.pow(0.986, effective_miss_count)
-
-        if Mod.Easy in score.mods:
-            difficulty_value *= 0.985
-
-        if Mod.Hidden in score.mods:
-            difficulty_value *= 1.025
-
-        if Mod.HardRock in score.mods:
-            difficulty_value *= 1.050
-
-        if Mod.Flashlight in score.mods:
-            difficulty_value *= 1.050 * length_bonus
-
-        difficulty_value *= math.pow(accuracy, 2.0)
-        return difficulty_value
-
-    def _compute_accuracy_value(
-        self,
-        score: Score,
-        total_hits: int,
-        accuracy: float,
-    ) -> float:
-        if self.difficulty_attributes.great_hit_window <= 0:  # type: ignore
-            return 0
-
-        accuracy_value = (
-            math.pow(60.0 / self.difficulty_attributes.great_hit_window, 1.1)  # type: ignore
-            * math.pow(accuracy, 8.0)
-            * math.pow(self.difficulty_attributes.star_rating, 0.4)
-            * 27.0
-        )
-
-        length_bonus = min(1.15, math.pow(total_hits / 1500.0, 0.3))
-        accuracy_value *= length_bonus
-
-        if Mod.Hidden in score.mods and Mod.Flashlight in score.mods:
-            accuracy_value *= max(1.050, 1.075 * length_bonus)
-
-        return accuracy_value
-
-    def _calculate_effective_miss_count(self, score: Score) -> float:
-        return (
-            max(
-                1.0,
-                1000.0
-                / (
-                    score.statistics.count_300
-                    + score.statistics.count_100
-                    + score.statistics.count_50
-                ),
-            )
-            * score.statistics.count_miss
-        )
-
-
-class ManiaPerformanceCalculator(AbstractPerformanceCalculator):
-    r"""osu!mania performance point calculator.
-
-    :param difficulty_attributes: API difficulty attributes for a beatmap
-    :type difficulty_attributes: BeatmapDifficultyAttributes
-    """
-
-    def calculate(self, score: Score) -> ManiaPerformanceAttributes:
-        r"""Calculates performance points for a score.
-
-        :param score: The score to calculate pp for
-        :type score: aiosu.models.score.Score
-        :return: Performance attributes for the score
-        :rtype: aiosu.models.performance.ManiaPerformanceAttributes
-        """
-        accuracy_calculator = ManiaAccuracyCalculator()
-        accuracy = accuracy_calculator.calculate_weighted(score)
-
-        total_hits = (
-            score.statistics.count_geki
-            + score.statistics.count_300
-            + score.statistics.count_katu
-            + score.statistics.count_100
-            + score.statistics.count_50
-            + score.statistics.count_miss
-        )
-
-        multiplier = MANIA_BASE_MULTIPLIER
-
-        if Mod.NoFail in score.mods:
-            multiplier *= 0.75
-
-        if Mod.Easy in score.mods:
-            multiplier *= 0.5
-
-        difficulty_value = self._compute_difficulty_value(accuracy, total_hits)
-        total_value = difficulty_value * multiplier
-
-        return ManiaPerformanceAttributes(
-            total=total_value,
-            difficulty=difficulty_value,
-        )
-
-    def _compute_difficulty_value(self, accuracy: float, total_hits: int) -> float:
-        difficulty_value = (
-            math.pow(max(self.difficulty_attributes.star_rating - 0.15, 0.05), 2.2)
-            * max(0.0, 5.0 * accuracy - 4.0)
-            * (1.0 + 0.1 * min(1.0, total_hits / 1500))
-        )
-
-        return difficulty_value
-
-
-class CatchPerformanceCalculator(AbstractPerformanceCalculator):
-    r"""osu!catch performance point calculator.
-
-    :param difficulty_attributes: API difficulty attributes for a beatmap
-    :type difficulty_attributes: BeatmapDifficultyAttributes
-    """
-
-    def calculate(self, score: Score) -> CatchPerformanceAttributes:
-        r"""Calculates performance points for a score.
-
-        :param score: The score to calculate pp for
-        :type score: aiosu.models.score.Score
-        :return: Performance attributes for the score
-        :rtype: aiosu.models.performance.CatchPerformanceAttributes
-        """
-        accuracy_calculator = CatchAccuracyCalculator()
-        accuracy = accuracy_calculator.calculate_weighted(score)
-
-        total_combo_hits = (
-            score.statistics.count_miss
-            + score.statistics.count_100
-            + score.statistics.count_300
-        )
-
-        multiplier = CATCH_BASE_MULTIPLIER
-
-        total_value = (
-            math.pow(
-                5.0 * max(1.0, self.difficulty_attributes.star_rating / 0.0049) - 4.0,
-                2.0,
-            )
-            / 100000.0
-        )
-
-        length_bonus = (
-            0.95
-            + 0.3 * min(1.0, total_combo_hits / 2500.0)
-            + (
-                (math.log10(total_combo_hits / 2500.0) * 0.475)
-                * int(total_combo_hits > 2500)
-            )
-        )
-        total_value *= length_bonus
-
-        total_value *= math.pow(0.97, score.statistics.count_miss)
-
-        if self.difficulty_attributes.max_combo > 0:
-            total_value *= min(
-                math.pow(score.max_combo, 0.8)
-                / math.pow(self.difficulty_attributes.max_combo, 0.8),
-                1.0,
-            )
-
-        approach_rate: float = self.difficulty_attributes.approach_rate  # type: ignore
-        approach_rate_factor = 1.0
-
-        if approach_rate > 9.0:
-            approach_rate_factor += 0.1 * (approach_rate - 9.0)
-
-        if approach_rate > 10.0:
-            approach_rate_factor += 0.1 * (approach_rate - 10.0)
-        elif approach_rate < 8.0:
-            approach_rate_factor += 0.025 * (8.0 - approach_rate)
-
-        total_value *= approach_rate_factor
-
-        if Mod.Hidden in score.mods:
-            if approach_rate <= 10.0:
-                total_value *= 1.05 + 0.075 * (10.0 - approach_rate)
-            elif approach_rate > 10.0:
-                total_value *= 1.01 + 0.04 * (11.0 - min(11.0, approach_rate))
-
-        if Mod.Flashlight in score.mods:
-            total_value *= 1.35 * length_bonus
-
-        total_value *= math.pow(accuracy, 5.5)
-
-        if Mod.NoFail in score.mods:
-            total_value *= 0.90
-
-        total_value *= multiplier
-
-        return CatchPerformanceAttributes(total=total_value)
+"""
+This module contains performance point calculators for osu! gamemodes.
+"""
+from __future__ import annotations
+
+import abc
+import math
+from typing import Callable
+from typing import TYPE_CHECKING
+
+from ..models import CatchPerformanceAttributes
+from ..models import Gamemode
+from ..models import ManiaPerformanceAttributes
+from ..models import Mod
+from ..models import OsuPerformanceAttributes
+from ..models import TaikoPerformanceAttributes
+from .accuracy import CatchAccuracyCalculator
+from .accuracy import ManiaAccuracyCalculator
+from .accuracy import OsuAccuracyCalculator
+from .accuracy import TaikoAccuracyCalculator
+
+if TYPE_CHECKING:
+    from typing import Type
+    from ..models.score import Score
+    from ..models.beatmap import BeatmapDifficultyAttributes
+    from ..models.performance import PerformanceAttributes
+
+
+__all__ = [
+    "OsuPerformanceCalculator",
+    "TaikoPerformanceCalculator",
+    "ManiaPerformanceCalculator",
+    "CatchPerformanceCalculator",
+]
+
+OSU_BASE_MULTIPLIER = 1.14
+TAIKO_BASE_MULTIPLIER = 1.13
+MANIA_BASE_MULTIPLIER = 8.0
+CATCH_BASE_MULTIPLIER = 1.0
+
+clamp: Callable[[float, float, float], float] = (
+    lambda x, l, u: l if x < l else u if x > u else x
+)
+
+
+class AbstractPerformanceCalculator(abc.ABC):
+    __slots__ = ("difficulty_attributes",)
+
+    def __init__(self, difficulty_attributes: BeatmapDifficultyAttributes):
+        self.difficulty_attributes = difficulty_attributes
+
+    @abc.abstractmethod
+    def calculate(self, score: Score) -> PerformanceAttributes:
+        ...
+
+
+def get_calculator(mode: Gamemode) -> Type[AbstractPerformanceCalculator]:
+    r"""Returns the performance calculator for the given gamemode.
+
+    :param mode: The gamemode to get the calculator for
+    :type mode: aiosu.models.gamemode.Gamemode
+    :raises ValueError: If the gamemode is unknown
+    :return: The performance calculator type for the given gamemode
+    :rtype: Type[AbstractPerformanceCalculator]
+    """
+    if mode == Gamemode.STANDARD:
+        return OsuPerformanceCalculator
+    elif mode == Gamemode.TAIKO:
+        return TaikoPerformanceCalculator
+    elif mode == Gamemode.MANIA:
+        return ManiaPerformanceCalculator
+    elif mode == Gamemode.CTB:
+        return CatchPerformanceCalculator
+    else:
+        raise ValueError(f"Unknown gamemode: {mode}")
+
+
+class OsuPerformanceCalculator(AbstractPerformanceCalculator):
+    r"""osu!std performance point calculator. Only compatible with scores from API v2.
+
+    :param difficulty_attributes: API difficulty attributes for a beatmap
+    :type difficulty_attributes: BeatmapDifficultyAttributes
+    """
+
+    def calculate(self, score: Score) -> OsuPerformanceAttributes:
+        r"""Calculates performance points for a score.
+
+        :param score: The score to calculate pp for
+        :type score: aiosu.models.score.Score
+        :raises ValueError: If score does not have an associated beatmap
+        :return: Performance attributes for the score
+        :rtype: aiosu.models.performance.OsuPerformanceAttributes
+        """
+        if score.beatmap is None:
+            raise ValueError("Given score does not have a beatmap.")
+
+        effective_miss_count = self._calculate_effective_miss_count(score)
+        total_hits = (
+            score.statistics.count_300
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        multiplier = OSU_BASE_MULTIPLIER
+
+        if Mod.NoFail in score.mods:
+            multiplier *= max(0.9, 1.0 - 0.02 * effective_miss_count)
+
+        if Mod.SpunOut in score.mods and total_hits > 0:
+            multiplier *= 1.0 - math.pow(
+                (score.beatmap.count_spinners / total_hits),  # type: ignore
+                0.85,
+            )
+
+        aim_value = self._compute_aim_value(score, effective_miss_count, total_hits)
+        speed_value = self._compute_speed_value(score, effective_miss_count, total_hits)
+        accuracy_value = self._compute_accuracy_value(score, total_hits)
+        flashlight_value = self._compute_flashlight_value(
+            score,
+            effective_miss_count,
+            total_hits,
+        )
+
+        total_value = (
+            math.pow(
+                math.pow(aim_value, 1.1)
+                + math.pow(speed_value, 1.1)
+                + math.pow(accuracy_value, 1.1)
+                + math.pow(flashlight_value, 1.1),
+                1.0 / 1.1,
+            )
+            * multiplier
+        )
+
+        return OsuPerformanceAttributes(
+            total=total_value,
+            aim=aim_value,
+            speed=speed_value,
+            accuracy=accuracy_value,
+            flashlight=flashlight_value,
+            effective_miss_count=effective_miss_count,
+        )
+
+    def _compute_aim_value(
+        self,
+        score: Score,
+        effective_miss_count: float,
+        total_hits: int,
+    ) -> float:
+        aim_value = (
+            math.pow(
+                5.0 * max(1.0, self.difficulty_attributes.aim_difficulty / 0.0675)  # type: ignore
+                - 4.0,
+                3.0,
+            )
+            / 100000.0
+        )
+
+        length_bonus = (
+            0.95
+            + 0.4 * min(1.0, total_hits / 2000.0)
+            + ((math.log10(total_hits / 2000.0) * 0.5) * int(total_hits > 2000))
+        )
+        aim_value *= length_bonus
+
+        if effective_miss_count > 0:
+            aim_value *= 0.97 * math.pow(
+                1 - math.pow(effective_miss_count / total_hits, 0.775),
+                effective_miss_count,
+            )
+
+        aim_value *= self._get_combo_scaling_factor(score)
+
+        approach_rate_factor = 0.0
+        if self.difficulty_attributes.approach_rate > 10.33:  # type: ignore
+            approach_rate_factor = 0.3 * (
+                self.difficulty_attributes.approach_rate - 10.33  # type: ignore
+            )
+        elif self.difficulty_attributes.approach_rate < 8.0:  # type: ignore
+            approach_rate_factor = 0.05 * (
+                8.0 - self.difficulty_attributes.approach_rate  # type: ignore
+            )
+
+        aim_value *= 1.0 + approach_rate_factor * length_bonus
+
+        if Mod.Hidden in score.mods:
+            aim_value *= 1.0 + 0.04 * (12.0 - self.difficulty_attributes.approach_rate)  # type: ignore
+
+        if score.beatmap.count_sliders > 0:  # type: ignore
+            estimate_difficult_sliders = score.beatmap.count_sliders * 0.15  # type: ignore
+
+            estimate_slider_ends_dropped = clamp(
+                min(
+                    score.statistics.count_100
+                    + score.statistics.count_50
+                    + score.statistics.count_miss,
+                    self.difficulty_attributes.max_combo - score.max_combo,
+                ),
+                0,
+                estimate_difficult_sliders,
+            )
+
+            slider_nerf_factor = (  # type: ignore
+                1 - self.difficulty_attributes.slider_factor  # type: ignore
+            ) * math.pow(
+                1 - estimate_slider_ends_dropped / estimate_difficult_sliders,
+                3,
+            ) + self.difficulty_attributes.slider_factor
+
+            aim_value *= slider_nerf_factor
+
+        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
+        aim_value *= accuracy
+        aim_value *= (
+            0.98 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 2500  # type: ignore
+        )
+
+        return aim_value
+
+    def _compute_speed_value(
+        self,
+        score: Score,
+        effective_miss_count: float,
+        total_hits: int,
+    ) -> float:
+        speed_value = (
+            math.pow(
+                5.0 * max(1.0, self.difficulty_attributes.speed_difficulty / 0.0675)  # type: ignore
+                - 4.0,
+                3.0,
+            )
+            / 100000.0
+        )
+
+        length_bonus = (
+            0.95
+            + 0.4 * min(1.0, total_hits / 2000.0)
+            + ((math.log10(total_hits / 2000.0) * 0.5) * int(total_hits > 2000))
+        )
+        speed_value *= length_bonus
+
+        if effective_miss_count > 0:
+            speed_value *= 0.97 * math.pow(
+                1 - math.pow(effective_miss_count / total_hits, 0.775),
+                math.pow(effective_miss_count, 0.875),
+            )
+
+        speed_value *= self._get_combo_scaling_factor(score)
+
+        approach_rate_factor = 0.0
+        if self.difficulty_attributes.approach_rate > 10.33:  # type: ignore
+            approach_rate_factor = 0.3 * (
+                self.difficulty_attributes.approach_rate - 10.33  # type: ignore
+            )
+
+        speed_value *= 1.0 + approach_rate_factor * length_bonus
+
+        if Mod.Hidden in score.mods:
+            speed_value *= 1.0 + 0.04 * (
+                12.0 - self.difficulty_attributes.approach_rate  # type: ignore
+            )
+
+        relevant_total_diff = total_hits - self.difficulty_attributes.speed_note_count  # type: ignore
+        relevant_count_great = max(0, score.statistics.count_300 - relevant_total_diff)
+        relevant_count_ok = max(
+            0,
+            score.statistics.count_100
+            - max(0, relevant_total_diff - score.statistics.count_300),
+        )
+        relevant_count_meh = max(
+            0,
+            score.statistics.count_50
+            - max(
+                0,
+                relevant_total_diff
+                - score.statistics.count_300
+                - score.statistics.count_100,
+            ),
+        )
+
+        relevant_accuracy = 0
+        if self.difficulty_attributes.speed_note_count > 0:  # type: ignore
+            relevant_accuracy = (
+                relevant_count_great * 6.0
+                + relevant_count_ok * 2.0
+                + relevant_count_meh
+            ) / (
+                self.difficulty_attributes.speed_note_count * 6.0  # type: ignore
+            )
+
+        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
+
+        speed_value *= (
+            0.95 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 750  # type: ignore
+        ) * math.pow(
+            (accuracy + relevant_accuracy) / 2.0,
+            (14.5 - max(self.difficulty_attributes.overall_difficulty, 8)) / 2,  # type: ignore
+        )
+
+        speed_value *= math.pow(
+            0.99,
+            (score.statistics.count_50 - total_hits / 500.0)
+            * int(score.statistics.count_50 > total_hits / 500.0),
+        )
+
+        return speed_value
+
+    def _compute_accuracy_value(
+        self,
+        score: Score,
+        total_hits: int,
+    ) -> float:
+        accuracy_calculator = OsuAccuracyCalculator()
+        better_accuracy_percentage = accuracy_calculator.calculate_weighted(score)
+
+        accuracy_value = (
+            math.pow(1.52163, self.difficulty_attributes.overall_difficulty)  # type: ignore
+            * math.pow(better_accuracy_percentage, 24)
+            * 2.83
+        )
+
+        accuracy_value *= min(
+            1.15,
+            math.pow(score.beatmap.count_circles / 1000.0, 0.3),  # type: ignore
+        )
+
+        if Mod.Hidden in score.mods:
+            accuracy_value *= 1.08
+
+        if Mod.Flashlight in score.mods:
+            accuracy_value *= 1.02
+
+        return accuracy_value
+
+    def _compute_flashlight_value(
+        self,
+        score: Score,
+        effective_miss_count: float,
+        total_hits: int,
+    ) -> float:
+        if Mod.Flashlight not in score.mods:
+            return 0.0
+
+        flashlight_value = (
+            math.pow(self.difficulty_attributes.flashlight_difficulty, 2.0) * 25.0  # type: ignore
+        )
+
+        if effective_miss_count > 0:
+            flashlight_value *= 0.97 * math.pow(
+                1 - math.pow(effective_miss_count / total_hits, 0.775),
+                math.pow(effective_miss_count, 0.875),
+            )
+
+        flashlight_value *= self._get_combo_scaling_factor(score)
+
+        flashlight_value *= (
+            0.7
+            + 0.1 * min(1.0, total_hits / 200.0)
+            + 0.2 * (min(1.0, (total_hits - 200) / 200.0) * int(total_hits > 200))
+        )
+
+        accuracy = score.accuracy if score.accuracy <= 1.0 else score.accuracy / 100
+        flashlight_value *= 0.5 + accuracy / 2.0
+        flashlight_value *= (
+            0.98 + math.pow(self.difficulty_attributes.overall_difficulty, 2) / 2500.0  # type: ignore
+        )
+
+        return flashlight_value
+
+    def _calculate_effective_miss_count(self, score: Score) -> float:
+        combo_based_miss_count = 0.0
+
+        if score.beatmap.count_sliders > 0:  # type: ignore
+            full_combo_threshold = (
+                self.difficulty_attributes.max_combo - 0.1 * score.beatmap.count_sliders  # type: ignore
+            )
+
+            if score.max_combo < full_combo_threshold:
+                combo_based_miss_count = full_combo_threshold / max(
+                    1.0,
+                    score.max_combo,
+                )
+
+        combo_based_miss_count = min(
+            combo_based_miss_count,
+            score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss,
+        )
+
+        return max(score.statistics.count_miss, combo_based_miss_count)
+
+    def _get_combo_scaling_factor(self, score: Score) -> float:
+        if self.difficulty_attributes.max_combo <= 0:
+            return 1.0
+
+        return min(
+            math.pow(score.max_combo, 0.8)
+            / math.pow(self.difficulty_attributes.max_combo, 0.8),
+            1.0,
+        )
+
+
+class TaikoPerformanceCalculator(AbstractPerformanceCalculator):
+    r"""osu!taiko performance point calculator.
+
+    :param difficulty_attributes: API difficulty attributes for a beatmap
+    :type difficulty_attributes: BeatmapDifficultyAttributes
+    """
+
+    def calculate(self, score: Score) -> TaikoPerformanceAttributes:
+        r"""Calculates performance points for a score
+
+        :param score: The score to calculate pp for
+        :type score: aiosu.models.score.Score
+        :return: Performance attributes for the score
+        :rtype: aiosu.models.performance.TaikoPerformanceAttributes
+        """
+        accuracy_calculator = TaikoAccuracyCalculator()
+        accuracy = accuracy_calculator.calculate_weighted(score)
+
+        effective_miss_count = self._calculate_effective_miss_count(score)
+        total_hits = (
+            score.statistics.count_300
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        multiplier = TAIKO_BASE_MULTIPLIER
+
+        if Mod.Hidden in score.mods:
+            multiplier *= 1.075
+
+        if Mod.Easy in score.mods:
+            multiplier *= 0.975
+
+        difficulty_value = self._compute_difficulty_value(
+            score,
+            total_hits,
+            effective_miss_count,
+            accuracy,
+        )
+        accuracy_value = self._compute_accuracy_value(
+            score,
+            total_hits,
+            accuracy,
+        )
+        total_value = (
+            math.pow(
+                math.pow(difficulty_value, 1.1) + math.pow(accuracy_value, 1.1),
+                1.0 / 1.1,
+            )
+            * multiplier
+        )
+
+        return TaikoPerformanceAttributes(
+            total=total_value,
+            difficulty=difficulty_value,
+            accuracy=accuracy_value,
+            effective_miss_count=effective_miss_count,
+        )
+
+    def _compute_difficulty_value(
+        self,
+        score: Score,
+        total_hits: int,
+        effective_miss_count: float,
+        accuracy: float,
+    ) -> float:
+        difficulty_value = (
+            math.pow(
+                5 * max(1.0, self.difficulty_attributes.star_rating / 0.115) - 4.0,
+                2.25,
+            )
+            / 1150.0
+        )
+
+        length_bonus = 1 + 0.1 * min(1.0, total_hits / 1500.0)
+        difficulty_value *= length_bonus
+
+        difficulty_value *= math.pow(0.986, effective_miss_count)
+
+        if Mod.Easy in score.mods:
+            difficulty_value *= 0.985
+
+        if Mod.Hidden in score.mods:
+            difficulty_value *= 1.025
+
+        if Mod.HardRock in score.mods:
+            difficulty_value *= 1.050
+
+        if Mod.Flashlight in score.mods:
+            difficulty_value *= 1.050 * length_bonus
+
+        difficulty_value *= math.pow(accuracy, 2.0)
+        return difficulty_value
+
+    def _compute_accuracy_value(
+        self,
+        score: Score,
+        total_hits: int,
+        accuracy: float,
+    ) -> float:
+        if self.difficulty_attributes.great_hit_window <= 0:  # type: ignore
+            return 0
+
+        accuracy_value = (
+            math.pow(60.0 / self.difficulty_attributes.great_hit_window, 1.1)  # type: ignore
+            * math.pow(accuracy, 8.0)
+            * math.pow(self.difficulty_attributes.star_rating, 0.4)
+            * 27.0
+        )
+
+        length_bonus = min(1.15, math.pow(total_hits / 1500.0, 0.3))
+        accuracy_value *= length_bonus
+
+        if Mod.Hidden in score.mods and Mod.Flashlight in score.mods:
+            accuracy_value *= max(1.050, 1.075 * length_bonus)
+
+        return accuracy_value
+
+    def _calculate_effective_miss_count(self, score: Score) -> float:
+        return (
+            max(
+                1.0,
+                1000.0
+                / (
+                    score.statistics.count_300
+                    + score.statistics.count_100
+                    + score.statistics.count_50
+                ),
+            )
+            * score.statistics.count_miss
+        )
+
+
+class ManiaPerformanceCalculator(AbstractPerformanceCalculator):
+    r"""osu!mania performance point calculator.
+
+    :param difficulty_attributes: API difficulty attributes for a beatmap
+    :type difficulty_attributes: BeatmapDifficultyAttributes
+    """
+
+    def calculate(self, score: Score) -> ManiaPerformanceAttributes:
+        r"""Calculates performance points for a score.
+
+        :param score: The score to calculate pp for
+        :type score: aiosu.models.score.Score
+        :return: Performance attributes for the score
+        :rtype: aiosu.models.performance.ManiaPerformanceAttributes
+        """
+        accuracy_calculator = ManiaAccuracyCalculator()
+        accuracy = accuracy_calculator.calculate_weighted(score)
+
+        total_hits = (
+            score.statistics.count_geki
+            + score.statistics.count_300
+            + score.statistics.count_katu
+            + score.statistics.count_100
+            + score.statistics.count_50
+            + score.statistics.count_miss
+        )
+
+        multiplier = MANIA_BASE_MULTIPLIER
+
+        if Mod.NoFail in score.mods:
+            multiplier *= 0.75
+
+        if Mod.Easy in score.mods:
+            multiplier *= 0.5
+
+        difficulty_value = self._compute_difficulty_value(accuracy, total_hits)
+        total_value = difficulty_value * multiplier
+
+        return ManiaPerformanceAttributes(
+            total=total_value,
+            difficulty=difficulty_value,
+        )
+
+    def _compute_difficulty_value(self, accuracy: float, total_hits: int) -> float:
+        difficulty_value = (
+            math.pow(max(self.difficulty_attributes.star_rating - 0.15, 0.05), 2.2)
+            * max(0.0, 5.0 * accuracy - 4.0)
+            * (1.0 + 0.1 * min(1.0, total_hits / 1500))
+        )
+
+        return difficulty_value
+
+
+class CatchPerformanceCalculator(AbstractPerformanceCalculator):
+    r"""osu!catch performance point calculator.
+
+    :param difficulty_attributes: API difficulty attributes for a beatmap
+    :type difficulty_attributes: BeatmapDifficultyAttributes
+    """
+
+    def calculate(self, score: Score) -> CatchPerformanceAttributes:
+        r"""Calculates performance points for a score.
+
+        :param score: The score to calculate pp for
+        :type score: aiosu.models.score.Score
+        :return: Performance attributes for the score
+        :rtype: aiosu.models.performance.CatchPerformanceAttributes
+        """
+        accuracy_calculator = CatchAccuracyCalculator()
+        accuracy = accuracy_calculator.calculate_weighted(score)
+
+        total_combo_hits = (
+            score.statistics.count_miss
+            + score.statistics.count_100
+            + score.statistics.count_300
+        )
+
+        multiplier = CATCH_BASE_MULTIPLIER
+
+        total_value = (
+            math.pow(
+                5.0 * max(1.0, self.difficulty_attributes.star_rating / 0.0049) - 4.0,
+                2.0,
+            )
+            / 100000.0
+        )
+
+        length_bonus = (
+            0.95
+            + 0.3 * min(1.0, total_combo_hits / 2500.0)
+            + (
+                (math.log10(total_combo_hits / 2500.0) * 0.475)
+                * int(total_combo_hits > 2500)
+            )
+        )
+        total_value *= length_bonus
+
+        total_value *= math.pow(0.97, score.statistics.count_miss)
+
+        if self.difficulty_attributes.max_combo > 0:
+            total_value *= min(
+                math.pow(score.max_combo, 0.8)
+                / math.pow(self.difficulty_attributes.max_combo, 0.8),
+                1.0,
+            )
+
+        approach_rate: float = self.difficulty_attributes.approach_rate  # type: ignore
+        approach_rate_factor = 1.0
+
+        if approach_rate > 9.0:
+            approach_rate_factor += 0.1 * (approach_rate - 9.0)
+
+        if approach_rate > 10.0:
+            approach_rate_factor += 0.1 * (approach_rate - 10.0)
+        elif approach_rate < 8.0:
+            approach_rate_factor += 0.025 * (8.0 - approach_rate)
+
+        total_value *= approach_rate_factor
+
+        if Mod.Hidden in score.mods:
+            if approach_rate <= 10.0:
+                total_value *= 1.05 + 0.075 * (10.0 - approach_rate)
+            elif approach_rate > 10.0:
+                total_value *= 1.01 + 0.04 * (11.0 - min(11.0, approach_rate))
+
+        if Mod.Flashlight in score.mods:
+            total_value *= 1.35 * length_bonus
+
+        total_value *= math.pow(accuracy, 5.5)
+
+        if Mod.NoFail in score.mods:
+            total_value *= 0.90
+
+        total_value *= multiplier
+
+        return CatchPerformanceAttributes(total=total_value)
```

### Comparing `aiosu-2.0.1/aiosu/v1/client.py` & `aiosu-2.0.2/aiosu/v1/client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,480 +1,480 @@
-"""
-This module handles API requests for API v1.
-
-You can read more about it here: https://github.com/ppy/osu-api/wiki
-"""
-from __future__ import annotations
-
-from io import BytesIO
-from io import StringIO
-from typing import Literal
-from typing import TYPE_CHECKING
-from warnings import warn
-
-import aiohttp
-import orjson
-from aiolimiter import AsyncLimiter
-
-from ..exceptions import APIException
-from ..helpers import add_param
-from ..helpers import from_list
-from ..models import Beatmapset
-from ..models import Gamemode
-from ..models import Mods
-from ..models import Score
-from ..models import User
-from ..models import UserQueryType
-from ..models.legacy import Match
-from ..models.legacy import ReplayCompact
-
-if TYPE_CHECKING:
-    from types import TracebackType
-    from typing import Any
-    from typing import Optional
-    from typing import Type
-    from typing import Union
-    from typing import Callable
-
-
-__all__ = ("Client",)
-
-ClientRequestType = Literal["GET", "POST", "DELETE", "PUT", "PATCH"]
-
-
-def get_content_type(content_type: str) -> str:
-    """Returns the content type."""
-    return content_type.split(";")[0]
-
-
-def _beatmap_score_conv(data: Any, mode: Gamemode, beatmap_id: int) -> Score:
-    data["beatmap_id"] = beatmap_id
-    return Score._from_api_v1(data, mode)
-
-
-class Client:
-    r"""osu! API v1 Client
-
-    :param token: The API key
-    :type token: str
-    :param \**kwargs:
-        See below
-
-    :Keyword Arguments:
-        * *base_url* (``str``) --
-            Optional, base API URL, defaults to "https://osu.ppy.sh"
-        * *limiter* (``tuple[int, int]``) --
-            Optional, rate limit, defaults to (600, 60) (600 requests per minute)
-    """
-
-    __slots__ = (
-        "token",
-        "base_url",
-        "_limiter",
-        "_session",
-    )
-
-    def __init__(self, token: str, **kwargs: Any) -> None:
-        self.token: str = token
-        self.base_url: str = kwargs.pop("base_url", "https://osu.ppy.sh")
-        max_rate, time_period = kwargs.pop("limiter", (600, 60))
-        if (max_rate / time_period) > (1000 / 60):
-            warn(
-                "You are running at an insanely high rate limit. Doing so may result in your account being banned.",
-            )
-        self._limiter: AsyncLimiter = AsyncLimiter(
-            max_rate=max_rate,
-            time_period=time_period,
-        )
-        self._session: Optional[aiohttp.ClientSession] = None
-
-    async def __aenter__(self) -> Client:
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc: Optional[BaseException],
-        traceback: Optional[TracebackType],
-    ) -> None:
-        await self.close()
-
-    async def _request(
-        self,
-        request_type: ClientRequestType,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Any:
-        if self._session is None:
-            self._session = aiohttp.ClientSession()
-
-        req: dict[str, Callable] = {
-            "GET": self._session.get,
-            "POST": self._session.post,
-            "DELETE": self._session.delete,
-            "PUT": self._session.put,
-            "PATCH": self._session.patch,
-        }
-
-        async with self._limiter:
-            async with req[request_type](*args, **kwargs) as resp:
-                body = await resp.read()
-                content_type = get_content_type(resp.headers.get("content-type", ""))
-                if resp.status != 200:
-                    json = orjson.loads(body)
-                    raise APIException(resp.status, json.get("error", ""))
-                if content_type == "application/json":
-                    return orjson.loads(body)
-                if content_type == "application/octet-stream":
-                    return BytesIO(body)
-                if content_type == "text/plain":
-                    return body.decode()
-                raise APIException(415, "Unhandled Content Type")
-
-    async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
-        r"""Gets a user by a query.
-
-        :param user_query: Username or ID to search by
-        :type user_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-            * *event_days* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, max number of days since last event, Min: 1, Max: 31, defaults to 1
-
-        :raises APIException: Contains status code and error message
-        :return: Requested user
-        :rtype: list[aiosu.models.user.User]
-        """
-        url = f"{self.base_url}/api/get_user"
-        params = {
-            "k": self.token,
-            "u": user_query,
-            "event_days": kwargs.pop("event_days", 1),
-            "m": int(Gamemode(kwargs.pop("mode", 0))),
-        }
-        add_param(
-            params,
-            kwargs,
-            key="qtype",
-            param_name="type",
-            converter=lambda x: UserQueryType(x).old_api_name,
-        )
-        json = await self._request("GET", url, params=params)
-        if not json:
-            raise APIException(404, "User not found")
-        return User._from_api_v1(json[0])
-
-    async def __get_type_scores(
-        self,
-        user_query: Union[str, int],
-        request_type: str,
-        **kwargs: Any,
-    ) -> list[Score]:
-        r"""INTERNAL: Get a user's scores by type
-
-        :param user_query: Username or ID to search by
-        :type user_query: Union[str, int]
-        :param request_type: "recent" or "best"
-        :type request_type: str
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *limit* (``int``) --
-                Optional, number of scores to get, defaults to 10
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If request_type is invalid
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        if request_type not in ("recent", "best"):
-            raise ValueError(
-                'Invalid request_type specified. Valid options are: "best", "recent"',
-            )
-        url = f"{self.base_url}/api/get_user_{request_type}"
-        params = {
-            "k": self.token,
-            "u": user_query,
-            "limit": kwargs.pop("limit", 10),
-        }
-        mode = Gamemode(kwargs.pop("mode", 0))
-        params["m"] = int(mode)
-        add_param(
-            params,
-            kwargs,
-            key="qtype",
-            param_name="type",
-            converter=lambda x: UserQueryType(x).old_api_name,
-        )
-        json = await self._request("GET", url, params=params)
-        score_conv = lambda x: Score._from_api_v1(x, mode)
-        return from_list(score_conv, json)
-
-    async def get_user_recents(
-        self,
-        user_query: Union[str, int],
-        **kwargs: Any,
-    ) -> list[Score]:
-        r"""Get a user's recent scores.
-
-        :param user_query: Username or ID to search by
-        :type user_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *limit* (``int``) --
-                Optional, number of scores to get, Min: 1, Max: 50, defaults to 50
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 50")
-        return await self.__get_type_scores(user_query, "recent", limit=limit, **kwargs)
-
-    async def get_user_bests(
-        self,
-        user_query: Union[str, int],
-        **kwargs: Any,
-    ) -> list[Score]:
-        r"""Get a user's best scores.
-
-        :param user_query: Username or ID to search by
-        :type user_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *limit* (``int``) --
-                Optional, number of scores to get, Min: 1, Max: 100, defaults to 100
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If limit is not between 1 and 100
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 100)) <= 100:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
-        return await self.__get_type_scores(user_query, "best", limit=limit, **kwargs)
-
-    async def get_beatmap(self, **kwargs: Any) -> list[Beatmapset]:
-        r"""Get beatmap data.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of scores to get, Min: 1, Max: 500, defaults to 500
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *converts* (``bool``) --
-                Optional, whether to return converts, defaults to False
-            * *mods* (``aiosu.models.mods.Mods``) --
-                Optional, mods to apply to the result
-            * *beatmap_id* (``int``) --
-                Optional, The ID of the beatmap
-            * *beatmapset_id* (``int``) --
-                Optional, The ID of the beatmapset
-            * *since* (``datetime.datetime``) --
-                Optional, Return all beatmaps with a leaderboard since this date
-            * *hash* (``str``) --
-                Optional, The MD5 hash of the beatmap
-            * *user_query* (``Union[str, int]``) --
-                Optional, username or ID to search by
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If limit is not between 1 and 500
-        :raises ValueError: If none of hash, since, user_query, beatmap_id or beatmapset_id specified.
-        :raises APIException: Contains status code and error message
-        :return: List of beatmapsets each containing one difficulty of the result
-        :rtype: list[aiosu.models.beatmap.Beatmapset]
-        """
-        if not 1 <= (limit := kwargs.get("limit", 500)) <= 500:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 500")
-        url = f"{self.base_url}/api/get_beatmaps"
-        params = {
-            "k": self.token,
-            "limit": limit,
-            "a": int(kwargs.pop("converts", False)),
-            "m": int(Gamemode(kwargs.pop("mode", 0))),
-        }
-        added = add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
-        added |= add_param(params, kwargs, key="beatmap_id", param_name="b")
-        added |= add_param(params, kwargs, key="beatmapset_id", param_name="s")
-        if add_param(params, kwargs, key="user_query", param_name="u"):
-            added = True
-            add_param(
-                params,
-                kwargs,
-                key="qtype",
-                param_name="type",
-                converter=lambda x: UserQueryType(x).old_api_name,
-            )
-        added |= add_param(params, kwargs, key="since", param_name="since")
-        added |= add_param(params, kwargs, key="hash", param_name="h")
-        if not added:
-            raise ValueError(
-                "Either hash, since, user_query, beatmap_id or beatmapset_id must be specified.",
-            )
-        json = await self._request("GET", url, params=params)
-        return from_list(Beatmapset._from_api_v1, json)
-
-    async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
-        r"""Get a user's best scores.
-
-        :param beatmap_id: The ID of the beatmap
-        :type beatmap_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *mods* (``aiosu.models.mods.Mods``) --
-                Optional, mods to search for
-            * *limit* (``int``) --
-                Optional, number of scores to get, Min: 1, Max: 100, defaults to 100
-            * *user_query* (``Union[str, int]``) --
-                Optional, username or ID to search by
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If limit is not between 1 and 100
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        if not 1 <= kwargs.get("limit", 100) <= 100:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
-        url = f"{self.base_url}/api/get_scores"
-        params = {
-            "k": self.token,
-            "b": beatmap_id,
-            "limit": kwargs.pop("limit", 50),
-        }
-        mode = Gamemode(kwargs.pop("mode", 0))
-        params["m"] = int(mode)
-        if add_param(params, kwargs, key="user_query", param_name="u"):
-            add_param(
-                params,
-                kwargs,
-                key="qtype",
-                param_name="type",
-                converter=lambda x: UserQueryType(x).old_api_name,
-            )
-        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
-        json = await self._request("GET", url, params=params)
-        score_conv = lambda x: _beatmap_score_conv(x, mode, beatmap_id)
-        return from_list(score_conv, json)
-
-    async def get_match(self, match_id: int) -> Match:
-        r"""Gets a multiplayer match. (WIP, currently returns raw JSON)
-
-        :param match_id: The ID of the match
-        :type match_id: int
-        :raises APIException: Contains status code and error message
-        :return: The requested multiplayer match
-        :rtype: aiosu.models.legacy.match.Match
-        """
-        url = f"{self.base_url}/api/get_match"
-        params = {
-            "k": self.token,
-            "mp": match_id,
-        }
-        json = await self._request("GET", url, params=params)
-        return Match.model_validate(json)
-
-    async def get_replay(self, **kwargs: Any) -> ReplayCompact:
-        r"""Gets data for a replay.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for, defaults to standard
-            * *mods* (``aiosu.models.mods.Mods``) --
-                Optional, mods to search for
-            * *score_id* (``int``) --
-                Optional, the ID of the score
-            * *beatmap_id* (``int``) --
-                Optional, the ID of the beatmap, specified together with user_query
-            * *user_query* (``Union[str, int]``) --
-                Optional, username or ID to search by, specified together with beatmap_id
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises ValueError: If neither score_id nor beatmap_id + user_id specified
-        :raises APIException: Contains status code and error message
-        :return: The data for the requested replay
-        :rtype: aiosu.models.legacy.replay.Replay
-        """
-        url = f"{self.base_url}/api/get_replay"
-        params = {
-            "k": self.token,
-            "m": int(Gamemode(kwargs.pop("mode", 0))),
-        }
-        added = add_param(params, kwargs, key="score_id", param_name="s")
-        if add_param(params, kwargs, key="beatmap_id", param_name="b") and add_param(
-            params,
-            kwargs,
-            key="user_query",
-            param_name="u",
-        ):
-            added = True
-            add_param(
-                params,
-                kwargs,
-                key="qtype",
-                param_name="type",
-                converter=lambda x: UserQueryType(x).old_api_name,
-            )
-        if not added:
-            raise ValueError(
-                "Either score_id or beatmap_id + user_id must be specified.",
-            )
-        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
-        json = await self._request("GET", url, params=params)
-        return ReplayCompact.model_validate(json)
-
-    async def get_beatmap_osu(self, beatmap_id: int) -> StringIO:
-        r"""Returns the Buffer of the beatmap file requested.
-
-        :param beatmap_id: The ID of the beatmap
-        :type beatmap_id: int
-
-        :return: File-like object of .osu data downloaded from the server.
-        :rtype: io.StringIO
-        """
-        url = f"{self.base_url}/osu/{beatmap_id}"
-        data = await self._request("GET", url)
-        return StringIO(data)
-
-    async def close(self) -> None:
-        """Closes the client session."""
-        if self._session:
-            await self._session.close()
-            self._session = None
+"""
+This module handles API requests for API v1.
+
+You can read more about it here: https://github.com/ppy/osu-api/wiki
+"""
+from __future__ import annotations
+
+from io import BytesIO
+from io import StringIO
+from typing import Literal
+from typing import TYPE_CHECKING
+from warnings import warn
+
+import aiohttp
+import orjson
+from aiolimiter import AsyncLimiter
+
+from ..exceptions import APIException
+from ..helpers import add_param
+from ..helpers import from_list
+from ..models import Beatmapset
+from ..models import Gamemode
+from ..models import Mods
+from ..models import Score
+from ..models import User
+from ..models import UserQueryType
+from ..models.legacy import Match
+from ..models.legacy import ReplayCompact
+
+if TYPE_CHECKING:
+    from types import TracebackType
+    from typing import Any
+    from typing import Optional
+    from typing import Type
+    from typing import Union
+    from typing import Callable
+
+
+__all__ = ("Client",)
+
+ClientRequestType = Literal["GET", "POST", "DELETE", "PUT", "PATCH"]
+
+
+def get_content_type(content_type: str) -> str:
+    """Returns the content type."""
+    return content_type.split(";")[0]
+
+
+def _beatmap_score_conv(data: Any, mode: Gamemode, beatmap_id: int) -> Score:
+    data["beatmap_id"] = beatmap_id
+    return Score._from_api_v1(data, mode)
+
+
+class Client:
+    r"""osu! API v1 Client
+
+    :param token: The API key
+    :type token: str
+    :param \**kwargs:
+        See below
+
+    :Keyword Arguments:
+        * *base_url* (``str``) --
+            Optional, base API URL, defaults to "https://osu.ppy.sh"
+        * *limiter* (``tuple[int, int]``) --
+            Optional, rate limit, defaults to (600, 60) (600 requests per minute)
+    """
+
+    __slots__ = (
+        "token",
+        "base_url",
+        "_limiter",
+        "_session",
+    )
+
+    def __init__(self, token: str, **kwargs: Any) -> None:
+        self.token: str = token
+        self.base_url: str = kwargs.pop("base_url", "https://osu.ppy.sh")
+        max_rate, time_period = kwargs.pop("limiter", (600, 60))
+        if (max_rate / time_period) > (1000 / 60):
+            warn(
+                "You are running at an insanely high rate limit. Doing so may result in your account being banned.",
+            )
+        self._limiter: AsyncLimiter = AsyncLimiter(
+            max_rate=max_rate,
+            time_period=time_period,
+        )
+        self._session: Optional[aiohttp.ClientSession] = None
+
+    async def __aenter__(self) -> Client:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        await self.close()
+
+    async def _request(
+        self,
+        request_type: ClientRequestType,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any:
+        if self._session is None:
+            self._session = aiohttp.ClientSession()
+
+        req: dict[str, Callable] = {
+            "GET": self._session.get,
+            "POST": self._session.post,
+            "DELETE": self._session.delete,
+            "PUT": self._session.put,
+            "PATCH": self._session.patch,
+        }
+
+        async with self._limiter:
+            async with req[request_type](*args, **kwargs) as resp:
+                body = await resp.read()
+                content_type = get_content_type(resp.headers.get("content-type", ""))
+                if resp.status != 200:
+                    json = orjson.loads(body)
+                    raise APIException(resp.status, json.get("error", ""))
+                if content_type == "application/json":
+                    return orjson.loads(body)
+                if content_type == "application/octet-stream":
+                    return BytesIO(body)
+                if content_type == "text/plain":
+                    return body.decode()
+                raise APIException(415, "Unhandled Content Type")
+
+    async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
+        r"""Gets a user by a query.
+
+        :param user_query: Username or ID to search by
+        :type user_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+            * *event_days* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, max number of days since last event, Min: 1, Max: 31, defaults to 1
+
+        :raises APIException: Contains status code and error message
+        :return: Requested user
+        :rtype: list[aiosu.models.user.User]
+        """
+        url = f"{self.base_url}/api/get_user"
+        params = {
+            "k": self.token,
+            "u": user_query,
+            "event_days": kwargs.pop("event_days", 1),
+            "m": int(Gamemode(kwargs.pop("mode", 0))),
+        }
+        add_param(
+            params,
+            kwargs,
+            key="qtype",
+            param_name="type",
+            converter=lambda x: UserQueryType(x).old_api_name,
+        )
+        json = await self._request("GET", url, params=params)
+        if not json:
+            raise APIException(404, "User not found")
+        return User._from_api_v1(json[0])
+
+    async def __get_type_scores(
+        self,
+        user_query: Union[str, int],
+        request_type: str,
+        **kwargs: Any,
+    ) -> list[Score]:
+        r"""INTERNAL: Get a user's scores by type
+
+        :param user_query: Username or ID to search by
+        :type user_query: Union[str, int]
+        :param request_type: "recent" or "best"
+        :type request_type: str
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *limit* (``int``) --
+                Optional, number of scores to get, defaults to 10
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If request_type is invalid
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        if request_type not in ("recent", "best"):
+            raise ValueError(
+                'Invalid request_type specified. Valid options are: "best", "recent"',
+            )
+        url = f"{self.base_url}/api/get_user_{request_type}"
+        params = {
+            "k": self.token,
+            "u": user_query,
+            "limit": kwargs.pop("limit", 10),
+        }
+        mode = Gamemode(kwargs.pop("mode", 0))
+        params["m"] = int(mode)
+        add_param(
+            params,
+            kwargs,
+            key="qtype",
+            param_name="type",
+            converter=lambda x: UserQueryType(x).old_api_name,
+        )
+        json = await self._request("GET", url, params=params)
+        score_conv = lambda x: Score._from_api_v1(x, mode)
+        return from_list(score_conv, json)
+
+    async def get_user_recents(
+        self,
+        user_query: Union[str, int],
+        **kwargs: Any,
+    ) -> list[Score]:
+        r"""Get a user's recent scores.
+
+        :param user_query: Username or ID to search by
+        :type user_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *limit* (``int``) --
+                Optional, number of scores to get, Min: 1, Max: 50, defaults to 50
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 50")
+        return await self.__get_type_scores(user_query, "recent", limit=limit, **kwargs)
+
+    async def get_user_bests(
+        self,
+        user_query: Union[str, int],
+        **kwargs: Any,
+    ) -> list[Score]:
+        r"""Get a user's best scores.
+
+        :param user_query: Username or ID to search by
+        :type user_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *limit* (``int``) --
+                Optional, number of scores to get, Min: 1, Max: 100, defaults to 100
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If limit is not between 1 and 100
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 100)) <= 100:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
+        return await self.__get_type_scores(user_query, "best", limit=limit, **kwargs)
+
+    async def get_beatmap(self, **kwargs: Any) -> list[Beatmapset]:
+        r"""Get beatmap data.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of scores to get, Min: 1, Max: 500, defaults to 500
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *converts* (``bool``) --
+                Optional, whether to return converts, defaults to False
+            * *mods* (``aiosu.models.mods.Mods``) --
+                Optional, mods to apply to the result
+            * *beatmap_id* (``int``) --
+                Optional, The ID of the beatmap
+            * *beatmapset_id* (``int``) --
+                Optional, The ID of the beatmapset
+            * *since* (``datetime.datetime``) --
+                Optional, Return all beatmaps with a leaderboard since this date
+            * *hash* (``str``) --
+                Optional, The MD5 hash of the beatmap
+            * *user_query* (``Union[str, int]``) --
+                Optional, username or ID to search by
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If limit is not between 1 and 500
+        :raises ValueError: If none of hash, since, user_query, beatmap_id or beatmapset_id specified.
+        :raises APIException: Contains status code and error message
+        :return: List of beatmapsets each containing one difficulty of the result
+        :rtype: list[aiosu.models.beatmap.Beatmapset]
+        """
+        if not 1 <= (limit := kwargs.get("limit", 500)) <= 500:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 500")
+        url = f"{self.base_url}/api/get_beatmaps"
+        params = {
+            "k": self.token,
+            "limit": limit,
+            "a": int(kwargs.pop("converts", False)),
+            "m": int(Gamemode(kwargs.pop("mode", 0))),
+        }
+        added = add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
+        added |= add_param(params, kwargs, key="beatmap_id", param_name="b")
+        added |= add_param(params, kwargs, key="beatmapset_id", param_name="s")
+        if add_param(params, kwargs, key="user_query", param_name="u"):
+            added = True
+            add_param(
+                params,
+                kwargs,
+                key="qtype",
+                param_name="type",
+                converter=lambda x: UserQueryType(x).old_api_name,
+            )
+        added |= add_param(params, kwargs, key="since", param_name="since")
+        added |= add_param(params, kwargs, key="hash", param_name="h")
+        if not added:
+            raise ValueError(
+                "Either hash, since, user_query, beatmap_id or beatmapset_id must be specified.",
+            )
+        json = await self._request("GET", url, params=params)
+        return from_list(Beatmapset._from_api_v1, json)
+
+    async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
+        r"""Get a user's best scores.
+
+        :param beatmap_id: The ID of the beatmap
+        :type beatmap_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *mods* (``aiosu.models.mods.Mods``) --
+                Optional, mods to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get, Min: 1, Max: 100, defaults to 100
+            * *user_query* (``Union[str, int]``) --
+                Optional, username or ID to search by
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If limit is not between 1 and 100
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        if not 1 <= kwargs.get("limit", 100) <= 100:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
+        url = f"{self.base_url}/api/get_scores"
+        params = {
+            "k": self.token,
+            "b": beatmap_id,
+            "limit": kwargs.pop("limit", 50),
+        }
+        mode = Gamemode(kwargs.pop("mode", 0))
+        params["m"] = int(mode)
+        if add_param(params, kwargs, key="user_query", param_name="u"):
+            add_param(
+                params,
+                kwargs,
+                key="qtype",
+                param_name="type",
+                converter=lambda x: UserQueryType(x).old_api_name,
+            )
+        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
+        json = await self._request("GET", url, params=params)
+        score_conv = lambda x: _beatmap_score_conv(x, mode, beatmap_id)
+        return from_list(score_conv, json)
+
+    async def get_match(self, match_id: int) -> Match:
+        r"""Gets a multiplayer match. (WIP, currently returns raw JSON)
+
+        :param match_id: The ID of the match
+        :type match_id: int
+        :raises APIException: Contains status code and error message
+        :return: The requested multiplayer match
+        :rtype: aiosu.models.legacy.match.Match
+        """
+        url = f"{self.base_url}/api/get_match"
+        params = {
+            "k": self.token,
+            "mp": match_id,
+        }
+        json = await self._request("GET", url, params=params)
+        return Match.model_validate(json)
+
+    async def get_replay(self, **kwargs: Any) -> ReplayCompact:
+        r"""Gets data for a replay.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for, defaults to standard
+            * *mods* (``aiosu.models.mods.Mods``) --
+                Optional, mods to search for
+            * *score_id* (``int``) --
+                Optional, the ID of the score
+            * *beatmap_id* (``int``) --
+                Optional, the ID of the beatmap, specified together with user_query
+            * *user_query* (``Union[str, int]``) --
+                Optional, username or ID to search by, specified together with beatmap_id
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises ValueError: If neither score_id nor beatmap_id + user_id specified
+        :raises APIException: Contains status code and error message
+        :return: The data for the requested replay
+        :rtype: aiosu.models.legacy.replay.Replay
+        """
+        url = f"{self.base_url}/api/get_replay"
+        params = {
+            "k": self.token,
+            "m": int(Gamemode(kwargs.pop("mode", 0))),
+        }
+        added = add_param(params, kwargs, key="score_id", param_name="s")
+        if add_param(params, kwargs, key="beatmap_id", param_name="b") and add_param(
+            params,
+            kwargs,
+            key="user_query",
+            param_name="u",
+        ):
+            added = True
+            add_param(
+                params,
+                kwargs,
+                key="qtype",
+                param_name="type",
+                converter=lambda x: UserQueryType(x).old_api_name,
+            )
+        if not added:
+            raise ValueError(
+                "Either score_id or beatmap_id + user_id must be specified.",
+            )
+        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
+        json = await self._request("GET", url, params=params)
+        return ReplayCompact.model_validate(json)
+
+    async def get_beatmap_osu(self, beatmap_id: int) -> StringIO:
+        r"""Returns the Buffer of the beatmap file requested.
+
+        :param beatmap_id: The ID of the beatmap
+        :type beatmap_id: int
+
+        :return: File-like object of .osu data downloaded from the server.
+        :rtype: io.StringIO
+        """
+        url = f"{self.base_url}/osu/{beatmap_id}"
+        data = await self._request("GET", url)
+        return StringIO(data)
+
+    async def close(self) -> None:
+        """Closes the client session."""
+        if self._session:
+            await self._session.close()
+            self._session = None
```

### Comparing `aiosu-2.0.1/aiosu/v2/client.py` & `aiosu-2.0.2/aiosu/v2/client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,2391 +1,2391 @@
-"""
-This module handles API requests for API v2 (OAuth).
-
-You can read more about it here: https://osu.ppy.sh/docs/index.html
-"""
-from __future__ import annotations
-
-import functools
-from datetime import datetime
-from functools import partial
-from io import BytesIO
-from typing import Any
-from typing import Callable
-from typing import cast
-from typing import Literal
-from typing import TYPE_CHECKING
-from typing import TypeVar
-from warnings import warn
-
-import aiohttp
-import orjson
-from aiolimiter import AsyncLimiter
-
-from ..events import ClientUpdateEvent
-from ..events import Eventable
-from ..exceptions import APIException
-from ..helpers import add_param
-from ..helpers import from_list
-from ..models import ArtistResponse
-from ..models import Beatmap
-from ..models import BeatmapDifficultyAttributes
-from ..models import Beatmapset
-from ..models import BeatmapsetDiscussionPostResponse
-from ..models import BeatmapsetDiscussionResponse
-from ..models import BeatmapsetDiscussionVoteResponse
-from ..models import BeatmapsetEvent
-from ..models import BeatmapsetSearchResponse
-from ..models import BeatmapUserPlaycount
-from ..models import Build
-from ..models import ChangelogListing
-from ..models import ChatChannel
-from ..models import ChatChannelResponse
-from ..models import ChatChannelTypes
-from ..models import ChatMessage
-from ..models import ChatMessageCreateResponse
-from ..models import ChatUpdateResponse
-from ..models import ChatUserSilence
-from ..models import CommentBundle
-from ..models import Event
-from ..models import ForumCreateTopicResponse
-from ..models import ForumPost
-from ..models import ForumTopic
-from ..models import ForumTopicResponse
-from ..models import Gamemode
-from ..models import KudosuHistory
-from ..models import LazerScore
-from ..models import Mods
-from ..models import MultiplayerLeaderboardResponse
-from ..models import MultiplayerMatchesResponse
-from ..models import MultiplayerMatchResponse
-from ..models import MultiplayerRoom
-from ..models import MultiplayerRoomMode
-from ..models import MultiplayerScoresResponse
-from ..models import NewsListing
-from ..models import NewsPost
-from ..models import OAuthToken
-from ..models import Rankings
-from ..models import RankingType
-from ..models import Scopes
-from ..models import Score
-from ..models import SearchResponse
-from ..models import SeasonalBackgroundSet
-from ..models import Spotlight
-from ..models import User
-from ..models import UserQueryType
-from ..models import WikiPage
-from .repository import BaseTokenRepository
-from .repository import SimpleTokenRepository
-
-if TYPE_CHECKING:
-    from types import TracebackType
-    from typing import Optional
-    from typing import Type
-    from typing import Union
-
-__all__ = ("Client",)
-
-F = TypeVar("F", bound=Callable[..., Any])
-ClientRequestType = Literal["GET", "POST", "DELETE", "PUT", "PATCH"]
-
-
-def to_lower_str(value: Any) -> str:
-    """Converts a value to a lowercase string."""
-    return str(value).lower()
-
-
-def get_content_type(content_type: str) -> str:
-    """Returns the content type."""
-    return content_type.split(";")[0]
-
-
-def prepare_token(func: F) -> F:
-    """A decorator that prepares the token for use, to be used as:
-    @prepare_token
-    """
-
-    @functools.wraps(func)
-    async def _prepare_token(self: Client, *args: Any, **kwargs: Any) -> Any:
-        await self._prepare_token()
-
-        return await func(self, *args, **kwargs)
-
-    return cast(F, _prepare_token)
-
-
-def check_token(func: F) -> F:
-    """
-    A decorator that checks the current token, to be used as:
-    @check_token
-    """
-
-    @functools.wraps(func)
-    async def _check_token(self: Client, *args: Any, **kwargs: Any) -> Any:
-        token = await self.get_current_token()
-        if datetime.utcnow().timestamp() > token.expires_on.timestamp():
-            await self._refresh()
-        return await func(self, *args, **kwargs)
-
-    return cast(F, _check_token)
-
-
-def requires_scope(
-    required_scopes: Scopes,
-    any_scope: bool = False,
-) -> Callable[[F], F]:
-    """
-    A decorator that enforces a scope, to be used as:
-    @requires_scope(Scopes.PUBLIC)
-    """
-
-    def _requires_scope(
-        func: F,
-    ) -> F:
-        @functools.wraps(func)
-        async def _wrap(self: Client, *args: Any, **kwargs: Any) -> Any:
-            token = await self.get_current_token()
-            if any_scope:
-                if not (required_scopes & token.scopes):
-                    raise APIException(403, "Missing required scopes.")
-            elif required_scopes & token.scopes != required_scopes:
-                raise APIException(403, "Missing required scopes.")
-
-            return await func(self, *args, **kwargs)
-
-        return cast(F, _wrap)
-
-    return _requires_scope
-
-
-class Client(Eventable):
-    r"""osu! API v2 Client
-
-    :param \**kwargs:
-        See below
-
-    :Keyword Arguments:
-        * *token_repository* (``aiosu.v2.repository.BaseTokenRepository``) --
-            Optional, defaults to ``aiosu.v2.repository.SimpleTokenRepository()``
-        * *session_id* (``int``) --
-            Optional, ID of the session to search in the repository, defaults to 0
-        * *client_id* (``int``) --
-            Optional, required to refresh tokens
-        * *client_secret* (``str``) --
-            Optional, required to refresh tokens
-        * *base_url* (``str``) --
-            Optional, base API URL, defaults to "https://osu.ppy.sh"
-        * *token* (``aiosu.models.oauthtoken.OAuthToken``) --
-            Optional, defaults to client credentials if not provided
-        * *limiter* (``tuple[int, int]``) --
-            Optional, rate limit, defaults to (600, 60) (600 requests per minute)
-    """
-
-    __slots__ = (
-        "_token_repository",
-        "_initial_token",
-        "_session",
-        "_limiter",
-        "session_id",
-        "client_id",
-        "client_secret",
-        "base_url",
-    )
-
-    def __init__(
-        self,
-        **kwargs: Any,
-    ) -> None:
-        super().__init__()
-        self._register_event(ClientUpdateEvent)
-        self._token_repository: BaseTokenRepository = kwargs.pop(
-            "token_repository",
-            SimpleTokenRepository(),
-        )
-        max_rate, time_period = kwargs.pop("limiter", (600, 60))
-        if (
-            not isinstance(self._token_repository, SimpleTokenRepository)
-            and "session_id" not in kwargs
-        ):
-            warn(
-                "You are using a custom token repository, but did not provide a session ID. This may cause unexpected behavior.",
-            )
-        if (max_rate / time_period) > (1000 / 60):
-            warn(
-                "You are running at an insanely high rate limit. Doing so may result in your account being banned.",
-            )
-        self.session_id: int = kwargs.pop("session_id", 0)
-        self.client_id: int = kwargs.pop("client_id", None)
-        self.client_secret: str = kwargs.pop("client_secret", None)
-        self._initial_token: Optional[OAuthToken] = kwargs.pop("token", None)
-        self.base_url: str = kwargs.pop("base_url", "https://osu.ppy.sh")
-        self._limiter: AsyncLimiter = AsyncLimiter(
-            max_rate=max_rate,
-            time_period=time_period,
-        )
-        self._session: Optional[aiohttp.ClientSession] = None
-
-    async def __aenter__(self) -> Client:
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc: Optional[BaseException],
-        traceback: Optional[TracebackType],
-    ) -> None:
-        await self.close()
-
-    def on_client_update(
-        self,
-        func: F,
-    ) -> F:
-        """
-        A decorator that is called whenever a client is updated, to be used as:
-
-            @client.on_client_update
-
-            async def func(event: ClientUpdateEvent)
-        """
-        self._register_listener(func, ClientUpdateEvent)
-
-        @functools.wraps(func)
-        async def _on_client_update(*args: Any, **kwargs: Any) -> Any:
-            return await func(*args, **kwargs)
-
-        return cast(F, _on_client_update)
-
-    async def get_current_token(self) -> OAuthToken:
-        """Get the current token"""
-        return await self._token_repository.get(self.session_id)
-
-    async def _prepare_token(self) -> None:
-        """Prepare the token for use."""
-        if not await self._token_exists():
-            token_to_add = self._initial_token
-            if token_to_add is None:
-                token_to_add = OAuthToken()
-            await self._add_token(token_to_add)
-        elif self._initial_token is not None:
-            await self._update_token(self._initial_token)
-        self._initial_token = None
-
-    async def _add_token(self, token: OAuthToken) -> None:
-        """Add a token to the current session"""
-        await self._token_repository.add(self.session_id, token)
-
-    async def _update_token(self, token: OAuthToken) -> None:
-        """Update the current token"""
-        await self._token_repository.update(self.session_id, token)
-
-    async def _token_exists(self) -> bool:
-        """Check if a token exists for the current session"""
-        return await self._token_repository.exists(self.session_id)
-
-    async def _delete_token(self) -> None:
-        """Delete the current token"""
-        await self._token_repository.delete(self.session_id)
-
-    async def _get_headers(self) -> dict[str, str]:
-        token = await self.get_current_token()
-        return {
-            "Authorization": f"Bearer {token.access_token}",
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-        }
-
-    async def _refresh_auth_data(self) -> dict[str, Union[str, int]]:
-        token = await self.get_current_token()
-        return {
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "grant_type": "refresh_token",
-            "refresh_token": token.refresh_token,
-        }
-
-    def _refresh_guest_data(self) -> dict[str, Union[str, int]]:
-        return {
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "grant_type": "client_credentials",
-            "scope": "public",
-        }
-
-    async def _request(
-        self,
-        request_type: ClientRequestType,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Any:
-        await self._prepare_token()
-
-        if self._session is None:
-            self._session = aiohttp.ClientSession(headers=await self._get_headers())
-
-        req: dict[str, Callable] = {
-            "GET": self._session.get,
-            "POST": self._session.post,
-            "DELETE": self._session.delete,
-            "PUT": self._session.put,
-            "PATCH": self._session.patch,
-        }
-
-        async with self._limiter:
-            async with req[request_type](*args, **kwargs) as resp:
-                if resp.status == 204:
-                    return
-
-                body = await resp.read()
-                content_type = get_content_type(resp.headers.get("content-type", ""))
-                if resp.status != 200:
-                    json = orjson.loads(body)
-                    raise APIException(resp.status, json.get("error", ""))
-                if content_type == "application/json":
-                    return orjson.loads(body)
-                if content_type == "application/octet-stream":
-                    return BytesIO(body)
-                if content_type.startswith("application/x-osu"):
-                    return BytesIO(body)
-                if content_type == "text/plain":
-                    return body.decode()
-                raise APIException(415, f"Unhandled Content Type '{content_type}'")
-
-    async def _refresh(self) -> None:
-        r"""INTERNAL: Refreshes the client's token
-
-        :raises APIException: Contains status code and error message
-        """
-        old_token = await self.get_current_token()
-        url = f"{self.base_url}/oauth/token"
-
-        data = {}
-        if old_token.can_refresh:
-            data = await self._refresh_auth_data()
-        else:
-            data = self._refresh_guest_data()
-
-        async with aiohttp.ClientSession() as temp_session:
-            async with self._limiter:
-                async with temp_session.post(url, json=data) as resp:
-                    try:
-                        body = await resp.read()
-                        content_type = get_content_type(
-                            resp.headers.get("content-type", ""),
-                        )
-                        if content_type != "application/json":
-                            raise APIException(
-                                415,
-                                f"Unhandled Content Type '{content_type}'",
-                            )
-                        json = orjson.loads(body)
-                        if resp.status != 200:
-                            raise APIException(resp.status, json.get("error", ""))
-                        if self._session:
-                            await self._session.close()
-                        new_token = OAuthToken.model_validate(json)
-                        await self._update_token(new_token)
-                        self._session = aiohttp.ClientSession(
-                            headers=await self._get_headers(),
-                        )
-                    except aiohttp.client_exceptions.ContentTypeError:
-                        raise APIException(403, "Invalid token specified.")
-
-        await self._process_event(
-            ClientUpdateEvent(client=self, old_token=old_token, new_token=new_token),
-        )
-
-    @prepare_token
-    async def get_featured_artists(self, **kwargs: Any) -> ArtistResponse:
-        r"""Gets the current featured artists.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the number of featured artists to return.
-            * *album* (``str``) --
-                Optional, the album to filter by.
-            * *artist* (``str``) --
-                Optional, the artist to filter by.
-            * *genre* (``int``) --
-                Optional, the genre ID to filter by.
-            * *length* (``list[int]``) --
-                Optional, the length range to filter by.
-            * *bpm* (``list[int]``) --
-                Optional, The BPM range to filter by.
-            * *query* (``str``) --
-                Optional, the search query to filter by.
-            * *is_default_sort* (``bool``) --
-                Optional, whether to sort by the default sort.
-            * *sort* (``str``) --
-                Optional, the sort to use.
-
-        :raises APIException: Contains status code and error message
-        :return: Featured artist response object
-        :rtype: aiosu.models.artist.ArtistResponse
-        """
-        url = f"{self.base_url}/beatmaps/artists/tracks"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="album")
-        add_param(params, kwargs, key="artist")
-        add_param(params, kwargs, key="genre")
-        add_param(params, kwargs, key="length")
-        add_param(params, kwargs, key="bpm")
-        add_param(params, kwargs, key="query")
-        add_param(params, kwargs, key="is_default_sort", converter=to_lower_str)
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url)
-        resp = ArtistResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_featured_artists, **kwargs)
-        return resp
-
-    @prepare_token
-    async def get_seasonal_backgrounds(self) -> SeasonalBackgroundSet:
-        r"""Gets the current seasonal background set.
-
-        :raises APIException: Contains status code and error message
-        :return: Seasonal background set object
-        :rtype: aiosu.models.backgrounds.SeasonalBackgroundSet
-        """
-        url = f"{self.base_url}/api/v2/seasonal-backgrounds"
-        json = await self._request("GET", url)
-        return SeasonalBackgroundSet.model_validate(json)
-
-    @prepare_token
-    async def get_changelog_listing(self, **kwargs: Any) -> ChangelogListing:
-        r"""Gets the changelog listing.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *message_formats* (``list[str]``) --
-                Optional, the message formats to return.
-            * *from* (``str``) --
-                Optional, the start date to return.
-            * *to* (``str``) --
-                Optional, the end date to return.
-            * *max_id* (``int``) --
-                Optional, the maximum ID to return.
-            * *stream* (``str``) --
-                Optional, the stream to return.
-            * *cursor_string* (``str``) --
-                Optional, the cursor string to use.
-
-        :raises APIException: Contains status code and error message
-        :return: Changelog listing object
-        :rtype: aiosu.models.changelog.ChangelogListing
-        """
-        url = f"{self.base_url}/api/v2/changelog"
-        params: dict[str, Any] = {
-            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
-        }
-        add_param(params, kwargs, key="from")
-        add_param(params, kwargs, key="to")
-        add_param(params, kwargs, key="max_id")
-        add_param(params, kwargs, key="stream")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = ChangelogListing.model_validate(json)
-        if resp.cursor_string:  # Unused: API does not return cursor_string
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_changelog_listing, **kwargs)
-        return resp
-
-    @prepare_token
-    async def get_changelog_build(self, stream: str, build: str) -> Build:
-        r"""Gets a specific build from the changelog.
-
-        :param stream: The stream to get the build from
-        :param build: The build to get
-        :raises APIException: Contains status code and error message
-        :return: Build object
-        :rtype: aiosu.models.changelog.Build
-        """
-        url = f"{self.base_url}/api/v2/changelog/{stream}/{build}"
-        json = await self._request("GET", url)
-        return Build.model_validate(json)
-
-    @prepare_token
-    async def lookup_changelog_build(
-        self,
-        changelog_query: Union[str, int],
-        **kwargs: Any,
-    ) -> Build:
-        r"""Looks up a build from the changelog.
-
-        :param changelog_query: The query to search for
-        :type changelog_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *is_id* (``bool``) --
-                Optional, whether the query is an ID or not, defaults to ``True`` if the query is an int
-            * *message_formats* (``list[aiosu.models.news.ChangelogMessageFormats]``) --
-                Optional, message formats to get, defaults to ``["html", "markdown"]``
-
-        :raises APIException: Contains status code and error message
-        :return: Build object
-        :rtype: aiosu.models.changelog.Build
-        """
-        url = f"{self.base_url}/api/v2/changelog/{changelog_query}"
-        params: dict[str, Any] = {
-            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
-        }
-        if "is_id" in kwargs or isinstance(changelog_query, int):
-            params["key"] = "id"
-        json = await self._request("GET", url, params=params)
-        return Build.model_validate(json)
-
-    @prepare_token
-    async def get_news_listing(self, **kwargs: Any) -> NewsListing:
-        r"""Gets the news listing.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the number of news posts to return. Min: 1, Max: 21, defaults to 12
-            * *year* (``int``) --
-                Optional, the year to filter by.
-            * *cursor_string* (``str``) --
-                Optional, the cursor string to use for pagination.
-
-        :raises APIException: Contains status code and error message
-        :return: News listing object
-        :rtype: aiosu.models.news.NewsListing
-        """
-        url = f"{self.base_url}/api/v2/news"
-        if not 1 <= (limit := kwargs.pop("limit", 12)) <= 21:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 21")
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="year")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = NewsListing.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_news_listing, **kwargs)
-        return resp
-
-    @prepare_token
-    async def get_news_post(
-        self,
-        news_query: Union[str, int],
-        **kwargs: Any,
-    ) -> NewsPost:
-        r"""Gets a news post.
-
-        :param news_query: The query to search for
-        :type news_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *is_id* (``bool``) --
-                Optional, whether the query is an ID or not, defaults to ``True`` if the query is an int
-
-        :raises APIException: Contains status code and error message
-        :return: News post object
-        :rtype: aiosu.models.news.NewsPost
-        """
-        url = f"{self.base_url}/api/v2/news/{news_query}"
-        params: dict[str, Any] = {
-            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
-        }
-        if "is_id" in kwargs or isinstance(news_query, int):
-            params["key"] = "id"
-        json = await self._request("GET", url, params=params)
-        return NewsPost.model_validate(json)
-
-    @prepare_token
-    async def get_wiki_page(self, locale: str, path: str) -> WikiPage:
-        r"""Gets a wiki page.
-
-        :param locale: The locale of the wiki page
-        :type locale: str
-        :param path: The path of the wiki page
-        :type path: str
-        :raises APIException: Contains status code and error message
-        :return: Wiki page object
-        :rtype: aiosu.models.wiki.WikiPage
-        """
-        url = f"{self.base_url}/api/v2/wiki/{locale}/{path}"
-        json = await self._request("GET", url)
-        return WikiPage.model_validate(json)
-
-    @prepare_token
-    async def get_comment(self, comment_id: int, **kwargs: Any) -> CommentBundle:
-        r"""Gets a comment.
-
-        :param comment_id: The ID of the comment
-        :type comment_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *cursor_string* (``str``) --
-                Optional, cursor string to get the next page of comments
-
-        :raises APIException: Contains status code and error message
-        :return: Comment bundle object
-        :rtype: aiosu.models.comment.CommentBundle
-        """
-        url = f"{self.base_url}/api/v2/comments/{comment_id}"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = CommentBundle.model_validate(json)
-        if resp.cursor_string:  # Unused: API does not return cursor_string
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_comment, comment_id=comment_id, **kwargs)
-        return resp
-
-    @prepare_token
-    async def get_comments(self, **kwargs: Any) -> CommentBundle:
-        r"""Gets comments.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *commentable_type* (``Literal["beatmapset", "build", "news_post", "user"]``) --
-                Optional, commentable type to get comments from
-            * *commentable_id* (``int``) --
-                Optional, commentable ID to get comments from
-            * *parent_id* (``int``) --
-                Optional, parent ID to get comments from
-            * *sort* (aiosu.models.comment.CommentSortType) --
-                Optional, sort order of comments, defaults to ``"new"``
-            * *cursor_string* (``str``) --
-                Optional, cursor string to get the next page of comments
-
-        :raises APIException: Contains status code and error message
-        :return: Comment bundle object
-        :rtype: aiosu.models.comment.CommentBundle
-        """
-        url = f"{self.base_url}/api/v2/comments"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="commentable_type")
-        add_param(params, kwargs, key="commentable_id")
-        add_param(params, kwargs, key="parent_id")
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = CommentBundle.model_validate(json)
-        if resp.cursor_string:  # Unused: API does not return cursor_string
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_comments, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def search(self, query: str, **kwargs: Any) -> SearchResponse:
-        r"""Searches for a user, beatmap, beatmapset, or wiki page.
-
-        :param query: The query to search for
-        :type query: str
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``Literal["all", "user", "wiki_page"]``) --
-                Optional, gamemode to search for, defaults to ``all``
-            * *page* (``int``) --
-                Optional, page to get, ignored if mode is ``all``
-
-        :raises APIException: Contains status code and error message
-        :return: Search response object
-        :rtype: aiosu.models.search.SearchResponse
-        """
-        url = f"{self.base_url}/api/v2/search"
-        params: dict[str, Any] = {
-            "query": query,
-            "mode": kwargs.pop("mode", "all"),
-        }
-        add_param(params, kwargs, key="page")
-        json = await self._request("GET", url, params=params)
-        return SearchResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_me(self, **kwargs: Any) -> User:
-        r"""Gets the user who owns the current token
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-
-        :raises APIException: Contains status code and error message
-        :return: Requested user
-        :rtype: aiosu.models.user.User
-        """
-        url = f"{self.base_url}/api/v2/me"
-        if "mode" in kwargs:
-            mode = Gamemode(kwargs.pop("mode"))
-            url += f"/{mode}"
-        json = await self._request("GET", url)
-        return User.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.FRIENDS_READ)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_own_friends(self) -> list[User]:
-        r"""Gets the token owner's friend list
-
-        :raises APIException: Contains status code and error message
-        :return: List of friends
-        :rtype: list[aiosu.models.user.User]
-        """
-        url = f"{self.base_url}/api/v2/friends"
-        json = await self._request("GET", url)
-        return from_list(User.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
-        r"""Gets a user by a query.
-
-        :param user_query: Username or ID to search by
-        :type user_query: Union[str, int]
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *qtype* (``str``) --
-                Optional, "string" or "id". Type of the user_query
-
-        :raises APIException: Contains status code and error message
-        :return: Requested user
-        :rtype: aiosu.models.user.User
-        """
-        url = f"{self.base_url}/api/v2/users/{user_query}"
-        params: dict[str, Any] = {}
-        if "mode" in kwargs:
-            mode = Gamemode(kwargs.pop("mode"))
-            url += f"/{mode}"
-        add_param(
-            params,
-            kwargs,
-            key="qtype",
-            param_name="type",
-            converter=lambda x: UserQueryType(x).new_api_name,
-        )
-        json = await self._request("GET", url, params=params)
-        return User.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_users(self, user_ids: list[int]) -> list[User]:
-        r"""Get multiple user data.
-
-        :param user_ids: The IDs of the users
-        :type user_ids: list[int]
-        :raises APIException: Contains status code and error message
-        :return: List of user data objects
-        :rtype: list[aiosu.models.user.User]
-        """
-        url = f"{self.base_url}/api/v2/users"
-        params: dict[str, Any] = {
-            "ids": user_ids,
-        }
-        json = await self._request("GET", url, params=params)
-        return from_list(User.model_validate, json.get("users", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user_kudosu(self, user_id: int, **kwargs: Any) -> list[KudosuHistory]:
-        r"""Get a user's kudosu history.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of scores to get
-            * *offset* (``int``) --
-                Optional, offset of the first score to get
-
-        :raises APIException: Contains status code and error message
-        :return: List of kudosu history objects
-        :rtype: list[aiosu.models.kudosu.KudosuHistory]
-        """
-        url = f"{self.base_url}/api/v2/users/{user_id}/kudosu"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="offset")
-        json = await self._request("GET", url, params=params)
-        return from_list(KudosuHistory.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def __get_type_scores(
-        self,
-        user_id: int,
-        request_type: str,
-        **kwargs: Any,
-    ) -> list[Union[Score, LazerScore]]:
-        r"""INTERNAL: Get a user's scores by type
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param request_type: "recent", "best" or "firsts"
-        :type request_type: str
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *offset* (``int``) --
-                Optional, page offset to start from, defaults to 0
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *include_fails* (``bool``) --
-                Optional, whether to include failed scores, defaults to ``False``
-            * *new_format* (``bool``) --
-                Optional, whether to use the new format, defaults to ``False``
-
-        :raises ValueError: If limit is not between 1 and 100
-        :raises ValueError: If type is invalid
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 100)) <= 100:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
-        if request_type not in ("recent", "best", "firsts", "pinned"):
-            raise ValueError(
-                f'"{request_type}" is not a valid request_type. Valid options are: "recent", "best", "firsts"',
-            )
-        url = f"{self.base_url}/api/v2/users/{user_id}/scores/{request_type}"
-        params: dict[str, Any] = {
-            "include_fails": int(kwargs.pop("include_fails", False)),
-            "limit": limit,
-            "offset": kwargs.pop("offset", 0),
-        }
-        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
-        headers = {}
-        new_format = kwargs.pop("new_format", False)
-        if new_format:
-            headers = {"x-api-version": "20220705"}
-        json = await self._request("GET", url, params=params, headers=headers)
-        if new_format:
-            return from_list(LazerScore.model_validate, json)
-        return from_list(Score.model_validate, json)
-
-    async def get_user_recents(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[Union[Score, LazerScore]]:
-        r"""Get a user's recent scores.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *include_fails* (``bool``) --
-                Optional, whether to include failed scores, defaults to ``False``
-            * *offset* (``int``) --
-                Optional, page offset to start from, defaults to 0
-            * *new_format* (``bool``) --
-                Optional, whether to use the new format, defaults to ``False``
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
-        """
-        return await self.__get_type_scores(user_id, "recent", **kwargs)
-
-    async def get_user_bests(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[Union[Score, LazerScore]]:
-        r"""Get a user's top scores.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *offset* (``int``) --
-                Optional, page offset to start from, defaults to 0
-            * *new_format* (``bool``) --
-                Optional, whether to use the new format, defaults to ``False``
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
-        """
-        return await self.__get_type_scores(user_id, "best", **kwargs)
-
-    async def get_user_firsts(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[Union[Score, LazerScore]]:
-        r"""Get a user's first place scores.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *offset* (``int``) --
-                Optional, page offset to start from, defaults to 0
-            * *new_format* (``bool``) --
-                Optional, whether to use the new format, defaults to ``False``
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
-        """
-        return await self.__get_type_scores(user_id, "firsts", **kwargs)
-
-    async def get_user_pinned(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[Union[Score, LazerScore]]:
-        r"""Get a user's pinned scores.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *offset* (``int``) --
-                Optional, page offset to start from, defaults to 0
-            * *new_format* (``bool``) --
-                Optional, whether to use the new format, defaults to ``False``
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
-        """
-        return await self.__get_type_scores(user_id, "pinned", **kwargs)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user_beatmap_scores(
-        self,
-        user_id: int,
-        beatmap_id: int,
-        **kwargs: Any,
-    ) -> list[Score]:
-        r"""Get a user's scores on a specific beatmap.
-
-        :param user_id: User ID to search by
-        :type user_id: int
-        :param beatmap_id: Beatmap ID to search by
-        :type beatmap_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores/users/{user_id}/all"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
-        json = await self._request("GET", url, params=params)
-        return from_list(Score.model_validate, json.get("scores", []))
-
-    UserBeatmapType = Literal["favourite", "graveyard", "loved", "ranked", "pending"]
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user_beatmaps(
-        self,
-        user_id: int,
-        type: UserBeatmapType,
-        **kwargs: Any,
-    ) -> list[Beatmapset]:
-        r"""Get a user's beatmaps.
-
-        :param user_id: ID of the user
-        :type user_id: int
-        :param type: Type of beatmaps to get
-        :type type: UserBeatmapType
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of beatmaps to get
-            * *offset* (``int``) --
-                Optional, offset of the first beatmap to get
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested beatmaps
-        :rtype: list[aiosu.models.beatmap.Beatmap]
-        """
-        url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/{type}"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="offset")
-        json = await self._request("GET", url, params=params)
-        return from_list(Beatmapset.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user_most_played(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[BeatmapUserPlaycount]:
-        r"""Get a user's most played beatmaps.
-
-        :param user_id: ID of the user
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of beatmaps to get
-            * *offset* (``int``) --
-                Optional, offset of the first beatmap to get
-
-        :raises APIException: Contains status code and error message
-        :return: List of user playcount objects
-        :rtype: list[aiosu.models.beatmap.BeatmapUserPlaycount]
-        """
-        url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/most_played"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="offset")
-        json = await self._request("GET", url, params=params)
-        return from_list(BeatmapUserPlaycount.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_user_recent_activity(
-        self,
-        user_id: int,
-        **kwargs: Any,
-    ) -> list[Event]:
-        r"""Get a user's recent activity.
-
-        :param user_id: ID of the user
-        :type user_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of events to get
-            * *offset* (``int``) --
-                Optional, offset of the first event to get
-
-        :raises APIException: Contains status code and error message
-        :return: List of events
-        :rtype: list[aiosu.models.event.Event]
-        """
-        url = f"{self.base_url}/api/v2/users/{user_id}/recent_activity"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="offset")
-        json = await self._request("GET", url, params=params)
-        return from_list(Event.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
-        r"""Get scores submitted on a specific beatmap.
-
-        :param beatmap_id: Beatmap ID to search by
-        :type beatmap_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *mods* (``aiosu.models.mods.Mods``) --
-                Optional, mods to search for
-            * *type* (``str``) --
-                Optional, beatmap score ranking type
-
-        :raises APIException: Contains status code and error message
-        :return: List of requested scores
-        :rtype: list[aiosu.models.score.Score]
-        """
-        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
-        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
-        add_param(params, kwargs, key="type")
-        json = await self._request("GET", url, params=params)
-        return from_list(Score.model_validate, json.get("scores", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmap(self, beatmap_id: int) -> Beatmap:
-        r"""Get beatmap data.
-
-        :param beatmap_id: The ID of the beatmap
-        :type beatmap_id: int
-        :raises APIException: Contains status code and error message
-        :return: Beatmap data object
-        :rtype: aiosu.models.beatmap.Beatmap
-        """
-        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}"
-        json = await self._request("GET", url)
-        return Beatmap.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmaps(self, beatmap_ids: list[int]) -> list[Beatmap]:
-        r"""Get multiple beatmap data.
-
-        :param beatmap_ids: The IDs of the beatmaps
-        :type beatmap_ids: list[int]
-        :raises APIException: Contains status code and error message
-        :return: List of beatmap data objects
-        :rtype: list[aiosu.models.beatmap.Beatmap]
-        """
-        url = f"{self.base_url}/api/v2/beatmaps"
-        params: dict[str, Any] = {
-            "ids": beatmap_ids,
-        }
-        json = await self._request("GET", url, params=params)
-        return from_list(Beatmap.model_validate, json.get("beatmaps", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def lookup_beatmap(self, **kwargs: Any) -> Beatmap:
-        r"""Lookup beatmap data.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *checksum* (``str``) --
-                Optional, the MD5 checksum of the beatmap
-            * *filename* (``str``) --
-                Optional, the filename of the beatmap
-            * *id* (``int``) --
-                Optional, the ID of the beatmap
-
-        :raises ValueError: If no arguments are specified
-        :raises APIException: Contains status code and error message
-        :return: Beatmap data object
-        :rtype: aiosu.models.beatmap.Beatmap
-        """
-        url = f"{self.base_url}/api/v2/beatmaps/lookup"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="checksum")
-        add_param(params, kwargs, key="filename")
-        add_param(params, kwargs, key="id")
-        if not params:
-            raise ValueError("One of checksum, filename or id must be provided.")
-        json = await self._request("GET", url, params=params)
-        return Beatmap.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmap_attributes(
-        self,
-        beatmap_id: int,
-        **kwargs: Any,
-    ) -> BeatmapDifficultyAttributes:
-        r"""Gets difficulty attributes for a beatmap.
-
-        :param beatmap_id: The ID of the beatmap
-        :type beatmap_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.gamemode.Gamemode``) --
-                Optional, gamemode to search for
-            * *mods* (``aiosu.models.mods.Mods``) --
-                Optional, mods to apply to the result
-
-        :raises APIException: Contains status code and error message
-        :return: Difficulty attributes for a beatmap
-        :rtype: aiosu.models.beatmap.BeatmapDifficultyAttributes
-        """
-        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/attributes"
-        data: dict[str, Any] = {}
-        add_param(
-            data,
-            kwargs,
-            key="mode",
-            param_name="ruleset_id",
-            converter=lambda x: int(Gamemode(x)),
-        )
-        add_param(data, kwargs, key="mods", converter=lambda x: int(Mods(x)))
-        json = await self._request("POST", url, json=data)
-        return BeatmapDifficultyAttributes.model_validate(json.get("attributes"))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
-        r"""Get beatmapset data.
-
-        :param beatmapset_id: The ID of the beatmapset
-        :type beatmapset_id: int
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset data object
-        :rtype: aiosu.models.beatmap.Beatmapset
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/{beatmapset_id}"
-        json = await self._request("GET", url)
-        return Beatmapset.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def lookup_beatmapset(self, beatmap_id: int) -> Beatmapset:
-        r"""Lookup beatmap data.
-
-        :param beatmap_id: The ID of a beatmap in the set
-        :type beatmap_id: int
-
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset data object
-        :rtype: aiosu.models.beatmap.Beatmapset
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/lookup"
-        params: dict[str, Any] = {
-            "beatmap_id": beatmap_id,
-        }
-        json = await self._request("GET", url, params=params)
-        return Beatmapset.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def search_beatmapsets(
-        self,
-        search_filter: Optional[str] = "",
-        **kwargs: Any,
-    ) -> BeatmapsetSearchResponse:
-        r"""Search beatmapset by filter.
-
-        :param search_filter: The search filter.
-        :type search_filter: str
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *cursor_string* (``str``) --
-                Optional, cursor string to get the next page of results
-
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset search response
-        :rtype: list[aiosu.models.beatmap.BeatmapsetSearchResponse]
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/search/{search_filter}"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url)
-        resp = BeatmapsetSearchResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.search_beatmapsets, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmapset_events(self, **kwargs: Any) -> list[BeatmapsetEvent]:
-        r"""Get beatmapset events.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of results per page
-            * *page* (``int``) --
-                Optional, page number
-            * *user_id* (``int``) --
-                Optional, user ID
-            * *min_date* (``datetime.datetime``) --
-                Optional, minimum date
-            * *max_date* (``datetime.datetime``) --
-                Optional, maximum date
-            * *types* (``list[aiosu.models.beatmap.BeatmapsetEventType]``) --
-                Optional, event types
-
-        :raises APIException: Contains status code and error message
-        :return: List of beatmapset events
-        :rtype: list[aiosu.models.event.Event]
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/events"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="page")
-        add_param(params, kwargs, key="user_id", param_name="user")
-        add_param(params, kwargs, key="min_date")
-        add_param(params, kwargs, key="max_date")
-        add_param(params, kwargs, key="types")
-        json = await self._request("GET", url, params=params)
-        return from_list(BeatmapsetEvent.model_validate, json.get("events", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmapset_discussions(
-        self,
-        **kwargs: Any,
-    ) -> BeatmapsetDiscussionResponse:
-        r"""Get beatmapset discussions.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *beatmap_id* (``int``) --
-                Optional, beatmap ID
-            * *beatmapset_id* (``int``) --
-                Optional, beatmapset ID
-            * *beatmapset_status* (``aiosu.models.beatmap.BeatmapsetRequestStatus``) --
-                Optional, beatmapset status
-            * *limit* (``int``) --
-                Optional, number of results per page
-            * *page* (``int``) --
-                Optional, page number
-            * *message_types* (``list[aiosu.models.beatmap.BeatmapsetDisscussionType]``) --
-                Optional, message types
-            * *only_unresolved* (``bool``) --
-                Optional, only unresolved discussions
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, sort order, defaults to ``id_desc``
-            * *user_id* (``int``) --
-                Optional, user ID
-            * with_deleted (``bool``) --
-                Optional, include deleted discussions
-            * cursor_string (``str``) --
-                Optional, cursor string
-
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset discussion response
-        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionResponse
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/discussions"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="beatmap_id")
-        add_param(params, kwargs, key="beatmapset_id")
-        add_param(params, kwargs, key="beatmapset_status")
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="page")
-        add_param(params, kwargs, key="message_types")
-        add_param(params, kwargs, key="only_unresolved", converter=to_lower_str)
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="user", param_name="user_id")
-        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_beatmapset_discussions, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmapset_discussion_posts(
-        self,
-        **kwargs: Any,
-    ) -> BeatmapsetDiscussionPostResponse:
-        r"""Get beatmapset discussion posts.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *beatmapset_discussion_id* (``int``) --
-                Optional, beatmapset discussion ID
-            * *limit* (``int``) --
-                Optional, number of results per page
-            * *page* (``int``) --
-                Optional, page number
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, sort order, defaults to ``id_desc``
-            * *types* (``list[str]``) --
-                Optional, post types
-            * *user_id* (``int``) --
-                Optional, user ID
-            * with_deleted (``bool``) --
-                Optional, include deleted discussions
-            * cursor_string (``str``) --
-                Optional, cursor string
-
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset discussion post response
-        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionPostResponse
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/discussions/posts"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="beatmapset_discussion_id")
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="page")
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="types")
-        add_param(params, kwargs, key="user", param_name="user_id")
-        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionPostResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_beatmapset_discussion_posts, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_beatmapset_discussion_votes(
-        self,
-        **kwargs: Any,
-    ) -> BeatmapsetDiscussionVoteResponse:
-        r"""Get beatmapset discussion votes.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *beatmapset_discussion_id* (``int``) --
-                Optional, beatmapset discussion ID
-            * *limit* (``int``) --
-                Optional, number of results per page
-            * *page* (``int``) --
-                Optional, page number
-            * *receiver_id* (``int``) --
-                Optional, receiver ID
-            * *score* (``aiosu.models.beatmap.BeatmapsetDiscussionVoteScore``) --
-                Optional, vote score
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, sort order, defaults to ``id_desc``
-            * *user_id* (``int``) --
-                Optional, user ID
-            * with_deleted (``bool``) --
-                Optional, include deleted discussions
-            * cursor_string (``str``) --
-                Optional, cursor string
-
-        :raises APIException: Contains status code and error message
-        :return: Beatmapset discussion vote response
-        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionVoteResponse
-        """
-        url = f"{self.base_url}/api/v2/beatmapsets/discussions/votes"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="beatmapset_discussion_id")
-        add_param(params, kwargs, key="limit")
-        add_param(params, kwargs, key="page")
-        add_param(params, kwargs, key="receiver", param_name="receiver_id")
-        add_param(params, kwargs, key="score")
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="user", param_name="user_id")
-        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = BeatmapsetDiscussionVoteResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_beatmapset_discussion_votes, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_score(
-        self,
-        score_id: int,
-        mode: Gamemode,
-    ) -> Score:
-        r"""Gets data about a score.
-
-        :param score_id: The ID of the score
-        :type score_id: int
-        :param mode: The gamemode to search for
-        :type mode: aiosu.models.gamemode.Gamemode
-
-        :raises APIException: Contains status code and error message
-        :return: Score data object
-        :rtype: aiosu.models.score.Score
-        """
-        url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}"
-        json = await self._request("GET", url)
-        return Score.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_score_replay(
-        self,
-        score_id: int,
-        mode: Gamemode,
-    ) -> BytesIO:
-        r"""Gets the replay file for a score.
-
-        :param score_id: The ID of the score
-        :type score_id: int
-        :param mode: The gamemode to search for
-        :type mode: aiosu.models.gamemode.Gamemode
-
-        :raises APIException: Contains status code and error message
-        :return: Replay file
-        :rtype: io.BytesIO
-        """
-        url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}/download"
-        return await self._request("GET", url)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_rankings(
-        self,
-        mode: Gamemode,
-        type: RankingType,
-        **kwargs: Any,
-    ) -> Rankings:
-        r"""Get rankings.
-
-        :param mode: The gamemode to search for
-        :type mode: aiosu.models.gamemode.Gamemode
-        :param type: The ranking type to search for
-        :type type: aiosu.models.rankings.RankingType
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *country* (``str``) --
-                Optional, country code
-            * *filter* (``aiosu.models.rankings.RankingFilter``) --
-                Optional, ranking filter
-            * *spotlight* (``int``) --
-                Optional, spotlight ID
-            * *variant* (``aiosu.models.rankings.RankingVariant``) --
-                Optional, ranking variant
-            * *cursor_string* (``str``) --
-                Optional, cursor string
-
-        :raises APIException: Contains status code and error message
-        :return: Rankings
-        :rtype: aiosu.models.rankings.Rankings
-        """
-        url = f"{self.base_url}/api/v2/rankings/{mode}/{type}"
-        params: dict[str, Any] = {}
-        add_param(params, kwargs, key="country")
-        add_param(params, kwargs, key="filter")
-        add_param(params, kwargs, key="spotlight")
-        add_param(params, kwargs, key="variant")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = Rankings.model_validate(json)
-        if resp.cursor_string:  # Unused: API does not return cursor_string
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_rankings, mode=mode, type=type, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_spotlights(self) -> list[Spotlight]:
-        r"""Gets the current spotlights.
-
-        :raises APIException: Contains status code and error message
-        :return: List of spotlights
-        :rtype: list[aiosu.models.spotlight.Spotlight]
-        """
-        url = f"{self.base_url}/api/v2/spotlights"
-        json = await self._request("GET", url)
-        return from_list(Spotlight.model_validate, json.get("spotlights", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_forum_topic(self, topic_id: int, **kwargs: Any) -> ForumTopicResponse:
-        r"""Gets a forum topic.
-
-        :param topic_id: The ID of the topic
-        :type topic_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the number of posts to return. Min: 1, Max: 50, defaults to 20
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, the sort type to use. Defaults to ``id_asc``
-            * *start* (``int``) --
-                Optional, the start post ID to use for pagination.
-            * *end* (``int``) --
-                Optional, the end post ID to use for pagination.
-            * *cursor_string* (``str``) --
-                Optional, the cursor string to use for pagination.
-
-        :raises APIException: Contains status code and error message
-        :return: Forum topic response object
-        :rtype: aiosu.models.forum.ForumTopicResponse
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 20)) <= 50:
-            raise ValueError("Invalid limit specified. Limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/forums/topics/{topic_id}"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="start")
-        add_param(params, kwargs, key="end")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = ForumTopicResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_forum_topic, topic_id, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.FORUM_WRITE)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def create_forum_topic(
-        self,
-        forum_id: int,
-        title: str,
-        content: str,
-        **kwargs: Any,
-    ) -> ForumCreateTopicResponse:
-        r"""Creates a forum topic.
-
-        :param forum_id: The ID of the forum to create the topic in
-        :type forum_id: int
-        :param title: The title of the topic
-        :type title: str
-        :param content: The content of the topic
-        :type content: str
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *with_poll* (``bool``) --
-                Optional, whether to create a poll with the topic. Defaults to ``False``
-            * *poll_title* (``str``) --
-                Optional, the title of the poll
-            * *poll_options* (``list[str]``) --
-                Optional, the options for the poll
-            * *poll_length_days* (``int``) --
-                Optional, the length of the poll in days. Defaults to 0
-            * *poll_vote_change* (``bool``) --
-                Optional, whether to allow users to change their vote. Defaults to ``False``
-            * *poll_hide_results* (``bool``) --
-                Optional, whether to hide the results of the poll. Defaults to ``False``
-            * *poll_max_votes* (``int``) --
-                Optional, the maximum number of votes a user can make. Defaults to 1
-
-        :raises APIException: Contains status code and error message
-        :return: Forum create topic response object
-        :rtype: aiosu.models.forum.ForumCreateTopicResponse
-        """
-        url = f"{self.base_url}/api/v2/forums/topics"
-        data: dict[str, Any] = {
-            "forum_id": forum_id,
-            "title": title,
-            "body": content,
-        }
-        add_param(data, kwargs, key="with_poll")
-        if data.get("with_poll"):
-            forum_topic_poll: dict[str, Any] = {
-                "title": kwargs["poll_title"],
-                "length_days": kwargs.pop("poll_length_days", 0),
-                "vote_change": kwargs.pop("poll_vote_change", False),
-                "hide_results": kwargs.pop("poll_hide_results", False),
-                "max_votes": kwargs.pop("poll_max_votes", 1),
-            }
-            add_param(
-                forum_topic_poll,
-                kwargs,
-                key="options",
-                param_name="poll_options",
-            )
-            data["forum_topic_poll"] = forum_topic_poll
-        json = await self._request("POST", url, json=data)
-        return ForumCreateTopicResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.FORUM_WRITE)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def reply_forum_topic(self, topic_id: int, content: str) -> ForumPost:
-        r"""Replies to a forum topic.
-
-        :param topic_id: The ID of the topic
-        :type topic_id: int
-        :param content: The content of the post
-        :type content: str
-        :raises APIException: Contains status code and error message
-        :return: Forum post object
-        :rtype: aiosu.models.forum.ForumPost
-        """
-        url = f"{self.base_url}/api/v2/forums/topics/{topic_id}/reply"
-        data: dict[str, str] = {
-            "body": content,
-        }
-        json = await self._request("POST", url, json=data)
-        return ForumPost.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.FORUM_WRITE)
-    async def edit_forum_topic_title(self, topid_id: int, new_title: str) -> ForumTopic:
-        r"""Edits a forum topic's title.
-
-        :param topid_id: The ID of the topic
-        :type topid_id: int
-        :param new_title: The new title of the topic
-        :type new_title: str
-        :raises APIException: Contains status code and error message
-        :return: Forum topic object
-        :rtype: aiosu.models.forum.ForumTopic
-        """
-        url = f"{self.base_url}/api/v2/forums/topics/{topid_id}/title"
-        data: dict[str, dict[str, str]] = {
-            "forum_topic": {
-                "topic_title": new_title,
-            },
-        }
-        json = await self._request("PUT", url, json=data)
-        return ForumTopic.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.FORUM_WRITE)
-    async def edit_forum_post(self, post_id: int, new_content: str) -> ForumPost:
-        r"""Edits a forum post.
-
-        :param post_id: The ID of the post
-        :type post_id: int
-        :param new_content: The new content of the post
-        :type new_content: str
-        :raises APIException: Contains status code and error message
-        :return: Forum post object
-        :rtype: aiosu.models.forum.ForumPost
-        """
-        url = f"{self.base_url}/api/v2/forums/posts/{post_id}"
-        data: dict[str, str] = {
-            "body": new_content,
-        }
-        json = await self._request("PUT", url, json=data)
-        return ForumPost.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_chat_ack(self, **kwargs: Any) -> list[ChatUserSilence]:
-        r"""Gets chat acknowledgement.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *since* (``int``) --
-                Optional, the last message ID received
-            * *silence_id_since* (``int``) --
-                Optional, the last silence ID received
-
-        :raises APIException: Contains status code and error message
-        :return: List of chat user silence objects
-        :rtype: list[aiosu.models.chat.ChatUserSilence]
-        """
-        url = f"{self.base_url}/api/v2/chat/ack"
-        data: dict[str, Any] = {}
-        add_param(data, kwargs, key="since")
-        add_param(data, kwargs, key="silence_id_since", param_name="history_since")
-        json = await self._request("POST", url, json=data)
-        return from_list(ChatUserSilence.model_validate, json.get("silences", []))
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_chat_updates(self, since: int, **kwargs: Any) -> ChatUpdateResponse:
-        r"""Gets chat updates.
-
-        :param since: The last message ID received
-        :type since: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the maximum number of messages to return. Min: 1, Max: 50. Defaults to 50
-            * *channel_id* (``int``) --
-                Optional, the channel ID to get messages from
-            * *silence_id_since* (``int``) --
-                Optional, the last silence ID received
-            * *includes* (``list[aiosu.models.chat.ChatIncludeTypes]``) --
-                Optional, the additional information to include. Defaults to all.
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: Chat update response object
-        :rtype: aiosu.models.chat.ChatUpdateResponse
-        """
-        if not 1 <= (limit := kwargs.get("limit", 50)) <= 50:
-            raise ValueError("limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/chat/updates"
-        params: dict[str, Any] = {
-            "since": since,
-            "limit:": limit,
-        }
-        add_param(params, kwargs, key="channel_id")
-        add_param(params, kwargs, key="includes")
-        add_param(params, kwargs, key="silence_id_since", param_name="history_since")
-        json = await self._request("GET", url, params=params)
-        return ChatUpdateResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_channel(self, channel_id: int) -> ChatChannelResponse:
-        r"""Gets channel.
-
-        :param channel_id: The channel ID to get
-        :type channel_id: int
-        :raises APIException: Contains status code and error message
-        :return: Chat channel object
-        :rtype: aiosu.models.chat.ChatChannelResponse
-        """
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}"
-        json = await self._request("GET", url)
-        return ChatChannelResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_channels(self) -> list[ChatChannel]:
-        r"""Gets a list of joinable public channels.
-
-        :raises APIException: Contains status code and error message
-        :return: List of chat channel objects
-        :rtype: list[aiosu.models.chat.ChatChannel]
-        """
-        url = f"{self.base_url}/api/v2/chat/channels"
-        json = await self._request("GET", url)
-        return from_list(ChatChannel.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_channel_messages(
-        self,
-        channel_id: int,
-        **kwargs: Any,
-    ) -> list[ChatMessage]:
-        r"""Gets channel messages.
-
-        :param channel_id: The channel ID to get messages from
-        :type channel_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the maximum number of messages to return. Min: 1, Max: 50. Defaults to 50
-            * *since* (``int``) --
-                Optional, the ID of the oldest message to return
-            * *until* (``int``) --
-                Optional, the ID of the newest message to return
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: List of chat message objects
-        :rtype: list[aiosu.models.chat.ChatMessage]
-        """
-        if not 1 <= (limit := kwargs.get("limit", 50)) <= 50:
-            raise ValueError("limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
-        params: dict[str, Any] = {
-            "limit:": limit,
-        }
-        add_param(params, kwargs, key="since")
-        add_param(params, kwargs, key="until")
-        json = await self._request("GET", url, params=params)
-        return from_list(ChatMessage.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.CHAT_WRITE)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def create_chat_channel(
-        self,
-        type: ChatChannelTypes,
-        **kwargs: Any,
-    ) -> ChatChannel:
-        r"""Creates a chat channel.
-
-        :param type: The type of the channel.
-        :type type: aiosu.models.chat.ChatChannelType
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *message* (``str``) --
-                Required if type is ``ANNOUNCE``, the message to send in the PM
-            * *target_id* (``int``) --
-                Only used if if type is ``PM``, the ID of the user to send a PM to
-            * *target_ids* (``List[int]``) --
-                Only used if type is ``ANNOUNCE``, the IDs of the users to send a PM to
-            * *channel_name* (``str``) --
-                Only used if type is ``ANNOUNCE``, the name of the channel
-            * *channel_description* (``str``) --
-                Only used if type is ``ANNOUNCE``, the description of the channel
-
-        :raises ValueError: If missing required parameters
-        :raises APIException: Contains status code and error message
-        :return: Chat channel object
-        :rtype: aiosu.models.chat.ChatChannel
-        """
-        url = f"{self.base_url}/api/v2/chat/channels"
-        data: dict[str, Any] = {
-            "type": type,
-        }
-        add_param(data, kwargs, key="message")
-        if type == "PM":
-            if not add_param(data, kwargs, key="target_id"):
-                raise ValueError("Missing target ID")
-        elif type == "ANNOUNCE":
-            if not add_param(data, kwargs, key="target_ids"):
-                raise ValueError("Missing target IDs")
-            if not data.get("message"):
-                raise ValueError("Missing message")
-            channel = {
-                "name": kwargs["channel_name"],
-                "description": kwargs["channel_description"],
-            }
-            data["channel"] = channel
-        json = await self._request("POST", url, json=data)
-        return ChatChannel.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def join_channel(self, channel_id: int, user_id: int) -> ChatChannel:
-        r"""Joins a channel.
-
-        :param channel_id: The channel ID to join
-        :type channel_id: int
-        :param user_id: The user ID to join as
-        :type user_id: int
-        :raises APIException: Contains status code and error message
-        :return: Chat channel object
-        :rtype: aiosu.models.chat.ChatChannel
-        """
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
-        json = await self._request("PUT", url)
-        return ChatChannel.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def leave_channel(self, channel_id: int, user_id: int) -> None:
-        r"""Leaves a channel.
-
-        :param channel_id: The channel ID to leave
-        :type channel_id: int
-        :param user_id: The user ID to leave as
-        :type user_id: int
-        :raises APIException: Contains status code and error message
-        """
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
-        await self._request("DELETE", url)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def mark_read(self, channel_id: int, message_id: int) -> None:
-        r"""Marks a channel as read.
-
-        :param channel_id: The channel ID to mark as read
-        :type channel_id: int
-        :param message_id: The message ID to mark as read up to
-        :type message_id: int
-        :raises APIException: Contains status code and error message
-        """
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/mark-as-read/{message_id}"
-        await self._request("PUT", url)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.LAZER)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def send_message(
-        self,
-        channel_id: int,
-        message: str,
-        is_action: bool,
-    ) -> ChatMessage:
-        r"""Sends a message to a channel.
-
-        :param channel_id: The ID of the channel
-        :type channel_id: int
-        :param message: The message to send
-        :type message: str
-        :param is_action: Whether the message is an action
-        :type is_action: bool
-        :raises APIException: Contains status code and error message
-        :return: Chat message object
-        :rtype: aiosu.models.chat.ChatMessage
-        """
-        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
-        data: dict[str, Any] = {
-            "message": message,
-            "is_action": is_action,
-        }
-        json = await self._request("POST", url, json=data)
-        return ChatMessage.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.CHAT_WRITE)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def send_private_message(
-        self,
-        user_id: int,
-        message: str,
-        is_action: bool,
-        **kwargs: Any,
-    ) -> ChatMessageCreateResponse:
-        r"""Sends a message to a user.
-
-        :param user_id: The ID of the user
-        :type user_id: int
-        :param message: The message to send
-        :type message: str
-        :param is_action: Whether the message is an action
-        :type is_action: bool
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *uuid* (``str``) --
-                Optional, client-side message identifier to be sent back in response and websocket json
-
-        :raises APIException: Contains status code and error message
-        :return: Chat message create response object
-        :rtype: aiosu.models.chat.ChatMessageCreateResponse
-        """
-        url = f"{self.base_url}/api/v2/chat/new"
-        data: dict[str, Any] = {
-            "target_id": user_id,
-            "message": message,
-            "is_action": is_action,
-        }
-        add_param(data, kwargs, key="uuid")
-        json = await self._request("POST", url, json=data)
-        return ChatMessageCreateResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_multiplayer_matches(
-        self,
-        **kwargs: Any,
-    ) -> MultiplayerMatchesResponse:
-        r"""Gets the multiplayer matches.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, the sort type
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
-            * *cursor_string* (``str``) --
-                Optional, the cursor string to get the next page of results
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: Multiplayer matches response object
-        :rtype: aiosu.models.multiplayer.MultiplayerMatchesResponse
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 50:
-            raise ValueError("Limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/matches"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="sort")
-        json = await self._request("GET", url, params=params)
-        resp = MultiplayerMatchesResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(self.get_multiplayer_matches, **kwargs)
-        return resp
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_multiplayer_match(
-        self,
-        match_id: int,
-        **kwargs: Any,
-    ) -> MultiplayerMatchResponse:
-        r"""Gets a multiplayer match.
-
-        :param match_id: The ID of the match
-        :type match_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
-            * *before* (``int``) --
-                Optional, the ID of the score to get the scores before
-            * *after* (``int``) --
-                Optional, the ID of the score to get the scores after
-
-        :raises ValueError: If limit is not between 1 and 100
-        :raises APIException: Contains status code and error message
-        :return: Multiplayer match response object
-        :rtype: aiosu.models.multiplayer.MultiplayerMatchResponse
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 100:
-            raise ValueError("Limit must be between 1 and 100")
-        url = f"{self.base_url}/api/v2/matches/{match_id}"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="before")
-        add_param(params, kwargs, key="after")
-        json = await self._request("GET", url)
-        return MultiplayerMatchResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_multiplayer_rooms(self, **kwargs: Any) -> list[MultiplayerRoom]:
-        r"""Gets the multiplayer rooms.
-
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *mode* (``aiosu.models.multiplayer.MultiplayerRoomMode``) --
-                Optional, the multiplayer room mode
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
-            * *sort* (``aiosu.models.common.SortTypes``) --
-                Optional, the sort type
-            * *category* (``aiosu.models.multiplayer.MultiplayerRoomCategories``) --
-                Optional, the multiplayer room category
-            * *type* (``aiosu.models.multiplayer.MultiplayerRoomTypeGroups``) --
-                Optional, the multiplayer room type group
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: List of multiplayer rooms
-        :rtype: list[aiosu.models.multiplayer.MultiplayerRoom]
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
-            raise ValueError("Limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/rooms"
-        if "mode" in kwargs:
-            mode: MultiplayerRoomMode = kwargs.pop("mode")
-            url += f"/{mode}"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="category")
-        add_param(params, kwargs, key="type", param_name="type_group")
-        json = await self._request("GET", url, params=params)
-        return from_list(MultiplayerRoom.model_validate, json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_multiplayer_room(self, room_id: int) -> MultiplayerRoom:
-        r"""Gets a multiplayer room.
-
-        :param room_id: The ID of the room
-        :type room_id: int
-
-        :raises APIException: Contains status code and error message
-        :return: Multiplayer room object
-        :rtype: aiosu.models.multiplayer.MultiplayerRoom
-        """
-        url = f"{self.base_url}/api/v2/rooms/{room_id}"
-        json = await self._request("GET", url)
-        return MultiplayerRoom.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
-    async def get_multiplayer_leaderboard(
-        self,
-        room_id: int,
-        **kwargs: Any,
-    ) -> MultiplayerLeaderboardResponse:
-        r"""Gets the multiplayer leaderboard for a room.
-
-        :param room_id: The ID of the room
-        :type room_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
-
-        :raises ValueError: If limit is not between 1 and 50
-        :raises APIException: Contains status code and error message
-        :return: Multiplayer leaderboard response object
-        :rtype: aiosu.models.multiplayer.MultiplayerLeaderboardResponse
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
-            raise ValueError("Limit must be between 1 and 50")
-        url = f"{self.base_url}/api/v2/rooms/{room_id}/leaderboard"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        json = await self._request("GET", url, params=params)
-        return MultiplayerLeaderboardResponse.model_validate(json)
-
-    @prepare_token
-    @check_token
-    @requires_scope(Scopes.PUBLIC)
-    async def get_multiplayer_scores(
-        self,
-        room_id: int,
-        playlist_id: int,
-        **kwargs: Any,
-    ) -> MultiplayerScoresResponse:
-        r"""Gets the multiplayer scores for a room.
-
-        :param room_id: The ID of the room
-        :type room_id: int
-        :param playlist_id: The ID of the playlist
-        :type playlist_id: int
-        :param \**kwargs:
-            See below
-
-        :Keyword Arguments:
-            * *limit* (``int``) --
-                Optional, the number of scores to return
-            * *sort* (``aiosu.models.multiplayer.MultiplayerScoreSortType``) --
-                Optional, the sort order of the scores
-            * *cursor_string* (``str``) --
-                Optional, the cursor string to use for pagination
-
-        :raises ValueError: If limit is not between 1 and 100
-        :raises APIException: Contains status code and error message
-        :return: Multiplayer scores response object
-        :rtype: aiosu.models.multiplayer.MultiplayerScoresResponse
-        """
-        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 100:
-            raise ValueError("Limit must be between 1 and 100")
-        url = f"{self.base_url}/api/v2/rooms/{room_id}/playlist/{playlist_id}/scores"
-        params: dict[str, Any] = {
-            "limit": limit,
-        }
-        add_param(params, kwargs, key="sort")
-        add_param(params, kwargs, key="cursor_string")
-        json = await self._request("GET", url, params=params)
-        resp = MultiplayerScoresResponse.model_validate(json)
-        if resp.cursor_string:
-            kwargs["cursor_string"] = resp.cursor_string
-            resp.next = partial(
-                self.get_multiplayer_scores,
-                room_id,
-                playlist_id,
-                **kwargs,
-            )
-        return resp
-
-    @prepare_token
-    @check_token
-    async def revoke_token(self) -> None:
-        r"""Revokes the current token and closes the session.
-
-        :raises APIException: Contains status code and error message
-        """
-        url = f"{self.base_url}/api/v2/oauth/tokens/current"
-        await self._request("DELETE", url)
-        await self._delete_token()
-        await self.close()
-
-    async def close(self) -> None:
-        """Closes the client session."""
-        if self._session:
-            await self._session.close()
-            self._session = None
+"""
+This module handles API requests for API v2 (OAuth).
+
+You can read more about it here: https://osu.ppy.sh/docs/index.html
+"""
+from __future__ import annotations
+
+import functools
+from datetime import datetime
+from functools import partial
+from io import BytesIO
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import Literal
+from typing import TYPE_CHECKING
+from typing import TypeVar
+from warnings import warn
+
+import aiohttp
+import orjson
+from aiolimiter import AsyncLimiter
+
+from ..events import ClientUpdateEvent
+from ..events import Eventable
+from ..exceptions import APIException
+from ..helpers import add_param
+from ..helpers import from_list
+from ..models import ArtistResponse
+from ..models import Beatmap
+from ..models import BeatmapDifficultyAttributes
+from ..models import Beatmapset
+from ..models import BeatmapsetDiscussionPostResponse
+from ..models import BeatmapsetDiscussionResponse
+from ..models import BeatmapsetDiscussionVoteResponse
+from ..models import BeatmapsetEvent
+from ..models import BeatmapsetSearchResponse
+from ..models import BeatmapUserPlaycount
+from ..models import Build
+from ..models import ChangelogListing
+from ..models import ChatChannel
+from ..models import ChatChannelResponse
+from ..models import ChatChannelTypes
+from ..models import ChatMessage
+from ..models import ChatMessageCreateResponse
+from ..models import ChatUpdateResponse
+from ..models import ChatUserSilence
+from ..models import CommentBundle
+from ..models import Event
+from ..models import ForumCreateTopicResponse
+from ..models import ForumPost
+from ..models import ForumTopic
+from ..models import ForumTopicResponse
+from ..models import Gamemode
+from ..models import KudosuHistory
+from ..models import LazerScore
+from ..models import Mods
+from ..models import MultiplayerLeaderboardResponse
+from ..models import MultiplayerMatchesResponse
+from ..models import MultiplayerMatchResponse
+from ..models import MultiplayerRoom
+from ..models import MultiplayerRoomMode
+from ..models import MultiplayerScoresResponse
+from ..models import NewsListing
+from ..models import NewsPost
+from ..models import OAuthToken
+from ..models import Rankings
+from ..models import RankingType
+from ..models import Scopes
+from ..models import Score
+from ..models import SearchResponse
+from ..models import SeasonalBackgroundSet
+from ..models import Spotlight
+from ..models import User
+from ..models import UserQueryType
+from ..models import WikiPage
+from .repository import BaseTokenRepository
+from .repository import SimpleTokenRepository
+
+if TYPE_CHECKING:
+    from types import TracebackType
+    from typing import Optional
+    from typing import Type
+    from typing import Union
+
+__all__ = ("Client",)
+
+F = TypeVar("F", bound=Callable[..., Any])
+ClientRequestType = Literal["GET", "POST", "DELETE", "PUT", "PATCH"]
+
+
+def to_lower_str(value: Any) -> str:
+    """Converts a value to a lowercase string."""
+    return str(value).lower()
+
+
+def get_content_type(content_type: str) -> str:
+    """Returns the content type."""
+    return content_type.split(";")[0]
+
+
+def prepare_token(func: F) -> F:
+    """A decorator that prepares the token for use, to be used as:
+    @prepare_token
+    """
+
+    @functools.wraps(func)
+    async def _prepare_token(self: Client, *args: Any, **kwargs: Any) -> Any:
+        await self._prepare_token()
+
+        return await func(self, *args, **kwargs)
+
+    return cast(F, _prepare_token)
+
+
+def check_token(func: F) -> F:
+    """
+    A decorator that checks the current token, to be used as:
+    @check_token
+    """
+
+    @functools.wraps(func)
+    async def _check_token(self: Client, *args: Any, **kwargs: Any) -> Any:
+        token = await self.get_current_token()
+        if datetime.utcnow().timestamp() > token.expires_on.timestamp():
+            await self._refresh()
+        return await func(self, *args, **kwargs)
+
+    return cast(F, _check_token)
+
+
+def requires_scope(
+    required_scopes: Scopes,
+    any_scope: bool = False,
+) -> Callable[[F], F]:
+    """
+    A decorator that enforces a scope, to be used as:
+    @requires_scope(Scopes.PUBLIC)
+    """
+
+    def _requires_scope(
+        func: F,
+    ) -> F:
+        @functools.wraps(func)
+        async def _wrap(self: Client, *args: Any, **kwargs: Any) -> Any:
+            token = await self.get_current_token()
+            if any_scope:
+                if not (required_scopes & token.scopes):
+                    raise APIException(403, "Missing required scopes.")
+            elif required_scopes & token.scopes != required_scopes:
+                raise APIException(403, "Missing required scopes.")
+
+            return await func(self, *args, **kwargs)
+
+        return cast(F, _wrap)
+
+    return _requires_scope
+
+
+class Client(Eventable):
+    r"""osu! API v2 Client
+
+    :param \**kwargs:
+        See below
+
+    :Keyword Arguments:
+        * *token_repository* (``aiosu.v2.repository.BaseTokenRepository``) --
+            Optional, defaults to ``aiosu.v2.repository.SimpleTokenRepository()``
+        * *session_id* (``int``) --
+            Optional, ID of the session to search in the repository, defaults to 0
+        * *client_id* (``int``) --
+            Optional, required to refresh tokens
+        * *client_secret* (``str``) --
+            Optional, required to refresh tokens
+        * *base_url* (``str``) --
+            Optional, base API URL, defaults to "https://osu.ppy.sh"
+        * *token* (``aiosu.models.oauthtoken.OAuthToken``) --
+            Optional, defaults to client credentials if not provided
+        * *limiter* (``tuple[int, int]``) --
+            Optional, rate limit, defaults to (600, 60) (600 requests per minute)
+    """
+
+    __slots__ = (
+        "_token_repository",
+        "_initial_token",
+        "_session",
+        "_limiter",
+        "session_id",
+        "client_id",
+        "client_secret",
+        "base_url",
+    )
+
+    def __init__(
+        self,
+        **kwargs: Any,
+    ) -> None:
+        super().__init__()
+        self._register_event(ClientUpdateEvent)
+        self._token_repository: BaseTokenRepository = kwargs.pop(
+            "token_repository",
+            SimpleTokenRepository(),
+        )
+        max_rate, time_period = kwargs.pop("limiter", (600, 60))
+        if (
+            not isinstance(self._token_repository, SimpleTokenRepository)
+            and "session_id" not in kwargs
+        ):
+            warn(
+                "You are using a custom token repository, but did not provide a session ID. This may cause unexpected behavior.",
+            )
+        if (max_rate / time_period) > (1000 / 60):
+            warn(
+                "You are running at an insanely high rate limit. Doing so may result in your account being banned.",
+            )
+        self.session_id: int = kwargs.pop("session_id", 0)
+        self.client_id: int = kwargs.pop("client_id", None)
+        self.client_secret: str = kwargs.pop("client_secret", None)
+        self._initial_token: Optional[OAuthToken] = kwargs.pop("token", None)
+        self.base_url: str = kwargs.pop("base_url", "https://osu.ppy.sh")
+        self._limiter: AsyncLimiter = AsyncLimiter(
+            max_rate=max_rate,
+            time_period=time_period,
+        )
+        self._session: Optional[aiohttp.ClientSession] = None
+
+    async def __aenter__(self) -> Client:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        await self.close()
+
+    def on_client_update(
+        self,
+        func: F,
+    ) -> F:
+        """
+        A decorator that is called whenever a client is updated, to be used as:
+
+            @client.on_client_update
+
+            async def func(event: ClientUpdateEvent)
+        """
+        self._register_listener(func, ClientUpdateEvent)
+
+        @functools.wraps(func)
+        async def _on_client_update(*args: Any, **kwargs: Any) -> Any:
+            return await func(*args, **kwargs)
+
+        return cast(F, _on_client_update)
+
+    async def get_current_token(self) -> OAuthToken:
+        """Get the current token"""
+        return await self._token_repository.get(self.session_id)
+
+    async def _prepare_token(self) -> None:
+        """Prepare the token for use."""
+        if not await self._token_exists():
+            token_to_add = self._initial_token
+            if token_to_add is None:
+                token_to_add = OAuthToken()
+            await self._add_token(token_to_add)
+        elif self._initial_token is not None:
+            await self._update_token(self._initial_token)
+        self._initial_token = None
+
+    async def _add_token(self, token: OAuthToken) -> None:
+        """Add a token to the current session"""
+        await self._token_repository.add(self.session_id, token)
+
+    async def _update_token(self, token: OAuthToken) -> None:
+        """Update the current token"""
+        await self._token_repository.update(self.session_id, token)
+
+    async def _token_exists(self) -> bool:
+        """Check if a token exists for the current session"""
+        return await self._token_repository.exists(self.session_id)
+
+    async def _delete_token(self) -> None:
+        """Delete the current token"""
+        await self._token_repository.delete(self.session_id)
+
+    async def _get_headers(self) -> dict[str, str]:
+        token = await self.get_current_token()
+        return {
+            "Authorization": f"Bearer {token.access_token}",
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+        }
+
+    async def _refresh_auth_data(self) -> dict[str, Union[str, int]]:
+        token = await self.get_current_token()
+        return {
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "grant_type": "refresh_token",
+            "refresh_token": token.refresh_token,
+        }
+
+    def _refresh_guest_data(self) -> dict[str, Union[str, int]]:
+        return {
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "grant_type": "client_credentials",
+            "scope": "public",
+        }
+
+    async def _request(
+        self,
+        request_type: ClientRequestType,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Any:
+        await self._prepare_token()
+
+        if self._session is None:
+            self._session = aiohttp.ClientSession(headers=await self._get_headers())
+
+        req: dict[str, Callable] = {
+            "GET": self._session.get,
+            "POST": self._session.post,
+            "DELETE": self._session.delete,
+            "PUT": self._session.put,
+            "PATCH": self._session.patch,
+        }
+
+        async with self._limiter:
+            async with req[request_type](*args, **kwargs) as resp:
+                if resp.status == 204:
+                    return
+
+                body = await resp.read()
+                content_type = get_content_type(resp.headers.get("content-type", ""))
+                if resp.status != 200:
+                    json = orjson.loads(body)
+                    raise APIException(resp.status, json.get("error", ""))
+                if content_type == "application/json":
+                    return orjson.loads(body)
+                if content_type == "application/octet-stream":
+                    return BytesIO(body)
+                if content_type.startswith("application/x-osu"):
+                    return BytesIO(body)
+                if content_type == "text/plain":
+                    return body.decode()
+                raise APIException(415, f"Unhandled Content Type '{content_type}'")
+
+    async def _refresh(self) -> None:
+        r"""INTERNAL: Refreshes the client's token
+
+        :raises APIException: Contains status code and error message
+        """
+        old_token = await self.get_current_token()
+        url = f"{self.base_url}/oauth/token"
+
+        data = {}
+        if old_token.can_refresh:
+            data = await self._refresh_auth_data()
+        else:
+            data = self._refresh_guest_data()
+
+        async with aiohttp.ClientSession() as temp_session:
+            async with self._limiter:
+                async with temp_session.post(url, json=data) as resp:
+                    try:
+                        body = await resp.read()
+                        content_type = get_content_type(
+                            resp.headers.get("content-type", ""),
+                        )
+                        if content_type != "application/json":
+                            raise APIException(
+                                415,
+                                f"Unhandled Content Type '{content_type}'",
+                            )
+                        json = orjson.loads(body)
+                        if resp.status != 200:
+                            raise APIException(resp.status, json.get("error", ""))
+                        if self._session:
+                            await self._session.close()
+                        new_token = OAuthToken.model_validate(json)
+                        await self._update_token(new_token)
+                        self._session = aiohttp.ClientSession(
+                            headers=await self._get_headers(),
+                        )
+                    except aiohttp.client_exceptions.ContentTypeError:
+                        raise APIException(403, "Invalid token specified.")
+
+        await self._process_event(
+            ClientUpdateEvent(client=self, old_token=old_token, new_token=new_token),
+        )
+
+    @prepare_token
+    async def get_featured_artists(self, **kwargs: Any) -> ArtistResponse:
+        r"""Gets the current featured artists.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the number of featured artists to return.
+            * *album* (``str``) --
+                Optional, the album to filter by.
+            * *artist* (``str``) --
+                Optional, the artist to filter by.
+            * *genre* (``int``) --
+                Optional, the genre ID to filter by.
+            * *length* (``list[int]``) --
+                Optional, the length range to filter by.
+            * *bpm* (``list[int]``) --
+                Optional, The BPM range to filter by.
+            * *query* (``str``) --
+                Optional, the search query to filter by.
+            * *is_default_sort* (``bool``) --
+                Optional, whether to sort by the default sort.
+            * *sort* (``str``) --
+                Optional, the sort to use.
+
+        :raises APIException: Contains status code and error message
+        :return: Featured artist response object
+        :rtype: aiosu.models.artist.ArtistResponse
+        """
+        url = f"{self.base_url}/beatmaps/artists/tracks"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="album")
+        add_param(params, kwargs, key="artist")
+        add_param(params, kwargs, key="genre")
+        add_param(params, kwargs, key="length")
+        add_param(params, kwargs, key="bpm")
+        add_param(params, kwargs, key="query")
+        add_param(params, kwargs, key="is_default_sort", converter=to_lower_str)
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url)
+        resp = ArtistResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_featured_artists, **kwargs)
+        return resp
+
+    @prepare_token
+    async def get_seasonal_backgrounds(self) -> SeasonalBackgroundSet:
+        r"""Gets the current seasonal background set.
+
+        :raises APIException: Contains status code and error message
+        :return: Seasonal background set object
+        :rtype: aiosu.models.backgrounds.SeasonalBackgroundSet
+        """
+        url = f"{self.base_url}/api/v2/seasonal-backgrounds"
+        json = await self._request("GET", url)
+        return SeasonalBackgroundSet.model_validate(json)
+
+    @prepare_token
+    async def get_changelog_listing(self, **kwargs: Any) -> ChangelogListing:
+        r"""Gets the changelog listing.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *message_formats* (``list[str]``) --
+                Optional, the message formats to return.
+            * *from* (``str``) --
+                Optional, the start date to return.
+            * *to* (``str``) --
+                Optional, the end date to return.
+            * *max_id* (``int``) --
+                Optional, the maximum ID to return.
+            * *stream* (``str``) --
+                Optional, the stream to return.
+            * *cursor_string* (``str``) --
+                Optional, the cursor string to use.
+
+        :raises APIException: Contains status code and error message
+        :return: Changelog listing object
+        :rtype: aiosu.models.changelog.ChangelogListing
+        """
+        url = f"{self.base_url}/api/v2/changelog"
+        params: dict[str, Any] = {
+            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
+        }
+        add_param(params, kwargs, key="from")
+        add_param(params, kwargs, key="to")
+        add_param(params, kwargs, key="max_id")
+        add_param(params, kwargs, key="stream")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = ChangelogListing.model_validate(json)
+        if resp.cursor_string:  # Unused: API does not return cursor_string
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_changelog_listing, **kwargs)
+        return resp
+
+    @prepare_token
+    async def get_changelog_build(self, stream: str, build: str) -> Build:
+        r"""Gets a specific build from the changelog.
+
+        :param stream: The stream to get the build from
+        :param build: The build to get
+        :raises APIException: Contains status code and error message
+        :return: Build object
+        :rtype: aiosu.models.changelog.Build
+        """
+        url = f"{self.base_url}/api/v2/changelog/{stream}/{build}"
+        json = await self._request("GET", url)
+        return Build.model_validate(json)
+
+    @prepare_token
+    async def lookup_changelog_build(
+        self,
+        changelog_query: Union[str, int],
+        **kwargs: Any,
+    ) -> Build:
+        r"""Looks up a build from the changelog.
+
+        :param changelog_query: The query to search for
+        :type changelog_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *is_id* (``bool``) --
+                Optional, whether the query is an ID or not, defaults to ``True`` if the query is an int
+            * *message_formats* (``list[aiosu.models.news.ChangelogMessageFormats]``) --
+                Optional, message formats to get, defaults to ``["html", "markdown"]``
+
+        :raises APIException: Contains status code and error message
+        :return: Build object
+        :rtype: aiosu.models.changelog.Build
+        """
+        url = f"{self.base_url}/api/v2/changelog/{changelog_query}"
+        params: dict[str, Any] = {
+            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
+        }
+        if "is_id" in kwargs or isinstance(changelog_query, int):
+            params["key"] = "id"
+        json = await self._request("GET", url, params=params)
+        return Build.model_validate(json)
+
+    @prepare_token
+    async def get_news_listing(self, **kwargs: Any) -> NewsListing:
+        r"""Gets the news listing.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the number of news posts to return. Min: 1, Max: 21, defaults to 12
+            * *year* (``int``) --
+                Optional, the year to filter by.
+            * *cursor_string* (``str``) --
+                Optional, the cursor string to use for pagination.
+
+        :raises APIException: Contains status code and error message
+        :return: News listing object
+        :rtype: aiosu.models.news.NewsListing
+        """
+        url = f"{self.base_url}/api/v2/news"
+        if not 1 <= (limit := kwargs.pop("limit", 12)) <= 21:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 21")
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="year")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = NewsListing.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_news_listing, **kwargs)
+        return resp
+
+    @prepare_token
+    async def get_news_post(
+        self,
+        news_query: Union[str, int],
+        **kwargs: Any,
+    ) -> NewsPost:
+        r"""Gets a news post.
+
+        :param news_query: The query to search for
+        :type news_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *is_id* (``bool``) --
+                Optional, whether the query is an ID or not, defaults to ``True`` if the query is an int
+
+        :raises APIException: Contains status code and error message
+        :return: News post object
+        :rtype: aiosu.models.news.NewsPost
+        """
+        url = f"{self.base_url}/api/v2/news/{news_query}"
+        params: dict[str, Any] = {
+            "message_formats": kwargs.pop("message_formats", ["html", "markdown"]),
+        }
+        if "is_id" in kwargs or isinstance(news_query, int):
+            params["key"] = "id"
+        json = await self._request("GET", url, params=params)
+        return NewsPost.model_validate(json)
+
+    @prepare_token
+    async def get_wiki_page(self, locale: str, path: str) -> WikiPage:
+        r"""Gets a wiki page.
+
+        :param locale: The locale of the wiki page
+        :type locale: str
+        :param path: The path of the wiki page
+        :type path: str
+        :raises APIException: Contains status code and error message
+        :return: Wiki page object
+        :rtype: aiosu.models.wiki.WikiPage
+        """
+        url = f"{self.base_url}/api/v2/wiki/{locale}/{path}"
+        json = await self._request("GET", url)
+        return WikiPage.model_validate(json)
+
+    @prepare_token
+    async def get_comment(self, comment_id: int, **kwargs: Any) -> CommentBundle:
+        r"""Gets a comment.
+
+        :param comment_id: The ID of the comment
+        :type comment_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *cursor_string* (``str``) --
+                Optional, cursor string to get the next page of comments
+
+        :raises APIException: Contains status code and error message
+        :return: Comment bundle object
+        :rtype: aiosu.models.comment.CommentBundle
+        """
+        url = f"{self.base_url}/api/v2/comments/{comment_id}"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = CommentBundle.model_validate(json)
+        if resp.cursor_string:  # Unused: API does not return cursor_string
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_comment, comment_id=comment_id, **kwargs)
+        return resp
+
+    @prepare_token
+    async def get_comments(self, **kwargs: Any) -> CommentBundle:
+        r"""Gets comments.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *commentable_type* (``Literal["beatmapset", "build", "news_post", "user"]``) --
+                Optional, commentable type to get comments from
+            * *commentable_id* (``int``) --
+                Optional, commentable ID to get comments from
+            * *parent_id* (``int``) --
+                Optional, parent ID to get comments from
+            * *sort* (aiosu.models.comment.CommentSortType) --
+                Optional, sort order of comments, defaults to ``"new"``
+            * *cursor_string* (``str``) --
+                Optional, cursor string to get the next page of comments
+
+        :raises APIException: Contains status code and error message
+        :return: Comment bundle object
+        :rtype: aiosu.models.comment.CommentBundle
+        """
+        url = f"{self.base_url}/api/v2/comments"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="commentable_type")
+        add_param(params, kwargs, key="commentable_id")
+        add_param(params, kwargs, key="parent_id")
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = CommentBundle.model_validate(json)
+        if resp.cursor_string:  # Unused: API does not return cursor_string
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_comments, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def search(self, query: str, **kwargs: Any) -> SearchResponse:
+        r"""Searches for a user, beatmap, beatmapset, or wiki page.
+
+        :param query: The query to search for
+        :type query: str
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``Literal["all", "user", "wiki_page"]``) --
+                Optional, gamemode to search for, defaults to ``all``
+            * *page* (``int``) --
+                Optional, page to get, ignored if mode is ``all``
+
+        :raises APIException: Contains status code and error message
+        :return: Search response object
+        :rtype: aiosu.models.search.SearchResponse
+        """
+        url = f"{self.base_url}/api/v2/search"
+        params: dict[str, Any] = {
+            "query": query,
+            "mode": kwargs.pop("mode", "all"),
+        }
+        add_param(params, kwargs, key="page")
+        json = await self._request("GET", url, params=params)
+        return SearchResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_me(self, **kwargs: Any) -> User:
+        r"""Gets the user who owns the current token
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+
+        :raises APIException: Contains status code and error message
+        :return: Requested user
+        :rtype: aiosu.models.user.User
+        """
+        url = f"{self.base_url}/api/v2/me"
+        if "mode" in kwargs:
+            mode = Gamemode(kwargs.pop("mode"))
+            url += f"/{mode}"
+        json = await self._request("GET", url)
+        return User.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.FRIENDS_READ)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_own_friends(self) -> list[User]:
+        r"""Gets the token owner's friend list
+
+        :raises APIException: Contains status code and error message
+        :return: List of friends
+        :rtype: list[aiosu.models.user.User]
+        """
+        url = f"{self.base_url}/api/v2/friends"
+        json = await self._request("GET", url)
+        return from_list(User.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user(self, user_query: Union[str, int], **kwargs: Any) -> User:
+        r"""Gets a user by a query.
+
+        :param user_query: Username or ID to search by
+        :type user_query: Union[str, int]
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *qtype* (``str``) --
+                Optional, "string" or "id". Type of the user_query
+
+        :raises APIException: Contains status code and error message
+        :return: Requested user
+        :rtype: aiosu.models.user.User
+        """
+        url = f"{self.base_url}/api/v2/users/{user_query}"
+        params: dict[str, Any] = {}
+        if "mode" in kwargs:
+            mode = Gamemode(kwargs.pop("mode"))
+            url += f"/{mode}"
+        add_param(
+            params,
+            kwargs,
+            key="qtype",
+            param_name="type",
+            converter=lambda x: UserQueryType(x).new_api_name,
+        )
+        json = await self._request("GET", url, params=params)
+        return User.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_users(self, user_ids: list[int]) -> list[User]:
+        r"""Get multiple user data.
+
+        :param user_ids: The IDs of the users
+        :type user_ids: list[int]
+        :raises APIException: Contains status code and error message
+        :return: List of user data objects
+        :rtype: list[aiosu.models.user.User]
+        """
+        url = f"{self.base_url}/api/v2/users"
+        params: dict[str, Any] = {
+            "ids": user_ids,
+        }
+        json = await self._request("GET", url, params=params)
+        return from_list(User.model_validate, json.get("users", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user_kudosu(self, user_id: int, **kwargs: Any) -> list[KudosuHistory]:
+        r"""Get a user's kudosu history.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of scores to get
+            * *offset* (``int``) --
+                Optional, offset of the first score to get
+
+        :raises APIException: Contains status code and error message
+        :return: List of kudosu history objects
+        :rtype: list[aiosu.models.kudosu.KudosuHistory]
+        """
+        url = f"{self.base_url}/api/v2/users/{user_id}/kudosu"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="offset")
+        json = await self._request("GET", url, params=params)
+        return from_list(KudosuHistory.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def __get_type_scores(
+        self,
+        user_id: int,
+        request_type: str,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""INTERNAL: Get a user's scores by type
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param request_type: "recent", "best" or "firsts"
+        :type request_type: str
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *include_fails* (``bool``) --
+                Optional, whether to include failed scores, defaults to ``False``
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises ValueError: If limit is not between 1 and 100
+        :raises ValueError: If type is invalid
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 100)) <= 100:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 100")
+        if request_type not in ("recent", "best", "firsts", "pinned"):
+            raise ValueError(
+                f'"{request_type}" is not a valid request_type. Valid options are: "recent", "best", "firsts"',
+            )
+        url = f"{self.base_url}/api/v2/users/{user_id}/scores/{request_type}"
+        params: dict[str, Any] = {
+            "include_fails": int(kwargs.pop("include_fails", False)),
+            "limit": limit,
+            "offset": kwargs.pop("offset", 0),
+        }
+        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
+        headers = {}
+        new_format = kwargs.pop("new_format", False)
+        if new_format:
+            headers = {"x-api-version": "20220705"}
+        json = await self._request("GET", url, params=params, headers=headers)
+        if new_format:
+            return from_list(LazerScore.model_validate, json)
+        return from_list(Score.model_validate, json)
+
+    async def get_user_recents(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""Get a user's recent scores.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *include_fails* (``bool``) --
+                Optional, whether to include failed scores, defaults to ``False``
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        return await self.__get_type_scores(user_id, "recent", **kwargs)
+
+    async def get_user_bests(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""Get a user's top scores.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        return await self.__get_type_scores(user_id, "best", **kwargs)
+
+    async def get_user_firsts(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""Get a user's first place scores.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        return await self.__get_type_scores(user_id, "firsts", **kwargs)
+
+    async def get_user_pinned(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Union[Score, LazerScore]]:
+        r"""Get a user's pinned scores.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *offset* (``int``) --
+                Optional, page offset to start from, defaults to 0
+            * *new_format* (``bool``) --
+                Optional, whether to use the new format, defaults to ``False``
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score] or list[aiosu.models.score.LazerScore]
+        """
+        return await self.__get_type_scores(user_id, "pinned", **kwargs)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user_beatmap_scores(
+        self,
+        user_id: int,
+        beatmap_id: int,
+        **kwargs: Any,
+    ) -> list[Score]:
+        r"""Get a user's scores on a specific beatmap.
+
+        :param user_id: User ID to search by
+        :type user_id: int
+        :param beatmap_id: Beatmap ID to search by
+        :type beatmap_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores/users/{user_id}/all"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
+        json = await self._request("GET", url, params=params)
+        return from_list(Score.model_validate, json.get("scores", []))
+
+    UserBeatmapType = Literal["favourite", "graveyard", "loved", "ranked", "pending"]
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user_beatmaps(
+        self,
+        user_id: int,
+        type: UserBeatmapType,
+        **kwargs: Any,
+    ) -> list[Beatmapset]:
+        r"""Get a user's beatmaps.
+
+        :param user_id: ID of the user
+        :type user_id: int
+        :param type: Type of beatmaps to get
+        :type type: UserBeatmapType
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of beatmaps to get
+            * *offset* (``int``) --
+                Optional, offset of the first beatmap to get
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested beatmaps
+        :rtype: list[aiosu.models.beatmap.Beatmap]
+        """
+        url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/{type}"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="offset")
+        json = await self._request("GET", url, params=params)
+        return from_list(Beatmapset.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user_most_played(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[BeatmapUserPlaycount]:
+        r"""Get a user's most played beatmaps.
+
+        :param user_id: ID of the user
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of beatmaps to get
+            * *offset* (``int``) --
+                Optional, offset of the first beatmap to get
+
+        :raises APIException: Contains status code and error message
+        :return: List of user playcount objects
+        :rtype: list[aiosu.models.beatmap.BeatmapUserPlaycount]
+        """
+        url = f"{self.base_url}/api/v2/users/{user_id}/beatmapsets/most_played"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="offset")
+        json = await self._request("GET", url, params=params)
+        return from_list(BeatmapUserPlaycount.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_user_recent_activity(
+        self,
+        user_id: int,
+        **kwargs: Any,
+    ) -> list[Event]:
+        r"""Get a user's recent activity.
+
+        :param user_id: ID of the user
+        :type user_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of events to get
+            * *offset* (``int``) --
+                Optional, offset of the first event to get
+
+        :raises APIException: Contains status code and error message
+        :return: List of events
+        :rtype: list[aiosu.models.event.Event]
+        """
+        url = f"{self.base_url}/api/v2/users/{user_id}/recent_activity"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="offset")
+        json = await self._request("GET", url, params=params)
+        return from_list(Event.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmap_scores(self, beatmap_id: int, **kwargs: Any) -> list[Score]:
+        r"""Get scores submitted on a specific beatmap.
+
+        :param beatmap_id: Beatmap ID to search by
+        :type beatmap_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *mods* (``aiosu.models.mods.Mods``) --
+                Optional, mods to search for
+            * *type* (``str``) --
+                Optional, beatmap score ranking type
+
+        :raises APIException: Contains status code and error message
+        :return: List of requested scores
+        :rtype: list[aiosu.models.score.Score]
+        """
+        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/scores"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="mode", converter=lambda x: str(Gamemode(x)))
+        add_param(params, kwargs, key="mods", converter=lambda x: str(Mods(x)))
+        add_param(params, kwargs, key="type")
+        json = await self._request("GET", url, params=params)
+        return from_list(Score.model_validate, json.get("scores", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmap(self, beatmap_id: int) -> Beatmap:
+        r"""Get beatmap data.
+
+        :param beatmap_id: The ID of the beatmap
+        :type beatmap_id: int
+        :raises APIException: Contains status code and error message
+        :return: Beatmap data object
+        :rtype: aiosu.models.beatmap.Beatmap
+        """
+        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}"
+        json = await self._request("GET", url)
+        return Beatmap.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmaps(self, beatmap_ids: list[int]) -> list[Beatmap]:
+        r"""Get multiple beatmap data.
+
+        :param beatmap_ids: The IDs of the beatmaps
+        :type beatmap_ids: list[int]
+        :raises APIException: Contains status code and error message
+        :return: List of beatmap data objects
+        :rtype: list[aiosu.models.beatmap.Beatmap]
+        """
+        url = f"{self.base_url}/api/v2/beatmaps"
+        params: dict[str, Any] = {
+            "ids": beatmap_ids,
+        }
+        json = await self._request("GET", url, params=params)
+        return from_list(Beatmap.model_validate, json.get("beatmaps", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def lookup_beatmap(self, **kwargs: Any) -> Beatmap:
+        r"""Lookup beatmap data.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *checksum* (``str``) --
+                Optional, the MD5 checksum of the beatmap
+            * *filename* (``str``) --
+                Optional, the filename of the beatmap
+            * *id* (``int``) --
+                Optional, the ID of the beatmap
+
+        :raises ValueError: If no arguments are specified
+        :raises APIException: Contains status code and error message
+        :return: Beatmap data object
+        :rtype: aiosu.models.beatmap.Beatmap
+        """
+        url = f"{self.base_url}/api/v2/beatmaps/lookup"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="checksum")
+        add_param(params, kwargs, key="filename")
+        add_param(params, kwargs, key="id")
+        if not params:
+            raise ValueError("One of checksum, filename or id must be provided.")
+        json = await self._request("GET", url, params=params)
+        return Beatmap.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmap_attributes(
+        self,
+        beatmap_id: int,
+        **kwargs: Any,
+    ) -> BeatmapDifficultyAttributes:
+        r"""Gets difficulty attributes for a beatmap.
+
+        :param beatmap_id: The ID of the beatmap
+        :type beatmap_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.gamemode.Gamemode``) --
+                Optional, gamemode to search for
+            * *mods* (``aiosu.models.mods.Mods``) --
+                Optional, mods to apply to the result
+
+        :raises APIException: Contains status code and error message
+        :return: Difficulty attributes for a beatmap
+        :rtype: aiosu.models.beatmap.BeatmapDifficultyAttributes
+        """
+        url = f"{self.base_url}/api/v2/beatmaps/{beatmap_id}/attributes"
+        data: dict[str, Any] = {}
+        add_param(
+            data,
+            kwargs,
+            key="mode",
+            param_name="ruleset_id",
+            converter=lambda x: int(Gamemode(x)),
+        )
+        add_param(data, kwargs, key="mods", converter=lambda x: int(Mods(x)))
+        json = await self._request("POST", url, json=data)
+        return BeatmapDifficultyAttributes.model_validate(json.get("attributes"))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmapset(self, beatmapset_id: int) -> Beatmapset:
+        r"""Get beatmapset data.
+
+        :param beatmapset_id: The ID of the beatmapset
+        :type beatmapset_id: int
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset data object
+        :rtype: aiosu.models.beatmap.Beatmapset
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/{beatmapset_id}"
+        json = await self._request("GET", url)
+        return Beatmapset.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def lookup_beatmapset(self, beatmap_id: int) -> Beatmapset:
+        r"""Lookup beatmap data.
+
+        :param beatmap_id: The ID of a beatmap in the set
+        :type beatmap_id: int
+
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset data object
+        :rtype: aiosu.models.beatmap.Beatmapset
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/lookup"
+        params: dict[str, Any] = {
+            "beatmap_id": beatmap_id,
+        }
+        json = await self._request("GET", url, params=params)
+        return Beatmapset.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def search_beatmapsets(
+        self,
+        search_filter: Optional[str] = "",
+        **kwargs: Any,
+    ) -> BeatmapsetSearchResponse:
+        r"""Search beatmapset by filter.
+
+        :param search_filter: The search filter.
+        :type search_filter: str
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *cursor_string* (``str``) --
+                Optional, cursor string to get the next page of results
+
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset search response
+        :rtype: list[aiosu.models.beatmap.BeatmapsetSearchResponse]
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/search/{search_filter}"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url)
+        resp = BeatmapsetSearchResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.search_beatmapsets, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmapset_events(self, **kwargs: Any) -> list[BeatmapsetEvent]:
+        r"""Get beatmapset events.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of results per page
+            * *page* (``int``) --
+                Optional, page number
+            * *user_id* (``int``) --
+                Optional, user ID
+            * *min_date* (``datetime.datetime``) --
+                Optional, minimum date
+            * *max_date* (``datetime.datetime``) --
+                Optional, maximum date
+            * *types* (``list[aiosu.models.beatmap.BeatmapsetEventType]``) --
+                Optional, event types
+
+        :raises APIException: Contains status code and error message
+        :return: List of beatmapset events
+        :rtype: list[aiosu.models.event.Event]
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/events"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="page")
+        add_param(params, kwargs, key="user_id", param_name="user")
+        add_param(params, kwargs, key="min_date")
+        add_param(params, kwargs, key="max_date")
+        add_param(params, kwargs, key="types")
+        json = await self._request("GET", url, params=params)
+        return from_list(BeatmapsetEvent.model_validate, json.get("events", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmapset_discussions(
+        self,
+        **kwargs: Any,
+    ) -> BeatmapsetDiscussionResponse:
+        r"""Get beatmapset discussions.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *beatmap_id* (``int``) --
+                Optional, beatmap ID
+            * *beatmapset_id* (``int``) --
+                Optional, beatmapset ID
+            * *beatmapset_status* (``aiosu.models.beatmap.BeatmapsetRequestStatus``) --
+                Optional, beatmapset status
+            * *limit* (``int``) --
+                Optional, number of results per page
+            * *page* (``int``) --
+                Optional, page number
+            * *message_types* (``list[aiosu.models.beatmap.BeatmapsetDisscussionType]``) --
+                Optional, message types
+            * *only_unresolved* (``bool``) --
+                Optional, only unresolved discussions
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, sort order, defaults to ``id_desc``
+            * *user_id* (``int``) --
+                Optional, user ID
+            * with_deleted (``bool``) --
+                Optional, include deleted discussions
+            * cursor_string (``str``) --
+                Optional, cursor string
+
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset discussion response
+        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionResponse
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/discussions"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="beatmap_id")
+        add_param(params, kwargs, key="beatmapset_id")
+        add_param(params, kwargs, key="beatmapset_status")
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="page")
+        add_param(params, kwargs, key="message_types")
+        add_param(params, kwargs, key="only_unresolved", converter=to_lower_str)
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="user", param_name="user_id")
+        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = BeatmapsetDiscussionResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_beatmapset_discussions, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmapset_discussion_posts(
+        self,
+        **kwargs: Any,
+    ) -> BeatmapsetDiscussionPostResponse:
+        r"""Get beatmapset discussion posts.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *beatmapset_discussion_id* (``int``) --
+                Optional, beatmapset discussion ID
+            * *limit* (``int``) --
+                Optional, number of results per page
+            * *page* (``int``) --
+                Optional, page number
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, sort order, defaults to ``id_desc``
+            * *types* (``list[str]``) --
+                Optional, post types
+            * *user_id* (``int``) --
+                Optional, user ID
+            * with_deleted (``bool``) --
+                Optional, include deleted discussions
+            * cursor_string (``str``) --
+                Optional, cursor string
+
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset discussion post response
+        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionPostResponse
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/discussions/posts"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="beatmapset_discussion_id")
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="page")
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="types")
+        add_param(params, kwargs, key="user", param_name="user_id")
+        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = BeatmapsetDiscussionPostResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_beatmapset_discussion_posts, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_beatmapset_discussion_votes(
+        self,
+        **kwargs: Any,
+    ) -> BeatmapsetDiscussionVoteResponse:
+        r"""Get beatmapset discussion votes.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *beatmapset_discussion_id* (``int``) --
+                Optional, beatmapset discussion ID
+            * *limit* (``int``) --
+                Optional, number of results per page
+            * *page* (``int``) --
+                Optional, page number
+            * *receiver_id* (``int``) --
+                Optional, receiver ID
+            * *score* (``aiosu.models.beatmap.BeatmapsetDiscussionVoteScore``) --
+                Optional, vote score
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, sort order, defaults to ``id_desc``
+            * *user_id* (``int``) --
+                Optional, user ID
+            * with_deleted (``bool``) --
+                Optional, include deleted discussions
+            * cursor_string (``str``) --
+                Optional, cursor string
+
+        :raises APIException: Contains status code and error message
+        :return: Beatmapset discussion vote response
+        :rtype: aiosu.models.beatmap.BeatmapsetDiscussionVoteResponse
+        """
+        url = f"{self.base_url}/api/v2/beatmapsets/discussions/votes"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="beatmapset_discussion_id")
+        add_param(params, kwargs, key="limit")
+        add_param(params, kwargs, key="page")
+        add_param(params, kwargs, key="receiver", param_name="receiver_id")
+        add_param(params, kwargs, key="score")
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="user", param_name="user_id")
+        add_param(params, kwargs, key="with_deleted", converter=to_lower_str)
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = BeatmapsetDiscussionVoteResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_beatmapset_discussion_votes, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_score(
+        self,
+        score_id: int,
+        mode: Gamemode,
+    ) -> Score:
+        r"""Gets data about a score.
+
+        :param score_id: The ID of the score
+        :type score_id: int
+        :param mode: The gamemode to search for
+        :type mode: aiosu.models.gamemode.Gamemode
+
+        :raises APIException: Contains status code and error message
+        :return: Score data object
+        :rtype: aiosu.models.score.Score
+        """
+        url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}"
+        json = await self._request("GET", url)
+        return Score.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_score_replay(
+        self,
+        score_id: int,
+        mode: Gamemode,
+    ) -> BytesIO:
+        r"""Gets the replay file for a score.
+
+        :param score_id: The ID of the score
+        :type score_id: int
+        :param mode: The gamemode to search for
+        :type mode: aiosu.models.gamemode.Gamemode
+
+        :raises APIException: Contains status code and error message
+        :return: Replay file
+        :rtype: io.BytesIO
+        """
+        url = f"{self.base_url}/api/v2/scores/{mode}/{score_id}/download"
+        return await self._request("GET", url)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_rankings(
+        self,
+        mode: Gamemode,
+        type: RankingType,
+        **kwargs: Any,
+    ) -> Rankings:
+        r"""Get rankings.
+
+        :param mode: The gamemode to search for
+        :type mode: aiosu.models.gamemode.Gamemode
+        :param type: The ranking type to search for
+        :type type: aiosu.models.rankings.RankingType
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *country* (``str``) --
+                Optional, country code
+            * *filter* (``aiosu.models.rankings.RankingFilter``) --
+                Optional, ranking filter
+            * *spotlight* (``int``) --
+                Optional, spotlight ID
+            * *variant* (``aiosu.models.rankings.RankingVariant``) --
+                Optional, ranking variant
+            * *cursor_string* (``str``) --
+                Optional, cursor string
+
+        :raises APIException: Contains status code and error message
+        :return: Rankings
+        :rtype: aiosu.models.rankings.Rankings
+        """
+        url = f"{self.base_url}/api/v2/rankings/{mode}/{type}"
+        params: dict[str, Any] = {}
+        add_param(params, kwargs, key="country")
+        add_param(params, kwargs, key="filter")
+        add_param(params, kwargs, key="spotlight")
+        add_param(params, kwargs, key="variant")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = Rankings.model_validate(json)
+        if resp.cursor_string:  # Unused: API does not return cursor_string
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_rankings, mode=mode, type=type, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_spotlights(self) -> list[Spotlight]:
+        r"""Gets the current spotlights.
+
+        :raises APIException: Contains status code and error message
+        :return: List of spotlights
+        :rtype: list[aiosu.models.spotlight.Spotlight]
+        """
+        url = f"{self.base_url}/api/v2/spotlights"
+        json = await self._request("GET", url)
+        return from_list(Spotlight.model_validate, json.get("spotlights", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_forum_topic(self, topic_id: int, **kwargs: Any) -> ForumTopicResponse:
+        r"""Gets a forum topic.
+
+        :param topic_id: The ID of the topic
+        :type topic_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the number of posts to return. Min: 1, Max: 50, defaults to 20
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, the sort type to use. Defaults to ``id_asc``
+            * *start* (``int``) --
+                Optional, the start post ID to use for pagination.
+            * *end* (``int``) --
+                Optional, the end post ID to use for pagination.
+            * *cursor_string* (``str``) --
+                Optional, the cursor string to use for pagination.
+
+        :raises APIException: Contains status code and error message
+        :return: Forum topic response object
+        :rtype: aiosu.models.forum.ForumTopicResponse
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 20)) <= 50:
+            raise ValueError("Invalid limit specified. Limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/forums/topics/{topic_id}"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="start")
+        add_param(params, kwargs, key="end")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = ForumTopicResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_forum_topic, topic_id, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.FORUM_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def create_forum_topic(
+        self,
+        forum_id: int,
+        title: str,
+        content: str,
+        **kwargs: Any,
+    ) -> ForumCreateTopicResponse:
+        r"""Creates a forum topic.
+
+        :param forum_id: The ID of the forum to create the topic in
+        :type forum_id: int
+        :param title: The title of the topic
+        :type title: str
+        :param content: The content of the topic
+        :type content: str
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *with_poll* (``bool``) --
+                Optional, whether to create a poll with the topic. Defaults to ``False``
+            * *poll_title* (``str``) --
+                Optional, the title of the poll
+            * *poll_options* (``list[str]``) --
+                Optional, the options for the poll
+            * *poll_length_days* (``int``) --
+                Optional, the length of the poll in days. Defaults to 0
+            * *poll_vote_change* (``bool``) --
+                Optional, whether to allow users to change their vote. Defaults to ``False``
+            * *poll_hide_results* (``bool``) --
+                Optional, whether to hide the results of the poll. Defaults to ``False``
+            * *poll_max_votes* (``int``) --
+                Optional, the maximum number of votes a user can make. Defaults to 1
+
+        :raises APIException: Contains status code and error message
+        :return: Forum create topic response object
+        :rtype: aiosu.models.forum.ForumCreateTopicResponse
+        """
+        url = f"{self.base_url}/api/v2/forums/topics"
+        data: dict[str, Any] = {
+            "forum_id": forum_id,
+            "title": title,
+            "body": content,
+        }
+        add_param(data, kwargs, key="with_poll")
+        if data.get("with_poll"):
+            forum_topic_poll: dict[str, Any] = {
+                "title": kwargs["poll_title"],
+                "length_days": kwargs.pop("poll_length_days", 0),
+                "vote_change": kwargs.pop("poll_vote_change", False),
+                "hide_results": kwargs.pop("poll_hide_results", False),
+                "max_votes": kwargs.pop("poll_max_votes", 1),
+            }
+            add_param(
+                forum_topic_poll,
+                kwargs,
+                key="options",
+                param_name="poll_options",
+            )
+            data["forum_topic_poll"] = forum_topic_poll
+        json = await self._request("POST", url, json=data)
+        return ForumCreateTopicResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.FORUM_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def reply_forum_topic(self, topic_id: int, content: str) -> ForumPost:
+        r"""Replies to a forum topic.
+
+        :param topic_id: The ID of the topic
+        :type topic_id: int
+        :param content: The content of the post
+        :type content: str
+        :raises APIException: Contains status code and error message
+        :return: Forum post object
+        :rtype: aiosu.models.forum.ForumPost
+        """
+        url = f"{self.base_url}/api/v2/forums/topics/{topic_id}/reply"
+        data: dict[str, str] = {
+            "body": content,
+        }
+        json = await self._request("POST", url, json=data)
+        return ForumPost.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.FORUM_WRITE)
+    async def edit_forum_topic_title(self, topid_id: int, new_title: str) -> ForumTopic:
+        r"""Edits a forum topic's title.
+
+        :param topid_id: The ID of the topic
+        :type topid_id: int
+        :param new_title: The new title of the topic
+        :type new_title: str
+        :raises APIException: Contains status code and error message
+        :return: Forum topic object
+        :rtype: aiosu.models.forum.ForumTopic
+        """
+        url = f"{self.base_url}/api/v2/forums/topics/{topid_id}/title"
+        data: dict[str, dict[str, str]] = {
+            "forum_topic": {
+                "topic_title": new_title,
+            },
+        }
+        json = await self._request("PUT", url, json=data)
+        return ForumTopic.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.FORUM_WRITE)
+    async def edit_forum_post(self, post_id: int, new_content: str) -> ForumPost:
+        r"""Edits a forum post.
+
+        :param post_id: The ID of the post
+        :type post_id: int
+        :param new_content: The new content of the post
+        :type new_content: str
+        :raises APIException: Contains status code and error message
+        :return: Forum post object
+        :rtype: aiosu.models.forum.ForumPost
+        """
+        url = f"{self.base_url}/api/v2/forums/posts/{post_id}"
+        data: dict[str, str] = {
+            "body": new_content,
+        }
+        json = await self._request("PUT", url, json=data)
+        return ForumPost.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_chat_ack(self, **kwargs: Any) -> list[ChatUserSilence]:
+        r"""Gets chat acknowledgement.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *since* (``int``) --
+                Optional, the last message ID received
+            * *silence_id_since* (``int``) --
+                Optional, the last silence ID received
+
+        :raises APIException: Contains status code and error message
+        :return: List of chat user silence objects
+        :rtype: list[aiosu.models.chat.ChatUserSilence]
+        """
+        url = f"{self.base_url}/api/v2/chat/ack"
+        data: dict[str, Any] = {}
+        add_param(data, kwargs, key="since")
+        add_param(data, kwargs, key="silence_id_since", param_name="history_since")
+        json = await self._request("POST", url, json=data)
+        return from_list(ChatUserSilence.model_validate, json.get("silences", []))
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_chat_updates(self, since: int, **kwargs: Any) -> ChatUpdateResponse:
+        r"""Gets chat updates.
+
+        :param since: The last message ID received
+        :type since: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the maximum number of messages to return. Min: 1, Max: 50. Defaults to 50
+            * *channel_id* (``int``) --
+                Optional, the channel ID to get messages from
+            * *silence_id_since* (``int``) --
+                Optional, the last silence ID received
+            * *includes* (``list[aiosu.models.chat.ChatIncludeTypes]``) --
+                Optional, the additional information to include. Defaults to all.
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: Chat update response object
+        :rtype: aiosu.models.chat.ChatUpdateResponse
+        """
+        if not 1 <= (limit := kwargs.get("limit", 50)) <= 50:
+            raise ValueError("limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/chat/updates"
+        params: dict[str, Any] = {
+            "since": since,
+            "limit:": limit,
+        }
+        add_param(params, kwargs, key="channel_id")
+        add_param(params, kwargs, key="includes")
+        add_param(params, kwargs, key="silence_id_since", param_name="history_since")
+        json = await self._request("GET", url, params=params)
+        return ChatUpdateResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_channel(self, channel_id: int) -> ChatChannelResponse:
+        r"""Gets channel.
+
+        :param channel_id: The channel ID to get
+        :type channel_id: int
+        :raises APIException: Contains status code and error message
+        :return: Chat channel object
+        :rtype: aiosu.models.chat.ChatChannelResponse
+        """
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}"
+        json = await self._request("GET", url)
+        return ChatChannelResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_channels(self) -> list[ChatChannel]:
+        r"""Gets a list of joinable public channels.
+
+        :raises APIException: Contains status code and error message
+        :return: List of chat channel objects
+        :rtype: list[aiosu.models.chat.ChatChannel]
+        """
+        url = f"{self.base_url}/api/v2/chat/channels"
+        json = await self._request("GET", url)
+        return from_list(ChatChannel.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_channel_messages(
+        self,
+        channel_id: int,
+        **kwargs: Any,
+    ) -> list[ChatMessage]:
+        r"""Gets channel messages.
+
+        :param channel_id: The channel ID to get messages from
+        :type channel_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the maximum number of messages to return. Min: 1, Max: 50. Defaults to 50
+            * *since* (``int``) --
+                Optional, the ID of the oldest message to return
+            * *until* (``int``) --
+                Optional, the ID of the newest message to return
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: List of chat message objects
+        :rtype: list[aiosu.models.chat.ChatMessage]
+        """
+        if not 1 <= (limit := kwargs.get("limit", 50)) <= 50:
+            raise ValueError("limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
+        params: dict[str, Any] = {
+            "limit:": limit,
+        }
+        add_param(params, kwargs, key="since")
+        add_param(params, kwargs, key="until")
+        json = await self._request("GET", url, params=params)
+        return from_list(ChatMessage.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.CHAT_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def create_chat_channel(
+        self,
+        type: ChatChannelTypes,
+        **kwargs: Any,
+    ) -> ChatChannel:
+        r"""Creates a chat channel.
+
+        :param type: The type of the channel.
+        :type type: aiosu.models.chat.ChatChannelType
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *message* (``str``) --
+                Required if type is ``ANNOUNCE``, the message to send in the PM
+            * *target_id* (``int``) --
+                Only used if if type is ``PM``, the ID of the user to send a PM to
+            * *target_ids* (``List[int]``) --
+                Only used if type is ``ANNOUNCE``, the IDs of the users to send a PM to
+            * *channel_name* (``str``) --
+                Only used if type is ``ANNOUNCE``, the name of the channel
+            * *channel_description* (``str``) --
+                Only used if type is ``ANNOUNCE``, the description of the channel
+
+        :raises ValueError: If missing required parameters
+        :raises APIException: Contains status code and error message
+        :return: Chat channel object
+        :rtype: aiosu.models.chat.ChatChannel
+        """
+        url = f"{self.base_url}/api/v2/chat/channels"
+        data: dict[str, Any] = {
+            "type": type,
+        }
+        add_param(data, kwargs, key="message")
+        if type == "PM":
+            if not add_param(data, kwargs, key="target_id"):
+                raise ValueError("Missing target ID")
+        elif type == "ANNOUNCE":
+            if not add_param(data, kwargs, key="target_ids"):
+                raise ValueError("Missing target IDs")
+            if not data.get("message"):
+                raise ValueError("Missing message")
+            channel = {
+                "name": kwargs["channel_name"],
+                "description": kwargs["channel_description"],
+            }
+            data["channel"] = channel
+        json = await self._request("POST", url, json=data)
+        return ChatChannel.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def join_channel(self, channel_id: int, user_id: int) -> ChatChannel:
+        r"""Joins a channel.
+
+        :param channel_id: The channel ID to join
+        :type channel_id: int
+        :param user_id: The user ID to join as
+        :type user_id: int
+        :raises APIException: Contains status code and error message
+        :return: Chat channel object
+        :rtype: aiosu.models.chat.ChatChannel
+        """
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
+        json = await self._request("PUT", url)
+        return ChatChannel.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def leave_channel(self, channel_id: int, user_id: int) -> None:
+        r"""Leaves a channel.
+
+        :param channel_id: The channel ID to leave
+        :type channel_id: int
+        :param user_id: The user ID to leave as
+        :type user_id: int
+        :raises APIException: Contains status code and error message
+        """
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/users/{user_id}"
+        await self._request("DELETE", url)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def mark_read(self, channel_id: int, message_id: int) -> None:
+        r"""Marks a channel as read.
+
+        :param channel_id: The channel ID to mark as read
+        :type channel_id: int
+        :param message_id: The message ID to mark as read up to
+        :type message_id: int
+        :raises APIException: Contains status code and error message
+        """
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/mark-as-read/{message_id}"
+        await self._request("PUT", url)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.LAZER)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def send_message(
+        self,
+        channel_id: int,
+        message: str,
+        is_action: bool,
+    ) -> ChatMessage:
+        r"""Sends a message to a channel.
+
+        :param channel_id: The ID of the channel
+        :type channel_id: int
+        :param message: The message to send
+        :type message: str
+        :param is_action: Whether the message is an action
+        :type is_action: bool
+        :raises APIException: Contains status code and error message
+        :return: Chat message object
+        :rtype: aiosu.models.chat.ChatMessage
+        """
+        url = f"{self.base_url}/api/v2/chat/channels/{channel_id}/messages"
+        data: dict[str, Any] = {
+            "message": message,
+            "is_action": is_action,
+        }
+        json = await self._request("POST", url, json=data)
+        return ChatMessage.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.CHAT_WRITE)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def send_private_message(
+        self,
+        user_id: int,
+        message: str,
+        is_action: bool,
+        **kwargs: Any,
+    ) -> ChatMessageCreateResponse:
+        r"""Sends a message to a user.
+
+        :param user_id: The ID of the user
+        :type user_id: int
+        :param message: The message to send
+        :type message: str
+        :param is_action: Whether the message is an action
+        :type is_action: bool
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *uuid* (``str``) --
+                Optional, client-side message identifier to be sent back in response and websocket json
+
+        :raises APIException: Contains status code and error message
+        :return: Chat message create response object
+        :rtype: aiosu.models.chat.ChatMessageCreateResponse
+        """
+        url = f"{self.base_url}/api/v2/chat/new"
+        data: dict[str, Any] = {
+            "target_id": user_id,
+            "message": message,
+            "is_action": is_action,
+        }
+        add_param(data, kwargs, key="uuid")
+        json = await self._request("POST", url, json=data)
+        return ChatMessageCreateResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_multiplayer_matches(
+        self,
+        **kwargs: Any,
+    ) -> MultiplayerMatchesResponse:
+        r"""Gets the multiplayer matches.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, the sort type
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
+            * *cursor_string* (``str``) --
+                Optional, the cursor string to get the next page of results
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: Multiplayer matches response object
+        :rtype: aiosu.models.multiplayer.MultiplayerMatchesResponse
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 50:
+            raise ValueError("Limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/matches"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="sort")
+        json = await self._request("GET", url, params=params)
+        resp = MultiplayerMatchesResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(self.get_multiplayer_matches, **kwargs)
+        return resp
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_multiplayer_match(
+        self,
+        match_id: int,
+        **kwargs: Any,
+    ) -> MultiplayerMatchResponse:
+        r"""Gets a multiplayer match.
+
+        :param match_id: The ID of the match
+        :type match_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 100, defaults to 100
+            * *before* (``int``) --
+                Optional, the ID of the score to get the scores before
+            * *after* (``int``) --
+                Optional, the ID of the score to get the scores after
+
+        :raises ValueError: If limit is not between 1 and 100
+        :raises APIException: Contains status code and error message
+        :return: Multiplayer match response object
+        :rtype: aiosu.models.multiplayer.MultiplayerMatchResponse
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 100:
+            raise ValueError("Limit must be between 1 and 100")
+        url = f"{self.base_url}/api/v2/matches/{match_id}"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="before")
+        add_param(params, kwargs, key="after")
+        json = await self._request("GET", url)
+        return MultiplayerMatchResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_multiplayer_rooms(self, **kwargs: Any) -> list[MultiplayerRoom]:
+        r"""Gets the multiplayer rooms.
+
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *mode* (``aiosu.models.multiplayer.MultiplayerRoomMode``) --
+                Optional, the multiplayer room mode
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
+            * *sort* (``aiosu.models.common.SortTypes``) --
+                Optional, the sort type
+            * *category* (``aiosu.models.multiplayer.MultiplayerRoomCategories``) --
+                Optional, the multiplayer room category
+            * *type* (``aiosu.models.multiplayer.MultiplayerRoomTypeGroups``) --
+                Optional, the multiplayer room type group
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: List of multiplayer rooms
+        :rtype: list[aiosu.models.multiplayer.MultiplayerRoom]
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
+            raise ValueError("Limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/rooms"
+        if "mode" in kwargs:
+            mode: MultiplayerRoomMode = kwargs.pop("mode")
+            url += f"/{mode}"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="category")
+        add_param(params, kwargs, key="type", param_name="type_group")
+        json = await self._request("GET", url, params=params)
+        return from_list(MultiplayerRoom.model_validate, json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_multiplayer_room(self, room_id: int) -> MultiplayerRoom:
+        r"""Gets a multiplayer room.
+
+        :param room_id: The ID of the room
+        :type room_id: int
+
+        :raises APIException: Contains status code and error message
+        :return: Multiplayer room object
+        :rtype: aiosu.models.multiplayer.MultiplayerRoom
+        """
+        url = f"{self.base_url}/api/v2/rooms/{room_id}"
+        json = await self._request("GET", url)
+        return MultiplayerRoom.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    @requires_scope(Scopes.IDENTIFY | Scopes.DELEGATE, any_scope=True)
+    async def get_multiplayer_leaderboard(
+        self,
+        room_id: int,
+        **kwargs: Any,
+    ) -> MultiplayerLeaderboardResponse:
+        r"""Gets the multiplayer leaderboard for a room.
+
+        :param room_id: The ID of the room
+        :type room_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, number of scores to get. Min: 1, Max: 50, defaults to 50
+
+        :raises ValueError: If limit is not between 1 and 50
+        :raises APIException: Contains status code and error message
+        :return: Multiplayer leaderboard response object
+        :rtype: aiosu.models.multiplayer.MultiplayerLeaderboardResponse
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 50)) <= 50:
+            raise ValueError("Limit must be between 1 and 50")
+        url = f"{self.base_url}/api/v2/rooms/{room_id}/leaderboard"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        json = await self._request("GET", url, params=params)
+        return MultiplayerLeaderboardResponse.model_validate(json)
+
+    @prepare_token
+    @check_token
+    @requires_scope(Scopes.PUBLIC)
+    async def get_multiplayer_scores(
+        self,
+        room_id: int,
+        playlist_id: int,
+        **kwargs: Any,
+    ) -> MultiplayerScoresResponse:
+        r"""Gets the multiplayer scores for a room.
+
+        :param room_id: The ID of the room
+        :type room_id: int
+        :param playlist_id: The ID of the playlist
+        :type playlist_id: int
+        :param \**kwargs:
+            See below
+
+        :Keyword Arguments:
+            * *limit* (``int``) --
+                Optional, the number of scores to return
+            * *sort* (``aiosu.models.multiplayer.MultiplayerScoreSortType``) --
+                Optional, the sort order of the scores
+            * *cursor_string* (``str``) --
+                Optional, the cursor string to use for pagination
+
+        :raises ValueError: If limit is not between 1 and 100
+        :raises APIException: Contains status code and error message
+        :return: Multiplayer scores response object
+        :rtype: aiosu.models.multiplayer.MultiplayerScoresResponse
+        """
+        if not 1 <= (limit := kwargs.pop("limit", 1)) <= 100:
+            raise ValueError("Limit must be between 1 and 100")
+        url = f"{self.base_url}/api/v2/rooms/{room_id}/playlist/{playlist_id}/scores"
+        params: dict[str, Any] = {
+            "limit": limit,
+        }
+        add_param(params, kwargs, key="sort")
+        add_param(params, kwargs, key="cursor_string")
+        json = await self._request("GET", url, params=params)
+        resp = MultiplayerScoresResponse.model_validate(json)
+        if resp.cursor_string:
+            kwargs["cursor_string"] = resp.cursor_string
+            resp.next = partial(
+                self.get_multiplayer_scores,
+                room_id,
+                playlist_id,
+                **kwargs,
+            )
+        return resp
+
+    @prepare_token
+    @check_token
+    async def revoke_token(self) -> None:
+        r"""Revokes the current token and closes the session.
+
+        :raises APIException: Contains status code and error message
+        """
+        url = f"{self.base_url}/api/v2/oauth/tokens/current"
+        await self._request("DELETE", url)
+        await self._delete_token()
+        await self.close()
+
+    async def close(self) -> None:
+        """Closes the client session."""
+        if self._session:
+            await self._session.close()
+            self._session = None
```

### Comparing `aiosu-2.0.1/pyproject.toml` & `aiosu-2.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-[tool.mypy]
-plugins = ["pydantic.mypy"]
-mypy_path = "./"
-files = ["aiosu"]
-disallow_untyped_defs = true
-disallow_any_unimported = true
-no_implicit_optional = true
-check_untyped_defs = true
-warn_unused_ignores = true
-show_error_codes = true
-[tools.pytest.ini_options]
-testpaths = ["tests"]
-[tool.poetry]
-name = "aiosu"
-version = "2.0.1"
-description = "Simple and fast osu! API v1 and v2 library"
-authors = ["Nice Aesthetics <nice@aesth.dev>"]
-license = "GPLv3+"
-readme = "README.rst"
-repository = "https://github.com/NiceAesth/aiosu"
-documentation = "https://aiosu.readthedocs.io/"
-keywords = ["osu!", "osu", "api"]
-classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Typing :: Typed"
-]
-include = ["py.typed"]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-aiohttp = "^3.8.3"
-aiolimiter = "^1.0.0"
-emojiflags = "^0.1.1"
-orjson = "^3.8.3"
-pydantic = "^2.0.3"
-pytest = {version="^7.2.0", optional = true}
-pytest-asyncio = {version="^0.21.0", optional = true}
-pytest-mock = {version="^3.10.0", optional = true}
-toml = {version="^0.10.2", optional = true}
-sphinx = {version="^7.0.0", optional = true}
-furo = {version="^2023.5.20", optional = true}
-types-toml = {version = "^0.10.8.1", optional = true}
-pyjwt = "^2.6.0"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-asyncio = "^0.21.0"
-pytest-mock = "^3.10.0"
-mypy = "^1.0"
-toml = "^0.10.2"
-types-toml = "^0.10.8.1"
-sphinx = "^7.0.0"
-furo = "^2023.5.20"
-pytest-cov = "^4.0.0"
-black = {version = "^23.0.0", allow-prereleases = true}
-pre-commit = "^3.2.2"
-
-[tool.poetry.extras]
-test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
-docs = ["Sphinx", "furo", "toml"]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.mypy]
+plugins = ["pydantic.mypy"]
+mypy_path = "./"
+files = ["aiosu"]
+disallow_untyped_defs = true
+disallow_any_unimported = true
+no_implicit_optional = true
+check_untyped_defs = true
+warn_unused_ignores = true
+show_error_codes = true
+[tools.pytest.ini_options]
+testpaths = ["tests"]
+[tool.poetry]
+name = "aiosu"
+version = "2.0.2"
+description = "Simple and fast osu! API v1 and v2 library"
+authors = ["Nice Aesthetics <nice@aesth.dev>"]
+license = "GPLv3+"
+readme = "README.rst"
+repository = "https://github.com/NiceAesth/aiosu"
+documentation = "https://aiosu.readthedocs.io/"
+keywords = ["osu!", "osu", "api"]
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Typing :: Typed"
+]
+include = ["py.typed"]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+aiohttp = "^3.8.3"
+aiolimiter = "^1.0.0"
+emojiflags = "^0.1.1"
+orjson = "^3.8.3"
+pydantic = "^2.0.3"
+pytest = {version="^7.2.0", optional = true}
+pytest-asyncio = {version="^0.21.0", optional = true}
+pytest-mock = {version="^3.10.0", optional = true}
+toml = {version="^0.10.2", optional = true}
+sphinx = {version="^7.0.0", optional = true}
+furo = {version="^2023.5.20", optional = true}
+types-toml = {version = "^0.10.8.1", optional = true}
+pyjwt = "^2.6.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+pytest-asyncio = "^0.21.0"
+pytest-mock = "^3.10.0"
+mypy = "^1.0"
+toml = "^0.10.2"
+types-toml = "^0.10.8.1"
+sphinx = "^7.0.0"
+furo = "^2023.5.20"
+pytest-cov = "^4.0.0"
+black = {version = "^23.0.0", allow-prereleases = true}
+pre-commit = "^3.2.2"
+
+[tool.poetry.extras]
+test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
+docs = ["Sphinx", "furo", "toml"]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `aiosu-2.0.1/PKG-INFO` & `aiosu-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosu
-Version: 2.0.1
+Version: 2.0.2
 Summary: Simple and fast osu! API v1 and v2 library
 Home-page: https://github.com/NiceAesth/aiosu
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
```

