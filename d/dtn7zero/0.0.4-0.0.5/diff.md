# Comparing `tmp/dtn7zero-0.0.4.tar.gz` & `tmp/dtn7zero-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtn7zero-0.0.4.tar", last modified: Wed Apr 19 14:22:13 2023, max compression
+gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-5f_zb515\dtn7zero-0.0.5.tar", last modified: Fri Apr 28 23:19:10 2023, max compression
```

## Comparing `dtn7zero-0.0.4.tar` & `dtn7zero-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.447435 dtn7zero-0.0.4/
--rw-rw-rw-   0        0        0    34523 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    10070 2023-04-19 14:22:13.447435 dtn7zero-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     9571 2023-04-19 14:05:01.000000 dtn7zero-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.347186 dtn7zero-0.0.4/dtn7zero/
--rw-rw-rw-   0        0        0      255 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/__init__.py
--rw-rw-rw-   0        0        0     9470 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/api.py
--rw-rw-rw-   0        0        0    20873 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/bundle_protocol_agent.py
--rw-rw-rw-   0        0        0     1452 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.378428 dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/
--rw-rw-rw-   0        0        0      598 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/__init__.py
--rw-rw-rw-   0        0        0     3198 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
--rw-rw-rw-   0        0        0    12776 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/mtcp.py
--rw-rw-rw-   0        0        0     2375 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/data.py
--rw-rw-rw-   0        0        0     7408 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/endpoints.py
--rw-rw-rw-   0        0        0    12703 2023-04-19 14:11:54.000000 dtn7zero-0.0.4/dtn7zero/ipnd.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.394050 dtn7zero-0.0.4/dtn7zero/routers/
--rw-rw-rw-   0        0        0     3064 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/routers/__init__.py
--rw-rw-rw-   0        0        0     4287 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/routers/simple_epidemic_router.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.394050 dtn7zero-0.0.4/dtn7zero/storage/
--rw-rw-rw-   0        0        0     1368 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/storage/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/storage/simple_in_memory_storage.py
--rw-rw-rw-   0        0        0     4194 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/dtn7zero/utility.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.378428 dtn7zero-0.0.4/dtn7zero.egg-info/
--rw-rw-rw-   0        0        0    10070 2023-04-19 14:22:13.000000 dtn7zero-0.0.4/dtn7zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-04-19 14:22:13.000000 dtn7zero-0.0.4/dtn7zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:22:13.000000 dtn7zero-0.0.4/dtn7zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:22:13.000000 dtn7zero-0.0.4/dtn7zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 14:22:13.000000 dtn7zero-0.0.4/dtn7zero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      617 2023-04-19 14:19:34.000000 dtn7zero-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 14:22:13.447435 dtn7zero-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 14:22:13.447435 dtn7zero-0.0.4/test/
--rw-rw-rw-   0        0        0      919 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-api-background.py
--rw-rw-rw-   0        0        0      665 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-api-ping.py
--rw-rw-rw-   0        0        0      538 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-api-pong.py
--rw-rw-rw-   0        0        0      865 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-api-synchronous.py
--rw-rw-rw-   0        0        0     1896 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-bundle-protocol-agent-receiver.py
--rw-rw-rw-   0        0        0     2041 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-bundle-protocol-agent-sender.py
--rw-rw-rw-   0        0        0     1391 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-bundle-protocol-agent.py
--rw-rw-rw-   0        0        0     1666 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-bundle-serialization.py
--rw-rw-rw-   0        0        0    15450 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-bundle-size.py
--rw-rw-rw-   0        0        0     1645 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-dtn7rs-rest-cla.py
--rw-rw-rw-   0        0        0     1204 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-ipnd.py
--rw-rw-rw-   0        0        0     1980 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-mtcp-intermediate.py
--rw-rw-rw-   0        0        0     2201 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-mtcp-receiver.py
--rw-rw-rw-   0        0        0     2498 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-mtcp-sender.py
--rw-rw-rw-   0        0        0     5168 2023-04-19 14:01:15.000000 dtn7zero-0.0.4/test/test-py-dtn7-functionality.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/
+-rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    10080 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9755 2023-04-28 23:14:49.000000 dtn7zero-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/
+-rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/__init__.py
+-rw-rw-rw-   0        0        0     9731 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/api.py
+-rw-rw-rw-   0        0        0    21246 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/bundle_protocol_agent.py
+-rw-rw-rw-   0        0        0     1506 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/
+-rw-rw-rw-   0        0        0      615 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+-rw-rw-rw-   0        0        0    13077 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/mtcp.py
+-rw-rw-rw-   0        0        0     2435 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/data.py
+-rw-rw-rw-   0        0        0     7598 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/endpoints.py
+-rw-rw-rw-   0        0        0    13381 2023-04-28 22:59:08.000000 dtn7zero-0.0.5/dtn7zero/ipnd.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/routers/
+-rw-rw-rw-   0        0        0     3128 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/routers/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/routers/simple_epidemic_router.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/storage/
+-rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/storage/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/storage/simple_in_memory_storage.py
+-rw-rw-rw-   0        0        0     4307 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/
+-rw-rw-rw-   0        0        0    10080 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-04-28 23:18:36.000000 dtn7zero-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/test/
+-rw-rw-rw-   0        0        0      956 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-background.py
+-rw-rw-rw-   0        0        0      694 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-ping.py
+-rw-rw-rw-   0        0        0      563 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-pong.py
+-rw-rw-rw-   0        0        0      899 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-synchronous.py
+-rw-rw-rw-   0        0        0     1944 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent-receiver.py
+-rw-rw-rw-   0        0        0     2095 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent-sender.py
+-rw-rw-rw-   0        0        0     1443 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent.py
+-rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-serialization.py
+-rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-size.py
+-rw-rw-rw-   0        0        0     1688 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-dtn7rs-rest-cla.py
+-rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-ipnd.py
+-rw-rw-rw-   0        0        0     2028 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-intermediate.py
+-rw-rw-rw-   0        0        0     2260 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-receiver.py
+-rw-rw-rw-   0        0        0     2563 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-sender.py
+-rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-py-dtn7-functionality.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dtn7zero-0.0.4/LICENSE` & `dtn7zero-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
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
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
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
-    it under the terms of the GNU Affero General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
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
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
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
+    it under the terms of the GNU Affero General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `dtn7zero-0.0.4/PKG-INFO` & `dtn7zero-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -119,15 +119,15 @@
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
 Simply run this in the project root folder (requires at least pip v21.1):
 ```shell
-$ pip install --editable .
+$ python -m pip install --editable .
 ```
 
 ### Build
 To build this project yourself you need the python [build](https://pypi.org/project/build/) tool, as well as [setuptools](https://pypi.org/project/setuptools/):
 ```shell
 $ pip install --upgrade setuptools
 $ pip install --upgrade build
```

### Comparing `dtn7zero-0.0.4/README.md` & `dtn7zero-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-# dtn7zero
-This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
-
-The current features are:
-- a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
-- a minimal TCP convergence layer
-- a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
-- automatic local-network node-discovery via ipnd module
-- a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
-- a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
-- full MicroPython support (tested on an ESP32-GENERIC)
-- (currently uses epidemic routing and in-memory storage managing)
-- (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
-
-## Getting Started
-To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
-```shell
-$ pip install --upgrade dtn7zero
-```
-The most simple example on what you can do:
-```python
-import time
-
-from dtn7zero import setup, start_background_update_thread
-
-node_endpoint = setup("dtn://node1/", print)
-
-start_background_update_thread()
-
-node_endpoint.send(b'hello world', "dtn://node1/")
-
-time.sleep(1)
-```
-Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
-
-For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
-`dtn7zero.api` module implementation and the tests under `./tests`.
-
-## MicroPython Installation Guide
-This whole project was tested on an ESP32 (GENERIC) and this installation guide is tailored for the ESP32.
-If you plan to use another microcontroller you might need to do adjustments 
-(most certainly the MicroPython installation, and the MPY_MARCH in esp-deployment.py).
-
-Important note for linux: it may be that mpremote assumes another USB device with higher priority than the ESP32.
-In that case all mpremote commands (especially inside esp-deployment.py) will fail as no communication is possible.
-Check all USB devices mpremote considers in priority order with `mpremote devs`.
-
-### First Time MicroPython Installation For ESP32 (GENERIC)
-1. download the newest [firmware](https://micropython.org/download/esp32/)
-2. install the esp flash tool: `pip install esptool`
-3. connect your ESP32 via USB and start a terminal at the location of the downloaded firmware
-4. start the following command (with the correct USB port), then hold **boot** until it starts erasing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash`
-5. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
-6. done, you may now connect to it via: `mpremote` (installation via pip: `pip install mpremote`)
-
-### Update To New MicroPython Version
-1. download the newest [firmware](https://micropython.org/download/esp32/)
-2. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
-`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
-3. done
-
-### First Time dtn7zero Deployment
-1. make sure you check out the repository and the submodules (especially py-dtn7)
-2. install the mpremote tool: `pip install mpremote`
-3. install the mpy-cross compiler tool: `pip install mpy-cross`
-4. populate wlan.json with an appropriate hostname and at least one ssid -> password mapping
-5. check your connection to the ESP32 with: `mpremote`
-6. copy wlan.json to your ESP32: `mpremote fs cp wlan.json :wlan.json`
-7. copy boot.py to your ESP32: `mpremote fs cp boot.py :boot.py`
-8. deploy the dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
-9. done
-
-### Continuous dtn7zero Deployment
-1. check your connection to the ESP32 with: `mpremote`
-2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
-3. done
-
-### First dtn7zero Functionality Check On MicroPython
-1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
-2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
-3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
-
-### Additional MicroPython Tips & Tricks
-The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
-can be exited by using `ctrl+~` (tested on windows).
-
-If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
-keeps running.
-
-If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
-ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
-state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
-
-You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
-You can also remove the script. MicroPython will only execute the script if it is present.
-```shell
-$ mpremote fs cp examples/remote_echo_callback.py :main.py
-$ mpremote fs rm :main.py
-```
-
-Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
-the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
-if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
-the `boot.py` and then the `main.py` if it is present.
-
-
-## Development Information
-
-### Development Mode
-You can install this project locally to directly reflect code changes in your environment.
-Simply run this in the project root folder (requires at least pip v21.1):
-```shell
-$ pip install --editable .
-```
-
-### Build
-To build this project yourself you need the python [build](https://pypi.org/project/build/) tool, as well as [setuptools](https://pypi.org/project/setuptools/):
-```shell
-$ pip install --upgrade setuptools
-$ pip install --upgrade build
-```
-Then you can simply run this command to build the project:
-```shell
-$ python -m build
-```
-
-### Publish
-To publish this project you will probably update the version in `pyproject.toml`, [build](#build) the project, and then use [twine](https://pypi.org/project/twine/) to upload the build:
-```shell
-$ pip install --upgrade twine
-```
-```shell
-$ python -m twine upload dist/*
-```
-
-
-## Useful Links
-the DTN7 website: https://dtn7.github.io \
-dtn7 go implementation: https://github.com/dtn7/dtn7-go \
-dtn7 rust implementation: https://github.com/dtn7/dtn7-rs \
-dtn7 python bundle implementation and dtn7rs-rest-api access: https://github.com/teschmitt/py-dtn7
-
-Bundle Protocol 7 RFC: https://datatracker.ietf.org/doc/html/rfc9171 \
-Bundle Protocol Security (BPSec) RFC: https://datatracker.ietf.org/doc/html/rfc9172 \
-Default Security Contexts for BPSec RFC: https://datatracker.ietf.org/doc/html/rfc9173 \
-TCP Convergence-Layer Protocol Version 4 RFC: https://datatracker.ietf.org/doc/html/rfc9174 \
-Minimal TCP Convergence-Layer Protocol RFC (draft): https://datatracker.ietf.org/doc/html/draft-ietf-dtn-mtcpcl-01 \
-UDP Convergence Layer RFC (draft): https://datatracker.ietf.org/doc/html/draft-sipos-dtn-udpcl-01
-
-Outdated Standards: \
-DTN URI Scheme: https://www.ietf.org/archive/id/draft-irtf-dtnrg-dtn-uri-scheme-00.html
-
-## Further Research
-This is some information gathered about future mesh extensions:
-
-1. [ESP-Mesh(ESP-WIFI-Mesh)](https://www.espressif.com/en/products/sdks/esp-wifi-mesh/overview)
-   - a special mesh standard which is based of Wi-Fi and uses the special AP_STA mode 
-   - no micropython implementation known
-
-2. [ESP-NOW](https://www.espressif.com/en/products/software/esp-now/overview)
-   - a special p2p mode, which is based of Wi-Fi and can send data to neighbouring devices via MAC addressing
-   - no mesh protocol, but broadcast is possible, looks promising to build an esp32-dtn-mesh
-   - non-official, but tested micropython [library](https://github.com/glenn20/micropython/blob/espnow-g20/docs/library/espnow.rst) available, as well as [builds](https://github.com/glenn20/micropython-espnow-images) with the current firmware
-
-3. Alternative: AP_STA mode for simultaneous AP and STA without explicit ESP-MESH usage
-   - only available for [Arduino+C](https://techtutorialsx.com/2021/01/04/esp32-soft-ap-and-station-modes/)
-   - [painlessMesh](https://gitlab.com/painlessMesh/painlessMesh) also uses this mode to build its mesh
-
-### Open End Topics / Known Issues
-- fragment, CRC, status-report generation support
-- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the dtn7rs-rest-cla is disabled in the simple API)
-- public documentation (currently all information must be gathered from doc-strings and examples)
+# dtn7zero
+This is a DTN7 [RFC9171](https://datatracker.ietf.org/doc/html/rfc9171) compliant python implementation (work-in-progress) with a [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API.
+
+The current features are:
+- a full bundle protocol agent (without fragment, CRC, and status-report generation support -> todo)
+- a minimal TCP convergence layer
+- a [dtn7-rs](https://github.com/dtn7/dtn7-rs) convergence layer, using the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md) interface
+- automatic local-network node-discovery via ipnd module
+- a standalone 'external' endpoint (which connects to a [dtn7-rs](https://github.com/dtn7/dtn7-rs) via the [HTTP/REST](https://github.com/dtn7/dtn7-rs/blob/master/doc/http-client-api.md)) interface
+- a simplified [NetworkZero](https://networkzero.readthedocs.io/en/latest/networkzero.html) like API to easily get started
+- full MicroPython support (tested on an ESP32-GENERIC)
+- (currently uses epidemic routing and in-memory storage managing)
+- (with extendability for new convergence layer adapters, routing algorithms, and storage managers)
+
+## Getting Started
+To use dtn7zero in your CPython environment, simply install it via pip (or pip3 on linux):
+```shell
+$ pip install --upgrade dtn7zero
+```
+The most simple example on what you can do:
+```python
+import time
+
+from dtn7zero import setup, start_background_update_thread
+
+node_endpoint = setup("dtn://node1/", print)
+
+start_background_update_thread()
+
+node_endpoint.send(b'hello world', "dtn://node1/")
+
+time.sleep(1)
+```
+Further examples for the 'simple' API can be found under `./examples` in the GitHub repository.
+
+For a deeper dive into the underlying concepts and the fully fletched dtn implementation, take a look at the 
+`dtn7zero.api` module implementation and the tests under `./tests`.
+
+## MicroPython Installation Guide
+This whole project was tested on an ESP32 (GENERIC) and this installation guide is tailored for the ESP32.
+If you plan to use another microcontroller you might need to do adjustments 
+(most certainly the MicroPython installation, and the MPY_MARCH in esp-deployment.py).
+
+Important note for linux: it may be that mpremote assumes another USB device with higher priority than the ESP32.
+In that case all mpremote commands (especially inside esp-deployment.py) will fail as no communication is possible.
+Check all USB devices mpremote considers in priority order with `mpremote devs`.
+
+### First Time MicroPython Installation For ESP32 (GENERIC)
+1. download the newest [firmware](https://micropython.org/download/esp32/)
+2. install the esp flash tool: `pip install esptool`
+3. connect your ESP32 via USB and start a terminal at the location of the downloaded firmware
+4. start the following command (with the correct USB port), then hold **boot** until it starts erasing: \
+`esptool --chip esp32 --port /dev/ttyUSB0 erase_flash`
+5. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+6. done, you may now connect to it via: `mpremote` (installation via pip: `pip install mpremote`)
+
+### Update To New MicroPython Version
+1. download the newest [firmware](https://micropython.org/download/esp32/)
+2. start the following command (with the correct USB port and firmware name), then hold **boot** until it starts flashing: \
+`esptool --chip esp32 --port /dev/ttyUSB0 --baud 460800 write_flash -z 0x1000 esp32-20220618-v1.19.1.bin`
+3. done
+
+### First Time dtn7zero Deployment
+1. make sure you check out the repository and the submodules (especially py-dtn7)
+2. install the mpremote tool: `pip install mpremote`
+3. install the mpy-cross compiler tool: `pip install mpy-cross`
+4. populate wlan.json with an appropriate hostname and at least one ssid -> password mapping
+5. check your connection to the ESP32 with: `mpremote`
+6. copy wlan.json to your ESP32: `mpremote fs cp wlan.json :wlan.json`
+7. copy boot.py to your ESP32: `mpremote fs cp boot.py :boot.py`
+8. deploy the dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
+9. done
+
+### Continuous dtn7zero Deployment
+1. check your connection to the ESP32 with: `mpremote`
+2. deploy the changes of dtn7zero and dependencies onto the ESP32 (this can take a while): `python scripts/esp-deployment.py`
+3. done
+
+### First dtn7zero Functionality Check On MicroPython
+1. you may check that wlan is connecting correctly (connect via `mpremote` and press **enable** for a soft reset)
+2. you may also check that you can import dtn7zero (connect via `mpremote` and `import dtn7zero`)
+3. you can also check that everything works (run the test script `mpremote run examples/local_ping_echo.py`)
+
+### Additional MicroPython Tips & Tricks
+The mpremote tool is normally interrupted by using `ctrl+c`. A special case is the REPL (simply call `mpremote`), which
+can be exited by using `ctrl+~` (tested on windows).
+
+If you start a script on MicroPython (`mpremote run ...`) and disconnect the console (`mpremote` -> `ctrl+c`) then the script 
+keeps running.
+
+If you must access the REPL via mpremote, but a script is blocking, then call `mpremote` and press EN (enable) on the 
+ESP32 for a soft-reset. Press `ctrl+c` a few times to interrupt the `boot.py` or `main.py` script execution. The session
+state is stored, so any subsequent `mpremote` call will start at REPL as long as no power disconnect is performed.
+
+You can deploy a script as `main.py` on MicroPython to be run every time the microcontroller gets power. \
+You can also remove the script. MicroPython will only execute the script if it is present.
+```shell
+$ mpremote fs cp examples/remote_echo_callback.py :main.py
+$ mpremote fs rm :main.py
+```
+
+Regarding `boot.py`, it is used for user-specific setup code and this framework uses a generic boot script that adjusts
+the ESP32's frequency and connects to a Wi-Fi network (blocking until success). MicroPython will create a dummy `boot.py`
+if none is present. MicroPython will not create a dummy `main.py` is none is present. MicroPython will first execute
+the `boot.py` and then the `main.py` if it is present.
+
+
+## Development Information
+
+### Development Mode
+You can install this project locally to directly reflect code changes in your environment.
+Simply run this in the project root folder (requires at least pip v21.1):
+```shell
+$ python -m pip install --editable .
+```
+
+### Build
+To build this project yourself you need the python [build](https://pypi.org/project/build/) tool, as well as [setuptools](https://pypi.org/project/setuptools/):
+```shell
+$ pip install --upgrade setuptools
+$ pip install --upgrade build
+```
+Then you can simply run this command to build the project:
+```shell
+$ python -m build
+```
+
+### Publish
+To publish this project you will probably update the version in `pyproject.toml`, [build](#build) the project, and then use [twine](https://pypi.org/project/twine/) to upload the build:
+```shell
+$ pip install --upgrade twine
+```
+```shell
+$ python -m twine upload dist/*
+```
+
+
+## Useful Links
+the DTN7 website: https://dtn7.github.io \
+dtn7 go implementation: https://github.com/dtn7/dtn7-go \
+dtn7 rust implementation: https://github.com/dtn7/dtn7-rs \
+dtn7 python bundle implementation and dtn7rs-rest-api access: https://github.com/teschmitt/py-dtn7
+
+Bundle Protocol 7 RFC: https://datatracker.ietf.org/doc/html/rfc9171 \
+Bundle Protocol Security (BPSec) RFC: https://datatracker.ietf.org/doc/html/rfc9172 \
+Default Security Contexts for BPSec RFC: https://datatracker.ietf.org/doc/html/rfc9173 \
+TCP Convergence-Layer Protocol Version 4 RFC: https://datatracker.ietf.org/doc/html/rfc9174 \
+Minimal TCP Convergence-Layer Protocol RFC (draft): https://datatracker.ietf.org/doc/html/draft-ietf-dtn-mtcpcl-01 \
+UDP Convergence Layer RFC (draft): https://datatracker.ietf.org/doc/html/draft-sipos-dtn-udpcl-01
+
+Outdated Standards: \
+DTN URI Scheme: https://www.ietf.org/archive/id/draft-irtf-dtnrg-dtn-uri-scheme-00.html
+
+## Further Research
+This is some information gathered about future mesh extensions:
+
+1. [ESP-Mesh(ESP-WIFI-Mesh)](https://www.espressif.com/en/products/sdks/esp-wifi-mesh/overview)
+   - a special mesh standard which is based of Wi-Fi and uses the special AP_STA mode 
+   - no micropython implementation known
+
+2. [ESP-NOW](https://www.espressif.com/en/products/software/esp-now/overview)
+   - a special p2p mode, which is based of Wi-Fi and can send data to neighbouring devices via MAC addressing
+   - no mesh protocol, but broadcast is possible, looks promising to build an esp32-dtn-mesh
+   - non-official, but tested micropython [library](https://github.com/glenn20/micropython/blob/espnow-g20/docs/library/espnow.rst) available, as well as [builds](https://github.com/glenn20/micropython-espnow-images) with the current firmware
+
+3. Alternative: AP_STA mode for simultaneous AP and STA without explicit ESP-MESH usage
+   - only available for [Arduino+C](https://techtutorialsx.com/2021/01/04/esp32-soft-ap-and-station-modes/)
+   - [painlessMesh](https://gitlab.com/painlessMesh/painlessMesh) also uses this mode to build its mesh
+
+### Open End Topics / Known Issues
+- fragment, CRC, status-report generation support
+- dtn7rs-rest-cla and in-memory storage together use too much RAM for MicroPython (therefore the dtn7rs-rest-cla is disabled in the simple API)
+- public documentation (currently all information must be gathered from doc-strings and examples)
```

### Comparing `dtn7zero-0.0.4/dtn7zero/api.py` & `dtn7zero-0.0.5/dtn7zero/api.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-"""
-DTN7-Zero API
-
-Inspired by the networkzero library.
-
-Provides a simple NDN (named data network) interface on top of DTN7.
-"""
-import time
-
-from typing import Optional, List, Tuple, Callable
-
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, RUNNING_MICROPYTHON
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.data import Node
-from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-from py_dtn7.bundle import Bundle, PrimaryBlock
-
-if RUNNING_MICROPYTHON:
-    import _thread
-else:
-    import threading
-
-
-BPA: Optional[BundleProtocolAgent] = None
-BPA_THREAD = None
-
-
-class SimpleEndpoint:
-
-    def __init__(self, service_name, callback=None):
-        self._callback = callback
-        self._endpoint = LocalEndpoint(service_name, self._simplifying_callback if callback is not None else None)
-
-    def _simplifying_callback(self, bundle: Bundle):
-        self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
-
-    def send(self, payload: bytes, full_destination_address: str, anonymous: bool = False):
-        """ sends a payload(message) to the specified node_id and service_name
-        """
-        self._endpoint.start_transmission(payload, full_destination_address, anonymous=anonymous)
-
-    def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
-        """ polls a passive endpoint (without callback) for a new payload(message)
-
-        use pythons value unpacking feature with the methods' signature like so:
-
-        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
-
-        the primary block is provided for direct access to additional information
-        """
-        bundle = self._endpoint.poll()
-
-        if bundle is not None:
-            return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
-        return None, None, None, None
-
-
-class SimpleGroupEndpoint:
-
-    def __init__(self, full_group_uri, callback=None):
-        self._callback = callback
-        self._endpoint = LocalGroupEndpoint(full_group_uri, self._simplifying_callback if callback is not None else None)
-
-    def _simplifying_callback(self, bundle: Bundle):
-        self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
-
-    def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
-        """ polls a passive endpoint (without callback) for a new payload(message)
-
-        use pythons value unpacking feature with the methods' signature like so:
-
-        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
-
-        the primary block is provided for direct access to additional information
-        """
-        bundle = self._endpoint.poll()
-
-        if bundle is not None:
-            return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
-        return None, None, None, None
-
-
-def setup(full_node_uri: str, node_receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleEndpoint:
-    """ initializes the bundle protocol agent with the provided full-node-id and returns the node-central endpoint
-
-    full_node_uri examples:
-            dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
-            ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
-
-    node_receive_callback -> may be None, but then you need to manually poll the endpoint
-
-    node_receive_callback signature/example:
-
-    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-        pass
-
-    the primary block is provided for direct access to additional information
-
-    call only once!
-    """
-    global BPA
-
-    if BPA is not None:
-        raise Exception('setup(node_id) was called twice!')
-
-    storage = SimpleInMemoryStorage()
-    router = SimpleEpidemicRouter({IPND_IDENTIFIER_MTCP: MTcpCLA()}, storage)
-    BPA = BundleProtocolAgent(full_node_uri, storage, router, use_ipnd=True)
-
-    # node specific endpoint works like a normal endpoint (only receives exactly matched bundles), but for the node itself
-    endpoint = SimpleEndpoint('', node_receive_callback)
-    BPA.register_endpoint(endpoint._endpoint)
-
-    return endpoint
-
-
-def register(endpoint_identifier: str, receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleEndpoint:
-    """ registers an endpoint at the bundle protocol agent over which you can send/receive bundles(messages)
-
-    endpoint_identifier examples:
-        dtn addressing scheme -> "echo", "echo/subecho"
-        ipn addressing scheme -> "12", "24.15.16"
-
-    receive_callback -> may be None, but then you need to manually poll the endpoint
-
-    receive_callback signature/example:
-
-    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-        pass
-
-    the primary block is provided for direct access to additional information
-    """
-    global BPA
-
-    if BPA is None:
-        raise Exception('setup(node_id) was not called!')
-
-    endpoint = SimpleEndpoint(endpoint_identifier, receive_callback)
-    BPA.register_endpoint(endpoint._endpoint)
-
-    return endpoint
-
-
-def register_group(full_group_uri: str, receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleGroupEndpoint:
-    """ registers a group-endpoint at the bundle protocol agent over which you can receive group-addressed bundles
-
-    full_group_uri examples:
-        "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
-
-    receive_callback -> may be None, but then you need to manually poll the endpoint
-
-    receive_callback signature/example:
-
-    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-        pass
-
-    the primary block is provided for direct access to additional information
-    """
-    global BPA
-
-    if BPA is None:
-        raise Exception('setup(node_id) was not called!')
-
-    endpoint = SimpleGroupEndpoint(full_group_uri, receive_callback)
-    BPA.register_group_endpoint(endpoint._endpoint)
-
-    return endpoint
-
-
-def discover() -> List[Node]:
-    """ returns a list of all currently known other nodes in the local network
-    """
-    global BPA
-
-    if BPA is None:
-        raise Exception('setup(node_id) was not called!')
-
-    return list(BPA.storage.get_nodes())
-
-
-def update():
-    """ explicitly updates the bundle protocol agent
-
-    to be called in an endless loop if you want to write the loop yourself
-
-    the alternative solution (or inspiration) is: run_forever()
-    """
-    global BPA
-
-    if BPA is None:
-        raise Exception('setup(node_id was not called!')
-
-    BPA.update()
-
-
-def run_forever(loop_callback=None, loop_callback_interval_milliseconds=1000, _sleep_time_seconds=0):
-    """ update loop to run the bundle protocol agent until KeyboardInterrupt
-
-    custom_logic_callback can be used for application specific logic after the bundle protocol agent was started
-
-    custom_logic_callback signature:
-
-    callback() -> None:
-        pass
-    """
-    global BPA
-
-    if BPA is None:
-        raise Exception('setup(node_id was not called!')
-
-    last_callback_execution = get_current_clock_millis()
-
-    try:
-        while True:
-            BPA.update()
-
-            if loop_callback is not None and is_timestamp_older_than_timeout(last_callback_execution, loop_callback_interval_milliseconds):
-                last_callback_execution = get_current_clock_millis()
-                loop_callback()
-
-            time.sleep(_sleep_time_seconds)
-    except KeyboardInterrupt:
-        pass
-
-
-def start_background_update_thread(_sleep_time_seconds=0):
-    """ (experimental) background update thread
-
-    On MicroPython the limited RAM can lead to crashes (most prominently a maximum-recursion-depth RuntimeError).
-    The _thread.stack_size(...) can be adjusted for compensation if needed and possible.
-    """
-    global BPA
-    global BPA_THREAD
-
-    if BPA is None:
-        raise Exception('setup(node_id was not called!')
-
-    if BPA_THREAD is not None:
-        raise Exception('start_background_update_thread() should only be called once!')
-
-    if RUNNING_MICROPYTHON:
-        _thread.stack_size(11500)  # experimental setting: 7000 does not run, 8000 does run, 11500 picked for leeway
-
-        def update_runner():
-            while True:
-                BPA.update()
-                time.sleep(_sleep_time_seconds)
-
-        BPA_THREAD = _thread.start_new_thread(update_runner, ())
-    else:
-        def self_stopping_update_runner():
-            while threading.main_thread().is_alive():
-                BPA.update()
-                time.sleep(_sleep_time_seconds)
-
-        BPA_THREAD = threading.Thread(target=self_stopping_update_runner)
-        BPA_THREAD.start()
+"""
+DTN7-Zero API
+
+Inspired by the networkzero library.
+
+Provides a simple NDN (named data network) interface on top of DTN7.
+"""
+import time
+
+from typing import Optional, List, Tuple, Callable
+
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP, RUNNING_MICROPYTHON
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.data import Node
+from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+from py_dtn7.bundle import Bundle, PrimaryBlock
+
+if RUNNING_MICROPYTHON:
+    import _thread
+else:
+    import threading
+
+
+BPA: Optional[BundleProtocolAgent] = None
+BPA_THREAD = None
+
+
+class SimpleEndpoint:
+
+    def __init__(self, service_name, callback=None):
+        self._callback = callback
+        self._endpoint = LocalEndpoint(service_name, self._simplifying_callback if callback is not None else None)
+
+    def _simplifying_callback(self, bundle: Bundle):
+        self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
+
+    def send(self, payload: bytes, full_destination_address: str, anonymous: bool = False):
+        """ sends a payload(message) to the specified node_id and service_name
+        """
+        self._endpoint.start_transmission(payload, full_destination_address, anonymous=anonymous)
+
+    def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
+        """ polls a passive endpoint (without callback) for a new payload(message)
+
+        use pythons value unpacking feature with the methods' signature like so:
+
+        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
+
+        the primary block is provided for direct access to additional information
+        """
+        bundle = self._endpoint.poll()
+
+        if bundle is not None:
+            return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
+        return None, None, None, None
+
+
+class SimpleGroupEndpoint:
+
+    def __init__(self, full_group_uri, callback=None):
+        self._callback = callback
+        self._endpoint = LocalGroupEndpoint(full_group_uri, self._simplifying_callback if callback is not None else None)
+
+    def _simplifying_callback(self, bundle: Bundle):
+        self._callback(bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block)
+
+    def poll(self) -> Tuple[Optional[bytes], Optional[str], Optional[str], Optional[PrimaryBlock]]:
+        """ polls a passive endpoint (without callback) for a new payload(message)
+
+        use pythons value unpacking feature with the methods' signature like so:
+
+        payload, full_source_uri, full_destination_uri, primary_block = my_endpoint.poll()
+
+        the primary block is provided for direct access to additional information
+        """
+        bundle = self._endpoint.poll()
+
+        if bundle is not None:
+            return bundle.payload_block.data, bundle.primary_block.full_source_uri, bundle.primary_block.full_destination_uri, bundle.primary_block
+        return None, None, None, None
+
+
+def setup(full_node_uri: str, node_receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleEndpoint:
+    """ initializes the bundle protocol agent with the provided full-node-id and returns the node-central endpoint
+
+    full_node_uri examples:
+            dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
+            ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
+
+    node_receive_callback -> may be None, but then you need to manually poll the endpoint
+
+    node_receive_callback signature/example:
+
+    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+        pass
+
+    the primary block is provided for direct access to additional information
+
+    call only once!
+    """
+    global BPA
+
+    if BPA is not None:
+        raise Exception('setup(node_id) was called twice!')
+
+    storage = SimpleInMemoryStorage()
+    router = SimpleEpidemicRouter({IPND_IDENTIFIER_MTCP: MTcpCLA()}, storage)
+    BPA = BundleProtocolAgent(full_node_uri, storage, router, use_ipnd=True)
+
+    # node specific endpoint works like a normal endpoint (only receives exactly matched bundles), but for the node itself
+    endpoint = SimpleEndpoint('', node_receive_callback)
+    BPA.register_endpoint(endpoint._endpoint)
+
+    return endpoint
+
+
+def register(endpoint_identifier: str, receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleEndpoint:
+    """ registers an endpoint at the bundle protocol agent over which you can send/receive bundles(messages)
+
+    endpoint_identifier examples:
+        dtn addressing scheme -> "echo", "echo/subecho"
+        ipn addressing scheme -> "12", "24.15.16"
+
+    receive_callback -> may be None, but then you need to manually poll the endpoint
+
+    receive_callback signature/example:
+
+    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+        pass
+
+    the primary block is provided for direct access to additional information
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id) was not called!')
+
+    endpoint = SimpleEndpoint(endpoint_identifier, receive_callback)
+    BPA.register_endpoint(endpoint._endpoint)
+
+    return endpoint
+
+
+def register_group(full_group_uri: str, receive_callback: Callable[[bytes, str, str, PrimaryBlock], None] = None) -> SimpleGroupEndpoint:
+    """ registers a group-endpoint at the bundle protocol agent over which you can receive group-addressed bundles
+
+    full_group_uri examples:
+        "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
+
+    receive_callback -> may be None, but then you need to manually poll the endpoint
+
+    receive_callback signature/example:
+
+    callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+        pass
+
+    the primary block is provided for direct access to additional information
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id) was not called!')
+
+    endpoint = SimpleGroupEndpoint(full_group_uri, receive_callback)
+    BPA.register_group_endpoint(endpoint._endpoint)
+
+    return endpoint
+
+
+def discover() -> List[Node]:
+    """ returns a list of all currently known other nodes in the local network
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id) was not called!')
+
+    return list(BPA.storage.get_nodes())
+
+
+def update():
+    """ explicitly updates the bundle protocol agent
+
+    to be called in an endless loop if you want to write the loop yourself
+
+    the alternative solution (or inspiration) is: run_forever()
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id was not called!')
+
+    BPA.update()
+
+
+def run_forever(loop_callback=None, loop_callback_interval_milliseconds=1000, _sleep_time_seconds=0):
+    """ update loop to run the bundle protocol agent until KeyboardInterrupt
+
+    custom_logic_callback can be used for application specific logic after the bundle protocol agent was started
+
+    custom_logic_callback signature:
+
+    callback() -> None:
+        pass
+    """
+    global BPA
+
+    if BPA is None:
+        raise Exception('setup(node_id was not called!')
+
+    last_callback_execution = get_current_clock_millis()
+
+    try:
+        while True:
+            BPA.update()
+
+            if loop_callback is not None and is_timestamp_older_than_timeout(last_callback_execution, loop_callback_interval_milliseconds):
+                last_callback_execution = get_current_clock_millis()
+                loop_callback()
+
+            time.sleep(_sleep_time_seconds)
+    except KeyboardInterrupt:
+        pass
+
+
+def start_background_update_thread(_sleep_time_seconds=0):
+    """ (experimental) background update thread
+
+    On MicroPython the limited RAM can lead to crashes (most prominently a maximum-recursion-depth RuntimeError).
+    The _thread.stack_size(...) can be adjusted for compensation if needed and possible.
+    """
+    global BPA
+    global BPA_THREAD
+
+    if BPA is None:
+        raise Exception('setup(node_id was not called!')
+
+    if BPA_THREAD is not None:
+        raise Exception('start_background_update_thread() should only be called once!')
+
+    if RUNNING_MICROPYTHON:
+        _thread.stack_size(11500)  # experimental setting: 7000 does not run, 8000 does run, 11500 picked for leeway
+
+        def update_runner():
+            while True:
+                BPA.update()
+                time.sleep(_sleep_time_seconds)
+
+        BPA_THREAD = _thread.start_new_thread(update_runner, ())
+    else:
+        def self_stopping_update_runner():
+            while threading.main_thread().is_alive():
+                BPA.update()
+                time.sleep(_sleep_time_seconds)
+
+        BPA_THREAD = threading.Thread(target=self_stopping_update_runner)
+        BPA_THREAD.start()
```

### Comparing `dtn7zero-0.0.4/dtn7zero/bundle_protocol_agent.py` & `dtn7zero-0.0.5/dtn7zero/bundle_protocol_agent.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-from datetime import datetime, timezone, timedelta
-from typing import Dict, List
-
-from dtn7zero.data import BundleInformation, BundleStatusReportReasonCodes
-from dtn7zero.constants import SEND_STATUS_REPORTS_ENABLED, RUNNING_MICROPYTHON
-from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint, _LocalEndpoint
-from dtn7zero.ipnd import IPND
-from dtn7zero.routers import Router
-from dtn7zero.storage import Storage
-from dtn7zero.utility import debug, is_correct_node_uri, is_correct_endpoint_uri, is_correct_group_uri
-from py_dtn7.bundle import PrimaryBlock
-
-if RUNNING_MICROPYTHON:
-    from wlan import connect, isconnected
-
-
-class BundleProtocolAgent:
-
-    def __init__(self, full_node_uri: str, storage: Storage, router: Router, use_ipnd=True):
-        """ The main RFC 9171 compliant bpa component.
-
-        full_node_uri examples:
-            dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
-            ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
-        """
-        assert is_correct_node_uri(full_node_uri)
-
-        self.full_node_uri = full_node_uri
-        self.storage = storage
-        self.router = router
-        self.local_registered_endpoints: Dict[str, List[_LocalEndpoint]] = {}
-
-        self.local_bundle_dispatch_queue: List[BundleInformation] = []  # this pipeline-stage is needed to prevent infinite-recursion if two local endpoints answer each other on every reception-callback
-        self.storage_retry_generator = None
-        self.router_poll_generator = None
-
-        self.use_ipnd = use_ipnd
-        if self.use_ipnd:
-            # on micropython we need to handle wireless connections manually
-            if RUNNING_MICROPYTHON and not isconnected():
-                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
-
-            scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
-            self.ipnd = IPND(scheme_encoded, node_encoded, storage)
-
-    def update(self):
-        # on micropython we need to handle wireless connections manually
-        if RUNNING_MICROPYTHON and not isconnected():
-            connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
-
-        # update discovery
-        if self.use_ipnd:
-            self.ipnd.update()
-
-        # process stored/delayed bundle
-        if self.storage_retry_generator is None:
-            self.storage_retry_generator = self.storage.get_bundles_to_retry()
-
-        try:
-            self.bundle_dispatching(next(self.storage_retry_generator))
-        except StopIteration:
-            self.storage_retry_generator = None
-
-        # process one new local bundle
-        if self.local_bundle_dispatch_queue:
-            self.bundle_reception(self.local_bundle_dispatch_queue.pop(0))
-
-        # process new remote bundle
-        if self.router_poll_generator is None:
-            self.router_poll_generator = self.router.generator_poll_bundles()
-
-        try:
-            self.bundle_reception(next(self.router_poll_generator))
-        except StopIteration:
-            self.router_poll_generator = None
-
-    def register_endpoint(self, endpoint: LocalEndpoint) -> LocalEndpoint:
-        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
-        […] * commencing a registration (registering the node in an endpoint).
-        """
-        endpoint.bpa_register(self)
-
-        assert is_correct_endpoint_uri(endpoint.full_endpoint_uri)
-
-        if endpoint.full_endpoint_uri in self.local_registered_endpoints:
-            endpoint.bpa_unregister()
-            raise Exception('tried to register local endpoint {}, which is already registered as a local endpoint'.format(endpoint.endpoint_identifier))
-
-        self.local_registered_endpoints[endpoint.full_endpoint_uri] = (endpoint,)
-
-        return endpoint
-
-    def register_group_endpoint(self, endpoint: LocalGroupEndpoint) -> LocalGroupEndpoint:
-        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
-        […] * commencing a registration (registering the node in an endpoint).
-        """
-        assert is_correct_group_uri(endpoint.full_endpoint_uri)
-
-        endpoint.bpa_register(self)
-
-        if endpoint.full_endpoint_uri in self.local_registered_endpoints:
-            self.local_registered_endpoints[endpoint.full_endpoint_uri].append(endpoint)
-        else:
-            self.local_registered_endpoints[endpoint.full_endpoint_uri] = [endpoint]
-
-        return endpoint
-
-    def unregister_endpoint(self, endpoint: LocalEndpoint):
-        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
-        […] * terminating a registration.
-        """
-        if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
-            raise Exception('tried to unregister non-existent local endpoint {}'.format(endpoint.endpoint_identifier))
-
-        full_endpoint_uri = endpoint.full_endpoint_uri
-        self.local_registered_endpoints[full_endpoint_uri][0].bpa_unregister()
-        del self.local_registered_endpoints[full_endpoint_uri]
-
-    def unregister_group_endpoint(self, endpoint: LocalGroupEndpoint):
-        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
-        […] * terminating a registration.
-        """
-        if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
-            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
-
-        try:
-            self.local_registered_endpoints[endpoint.full_endpoint_uri].remove(endpoint)
-        except ValueError:
-            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
-
-        if not self.local_registered_endpoints[endpoint.full_endpoint_uri]:
-            del self.local_registered_endpoints[endpoint.full_endpoint_uri]
-
-    def cancel_transmission(self, bundle_id: str) -> bool:
-        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
-        […] * canceling a transmission.
-        """
-        # should only be called by a local endpoint
-        # returns True if the bundle was still in local storage to delete, False otherwise
-        return self.storage.remove_bundle(bundle_id)
-
-    def bundle_reception(self, bundle_information: BundleInformation):
-        # bundles with the same ID should never land here -> either they are filtered by the router or uniquely created from an endpoint
-
-        bundle = bundle_information.bundle
-
-        """ RFC 9171, 5.6 Bundle Reception
-        […] Step 1: The retention constraint "Dispatch pending" MUST be added to the bundle. […]
-        """
-        bundle_information.retention_constraint = BundleInformation.RETENTION_CONSTRAINT_DISPATCH_PENDING
-
-        """ RFC 9171, 5.6 Bundle Reception
-        […] Step 2: If the "request reporting of bundle reception" flag in the bundle's status report request field 
-        is set to 1 and status reporting is enabled, then a bundle reception status report with reason code 
-        "No additional information" SHOULD be generated, destined for the bundle's report-to endpoint ID. […]
-        """
-        if bundle.primary_block.bundle_processing_control_flags.status_of_report_reception_is_requested:
-            # todo: create a status report
-            pass
-
-        """ RFC 9171, 5.6 Bundle Reception
-        […] Step 3: CRCs SHOULD be computed for every block of the bundle that has an attached CRC. 
-        If any block of the bundle is malformed according to this specification (including syntactically invalid CBOR), 
-        or if any block has an attached CRC and the CRC computed for this block upon reception differs from that 
-        attached CRC, then the BPA MUST delete the bundle for the reason "Block unintelligible". The Bundle Deletion 
-        procedure defined in Section 5.10 MUST be followed, and all remaining steps of the Bundle Reception procedure 
-        MUST be skipped. […]
-        """
-        # currently there is no CRC implemented and bundles with CRC are rejected at bundle deserialization
-        # todo: implement CRC support
-
-        """ RFC 9171, 5.6 Bundle Reception
-        […] Step 4: For each block in the bundle that is an extension block that the BPA cannot process:
-        
-        * If the block processing control flags in that block indicate that a status report is requested in this event 
-        and if status reporting is enabled, then a bundle reception status report with reason code "Block unsupported" 
-        SHOULD be generated, destined for the bundle's report-to endpoint ID.
-        
-        * If the block processing control flags in that block indicate that the bundle must be deleted in this event, 
-        then the BPA MUST delete the bundle for the reason "Block unsupported"; the Bundle Deletion procedure defined 
-        in Section 5.10 MUST be followed, and all remaining steps of the Bundle Reception procedure MUST be skipped.
-        
-        * If the block processing control flags in that block do NOT indicate that the bundle must be deleted in this 
-        event but do indicate that the block must be discarded, then the BPA MUST remove this block from the bundle.
-        
-        * If the block processing control flags in that block neither indicate that the bundle must be deleted nor 
-        indicate that the block must be discarded, then processing continues with the next extension block that the 
-        BPA cannot process, if any; otherwise, processing proceeds from Step 5. […]
-        """
-        for block in bundle.other_blocks[:]:
-            flags = block.block_processing_control_flags
-
-            if flags.report_status_if_block_cant_be_processed and SEND_STATUS_REPORTS_ENABLED:
-                # todo: generate a status report
-                pass
-
-            if flags.delete_bundle_if_block_cant_be_processed:
-                self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.BLOCK_UNSUPPORTED)
-                return
-            elif flags.discard_block_if_block_cant_be_processed:
-                bundle.other_blocks.remove(block)
-
-        """ 4.4.3 Hop Count
-        […] When a bundle's hop count exceeds its hop limit, the bundle SHOULD be deleted for the reason "Hop limit 
-        exceeded", following the Bundle Deletion procedure defined in Section 5.10.
-        """
-        if bundle.hop_count_block and bundle.hop_count_block.hop_count >= bundle.hop_count_block.hop_limit:
-            self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.HOP_LIMIT_EXCEEDED)
-            return
-        if bundle.bundle_age_block and bundle.bundle_age_block.age_milliseconds >= bundle.primary_block.lifetime:
-            self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.LIFETIME_EXPIRED)
-            return
-        if not RUNNING_MICROPYTHON and bundle.primary_block.bundle_creation_time != 0:
-            expiration_time = bundle.primary_block.bundle_creation_time_datetime + timedelta(milliseconds=bundle.primary_block.lifetime)
-            if expiration_time < datetime.now(timezone.utc):
-                self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.LIFETIME_EXPIRED)
-                return
-
-        """ RFC 9171, 5.6 Bundle Reception
-        […] Step 5: Processing proceeds from Step 1 of Section 5.3.
-        """
-        self.bundle_dispatching(bundle_information)
-
-    def bundle_dispatching(self, bundle_information: BundleInformation):
-        """ RFC 9171, 5.3 Bundle Dispatching
-        […] Step 1: If the bundle's destination endpoint is an endpoint of which the node is a member, 
-        the Bundle Delivery procedure defined in Section 5.7 MUST be followed and, […] the node SHALL NOT undertake to 
-        forward the bundle to itself in the course of performing the procedure described in Section 5.4. […]
-        """
-        if not bundle_information.locally_delivered and bundle_information.bundle.primary_block.full_destination_uri in self.local_registered_endpoints:
-            self.local_bundle_delivery(bundle_information)
-
-        """ RFC 9171, 5.3 Bundle Dispatching
-        […] Step 2: Processing proceeds from Step 1 of Section 5.4.
-        """
-        self.bundle_forwarding(bundle_information)
-
-    def local_bundle_delivery(self, bundle_information: BundleInformation):
-
-        """ RFC 9171, 5.7 Local Bundle Delivery
-        […] Step 1: If the received bundle is a fragment, the ADU Reassembly procedure described in Section 5.9 
-        MUST be followed. If this procedure results in reassembly of the entire original ADU, processing of the 
-        fragmentary bundle whose payload has been replaced by the reassembled ADU (whether this bundle or a previously 
-        received fragment) proceeds from Step 2; otherwise, the retention constraint "Reassembly pending" MUST be added 
-        to the bundle, and all remaining steps of this procedure MUST be skipped. […]
-        """
-        # there is currently no fragment support implemented and fragmented bundles are rejected at deserialization
-        # todo: implement fragment support
-
-        """ RFC 9171, 5.7 Local Bundle Delivery
-        […] Step 2: Delivery depends on the state of the registration whose endpoint ID matches that of the destination 
-        of the bundle:
-        
-        * An additional implementation-specific delivery deferral procedure MAY optionally be associated with the 
-        registration. […]
-        """
-        bundle_information.locally_delivered = True
-
-        # on group-endpoints there can be multiple registrations, on unicast-endpoints this is a 1-tuple
-        for endpoint in self.local_registered_endpoints[bundle_information.bundle.primary_block.full_destination_uri]:
-            endpoint.bpa_local_bundle_delivery(bundle_information.bundle)
-
-    def bundle_forwarding(self, bundle_information: BundleInformation):
-
-        """ RFC 9171, 5.4 Bundle Forwarding
-        […] Step 1: The retention constraint "Forward pending" MUST be added to the bundle, and the bundle's 
-        "Dispatch pending" retention constraint MUST be removed. […]
-        """
-        bundle_information.retention_constraint = BundleInformation.RETENTION_CONSTRAINT_FORWARD_PENDING
-
-        """ RFC 9171, 5.4 Bundle Forwarding
-        […] Step 2: The BPA MUST determine whether or not forwarding is contraindicated (that is, rendered inadvisable)
-        […] * […] If the BPA elects to forward the bundle to some other node(s) for further forwarding but finds it 
-        impossible to select any node(s) to forward the bundle to, then forwarding is contraindicated. […]
-        """
-        success, reason = self.router.immediate_forwarding_attempt(self.full_node_uri, bundle_information)
-
-        """ RFC 9171, 5.4 Bundle Forwarding
-        […] Step 3: If forwarding of the bundle is determined to be contraindicated for any of the reasons listed in 
-        the IANA "Bundle Status Report Reason Codes" registry (see Section 9.5), then the Forwarding Contraindicated 
-        procedure defined in Section 5.4.1 MUST be followed; the remaining steps of this Bundle Forwarding procedure 
-        are skipped at this time. […]
-        """
-        if not success:
-            """ RFC 9171, 5.4.1 Forwarding Contraindicated
-            […] Step 1: The BPA MUST determine whether or not to declare failure in forwarding the bundle. 
-            Note: This decision is likely to be influenced by the reason for which forwarding is contraindicated. […]
-            """
-            no_failure_codes = (
-                BundleStatusReportReasonCodes.NO_KNOWN_ROUTE_TO_DESTINATION_FROM_HERE,
-                BundleStatusReportReasonCodes.NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE,
-                BundleStatusReportReasonCodes.TRAFFIC_PARED
-            )
-
-            if reason in no_failure_codes:
-                """ RFC 9171, 5.4.1 Forwarding Contraindicated
-                […] when -- at some future time -- the forwarding of this bundle ceases to be contraindicated, 
-                processing proceeds from Step 4 of Section 5.4. […]
-                """
-                storage_success, removed_bundle_informations = self.storage.delay_bundle(bundle_information)
-
-                if not storage_success:
-                    reason = BundleStatusReportReasonCodes.DEPLETED_STORAGE
-
-                for removed_bundle_information in removed_bundle_informations:
-                    if len(removed_bundle_information.forwarded_to_nodes) > 0:
-                        removed_bundle_reason = BundleStatusReportReasonCodes.NO_ADDITIONAL_INFORMATION
-                    else:
-                        removed_bundle_reason = BundleStatusReportReasonCodes.DEPLETED_STORAGE
-
-                    self.bundle_deletion(removed_bundle_information, removed_bundle_reason)
-
-            if reason not in no_failure_codes:
-                """ RFC 9171, 5.4.1 Forwarding Contraindicated
-                […] Step 2: If forwarding failure is declared, then the Forwarding Failed procedure defined in 
-                Section 5.4.2 MUST be followed. […]
-                """
-                """ RFC 9171, 5.4.2 Forwarding Failed
-                […] Step 1: The BPA MAY forward the bundle back to the node that sent it, as identified by the Previous 
-                Node Block, if present. This forwarding, if performed, SHALL be accomplished by performing Step 4 and 
-                Step 5 of Section 5.4 where the sole node selected for forwarding SHALL be the node that sent the 
-                bundle. […]
-                """
-                if bundle_information.bundle.previous_node_block:
-                    self.router.send_to_previous_node(self.full_node_uri, bundle_information)
-
-                """ RFC 9171, 5.4.2 Forwarding Failed
-                […] Step 2: If the bundle's destination endpoint is an endpoint of which the node is a member, 
-                then the bundle's "Forward pending" retention constraint MUST be removed. Otherwise, the bundle MUST be 
-                deleted: the Bundle Deletion procedure defined in Section 5.10 MUST be followed, citing the reason for 
-                which forwarding was determined to be contraindicated.
-                """
-                if bundle_information.bundle.primary_block.destination_specific_part in self.local_registered_endpoints:
-                    bundle_information.retention_constraint = None
-                else:
-                    self.bundle_deletion(bundle_information, reason)
-        else:
-            """ RFC 9171, 5.4 Bundle Forwarding
-            […] If completion of the data-sending procedures by all selected CLAs HAS resulted in successful forwarding 
-            of the bundle, or if it has not but the BPA does not choose to initiate another attempt to forward the 
-            bundle, then:
-            
-            * If the "request reporting of bundle forwarding" flag in the bundle's status report request field is set 
-            to 1 and status reporting is enabled, then a bundle forwarding status report SHOULD be generated, destined 
-            for the bundle's report-to endpoint ID. The reason code on this bundle forwarding status report MUST 
-            be "no additional information". […]
-            """
-            if bundle_information.bundle.primary_block.bundle_processing_control_flags.status_of_report_forwarding_is_requested:
-                # todo: generate a status report
-                pass
-
-            """ RFC 9171, 5.4 Bundle Forwarding
-            […] * The bundle's "Forward pending" retention constraint MUST be removed.
-            """
-            bundle_information.retention_constraint = None
-
-    def bundle_deletion(self, bundle_information: BundleInformation, reason: int):
-        """ RFC 9171, 5.10 Bundle Deletion
-        […] Step 1: If the "request reporting of bundle deletion" flag in the bundle's status report request field is
-        set to 1 and if status reporting is enabled, then a bundle deletion status report citing the reason for
-        deletion SHOULD be generated, destined for the bundle's report-to endpoint ID. […]
-        """
-        flags = bundle_information.bundle.primary_block.bundle_processing_control_flags
-        if flags.status_of_report_deletion_is_requested and SEND_STATUS_REPORTS_ENABLED:
-            # todo: generate a status report
-            pass
-
-        """ RFC 9171, 5.10 Bundle Deletion
-        […] Step 2: All of the bundle's retention constraints MUST be removed.
-        """
-        bundle_information.retention_constraint = None
-
-        debug('bundle scheduled for deletion, reason: {}, bundle: {}'.format(reason, bundle_information.bundle.bundle_id))
+from datetime import datetime, timezone, timedelta
+from typing import Dict, List
+
+from dtn7zero.data import BundleInformation, BundleStatusReportReasonCodes
+from dtn7zero.constants import SEND_STATUS_REPORTS_ENABLED, RUNNING_MICROPYTHON
+from dtn7zero.endpoints import LocalEndpoint, LocalGroupEndpoint, _LocalEndpoint
+from dtn7zero.ipnd import IPND
+from dtn7zero.routers import Router
+from dtn7zero.storage import Storage
+from dtn7zero.utility import debug, is_correct_node_uri, is_correct_endpoint_uri, is_correct_group_uri
+from py_dtn7.bundle import PrimaryBlock
+
+if RUNNING_MICROPYTHON:
+    from wlan import connect, isconnected
+
+
+class BundleProtocolAgent:
+
+    def __init__(self, full_node_uri: str, storage: Storage, router: Router, use_ipnd=True):
+        """ The main RFC 9171 compliant bpa component.
+
+        full_node_uri examples:
+            dtn addressing scheme -> "dtn://node1/", "dtn://cool-node/"  # '/' at the end is mandatory
+            ipn addressing scheme -> "ipn://12", "ipn://24.25"  # will be joined with the endpoints via '.'
+        """
+        assert is_correct_node_uri(full_node_uri)
+
+        self.full_node_uri = full_node_uri
+        self.storage = storage
+        self.router = router
+        self.local_registered_endpoints: Dict[str, List[_LocalEndpoint]] = {}
+
+        self.local_bundle_dispatch_queue: List[BundleInformation] = []  # this pipeline-stage is needed to prevent infinite-recursion if two local endpoints answer each other on every reception-callback
+        self.storage_retry_generator = None
+        self.router_poll_generator = None
+
+        self.use_ipnd = use_ipnd
+        if self.use_ipnd:
+            # on micropython we need to handle wireless connections manually
+            if RUNNING_MICROPYTHON and not isconnected():
+                connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+
+            scheme_encoded, node_encoded = PrimaryBlock.from_full_uri(full_node_uri)
+            self.ipnd = IPND(scheme_encoded, node_encoded, storage)
+
+    def update(self):
+        # on micropython we need to handle wireless connections manually
+        if RUNNING_MICROPYTHON and not isconnected():
+            connect()  # the microcontroller may be moved around, so connect to any available network instead of reconnect
+
+        # update discovery
+        if self.use_ipnd:
+            self.ipnd.update()
+
+        # process stored/delayed bundle
+        if self.storage_retry_generator is None:
+            self.storage_retry_generator = self.storage.get_bundles_to_retry()
+
+        try:
+            self.bundle_dispatching(next(self.storage_retry_generator))
+        except StopIteration:
+            self.storage_retry_generator = None
+
+        # process one new local bundle
+        if self.local_bundle_dispatch_queue:
+            self.bundle_reception(self.local_bundle_dispatch_queue.pop(0))
+
+        # process new remote bundle
+        if self.router_poll_generator is None:
+            self.router_poll_generator = self.router.generator_poll_bundles()
+
+        try:
+            self.bundle_reception(next(self.router_poll_generator))
+        except StopIteration:
+            self.router_poll_generator = None
+
+    def register_endpoint(self, endpoint: LocalEndpoint) -> LocalEndpoint:
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * commencing a registration (registering the node in an endpoint).
+        """
+        endpoint.bpa_register(self)
+
+        assert is_correct_endpoint_uri(endpoint.full_endpoint_uri)
+
+        if endpoint.full_endpoint_uri in self.local_registered_endpoints:
+            endpoint.bpa_unregister()
+            raise Exception('tried to register local endpoint {}, which is already registered as a local endpoint'.format(endpoint.endpoint_identifier))
+
+        self.local_registered_endpoints[endpoint.full_endpoint_uri] = (endpoint,)
+
+        return endpoint
+
+    def register_group_endpoint(self, endpoint: LocalGroupEndpoint) -> LocalGroupEndpoint:
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * commencing a registration (registering the node in an endpoint).
+        """
+        assert is_correct_group_uri(endpoint.full_endpoint_uri)
+
+        endpoint.bpa_register(self)
+
+        if endpoint.full_endpoint_uri in self.local_registered_endpoints:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri].append(endpoint)
+        else:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri] = [endpoint]
+
+        return endpoint
+
+    def unregister_endpoint(self, endpoint: LocalEndpoint):
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * terminating a registration.
+        """
+        if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
+            raise Exception('tried to unregister non-existent local endpoint {}'.format(endpoint.endpoint_identifier))
+
+        full_endpoint_uri = endpoint.full_endpoint_uri
+        self.local_registered_endpoints[full_endpoint_uri][0].bpa_unregister()
+        del self.local_registered_endpoints[full_endpoint_uri]
+
+    def unregister_group_endpoint(self, endpoint: LocalGroupEndpoint):
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * terminating a registration.
+        """
+        if endpoint.full_endpoint_uri not in self.local_registered_endpoints:
+            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
+
+        try:
+            self.local_registered_endpoints[endpoint.full_endpoint_uri].remove(endpoint)
+        except ValueError:
+            raise Exception('tried to unregister non-existent local group endpoint {}'.format(endpoint.full_endpoint_uri))
+
+        if not self.local_registered_endpoints[endpoint.full_endpoint_uri]:
+            del self.local_registered_endpoints[endpoint.full_endpoint_uri]
+
+    def cancel_transmission(self, bundle_id: str) -> bool:
+        """ RFC 9171, 3.3 Services Offered by Bundle Protocol Agents
+        […] * canceling a transmission.
+        """
+        # should only be called by a local endpoint
+        # returns True if the bundle was still in local storage to delete, False otherwise
+        return self.storage.remove_bundle(bundle_id)
+
+    def bundle_reception(self, bundle_information: BundleInformation):
+        # bundles with the same ID should never land here -> either they are filtered by the router or uniquely created from an endpoint
+
+        bundle = bundle_information.bundle
+
+        """ RFC 9171, 5.6 Bundle Reception
+        […] Step 1: The retention constraint "Dispatch pending" MUST be added to the bundle. […]
+        """
+        bundle_information.retention_constraint = BundleInformation.RETENTION_CONSTRAINT_DISPATCH_PENDING
+
+        """ RFC 9171, 5.6 Bundle Reception
+        […] Step 2: If the "request reporting of bundle reception" flag in the bundle's status report request field 
+        is set to 1 and status reporting is enabled, then a bundle reception status report with reason code 
+        "No additional information" SHOULD be generated, destined for the bundle's report-to endpoint ID. […]
+        """
+        if bundle.primary_block.bundle_processing_control_flags.status_of_report_reception_is_requested:
+            # todo: create a status report
+            pass
+
+        """ RFC 9171, 5.6 Bundle Reception
+        […] Step 3: CRCs SHOULD be computed for every block of the bundle that has an attached CRC. 
+        If any block of the bundle is malformed according to this specification (including syntactically invalid CBOR), 
+        or if any block has an attached CRC and the CRC computed for this block upon reception differs from that 
+        attached CRC, then the BPA MUST delete the bundle for the reason "Block unintelligible". The Bundle Deletion 
+        procedure defined in Section 5.10 MUST be followed, and all remaining steps of the Bundle Reception procedure 
+        MUST be skipped. […]
+        """
+        # currently there is no CRC implemented and bundles with CRC are rejected at bundle deserialization
+        # todo: implement CRC support
+
+        """ RFC 9171, 5.6 Bundle Reception
+        […] Step 4: For each block in the bundle that is an extension block that the BPA cannot process:
+        
+        * If the block processing control flags in that block indicate that a status report is requested in this event 
+        and if status reporting is enabled, then a bundle reception status report with reason code "Block unsupported" 
+        SHOULD be generated, destined for the bundle's report-to endpoint ID.
+        
+        * If the block processing control flags in that block indicate that the bundle must be deleted in this event, 
+        then the BPA MUST delete the bundle for the reason "Block unsupported"; the Bundle Deletion procedure defined 
+        in Section 5.10 MUST be followed, and all remaining steps of the Bundle Reception procedure MUST be skipped.
+        
+        * If the block processing control flags in that block do NOT indicate that the bundle must be deleted in this 
+        event but do indicate that the block must be discarded, then the BPA MUST remove this block from the bundle.
+        
+        * If the block processing control flags in that block neither indicate that the bundle must be deleted nor 
+        indicate that the block must be discarded, then processing continues with the next extension block that the 
+        BPA cannot process, if any; otherwise, processing proceeds from Step 5. […]
+        """
+        for block in bundle.other_blocks[:]:
+            flags = block.block_processing_control_flags
+
+            if flags.report_status_if_block_cant_be_processed and SEND_STATUS_REPORTS_ENABLED:
+                # todo: generate a status report
+                pass
+
+            if flags.delete_bundle_if_block_cant_be_processed:
+                self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.BLOCK_UNSUPPORTED)
+                return
+            elif flags.discard_block_if_block_cant_be_processed:
+                bundle.other_blocks.remove(block)
+
+        """ 4.4.3 Hop Count
+        […] When a bundle's hop count exceeds its hop limit, the bundle SHOULD be deleted for the reason "Hop limit 
+        exceeded", following the Bundle Deletion procedure defined in Section 5.10.
+        """
+        if bundle.hop_count_block and bundle.hop_count_block.hop_count >= bundle.hop_count_block.hop_limit:
+            self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.HOP_LIMIT_EXCEEDED)
+            return
+        if bundle.bundle_age_block and bundle.bundle_age_block.age_milliseconds >= bundle.primary_block.lifetime:
+            self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.LIFETIME_EXPIRED)
+            return
+        if not RUNNING_MICROPYTHON and bundle.primary_block.bundle_creation_time != 0:
+            expiration_time = bundle.primary_block.bundle_creation_time_datetime + timedelta(milliseconds=bundle.primary_block.lifetime)
+            if expiration_time < datetime.now(timezone.utc):
+                self.bundle_deletion(bundle_information, BundleStatusReportReasonCodes.LIFETIME_EXPIRED)
+                return
+
+        """ RFC 9171, 5.6 Bundle Reception
+        […] Step 5: Processing proceeds from Step 1 of Section 5.3.
+        """
+        self.bundle_dispatching(bundle_information)
+
+    def bundle_dispatching(self, bundle_information: BundleInformation):
+        """ RFC 9171, 5.3 Bundle Dispatching
+        […] Step 1: If the bundle's destination endpoint is an endpoint of which the node is a member, 
+        the Bundle Delivery procedure defined in Section 5.7 MUST be followed and, […] the node SHALL NOT undertake to 
+        forward the bundle to itself in the course of performing the procedure described in Section 5.4. […]
+        """
+        if not bundle_information.locally_delivered and bundle_information.bundle.primary_block.full_destination_uri in self.local_registered_endpoints:
+            self.local_bundle_delivery(bundle_information)
+
+        """ RFC 9171, 5.3 Bundle Dispatching
+        […] Step 2: Processing proceeds from Step 1 of Section 5.4.
+        """
+        self.bundle_forwarding(bundle_information)
+
+    def local_bundle_delivery(self, bundle_information: BundleInformation):
+
+        """ RFC 9171, 5.7 Local Bundle Delivery
+        […] Step 1: If the received bundle is a fragment, the ADU Reassembly procedure described in Section 5.9 
+        MUST be followed. If this procedure results in reassembly of the entire original ADU, processing of the 
+        fragmentary bundle whose payload has been replaced by the reassembled ADU (whether this bundle or a previously 
+        received fragment) proceeds from Step 2; otherwise, the retention constraint "Reassembly pending" MUST be added 
+        to the bundle, and all remaining steps of this procedure MUST be skipped. […]
+        """
+        # there is currently no fragment support implemented and fragmented bundles are rejected at deserialization
+        # todo: implement fragment support
+
+        """ RFC 9171, 5.7 Local Bundle Delivery
+        […] Step 2: Delivery depends on the state of the registration whose endpoint ID matches that of the destination 
+        of the bundle:
+        
+        * An additional implementation-specific delivery deferral procedure MAY optionally be associated with the 
+        registration. […]
+        """
+        bundle_information.locally_delivered = True
+
+        # on group-endpoints there can be multiple registrations, on unicast-endpoints this is a 1-tuple
+        for endpoint in self.local_registered_endpoints[bundle_information.bundle.primary_block.full_destination_uri]:
+            endpoint.bpa_local_bundle_delivery(bundle_information.bundle)
+
+    def bundle_forwarding(self, bundle_information: BundleInformation):
+
+        """ RFC 9171, 5.4 Bundle Forwarding
+        […] Step 1: The retention constraint "Forward pending" MUST be added to the bundle, and the bundle's 
+        "Dispatch pending" retention constraint MUST be removed. […]
+        """
+        bundle_information.retention_constraint = BundleInformation.RETENTION_CONSTRAINT_FORWARD_PENDING
+
+        """ RFC 9171, 5.4 Bundle Forwarding
+        […] Step 2: The BPA MUST determine whether or not forwarding is contraindicated (that is, rendered inadvisable)
+        […] * […] If the BPA elects to forward the bundle to some other node(s) for further forwarding but finds it 
+        impossible to select any node(s) to forward the bundle to, then forwarding is contraindicated. […]
+        """
+        success, reason = self.router.immediate_forwarding_attempt(self.full_node_uri, bundle_information)
+
+        """ RFC 9171, 5.4 Bundle Forwarding
+        […] Step 3: If forwarding of the bundle is determined to be contraindicated for any of the reasons listed in 
+        the IANA "Bundle Status Report Reason Codes" registry (see Section 9.5), then the Forwarding Contraindicated 
+        procedure defined in Section 5.4.1 MUST be followed; the remaining steps of this Bundle Forwarding procedure 
+        are skipped at this time. […]
+        """
+        if not success:
+            """ RFC 9171, 5.4.1 Forwarding Contraindicated
+            […] Step 1: The BPA MUST determine whether or not to declare failure in forwarding the bundle. 
+            Note: This decision is likely to be influenced by the reason for which forwarding is contraindicated. […]
+            """
+            no_failure_codes = (
+                BundleStatusReportReasonCodes.NO_KNOWN_ROUTE_TO_DESTINATION_FROM_HERE,
+                BundleStatusReportReasonCodes.NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE,
+                BundleStatusReportReasonCodes.TRAFFIC_PARED
+            )
+
+            if reason in no_failure_codes:
+                """ RFC 9171, 5.4.1 Forwarding Contraindicated
+                […] when -- at some future time -- the forwarding of this bundle ceases to be contraindicated, 
+                processing proceeds from Step 4 of Section 5.4. […]
+                """
+                storage_success, removed_bundle_informations = self.storage.delay_bundle(bundle_information)
+
+                if not storage_success:
+                    reason = BundleStatusReportReasonCodes.DEPLETED_STORAGE
+
+                for removed_bundle_information in removed_bundle_informations:
+                    if len(removed_bundle_information.forwarded_to_nodes) > 0:
+                        removed_bundle_reason = BundleStatusReportReasonCodes.NO_ADDITIONAL_INFORMATION
+                    else:
+                        removed_bundle_reason = BundleStatusReportReasonCodes.DEPLETED_STORAGE
+
+                    self.bundle_deletion(removed_bundle_information, removed_bundle_reason)
+
+            if reason not in no_failure_codes:
+                """ RFC 9171, 5.4.1 Forwarding Contraindicated
+                […] Step 2: If forwarding failure is declared, then the Forwarding Failed procedure defined in 
+                Section 5.4.2 MUST be followed. […]
+                """
+                """ RFC 9171, 5.4.2 Forwarding Failed
+                […] Step 1: The BPA MAY forward the bundle back to the node that sent it, as identified by the Previous 
+                Node Block, if present. This forwarding, if performed, SHALL be accomplished by performing Step 4 and 
+                Step 5 of Section 5.4 where the sole node selected for forwarding SHALL be the node that sent the 
+                bundle. […]
+                """
+                if bundle_information.bundle.previous_node_block:
+                    self.router.send_to_previous_node(self.full_node_uri, bundle_information)
+
+                """ RFC 9171, 5.4.2 Forwarding Failed
+                […] Step 2: If the bundle's destination endpoint is an endpoint of which the node is a member, 
+                then the bundle's "Forward pending" retention constraint MUST be removed. Otherwise, the bundle MUST be 
+                deleted: the Bundle Deletion procedure defined in Section 5.10 MUST be followed, citing the reason for 
+                which forwarding was determined to be contraindicated.
+                """
+                if bundle_information.bundle.primary_block.destination_specific_part in self.local_registered_endpoints:
+                    bundle_information.retention_constraint = None
+                else:
+                    self.bundle_deletion(bundle_information, reason)
+        else:
+            """ RFC 9171, 5.4 Bundle Forwarding
+            […] If completion of the data-sending procedures by all selected CLAs HAS resulted in successful forwarding 
+            of the bundle, or if it has not but the BPA does not choose to initiate another attempt to forward the 
+            bundle, then:
+            
+            * If the "request reporting of bundle forwarding" flag in the bundle's status report request field is set 
+            to 1 and status reporting is enabled, then a bundle forwarding status report SHOULD be generated, destined 
+            for the bundle's report-to endpoint ID. The reason code on this bundle forwarding status report MUST 
+            be "no additional information". […]
+            """
+            if bundle_information.bundle.primary_block.bundle_processing_control_flags.status_of_report_forwarding_is_requested:
+                # todo: generate a status report
+                pass
+
+            """ RFC 9171, 5.4 Bundle Forwarding
+            […] * The bundle's "Forward pending" retention constraint MUST be removed.
+            """
+            bundle_information.retention_constraint = None
+
+    def bundle_deletion(self, bundle_information: BundleInformation, reason: int):
+        """ RFC 9171, 5.10 Bundle Deletion
+        […] Step 1: If the "request reporting of bundle deletion" flag in the bundle's status report request field is
+        set to 1 and if status reporting is enabled, then a bundle deletion status report citing the reason for
+        deletion SHOULD be generated, destined for the bundle's report-to endpoint ID. […]
+        """
+        flags = bundle_information.bundle.primary_block.bundle_processing_control_flags
+        if flags.status_of_report_deletion_is_requested and SEND_STATUS_REPORTS_ENABLED:
+            # todo: generate a status report
+            pass
+
+        """ RFC 9171, 5.10 Bundle Deletion
+        […] Step 2: All of the bundle's retention constraints MUST be removed.
+        """
+        bundle_information.retention_constraint = None
+
+        debug('bundle scheduled for deletion, reason: {}, bundle: {}'.format(reason, bundle_information.bundle.bundle_id))
```

### Comparing `dtn7zero-0.0.4/dtn7zero/constants.py` & `dtn7zero-0.0.5/dtn7zero/constants.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import sys
-
-RUNNING_MICROPYTHON = sys.implementation.name == 'micropython'
-
-
-ATTACH_PREVIOUS_NODE_BLOCK = True
-
-BROADCAST_SEND_INTERVAL_SECONDS = 30
-
-BROADCAST_TIMEOUT_SECONDS = 120
-
-ENCODING = 'utf-8'
-
-IPND_IDENTIFIER_MTCP = 'mtcp'
-IPND_IDENTIFIER_REST = 'rest'  # unofficial, to be used to manually add the rest-cla to a known dtn7rs-node
-IPND_SEND_INTERVAL_MILLISECONDS = 10000
-
-if RUNNING_MICROPYTHON:
-    IPND_BEACON_MAX_SIZE = 256  # for some reason a bigger datagram receive leads to memory leaks ???
-else:
-    IPND_BEACON_MAX_SIZE = 4096
-
-if RUNNING_MICROPYTHON:
-    MTCP_MAX_CONNECTIONS_STATE_WAITING = 2
-    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 3
-    MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 5000
-else:
-    MTCP_MAX_CONNECTIONS_STATE_WAITING = 5
-    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 10000
-    MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 1000000
-
-MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND = 2000
-
-PORT_BEACON_UDP = 7000
-PORT_REST = 3000
-PORT_MTCP = 16162
-PORT_IPND = 3003
-
-SEND_STATUS_REPORTS_ENABLED = False
-
-SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO = 3
-
-if RUNNING_MICROPYTHON:
-    SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 7  # experimental setting
-    SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 18  # experimental setting
-else:
-    SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 10000
-    SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 100000
-
-SOCKET_RECEIVE_BUFFER_SIZE = 512
-
-
-DEBUG = False
-WARNING = True
+import sys
+
+RUNNING_MICROPYTHON = sys.implementation.name == 'micropython'
+
+
+ATTACH_PREVIOUS_NODE_BLOCK = True
+
+BROADCAST_SEND_INTERVAL_SECONDS = 30
+
+BROADCAST_TIMEOUT_SECONDS = 120
+
+ENCODING = 'utf-8'
+
+IPND_IDENTIFIER_MTCP = 'mtcp'
+IPND_IDENTIFIER_REST = 'rest'  # unofficial, to be used to manually add the rest-cla to a known dtn7rs-node
+IPND_SEND_INTERVAL_MILLISECONDS = 10000
+
+if RUNNING_MICROPYTHON:
+    IPND_BEACON_MAX_SIZE = 256  # for some reason a bigger datagram receive leads to memory leaks ???
+else:
+    IPND_BEACON_MAX_SIZE = 4096
+
+if RUNNING_MICROPYTHON:
+    MTCP_MAX_CONNECTIONS_STATE_WAITING = 2
+    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 3
+    MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 5000
+else:
+    MTCP_MAX_CONNECTIONS_STATE_WAITING = 5
+    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE = 10000
+    MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE = 1000000
+
+MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND = 2000
+
+PORT_BEACON_UDP = 7000
+PORT_REST = 3000
+PORT_MTCP = 16162
+PORT_IPND = 3003
+
+SEND_STATUS_REPORTS_ENABLED = False
+
+SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO = 3
+
+if RUNNING_MICROPYTHON:
+    SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 7  # experimental setting
+    SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 18  # experimental setting
+else:
+    SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES = 10000
+    SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS = 100000
+
+SOCKET_RECEIVE_BUFFER_SIZE = 512
+
+
+DEBUG = False
+WARNING = True
```

### Comparing `dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/__init__.py` & `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from abc import ABC
-from typing import Optional, List, Tuple
-
-from dtn7zero.data import Node
-from py_dtn7 import Bundle
-
-
-class CLA(ABC):
-
-    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
-        raise NotImplementedError('do not instantiate CLA class directly')
-
-    def poll_ids(self, node: Node) -> Optional[List[str]]:
-        raise NotImplementedError('do not instantiate CLA class directly')
-
-    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
-        raise NotImplementedError('do not instantiate CLA class directly')
+from abc import ABC
+from typing import Optional, List, Tuple
+
+from dtn7zero.data import Node
+from py_dtn7 import Bundle
+
+
+class CLA(ABC):
+
+    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
+        raise NotImplementedError('do not instantiate CLA class directly')
+
+    def poll_ids(self, node: Node) -> Optional[List[str]]:
+        raise NotImplementedError('do not instantiate CLA class directly')
+
+    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
+        raise NotImplementedError('do not instantiate CLA class directly')
```

### Comparing `dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py` & `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from typing import Dict, List, Optional, Tuple
-
-from dtn7zero.convergence_layer_adapters import CLA
-from dtn7zero.data import Node
-from dtn7zero.utility import debug, warning
-
-try:
-    import requests
-except ImportError:
-    import urequests as requests
-
-from py_dtn7 import DTNRESTClient, Bundle
-
-from dtn7zero.constants import IPND_IDENTIFIER_REST
-
-
-class Dtn7RsRestCLA(CLA):
-
-    def __init__(self):
-        self.connections: Dict[Node, DTNRESTClient] = {}
-
-    def add_connection(self, node: Node):
-        http_address = 'http://{}'.format(node.address)
-        port = node.clas[IPND_IDENTIFIER_REST]
-        try:
-            # we assume if there is a dtn7rs-like HTTP-API present, then we can proceed
-            dtn7rs_rest_client = DTNRESTClient(host=http_address, port=port)
-        except OSError as e:  # urequests only uses default exceptions
-            warning('could not add node: {}:{} error: {}'.format(http_address, port, e))
-            return
-
-        self.connections[node] = dtn7rs_rest_client
-        node.eid = (1, self.connections[node].node_id)  # todo: remove hardcoded dtn uri scheme assignment
-        debug('added new rest cla connection: {} {}'.format(node.eid, http_address))
-
-    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
-        if bundle_id is None or node is None:
-            return None, None
-
-        if node not in self.connections:
-            return None, None
-
-        try:
-            raw_bundle = self.connections[node].download(bundle_id=bundle_id)
-        except OSError:  # urequests only uses default exceptions
-            del self.connections[node]
-            return None, None
-
-        if raw_bundle == b'Bundle not found':
-            return None, None
-
-        return Bundle.from_cbor(raw_bundle), node.address
-
-    def poll_ids(self, node: Node) -> Optional[List[str]]:
-        if node not in self.connections:
-            # try to establish a new node connection, todo: what to do on repeated failures (slowing the framework down)?
-            self.add_connection(node)
-
-        try:
-            return self.connections[node].bundles
-        except (OSError, ValueError):  # urequests only uses default exceptions
-            del self.connections[node]
-        return None
-
-    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
-        if IPND_IDENTIFIER_REST not in node.clas:
-            return False
-
-        if node not in self.connections:
-            # try to establish a new node connection, todo: what to do on repeated failures (slowing the framework down)?
-            self.add_connection(node)
-
-        try:
-            response = self.connections[node].push(serialized_bundle)
-            if response.status_code != 200:
-                warning('connection {} did not accept our bundle: {} {}'.format(node.address, response.status_code, response.content))
-                return False
-            return True
-        except OSError:  # urequests only uses default exceptions
-            warning('removing bad connection {}'.format(node.address))
-            del self.connections[node]
-        except KeyError:
-            return False
-        return False
+from typing import Dict, List, Optional, Tuple
+
+from dtn7zero.convergence_layer_adapters import CLA
+from dtn7zero.data import Node
+from dtn7zero.utility import debug, warning
+
+try:
+    import requests
+except ImportError:
+    import urequests as requests
+
+from py_dtn7 import DTNRESTClient, Bundle
+
+from dtn7zero.constants import IPND_IDENTIFIER_REST
+
+
+class Dtn7RsRestCLA(CLA):
+
+    def __init__(self):
+        self.connections: Dict[Node, DTNRESTClient] = {}
+
+    def add_connection(self, node: Node):
+        http_address = 'http://{}'.format(node.address)
+        port = node.clas[IPND_IDENTIFIER_REST]
+        try:
+            # we assume if there is a dtn7rs-like HTTP-API present, then we can proceed
+            dtn7rs_rest_client = DTNRESTClient(host=http_address, port=port)
+        except OSError as e:  # urequests only uses default exceptions
+            warning('could not add node: {}:{} error: {}'.format(http_address, port, e))
+            return
+
+        self.connections[node] = dtn7rs_rest_client
+        node.eid = (1, self.connections[node].node_id)  # todo: remove hardcoded dtn uri scheme assignment
+        debug('added new rest cla connection: {} {}'.format(node.eid, http_address))
+
+    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
+        if bundle_id is None or node is None:
+            return None, None
+
+        if node not in self.connections:
+            return None, None
+
+        try:
+            raw_bundle = self.connections[node].download(bundle_id=bundle_id)
+        except OSError:  # urequests only uses default exceptions
+            del self.connections[node]
+            return None, None
+
+        if raw_bundle == b'Bundle not found':
+            return None, None
+
+        return Bundle.from_cbor(raw_bundle), node.address
+
+    def poll_ids(self, node: Node) -> Optional[List[str]]:
+        if node not in self.connections:
+            # try to establish a new node connection, todo: what to do on repeated failures (slowing the framework down)?
+            self.add_connection(node)
+
+        try:
+            return self.connections[node].bundles
+        except (OSError, ValueError):  # urequests only uses default exceptions
+            del self.connections[node]
+        return None
+
+    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
+        if IPND_IDENTIFIER_REST not in node.clas:
+            return False
+
+        if node not in self.connections:
+            # try to establish a new node connection, todo: what to do on repeated failures (slowing the framework down)?
+            self.add_connection(node)
+
+        try:
+            response = self.connections[node].push(serialized_bundle)
+            if response.status_code != 200:
+                warning('connection {} did not accept our bundle: {} {}'.format(node.address, response.status_code, response.content))
+                return False
+            return True
+        except OSError:  # urequests only uses default exceptions
+            warning('removing bad connection {}'.format(node.address))
+            del self.connections[node]
+        except KeyError:
+            return False
+        return False
```

### Comparing `dtn7zero-0.0.4/dtn7zero/convergence_layer_adapters/mtcp.py` & `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/mtcp.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,301 @@
-import socket
-import struct
-from typing import Optional, Dict, List, Tuple
-
-try:
-    from cbor2 import dumps
-except ImportError:
-    from cbor import dumps
-
-from dtn7zero.constants import PORT_MTCP, MTCP_MAX_CONNECTIONS_STATE_WAITING, SOCKET_RECEIVE_BUFFER_SIZE, \
-    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE, \
-    MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND, RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP
-from dtn7zero.convergence_layer_adapters import CLA
-from dtn7zero.data import Node
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout, debug, warning
-from py_dtn7 import Bundle
-
-
-TYPE_BYTES = 0x40
-
-_CBOR_TYPE_MASK = 0xE0
-_CBOR_INFO_BITS = 0x1F
-
-_CBOR_UINT8_FOLLOWS = 24  # 0x18
-_CBOR_UINT16_FOLLOWS = 25  # 0x19
-_CBOR_UINT32_FOLLOWS = 26  # 0x1a
-_CBOR_UINT64_FOLLOWS = 27  # 0x1b
-
-
-class RemoteClosedConnectionException(Exception):
-    pass
-
-
-class RemoteStalledConnectionException(Exception):
-    pass
-
-
-class ReceivedInvalidDataOnSocketException(Exception):
-    pass
-
-
-def _poll_one_byte(connection):
-    try:
-        buf = connection.recv(1)
-    # if a non-blocking read fails we have read everything there is to read at the moment
-    # ,but we need to read exactly n bytes
-    except OSError:
-        return None
-    else:
-        # on 0 bytes received the socket connection is closed
-        # the desired 1 byte could not be received -> incomplete data -> discard
-        if len(buf) == 0:
-            raise RemoteClosedConnectionException()
-
-        return buf
-
-
-def _receive_exactly_n_bytes(connection, num_bytes):
-    result = b''
-
-    while True:
-        try:
-            buf = connection.recv(min(num_bytes, SOCKET_RECEIVE_BUFFER_SIZE))
-        # if a non-blocking read fails we have read everything there is to read at the moment
-        # ,but we need to read exactly n bytes
-        except OSError:
-            pass
-        else:
-            # on 0 bytes received the socket connection is closed
-            # the desired num_bytes could not be received in total -> incomplete data -> discard
-            if len(buf) == 0:
-                raise RemoteClosedConnectionException()
-
-            result += buf
-            num_bytes -= len(buf)
-
-            if num_bytes == 0:
-                return result
-
-
-def _read_full_message_or_none(connection):
-    header = _poll_one_byte(connection)
-
-    if header is None:
-        return None
-
-    header = struct.unpack_from('!B', header, 0)[0]
-
-    tag = header & _CBOR_TYPE_MASK
-    tag_aux = header & _CBOR_INFO_BITS
-
-    if tag != TYPE_BYTES:
-        raise ReceivedInvalidDataOnSocketException('mtcp cla received invalid header: only accepting type byte-string')
-
-    if tag_aux <= 23:
-        aux = tag_aux
-    elif tag_aux == _CBOR_UINT8_FOLLOWS:
-        data = _receive_exactly_n_bytes(connection, 1)
-        aux = struct.unpack_from('!B', data, 0)[0]
-    elif tag_aux == _CBOR_UINT16_FOLLOWS:
-        data = _receive_exactly_n_bytes(connection, 2)
-        aux = struct.unpack_from('!H', data, 0)[0]
-    elif tag_aux == _CBOR_UINT32_FOLLOWS:
-        data = _receive_exactly_n_bytes(connection, 4)
-        aux = struct.unpack_from('!I', data, 0)[0]
-    elif tag_aux == _CBOR_UINT64_FOLLOWS:
-        data = _receive_exactly_n_bytes(connection, 8)
-        aux = struct.unpack_from('!Q', data, 0)[0]
-    else:
-        raise ReceivedInvalidDataOnSocketException('mtcp cla received invalid header: only accepting definite length byte-strings')
-
-    return _receive_exactly_n_bytes(connection, aux)
-
-
-def _send_message(address, port, message):
-    # create a standard ipv4 stream socket
-    client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    client_socket.settimeout(0)
-
-    '''
-    Connection Establishment Analysis
-
-    Problem
-    socket.settimeout(1) -> does not set the desired timeout on MicroPython (ESP32-GENERIC), 
-    but instead keeps the default timeout of about 12 seconds.
-
-    Analysis
-    The following OSError numbers (e.errno) are thrown on MicroPython on connecting with a non-blocking socket:
-    119 EINPROGRESS  -> thrown by the connect request on a non-blocking socket
-     11 EAGAIN       -> thrown if no data could be sent (also thrown on sending b'')
-
-    Solution
-    As we cannot be sure when the socket is connected we just skip the connect timeout and go straight to the deadlock timeout.
-    To be consistent on MicroPython and CPython we do this on both.
-    '''
-
-    try:
-        client_socket.connect((address, port))
-    except OSError:
-        # this will raise an exception on non-blocking sockets
-        pass
-
-    deadlock_check = get_current_clock_millis()
-    while len(message) > 0 and not is_timestamp_older_than_timeout(deadlock_check, MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND):
-        try:
-            bytes_sent = client_socket.send(message)
-        # Windows behaviour??? If other end is forcibly closed it raises an ConnectionResetError -> OSError
-        except OSError:
-            # We ignore all OSErrors.
-            # The correct way would be to check the errno for "busy" (MicroPython -> 11, CPython+Windows -> 10035)
-            # but, because it is implementation dependent, and we do not expect the receiver to immediately close the
-            # connection, we accept the rare case of a deadlock-timeout because of an early-closed socket.
-            pass
-        else:
-            # on 0 bytes sent the socket connection is closed
-            if bytes_sent == 0:
-                client_socket.close()
-                raise RemoteClosedConnectionException("0 bytes")
-            # update the message and length to send
-            message = message[bytes_sent:]
-            # update our deadlock-check as we managed to send some data
-            deadlock_check = get_current_clock_millis()
-
-    if len(message) > 0:
-        client_socket.close()
-        raise RemoteStalledConnectionException()
-
-    client_socket.close()
-
-
-class MTcpCLA(CLA):
-
-    def __init__(self):
-        # a standard ipv4 stream socket
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-
-        # allow immediate rebind to a floating socket (last app crashed or otherwise non fully closed server socket)
-        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        # bind to all interfaces available
-        self.socket.bind(('0.0.0.0', PORT_MTCP))
-        # We will accept a maximum of x connect requests into our connect queue before we are busy
-        # A connection gets out of this queue on socket creation
-        self.socket.listen(MTCP_MAX_CONNECTIONS_STATE_WAITING)
-        # change to non-blocking mode
-        # MicroPython supports only one thread/process, and therefore we need to implement everything synchronous
-        self.socket.settimeout(0)
-
-        self.open_receive_connections: Dict[str, (socket.socket, int)] = {}
-        self.gracefully_shutdown_connections: Dict[str, socket.socket] = {}
-
-    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
-        if bundle_id is not None or node is not None:
-            raise Exception('cannot poll specific bundle from specific node with mtcp cla')
-
-        # check for new incoming connections
-        self._check_for_new_connections()
-
-        # try to receive one bundle
-        serialized_bundle, from_node_address = self._poll_from_open_receive_connections()
-
-        if serialized_bundle is None:
-            serialized_bundle, from_node_address = self._poll_from_gracefully_shutdown_connections()
-
-        if serialized_bundle is None:
-            return None, None
-
-        try:
-            return Bundle.from_cbor(serialized_bundle), from_node_address
-        except Exception as e:
-            warning('error during mtcp bundle deserialization, ignoring bundle. error: {}'.format(e))
-        return None, None
-
-    def _poll_from_open_receive_connections(self):
-        serialized_bundle, from_node_address = None, None
-
-        for address_tuple, (connection, last_received) in tuple(self.open_receive_connections.items()):
-            try:
-                serialized_bundle = _read_full_message_or_none(connection)
-            except RemoteClosedConnectionException:
-                debug('remote closed down incoming mtcp connection {}'.format(address_tuple))
-                if not RUNNING_MICROPYTHON:
-                    connection.shutdown(socket.SHUT_RDWR)
-                connection.close()
-                del self.open_receive_connections[address_tuple]
-            except ReceivedInvalidDataOnSocketException as e:
-                warning('incoming mtcp connection {} sent invalid data, discarding connection, error: {}'.format(address_tuple, e))
-                if not RUNNING_MICROPYTHON:
-                    connection.shutdown(socket.SHUT_RDWR)
-                connection.close()
-                del self.open_receive_connections[address_tuple]
-            else:
-                if serialized_bundle is not None:
-                    from_node_address = address_tuple[0]
-                    self.open_receive_connections[address_tuple] = (connection, get_current_clock_millis())
-                    break
-                elif is_timestamp_older_than_timeout(last_received, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE):
-                    if not RUNNING_MICROPYTHON:
-                        debug('gracefully closing incoming mtcp connection {} due to inactivity timeout'.format(address_tuple))
-                        connection.shutdown(socket.SHUT_WR)
-                        self.gracefully_shutdown_connections[address_tuple] = connection
-                    else:
-                        debug('forcefully closing incoming mtcp connection {} due to inactivity timeout (no shutdown support on micropython)'.format(address_tuple))
-                        connection.close()
-                    del self.open_receive_connections[address_tuple]
-
-        return serialized_bundle, from_node_address
-
-    def _poll_from_gracefully_shutdown_connections(self):
-        serialized_bundle, from_node_address = None, None
-
-        for address_tuple, connection in tuple(self.gracefully_shutdown_connections.items()):
-            try:
-                serialized_bundle = _read_full_message_or_none(connection)
-            except RemoteClosedConnectionException:
-                debug('gracefully shutdown mtcp connection closed by remote {}'.format(address_tuple))
-                connection.close()
-                del self.gracefully_shutdown_connections[address_tuple]
-            except ReceivedInvalidDataOnSocketException as e:
-                debug('gracefully shutdown mtcp connection {} sent invalid data, discarding connection, error: {}'.format(address_tuple, e))
-                connection.close()
-                del self.gracefully_shutdown_connections[address_tuple]
-            else:
-                if serialized_bundle is not None:
-                    from_node_address = address_tuple[0]
-                    break
-
-        return serialized_bundle, from_node_address
-
-    def _check_for_new_connections(self):
-        if len(self.open_receive_connections) < MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
-            try:
-                client_socket, address_tuple = self.socket.accept()
-            except OSError:
-                # no new connect request waiting
-                pass
-            else:
-                # change to non-blocking mode to be able to poll without blocking
-                client_socket.settimeout(0)
-
-                # we allow multiple connections from one IP address, because if we accept the connection, the whole bundle
-                #  could be already transmitted before we can close the connection from our checks
-                #  -> would lead to false positive on the sender side
-                # next best thing: limit number of open-receive-connections
-                # print('new mtcp receive connection opened from address {}'.format(address_tuple))
-                self.open_receive_connections[address_tuple] = (client_socket, get_current_clock_millis())
-
-    def poll_ids(self, node: Node) -> Optional[List[str]]:
-        return None  # we cannot poll ids, and None signals that
-
-    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
-        message = dumps(serialized_bundle)
-
-        if IPND_IDENTIFIER_MTCP in node.clas:
-            try:
-                port = node.clas[IPND_IDENTIFIER_MTCP]
-                _send_message(node.address, port, message)
-            except (RemoteClosedConnectionException, RemoteStalledConnectionException):
-                del node.clas[IPND_IDENTIFIER_MTCP]  # the node can re-announce it, but currently we cannot connect
-                return False
-            return True
-        return False
+import socket
+import struct
+from typing import Optional, Dict, List, Tuple
+
+try:
+    from cbor2 import dumps
+except ImportError:
+    from cbor import dumps
+
+from dtn7zero.constants import PORT_MTCP, MTCP_MAX_CONNECTIONS_STATE_WAITING, SOCKET_RECEIVE_BUFFER_SIZE, \
+    MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE, \
+    MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND, RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP
+from dtn7zero.convergence_layer_adapters import CLA
+from dtn7zero.data import Node
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout, debug, warning
+from py_dtn7 import Bundle
+
+
+TYPE_BYTES = 0x40
+
+_CBOR_TYPE_MASK = 0xE0
+_CBOR_INFO_BITS = 0x1F
+
+_CBOR_UINT8_FOLLOWS = 24  # 0x18
+_CBOR_UINT16_FOLLOWS = 25  # 0x19
+_CBOR_UINT32_FOLLOWS = 26  # 0x1a
+_CBOR_UINT64_FOLLOWS = 27  # 0x1b
+
+
+class RemoteClosedConnectionException(Exception):
+    pass
+
+
+class RemoteStalledConnectionException(Exception):
+    pass
+
+
+class ReceivedInvalidDataOnSocketException(Exception):
+    pass
+
+
+def _poll_one_byte(connection):
+    try:
+        buf = connection.recv(1)
+    # if a non-blocking read fails we have read everything there is to read at the moment
+    # ,but we need to read exactly n bytes
+    except OSError:
+        return None
+    else:
+        # on 0 bytes received the socket connection is closed
+        # the desired 1 byte could not be received -> incomplete data -> discard
+        if len(buf) == 0:
+            raise RemoteClosedConnectionException()
+
+        return buf
+
+
+def _receive_exactly_n_bytes(connection, num_bytes):
+    result = b''
+
+    while True:
+        try:
+            buf = connection.recv(min(num_bytes, SOCKET_RECEIVE_BUFFER_SIZE))
+        # if a non-blocking read fails we have read everything there is to read at the moment
+        # ,but we need to read exactly n bytes
+        except OSError:
+            pass
+        else:
+            # on 0 bytes received the socket connection is closed
+            # the desired num_bytes could not be received in total -> incomplete data -> discard
+            if len(buf) == 0:
+                raise RemoteClosedConnectionException()
+
+            result += buf
+            num_bytes -= len(buf)
+
+            if num_bytes == 0:
+                return result
+
+
+def _read_full_message_or_none(connection):
+    header = _poll_one_byte(connection)
+
+    if header is None:
+        return None
+
+    header = struct.unpack_from('!B', header, 0)[0]
+
+    tag = header & _CBOR_TYPE_MASK
+    tag_aux = header & _CBOR_INFO_BITS
+
+    if tag != TYPE_BYTES:
+        raise ReceivedInvalidDataOnSocketException('mtcp cla received invalid header: only accepting type byte-string')
+
+    if tag_aux <= 23:
+        aux = tag_aux
+    elif tag_aux == _CBOR_UINT8_FOLLOWS:
+        data = _receive_exactly_n_bytes(connection, 1)
+        aux = struct.unpack_from('!B', data, 0)[0]
+    elif tag_aux == _CBOR_UINT16_FOLLOWS:
+        data = _receive_exactly_n_bytes(connection, 2)
+        aux = struct.unpack_from('!H', data, 0)[0]
+    elif tag_aux == _CBOR_UINT32_FOLLOWS:
+        data = _receive_exactly_n_bytes(connection, 4)
+        aux = struct.unpack_from('!I', data, 0)[0]
+    elif tag_aux == _CBOR_UINT64_FOLLOWS:
+        data = _receive_exactly_n_bytes(connection, 8)
+        aux = struct.unpack_from('!Q', data, 0)[0]
+    else:
+        raise ReceivedInvalidDataOnSocketException('mtcp cla received invalid header: only accepting definite length byte-strings')
+
+    return _receive_exactly_n_bytes(connection, aux)
+
+
+def _send_message(address, port, message):
+    # create a standard ipv4 stream socket
+    client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    client_socket.settimeout(0)
+
+    '''
+    Connection Establishment Analysis
+
+    Problem
+    socket.settimeout(1) -> does not set the desired timeout on MicroPython (ESP32-GENERIC), 
+    but instead keeps the default timeout of about 12 seconds.
+
+    Analysis
+    The following OSError numbers (e.errno) are thrown on MicroPython on connecting with a non-blocking socket:
+    119 EINPROGRESS  -> thrown by the connect request on a non-blocking socket
+     11 EAGAIN       -> thrown if no data could be sent (also thrown on sending b'')
+
+    Solution
+    As we cannot be sure when the socket is connected we just skip the connect timeout and go straight to the deadlock timeout.
+    To be consistent on MicroPython and CPython we do this on both.
+    '''
+
+    try:
+        client_socket.connect((address, port))
+    except OSError:
+        # this will raise an exception on non-blocking sockets
+        pass
+
+    deadlock_check = get_current_clock_millis()
+    while len(message) > 0 and not is_timestamp_older_than_timeout(deadlock_check, MTCP_TIMEOUT_MILLISECONDS_STALLED_SEND):
+        try:
+            bytes_sent = client_socket.send(message)
+        # Windows behaviour??? If other end is forcibly closed it raises an ConnectionResetError -> OSError
+        except OSError:
+            # We ignore all OSErrors.
+            # The correct way would be to check the errno for "busy" (MicroPython -> 11, CPython+Windows -> 10035)
+            # but, because it is implementation dependent, and we do not expect the receiver to immediately close the
+            # connection, we accept the rare case of a deadlock-timeout because of an early-closed socket.
+            pass
+        else:
+            # on 0 bytes sent the socket connection is closed
+            if bytes_sent == 0:
+                client_socket.close()
+                raise RemoteClosedConnectionException("0 bytes")
+            # update the message and length to send
+            message = message[bytes_sent:]
+            # update our deadlock-check as we managed to send some data
+            deadlock_check = get_current_clock_millis()
+
+    if len(message) > 0:
+        client_socket.close()
+        raise RemoteStalledConnectionException()
+
+    client_socket.close()
+
+
+class MTcpCLA(CLA):
+
+    def __init__(self):
+        # a standard ipv4 stream socket
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
+        # allow immediate rebind to a floating socket (last app crashed or otherwise non fully closed server socket)
+        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        # bind to all interfaces available
+        self.socket.bind(('0.0.0.0', PORT_MTCP))
+        # We will accept a maximum of x connect requests into our connect queue before we are busy
+        # A connection gets out of this queue on socket creation
+        self.socket.listen(MTCP_MAX_CONNECTIONS_STATE_WAITING)
+        # change to non-blocking mode
+        # MicroPython supports only one thread/process, and therefore we need to implement everything synchronous
+        self.socket.settimeout(0)
+
+        self.open_receive_connections: Dict[str, (socket.socket, int)] = {}
+        self.gracefully_shutdown_connections: Dict[str, socket.socket] = {}
+
+    def poll(self, bundle_id: str = None, node: Node = None) -> Tuple[Optional[Bundle], Optional[str]]:
+        if bundle_id is not None or node is not None:
+            raise Exception('cannot poll specific bundle from specific node with mtcp cla')
+
+        # check for new incoming connections
+        self._check_for_new_connections()
+
+        # try to receive one bundle
+        serialized_bundle, from_node_address = self._poll_from_open_receive_connections()
+
+        if serialized_bundle is None:
+            serialized_bundle, from_node_address = self._poll_from_gracefully_shutdown_connections()
+
+        if serialized_bundle is None:
+            return None, None
+
+        try:
+            return Bundle.from_cbor(serialized_bundle), from_node_address
+        except Exception as e:
+            warning('error during mtcp bundle deserialization, ignoring bundle. error: {}'.format(e))
+        return None, None
+
+    def _poll_from_open_receive_connections(self):
+        serialized_bundle, from_node_address = None, None
+
+        for address_tuple, (connection, last_received) in tuple(self.open_receive_connections.items()):
+            try:
+                serialized_bundle = _read_full_message_or_none(connection)
+            except RemoteClosedConnectionException:
+                debug('remote closed down incoming mtcp connection {}'.format(address_tuple))
+                if not RUNNING_MICROPYTHON:
+                    connection.shutdown(socket.SHUT_RDWR)
+                connection.close()
+                del self.open_receive_connections[address_tuple]
+            except ReceivedInvalidDataOnSocketException as e:
+                warning('incoming mtcp connection {} sent invalid data, discarding connection, error: {}'.format(address_tuple, e))
+                if not RUNNING_MICROPYTHON:
+                    connection.shutdown(socket.SHUT_RDWR)
+                connection.close()
+                del self.open_receive_connections[address_tuple]
+            else:
+                if serialized_bundle is not None:
+                    from_node_address = address_tuple[0]
+                    self.open_receive_connections[address_tuple] = (connection, get_current_clock_millis())
+                    break
+                elif is_timestamp_older_than_timeout(last_received, MTCP_TIMEOUT_MILLISECONDS_INACTIVE_RECEIVE):
+                    if not RUNNING_MICROPYTHON:
+                        debug('gracefully closing incoming mtcp connection {} due to inactivity timeout'.format(address_tuple))
+                        connection.shutdown(socket.SHUT_WR)
+                        self.gracefully_shutdown_connections[address_tuple] = connection
+                    else:
+                        debug('forcefully closing incoming mtcp connection {} due to inactivity timeout (no shutdown support on micropython)'.format(address_tuple))
+                        connection.close()
+                    del self.open_receive_connections[address_tuple]
+
+        return serialized_bundle, from_node_address
+
+    def _poll_from_gracefully_shutdown_connections(self):
+        serialized_bundle, from_node_address = None, None
+
+        for address_tuple, connection in tuple(self.gracefully_shutdown_connections.items()):
+            try:
+                serialized_bundle = _read_full_message_or_none(connection)
+            except RemoteClosedConnectionException:
+                debug('gracefully shutdown mtcp connection closed by remote {}'.format(address_tuple))
+                connection.close()
+                del self.gracefully_shutdown_connections[address_tuple]
+            except ReceivedInvalidDataOnSocketException as e:
+                debug('gracefully shutdown mtcp connection {} sent invalid data, discarding connection, error: {}'.format(address_tuple, e))
+                connection.close()
+                del self.gracefully_shutdown_connections[address_tuple]
+            else:
+                if serialized_bundle is not None:
+                    from_node_address = address_tuple[0]
+                    break
+
+        return serialized_bundle, from_node_address
+
+    def _check_for_new_connections(self):
+        if len(self.open_receive_connections) < MTCP_MAX_CONNECTIONS_STATE_OPEN_RECEIVE:
+            try:
+                client_socket, address_tuple = self.socket.accept()
+            except OSError:
+                # no new connect request waiting
+                pass
+            else:
+                # change to non-blocking mode to be able to poll without blocking
+                client_socket.settimeout(0)
+
+                # we allow multiple connections from one IP address, because if we accept the connection, the whole bundle
+                #  could be already transmitted before we can close the connection from our checks
+                #  -> would lead to false positive on the sender side
+                # next best thing: limit number of open-receive-connections
+                # print('new mtcp receive connection opened from address {}'.format(address_tuple))
+                self.open_receive_connections[address_tuple] = (client_socket, get_current_clock_millis())
+
+    def poll_ids(self, node: Node) -> Optional[List[str]]:
+        return None  # we cannot poll ids, and None signals that
+
+    def send_to(self, node: Node, serialized_bundle: bytes) -> bool:
+        message = dumps(serialized_bundle)
+
+        if IPND_IDENTIFIER_MTCP in node.clas:
+            try:
+                port = node.clas[IPND_IDENTIFIER_MTCP]
+                _send_message(node.address, port, message)
+            except (RemoteClosedConnectionException, RemoteStalledConnectionException):
+                del node.clas[IPND_IDENTIFIER_MTCP]  # the node can re-announce it, but currently we cannot connect
+                return False
+            return True
+        return False
```

### Comparing `dtn7zero-0.0.4/dtn7zero/data.py` & `dtn7zero-0.0.5/dtn7zero/data.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from typing import List, Tuple, Dict
-
-from dtn7zero.utility import get_current_clock_millis
-from py_dtn7 import Bundle
-
-
-class BundleStatusReportReasonCodes:
-    """
-    RFC 9171, 9.5 Bundle Status Report Reason Codes
-    """
-    NO_ADDITIONAL_INFORMATION = 0
-    LIFETIME_EXPIRED = 1
-    FORWARDED_OVER_UNIDIRECTIONAL_LINK = 2
-    TRANSMISSION_CANCELED = 3
-    DEPLETED_STORAGE = 4
-    DESTINATION_ENDPOINT_ID_UNAVAILABLE = 5
-    NO_KNOWN_ROUTE_TO_DESTINATION_FROM_HERE = 6
-    NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE = 7
-    BLOCK_UNINTELLIGIBLE = 8
-    HOP_LIMIT_EXCEEDED = 9
-    TRAFFIC_PARED = 10
-    BLOCK_UNSUPPORTED = 11
-
-
-class Node:
-
-    def __init__(self, address: str, eid: Tuple[int, str], clas: Dict[str, int], sequence_number: int):
-        self.address = address  # the IP address of the node
-        # todo: currently a node is identified by its IP address, maybe this requires changes sometime in the future.
-        # storage also depends on the address field as the unique identifier of a node
-
-        self.eid = eid  # DTN node id, a tuple of "address-type" (1 or 2) and "the node-id" in the correct format -> for type 1 (DTN) -> example: "//node1/"
-        self.clas = clas  # a list of tuples, consisting of the ipnd-cla-identifier + application port
-        self.sequence_number = sequence_number
-
-        self.latest_discovery = get_current_clock_millis()
-
-    def merge_new_info(self, eid_scheme: int, eid_specific_part: str, clas: Dict[str, int]):
-        if eid_specific_part is not None:
-            self.eid = (eid_scheme, eid_specific_part)
-        self.clas = clas  # replace with new information -> clas might have gotten deactivated
-
-        self.latest_discovery = get_current_clock_millis()
-
-    def advance_sequence_number(self, new_sequence_number: int) -> bool:
-        old_sequence_number = self.sequence_number
-        self.sequence_number = new_sequence_number
-        return old_sequence_number + 1 == new_sequence_number
-
-
-class BundleInformation:
-    RETENTION_CONSTRAINT_DISPATCH_PENDING = 'Dispatch pending'
-    RETENTION_CONSTRAINT_FORWARD_PENDING = 'Forward pending'
-
-    def __init__(self, bundle: Bundle):
-        self.bundle = bundle
-        self.retention_constraint = None
-        self.locally_delivered = False
-        self.received_at_ms = get_current_clock_millis()
-        self.forwarded_to_nodes: List[Node] = []
+from typing import List, Tuple, Dict
+
+from dtn7zero.utility import get_current_clock_millis
+from py_dtn7 import Bundle
+
+
+class BundleStatusReportReasonCodes:
+    """
+    RFC 9171, 9.5 Bundle Status Report Reason Codes
+    """
+    NO_ADDITIONAL_INFORMATION = 0
+    LIFETIME_EXPIRED = 1
+    FORWARDED_OVER_UNIDIRECTIONAL_LINK = 2
+    TRANSMISSION_CANCELED = 3
+    DEPLETED_STORAGE = 4
+    DESTINATION_ENDPOINT_ID_UNAVAILABLE = 5
+    NO_KNOWN_ROUTE_TO_DESTINATION_FROM_HERE = 6
+    NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE = 7
+    BLOCK_UNINTELLIGIBLE = 8
+    HOP_LIMIT_EXCEEDED = 9
+    TRAFFIC_PARED = 10
+    BLOCK_UNSUPPORTED = 11
+
+
+class Node:
+
+    def __init__(self, address: str, eid: Tuple[int, str], clas: Dict[str, int], sequence_number: int):
+        self.address = address  # the IP address of the node
+        # todo: currently a node is identified by its IP address, maybe this requires changes sometime in the future.
+        # storage also depends on the address field as the unique identifier of a node
+
+        self.eid = eid  # DTN node id, a tuple of "address-type" (1 or 2) and "the node-id" in the correct format -> for type 1 (DTN) -> example: "//node1/"
+        self.clas = clas  # a list of tuples, consisting of the ipnd-cla-identifier + application port
+        self.sequence_number = sequence_number
+
+        self.latest_discovery = get_current_clock_millis()
+
+    def merge_new_info(self, eid_scheme: int, eid_specific_part: str, clas: Dict[str, int]):
+        if eid_specific_part is not None:
+            self.eid = (eid_scheme, eid_specific_part)
+        self.clas = clas  # replace with new information -> clas might have gotten deactivated
+
+        self.latest_discovery = get_current_clock_millis()
+
+    def advance_sequence_number(self, new_sequence_number: int) -> bool:
+        old_sequence_number = self.sequence_number
+        self.sequence_number = new_sequence_number
+        return old_sequence_number + 1 == new_sequence_number
+
+
+class BundleInformation:
+    RETENTION_CONSTRAINT_DISPATCH_PENDING = 'Dispatch pending'
+    RETENTION_CONSTRAINT_FORWARD_PENDING = 'Forward pending'
+
+    def __init__(self, bundle: Bundle):
+        self.bundle = bundle
+        self.retention_constraint = None
+        self.locally_delivered = False
+        self.received_at_ms = get_current_clock_millis()
+        self.forwarded_to_nodes: List[Node] = []
```

### Comparing `dtn7zero-0.0.4/dtn7zero/endpoints.py` & `dtn7zero-0.0.5/dtn7zero/endpoints.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-from typing import Callable
-
-from dtn7zero.constants import RUNNING_MICROPYTHON, PORT_REST
-from dtn7zero.data import BundleInformation
-from dtn7zero.utility import debug
-from py_dtn7 import Bundle, DTNRESTClient, to_dtn_timestamp
-from py_dtn7.bundle import BundleProcessingControlFlags, PrimaryBlock, HopCountBlock, PayloadBlock, BundleAgeBlock, \
-    NONE_ENDPOINT_SPECIFIC_PART_NAME, URI_SCHEME_DTN_NAME
-
-
-class _LocalEndpoint:
-
-    def __init__(self, receive_callback: Callable[[Bundle], None] = None):
-        self.bpa = None
-        self.receive_callback = receive_callback
-
-        if receive_callback is None:
-            self.bundle_buffer: list[Bundle] = []
-
-    def bpa_local_bundle_delivery(self, bundle: Bundle):
-        if self.receive_callback is None:
-            self.bundle_buffer.append(bundle)
-        else:
-            self.receive_callback(bundle)
-
-    def bpa_register(self, bpa):
-        self.bpa = bpa
-
-    def bpa_unregister(self):
-        self.bpa = None
-
-    def poll(self):
-        if self.receive_callback is not None:
-            raise Exception('cannot poll active endpoint with callback {}'.format(self.full_endpoint_uri))
-        if not self.bundle_buffer:
-            return None
-        return self.bundle_buffer.pop(0)
-
-    @property
-    def full_endpoint_uri(self) -> str:
-        return 'dtn://none'
-
-
-class LocalEndpoint(_LocalEndpoint):
-    def __init__(self, endpoint_identifier: str, receive_callback: Callable[[Bundle], None] = None):
-        """ The LocalEndpoint is the entry-point for the application to send/receive bundles.
-
-        endpoint_identifier examples:
-            dtn addressing scheme -> "echo", "echo/subecho"
-            ipn addressing scheme -> "12", "24.15.16"
-
-        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
-        """
-        super().__init__(receive_callback)
-
-        self.endpoint_identifier = endpoint_identifier
-
-        self.last_bundle_creation_time = 0
-        self.last_sequence_number = 0
-
-    @property
-    def full_endpoint_uri(self) -> str:
-        if self.bpa.full_node_uri.startswith(URI_SCHEME_DTN_NAME):
-            return '{}{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
-        elif not self.endpoint_identifier:
-            return self.bpa.full_node_uri  # special case -> ipn addressing + '' empty endpoint (direct node endpoint)
-        else:
-            return '{}.{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
-
-    def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000, anonymous=False) -> str:
-        if self.bpa is None:
-            raise Exception('cannot start transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
-
-        bundle_processing_control_flags = BundleProcessingControlFlags(0)
-        bundle_processing_control_flags.set_flag(2)  # do not fragment bundle
-
-        bundle_age_block = None
-
-        if RUNNING_MICROPYTHON:
-            self.last_sequence_number += 1
-
-            bundle_age_block = BundleAgeBlock.from_objects()
-        else:
-            current_time = to_dtn_timestamp()
-            if current_time == self.last_bundle_creation_time:
-                self.last_sequence_number += 1
-            else:
-                self.last_bundle_creation_time = current_time
-                self.last_sequence_number = 0
-
-        if full_destination_uri.startswith(URI_SCHEME_DTN_NAME):
-            anonymous_uri = 'dtn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
-        else:
-            anonymous_uri = 'ipn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
-
-        primary_block = PrimaryBlock.from_objects(
-            full_destination_uri=full_destination_uri,
-            full_source_uri=anonymous_uri if anonymous else self.full_endpoint_uri,
-            full_report_to_uri=anonymous_uri if anonymous else self.bpa.full_node_uri,
-            bundle_processing_control_flags=bundle_processing_control_flags,
-            bundle_creation_time=self.last_bundle_creation_time,
-            sequence_number=self.last_sequence_number,
-            lifetime=lifetime
-        )
-
-        hop_count_block = HopCountBlock.from_objects(hop_limit=32, hop_count=0)
-
-        payload_block = PayloadBlock.from_objects(data=payload)
-
-        bundle = Bundle(
-            primary_block=primary_block,
-            bundle_age_block=bundle_age_block,
-            hop_count_block=hop_count_block,
-            payload_block=payload_block
-        )
-
-        debug('starting transmission of bundle: {}'.format(bundle.bundle_id))
-
-        self.bpa.local_bundle_dispatch_queue.append(BundleInformation(bundle))
-
-        return bundle.bundle_id
-
-    def cancel_transmission(self, bundle_id: str) -> bool:
-        if self.bpa is None:
-            raise Exception('cannot cancel transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
-
-        return self.bpa.cancel_transmission(bundle_id)
-
-
-class LocalGroupEndpoint(_LocalEndpoint):
-
-    def __init__(self, full_group_uri: str, receive_callback: Callable[[Bundle], None] = None):
-        """ The LocalGroupEndpoint can be used to receive bundles which are addressed to groups.
-
-        full_group_uri examples:
-            "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
-
-        Like the with unicast-endpoint (LocalEndpoint), an uri is matched in full.
-        There is no subgroup matching functionality.
-
-        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
-        """
-        super().__init__(receive_callback)
-
-        self.full_group_uri = full_group_uri
-
-    @property
-    def full_endpoint_uri(self) -> str:
-        return self.full_group_uri
-
-
-class ExternalEndpoint:
-
-    def __init__(self, dtn7rs_ip: str, endpoint_identifier: str):
-        """
-        This is a relic of a time when we could not generate bundles on our own.
-
-        It is functional and encapsulated, meaning it requires no other dtn7zero dependencies to operate.
-        """
-        self.endpoint_identifier = endpoint_identifier
-
-        self.dtn_rest_client: DTNRESTClient = DTNRESTClient('http://{}'.format(dtn7rs_ip), PORT_REST)
-
-        self.dtn_rest_client.register(self.endpoint_identifier)
-
-    def __del__(self):
-        self.dtn_rest_client.unregister(self.endpoint_identifier)
-
-    @property
-    def full_endpoint_address(self):
-        return '//{}/{}'.format(self.dtn_rest_client.node_id, self.endpoint_identifier)
-
-    def poll(self):
-        raw_bundle = self.dtn_rest_client.fetch_endpoint(self.endpoint_identifier)
-
-        if b'Nothing to receive' == raw_bundle:
-            return None
-        else:
-            return Bundle.from_cbor(raw_bundle)
-
-    def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000) -> str:
-        if self.dtn_rest_client is None:
-            raise Exception('cannot start transmission on unregistered RemoteEndpoint {}'.format(self.endpoint_identifier))
-
-        response = self.dtn_rest_client.send(payload=payload, destination=full_destination_uri, lifetime=lifetime)
-
-        if response.status_code != 200:
-            raise Exception('error occurred on generating a bundle on RemoteEndpoint {}'.format(self.full_endpoint_address))
-
-        return ''  # currently we do not get the bundle-id of the generated bundle from the remote :(
+from typing import Callable
+
+from dtn7zero.constants import RUNNING_MICROPYTHON, PORT_REST
+from dtn7zero.data import BundleInformation
+from dtn7zero.utility import debug
+from py_dtn7 import Bundle, DTNRESTClient, to_dtn_timestamp
+from py_dtn7.bundle import BundleProcessingControlFlags, PrimaryBlock, HopCountBlock, PayloadBlock, BundleAgeBlock, \
+    NONE_ENDPOINT_SPECIFIC_PART_NAME, URI_SCHEME_DTN_NAME
+
+
+class _LocalEndpoint:
+
+    def __init__(self, receive_callback: Callable[[Bundle], None] = None):
+        self.bpa = None
+        self.receive_callback = receive_callback
+
+        if receive_callback is None:
+            self.bundle_buffer: list[Bundle] = []
+
+    def bpa_local_bundle_delivery(self, bundle: Bundle):
+        if self.receive_callback is None:
+            self.bundle_buffer.append(bundle)
+        else:
+            self.receive_callback(bundle)
+
+    def bpa_register(self, bpa):
+        self.bpa = bpa
+
+    def bpa_unregister(self):
+        self.bpa = None
+
+    def poll(self):
+        if self.receive_callback is not None:
+            raise Exception('cannot poll active endpoint with callback {}'.format(self.full_endpoint_uri))
+        if not self.bundle_buffer:
+            return None
+        return self.bundle_buffer.pop(0)
+
+    @property
+    def full_endpoint_uri(self) -> str:
+        return 'dtn://none'
+
+
+class LocalEndpoint(_LocalEndpoint):
+    def __init__(self, endpoint_identifier: str, receive_callback: Callable[[Bundle], None] = None):
+        """ The LocalEndpoint is the entry-point for the application to send/receive bundles.
+
+        endpoint_identifier examples:
+            dtn addressing scheme -> "echo", "echo/subecho"
+            ipn addressing scheme -> "12", "24.15.16"
+
+        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
+        """
+        super().__init__(receive_callback)
+
+        self.endpoint_identifier = endpoint_identifier
+
+        self.last_bundle_creation_time = 0
+        self.last_sequence_number = 0
+
+    @property
+    def full_endpoint_uri(self) -> str:
+        if self.bpa.full_node_uri.startswith(URI_SCHEME_DTN_NAME):
+            return '{}{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
+        elif not self.endpoint_identifier:
+            return self.bpa.full_node_uri  # special case -> ipn addressing + '' empty endpoint (direct node endpoint)
+        else:
+            return '{}.{}'.format(self.bpa.full_node_uri, self.endpoint_identifier)
+
+    def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000, anonymous=False) -> str:
+        if self.bpa is None:
+            raise Exception('cannot start transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
+
+        bundle_processing_control_flags = BundleProcessingControlFlags(0)
+        bundle_processing_control_flags.set_flag(2)  # do not fragment bundle
+
+        bundle_age_block = None
+
+        if RUNNING_MICROPYTHON:
+            self.last_sequence_number += 1
+
+            bundle_age_block = BundleAgeBlock.from_objects()
+        else:
+            current_time = to_dtn_timestamp()
+            if current_time == self.last_bundle_creation_time:
+                self.last_sequence_number += 1
+            else:
+                self.last_bundle_creation_time = current_time
+                self.last_sequence_number = 0
+
+        if full_destination_uri.startswith(URI_SCHEME_DTN_NAME):
+            anonymous_uri = 'dtn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
+        else:
+            anonymous_uri = 'ipn:{}'.format(NONE_ENDPOINT_SPECIFIC_PART_NAME)
+
+        primary_block = PrimaryBlock.from_objects(
+            full_destination_uri=full_destination_uri,
+            full_source_uri=anonymous_uri if anonymous else self.full_endpoint_uri,
+            full_report_to_uri=anonymous_uri if anonymous else self.bpa.full_node_uri,
+            bundle_processing_control_flags=bundle_processing_control_flags,
+            bundle_creation_time=self.last_bundle_creation_time,
+            sequence_number=self.last_sequence_number,
+            lifetime=lifetime
+        )
+
+        hop_count_block = HopCountBlock.from_objects(hop_limit=32, hop_count=0)
+
+        payload_block = PayloadBlock.from_objects(data=payload)
+
+        bundle = Bundle(
+            primary_block=primary_block,
+            bundle_age_block=bundle_age_block,
+            hop_count_block=hop_count_block,
+            payload_block=payload_block
+        )
+
+        debug('starting transmission of bundle: {}'.format(bundle.bundle_id))
+
+        self.bpa.local_bundle_dispatch_queue.append(BundleInformation(bundle))
+
+        return bundle.bundle_id
+
+    def cancel_transmission(self, bundle_id: str) -> bool:
+        if self.bpa is None:
+            raise Exception('cannot cancel transmission on unregistered LocalEndpoint {}'.format(self.endpoint_identifier))
+
+        return self.bpa.cancel_transmission(bundle_id)
+
+
+class LocalGroupEndpoint(_LocalEndpoint):
+
+    def __init__(self, full_group_uri: str, receive_callback: Callable[[Bundle], None] = None):
+        """ The LocalGroupEndpoint can be used to receive bundles which are addressed to groups.
+
+        full_group_uri examples:
+            "dtn://news/~sport", "dtn://my-group/interesting/new/~topics"
+
+        Like the with unicast-endpoint (LocalEndpoint), an uri is matched in full.
+        There is no subgroup matching functionality.
+
+        receive_callback may be None, but then the endpoint should be regularly polled for new bundles.
+        """
+        super().__init__(receive_callback)
+
+        self.full_group_uri = full_group_uri
+
+    @property
+    def full_endpoint_uri(self) -> str:
+        return self.full_group_uri
+
+
+class ExternalEndpoint:
+
+    def __init__(self, dtn7rs_ip: str, endpoint_identifier: str):
+        """
+        This is a relic of a time when we could not generate bundles on our own.
+
+        It is functional and encapsulated, meaning it requires no other dtn7zero dependencies to operate.
+        """
+        self.endpoint_identifier = endpoint_identifier
+
+        self.dtn_rest_client: DTNRESTClient = DTNRESTClient('http://{}'.format(dtn7rs_ip), PORT_REST)
+
+        self.dtn_rest_client.register(self.endpoint_identifier)
+
+    def __del__(self):
+        self.dtn_rest_client.unregister(self.endpoint_identifier)
+
+    @property
+    def full_endpoint_address(self):
+        return '//{}/{}'.format(self.dtn_rest_client.node_id, self.endpoint_identifier)
+
+    def poll(self):
+        raw_bundle = self.dtn_rest_client.fetch_endpoint(self.endpoint_identifier)
+
+        if b'Nothing to receive' == raw_bundle:
+            return None
+        else:
+            return Bundle.from_cbor(raw_bundle)
+
+    def start_transmission(self, payload: bytes, full_destination_uri: str, lifetime: int = 3600 * 24 * 1000) -> str:
+        if self.dtn_rest_client is None:
+            raise Exception('cannot start transmission on unregistered RemoteEndpoint {}'.format(self.endpoint_identifier))
+
+        response = self.dtn_rest_client.send(payload=payload, destination=full_destination_uri, lifetime=lifetime)
+
+        if response.status_code != 200:
+            raise Exception('error occurred on generating a bundle on RemoteEndpoint {}'.format(self.full_endpoint_address))
+
+        return ''  # currently we do not get the bundle-id of the generated bundle from the remote :(
```

### Comparing `dtn7zero-0.0.4/dtn7zero/ipnd.py` & `dtn7zero-0.0.5/dtn7zero/ipnd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,287 +1,295 @@
-import socket
-from typing import Tuple, Optional, List, Dict
-
-from dtn7zero.constants import RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP, PORT_MTCP, PORT_IPND, IPND_SEND_INTERVAL_MILLISECONDS, IPND_BEACON_MAX_SIZE
-from dtn7zero.data import Node
-from dtn7zero.storage import Storage
-from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning
-from py_dtn7.bundle import Flags
-
-if RUNNING_MICROPYTHON:
-    import wlan
-else:
-    import netifaces
-
-try:
-    from cbor2 import dumps, loads
-except ImportError:
-    from cbor import dumps, loads
-
-
-class BeaconFlags(Flags):
-
-    @property
-    def eid_present(self) -> bool:
-        """
-        :return: True if the source endpoint identifier is present in this beacon
-        """
-        return self.get_flag(0)
-
-    @property
-    def service_block_present(self) -> bool:
-        """
-        :return: True if the service block is present in this beacon
-        """
-        return self.get_flag(1)
-
-    @property
-    def beacon_period_present(self) -> bool:
-        """
-        :return: True if the service block is present in this beacon
-        """
-        return self.get_flag(2)
-
-    @property
-    def reserved_3_to_7(self) -> int:
-        """
-        :return: shift to zero of bits 3 to 7 that are reserved for future use
-        """
-        return (self.flags >> 3) & 3
-
-
-class Beacon:
-
-    def __init__(
-            self,
-            version: int,
-            beacon_flags: BeaconFlags,
-            eid_scheme: Optional[int],
-            eid_specific_part: Optional[str],
-            beacon_sequence_number: int,
-            service_block: Tuple[List[Tuple[str, int]], Dict[int, bytes]],
-            beacon_period: Optional[int]
-    ):
-        self.version: int = version
-        self.beacon_flags: BeaconFlags = beacon_flags
-        self.eid_scheme: Optional[int] = eid_scheme
-        self.eid_specific_part: Optional[str] = eid_specific_part
-        self.beacon_sequence_number: int = beacon_sequence_number
-        self.service_block: Tuple[List[Tuple[str, int]], Dict[int, bytes]] = service_block
-        self.beacon_period: Optional[int] = beacon_period
-
-        if version != 7:
-            raise NotImplementedError('beacons with other versions than 7 are currently not supported')
-
-        assert not beacon_flags.eid_present or eid_scheme is not None and eid_specific_part is not None
-        assert not beacon_flags.service_block_present or service_block is not None
-        assert not beacon_flags.beacon_period_present or beacon_period is not None
-
-    def __repr__(self) -> str:
-        return '<Beacon: {}]>'.format(self.to_block_data())
-
-    @staticmethod
-    def from_block_data(beacon: list):
-        version = beacon[0]
-        beacon_flags = BeaconFlags(beacon[1])
-        beacon_sequence_number = None
-        eid_scheme = None
-        eid_specific_part = None
-        service_block = ([], {})
-        beacon_period = None
-
-        expected_length = 3 + int(beacon_flags.eid_present) + int(beacon_flags.service_block_present) + int(beacon_flags.beacon_period_present)
-        if len(beacon) != expected_length:
-            raise IndexError('cannot decode beacon because actual length {} differs from length, suggested by flags {}. block data: {}'.format(len(beacon), expected_length, beacon))
-
-        # there are some uncertainties I want to circumvent with this approach:
-        #  1. the EID and Beacon Sequence Number might be switched in position (indexes 2 and 3)
-        #     (ipnd-thesis describes EID at index 3, while dtn7rs places EID at index 2)
-        #  2. EID, Service Block, and Beacon Period might be omitted
-        #     (ipdn-thesis describes to omit empty fields, which can place later items at earlier indexes)
-        for item in beacon[2:]:
-            if isinstance(item, int):
-                if beacon_sequence_number is None:  # Beacon Sequence Number is set first (in accordance with beacon order)
-                    beacon_sequence_number = item
-                elif beacon_flags.beacon_period_present:  # Beacon Period is set second (skips unknown integer field if flag is not set)
-                    beacon_period = item
-            elif isinstance(item, list):
-                if eid_scheme is None and beacon_flags.eid_present:  # EID is set first (if flag is set)
-                    eid_scheme, eid_specific_part = item
-                elif beacon_flags.service_block_present:  # Service Block is set second (if flag is set)
-                    service_block = item
-
-        return Beacon(version, beacon_flags, eid_scheme, eid_specific_part, beacon_sequence_number, service_block, beacon_period)
-
-    def to_block_data(self):
-        block = [self.version, self.beacon_flags.flags]
-
-        # order is inspired by the dtn7rs implementation and not the ipnd-thesis (EID and Beacon Sequence Number switched)
-        if self.beacon_flags.eid_present:
-            block.append((self.eid_scheme, self.eid_specific_part))
-        block.append(self.beacon_sequence_number)
-        if self.beacon_flags.service_block_present:
-            block.append(self.service_block)
-        if self.beacon_flags.beacon_period_present:
-            block.append(self.beacon_period)
-
-        return block
-
-    def to_cbor(self) -> bytes:
-        # although bundles must be an infinite array, nothing is specified here, so keep the finite array
-        return dumps(self.to_block_data())
-
-    @staticmethod
-    def from_objects(
-            beacon_sequence_number: int,
-            eid_scheme: Optional[int] = None,
-            eid_specific_part: Optional[str] = None,
-            service_block: Optional[Tuple[List[Tuple[str, int]], Dict[int, bytes]]] = None,
-            beacon_period: Optional[int] = None
-    ):
-        beacon_flags = BeaconFlags()
-
-        if bool(eid_scheme) != bool(eid_specific_part):
-            raise IndexError('EID must be complete, got: {}, {}'.format(eid_scheme, eid_specific_part))
-        if eid_scheme is not None:
-            beacon_flags.set_flag(0)
-        if service_block is not None:
-            beacon_flags.set_flag(1)
-        else:
-            service_block = ([], {})
-        if beacon_period is not None:
-            beacon_flags.set_flag(2)
-
-        return Beacon(7, beacon_flags, eid_scheme, eid_specific_part, beacon_sequence_number, service_block, beacon_period)
-
-    @staticmethod
-    def from_cbor(data: bytes):
-        return Beacon.from_block_data(loads(data))
-
-    def increment_beacon_sequence_number_by_one(self):
-        # ipnd-thesis states to use an unsigned 32bit integer and wrap around on overflow
-        self.beacon_sequence_number = (self.beacon_sequence_number + 1) & 0xffffffff
-
-    def is_continuous_with_old_beacon_sequence_number(self, old_beacon_sequence_number: int):
-        if old_beacon_sequence_number == 0xffffffff:
-            return self.beacon_sequence_number == 0
-        return self.beacon_sequence_number == old_beacon_sequence_number
-
-
-class IPND:
-
-    """
-    for now, we only support broadcast on all interfaces and IPv4 only.
-    todo: extend functionality to filter network interfaces and support IPv6
-    todo: extend functionality to delete nodes after a beacon timeout
-    """
-    def __init__(self, eid_scheme: int, eid_specific_part: str, storage: Storage):
-        self.storage = storage
-
-        # todo: check dynamically for new networks -> also test with changing networks
-        if RUNNING_MICROPYTHON:
-            self.broadcast_addresses, self.own_addresses = IPND.get_micropython_ipv4_broadcast_addresses()
-        else:
-            self.broadcast_addresses, self.own_addresses = IPND.get_cpython_ipv4_broadcast_addresses()
-
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-
-        if not RUNNING_MICROPYTHON:
-            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.sock.settimeout(0)
-
-        self.sock.bind(('', 3003))
-
-        # self.own_beacon = create_minimal_output_beacon(eid_scheme, eid_specific_part)
-        self.own_beacon = Beacon.from_objects(
-            beacon_sequence_number=0,
-            eid_scheme=eid_scheme,
-            eid_specific_part=eid_specific_part,
-            service_block=([(IPND_IDENTIFIER_MTCP, PORT_MTCP)], {})  # todo: extend for all and active clas'
-        )
-
-        self.last_beacon_broadcast = 0
-
-    def update(self):
-        try:
-            # todo: for now it seems one full datagram is returned here, as long as the datagram is smaller than bytes-trying-to-receive
-            raw_data, (address, port) = self.sock.recvfrom(IPND_BEACON_MAX_SIZE)
-        except OSError:
-            pass
-        except MemoryError:
-            warning('MEMORY ERROR DURING BEACON RECEIVE, PASS')
-        else:
-            try:
-                # eid_scheme, eid_specific_part, clas, services = extract_beacon_information_from(raw_data)
-                beacon = Beacon.from_cbor(raw_data)
-            except Exception as e:
-                warning('could not decode beacon. error: {}'.format(e))
-            else:
-                if address not in self.own_addresses:
-                    existing_node = self.storage.get_node(address)
-
-                    if existing_node is None:
-                        debug('received beacon from new node: {}, size: {}'.format(address, len(raw_data)))
-
-                        new_node = Node(address, (beacon.eid_scheme, beacon.eid_specific_part), dict(beacon.service_block[0]), beacon.beacon_sequence_number)
-                        self.storage.add_node(new_node)
-
-                        sequence_number_matches = False
-                    else:
-                        debug('received beacon from known node: {}, size: {}'.format(address, len(raw_data)))
-                        # existing_node.merge_new_info(eid_scheme, eid_specific_part, dict(clas))
-                        existing_node.merge_new_info(beacon.eid_scheme, beacon.eid_specific_part, dict(beacon.service_block[0]))
-
-                        sequence_number_matches = existing_node.advance_sequence_number(beacon.beacon_sequence_number)
-
-                    if not sequence_number_matches:
-                        # send back a uni-cast beacon to a previously unknown node for faster knowledge spread
-                        # ideal case: it never received a beacon from us -> current state (sequence number) is new to the node
-                        # not ideal case: beacons were exchanged concurrently -> state (sequence number) is duplicate, which is unspecified and ideally ignored
-                        # dtn7zero specific detail: we add unicast information to the beacon, so there is no second unicast beacon sent back to us
-
-                        if not (42 in beacon.service_block[1] and beacon.service_block[1][42] == b'unicast'):
-                            self.own_beacon.service_block[1][42] = b'unicast'
-                            self.send_own_beacon_to(address)
-                            del self.own_beacon.service_block[1][42]
-
-        if is_timestamp_older_than_timeout(self.last_beacon_broadcast, IPND_SEND_INTERVAL_MILLISECONDS):
-            for address in self.broadcast_addresses:
-                self.send_own_beacon_to(address)
-            # minimal_output_beacon_increase_counter_by_one(self.own_beacon)
-            self.own_beacon.increment_beacon_sequence_number_by_one()
-            self.last_beacon_broadcast = get_current_clock_millis()
-
-    def send_own_beacon_to(self, address: str):
-        message = self.own_beacon.to_cbor()
-
-        while len(message) > 0:
-            sent_bytes = self.sock.sendto(message, (address, PORT_IPND))
-            message = message[sent_bytes:]
-
-    @staticmethod
-    def get_micropython_ipv4_broadcast_addresses() -> (list, list):
-        address, subnet, _, _ = wlan.ifconfig()
-
-        if address == '0.0.0.0':
-            warning('wlan is not connected, cannot form broadcast address')
-            return []
-
-        address_parts = address.split('.')
-
-        for idx, subnet_part_str in enumerate(subnet.split('.')):
-            subnet_part = int(subnet_part_str)
-            inverse_subnet_part = ~subnet_part & 0xff
-
-            address_parts[idx] = str(int(address_parts[idx]) & subnet_part | inverse_subnet_part)
-
-        return ['.'.join(address_parts)], [address]
-
-    @staticmethod
-    def get_cpython_ipv4_broadcast_addresses() -> (list, list):
-        address_dicts = []
-
-        for interface in netifaces.interfaces():
-            address_dicts += netifaces.ifaddresses(interface).get(netifaces.AF_INET, [])
-
-        return list(map(lambda d: d['broadcast'], address_dicts)), list(map(lambda d: d['addr'], address_dicts))
+import socket
+from typing import Tuple, Optional, List, Dict
+
+from dtn7zero.constants import RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP, PORT_MTCP, PORT_IPND, IPND_SEND_INTERVAL_MILLISECONDS, IPND_BEACON_MAX_SIZE
+from dtn7zero.data import Node
+from dtn7zero.storage import Storage
+from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning
+from py_dtn7.bundle import Flags
+
+if RUNNING_MICROPYTHON:
+    import wlan
+else:
+    import netifaces
+
+try:
+    from cbor2 import dumps, loads
+except ImportError:
+    from cbor import dumps, loads
+
+
+class BeaconFlags(Flags):
+
+    @property
+    def eid_present(self) -> bool:
+        """
+        :return: True if the source endpoint identifier is present in this beacon
+        """
+        return self.get_flag(0)
+
+    @property
+    def service_block_present(self) -> bool:
+        """
+        :return: True if the service block is present in this beacon
+        """
+        return self.get_flag(1)
+
+    @property
+    def beacon_period_present(self) -> bool:
+        """
+        :return: True if the service block is present in this beacon
+        """
+        return self.get_flag(2)
+
+    @property
+    def reserved_3_to_7(self) -> int:
+        """
+        :return: shift to zero of bits 3 to 7 that are reserved for future use
+        """
+        return (self.flags >> 3) & 3
+
+
+class Beacon:
+
+    def __init__(
+            self,
+            version: int,
+            beacon_flags: BeaconFlags,
+            eid_scheme: Optional[int],
+            eid_specific_part: Optional[str],
+            beacon_sequence_number: int,
+            service_block: Tuple[List[Tuple[str, int]], Dict[int, bytes]],
+            beacon_period: Optional[int]
+    ):
+        self.version: int = version
+        self.beacon_flags: BeaconFlags = beacon_flags
+        self.eid_scheme: Optional[int] = eid_scheme
+        self.eid_specific_part: Optional[str] = eid_specific_part
+        self.beacon_sequence_number: int = beacon_sequence_number
+        self.service_block: Tuple[List[Tuple[str, int]], Dict[int, bytes]] = service_block
+        self.beacon_period: Optional[int] = beacon_period
+
+        if version != 7:
+            raise NotImplementedError('beacons with other versions than 7 are currently not supported')
+
+        assert not beacon_flags.eid_present or eid_scheme is not None and eid_specific_part is not None
+        assert not beacon_flags.service_block_present or service_block is not None
+        assert not beacon_flags.beacon_period_present or beacon_period is not None
+
+    def __repr__(self) -> str:
+        return '<Beacon: {}]>'.format(self.to_block_data())
+
+    @staticmethod
+    def from_block_data(beacon: list):
+        version = beacon[0]
+        beacon_flags = BeaconFlags(beacon[1])
+        beacon_sequence_number = None
+        eid_scheme = None
+        eid_specific_part = None
+        service_block = ([], {})
+        beacon_period = None
+
+        expected_length = 3 + int(beacon_flags.eid_present) + int(beacon_flags.service_block_present) + int(beacon_flags.beacon_period_present)
+        if len(beacon) != expected_length:
+            raise IndexError('cannot decode beacon because actual length {} differs from length, suggested by flags {}. block data: {}'.format(len(beacon), expected_length, beacon))
+
+        # there are some uncertainties I want to circumvent with this approach:
+        #  1. the EID and Beacon Sequence Number might be switched in position (indexes 2 and 3)
+        #     (ipnd-thesis describes EID at index 3, while dtn7rs places EID at index 2)
+        #  2. EID, Service Block, and Beacon Period might be omitted
+        #     (ipdn-thesis describes to omit empty fields, which can place later items at earlier indexes)
+        for item in beacon[2:]:
+            if isinstance(item, int):
+                if beacon_sequence_number is None:  # Beacon Sequence Number is set first (in accordance with beacon order)
+                    beacon_sequence_number = item
+                elif beacon_flags.beacon_period_present:  # Beacon Period is set second (skips unknown integer field if flag is not set)
+                    beacon_period = item
+            elif isinstance(item, list):
+                if eid_scheme is None and beacon_flags.eid_present:  # EID is set first (if flag is set)
+                    eid_scheme, eid_specific_part = item
+                elif beacon_flags.service_block_present:  # Service Block is set second (if flag is set)
+                    service_block = item
+
+        return Beacon(version, beacon_flags, eid_scheme, eid_specific_part, beacon_sequence_number, service_block, beacon_period)
+
+    def to_block_data(self):
+        block = [self.version, self.beacon_flags.flags]
+
+        # order is inspired by the dtn7rs implementation and not the ipnd-thesis (EID and Beacon Sequence Number switched)
+        if self.beacon_flags.eid_present:
+            block.append((self.eid_scheme, self.eid_specific_part))
+        block.append(self.beacon_sequence_number)
+        if self.beacon_flags.service_block_present:
+            block.append(self.service_block)
+        if self.beacon_flags.beacon_period_present:
+            block.append(self.beacon_period)
+
+        return block
+
+    def to_cbor(self) -> bytes:
+        # although bundles must be an infinite array, nothing is specified here, so keep the finite array
+        return dumps(self.to_block_data())
+
+    @staticmethod
+    def from_objects(
+            beacon_sequence_number: int,
+            eid_scheme: Optional[int] = None,
+            eid_specific_part: Optional[str] = None,
+            service_block: Optional[Tuple[List[Tuple[str, int]], Dict[int, bytes]]] = None,
+            beacon_period: Optional[int] = None
+    ):
+        beacon_flags = BeaconFlags()
+
+        if bool(eid_scheme) != bool(eid_specific_part):
+            raise IndexError('EID must be complete, got: {}, {}'.format(eid_scheme, eid_specific_part))
+        if eid_scheme is not None:
+            beacon_flags.set_flag(0)
+        if service_block is not None:
+            beacon_flags.set_flag(1)
+        else:
+            service_block = ([], {})
+        if beacon_period is not None:
+            beacon_flags.set_flag(2)
+
+        return Beacon(7, beacon_flags, eid_scheme, eid_specific_part, beacon_sequence_number, service_block, beacon_period)
+
+    @staticmethod
+    def from_cbor(data: bytes):
+        return Beacon.from_block_data(loads(data))
+
+    def increment_beacon_sequence_number_by_one(self):
+        # ipnd-thesis states to use an unsigned 32bit integer and wrap around on overflow
+        self.beacon_sequence_number = (self.beacon_sequence_number + 1) & 0xffffffff
+
+    def is_continuous_with_old_beacon_sequence_number(self, old_beacon_sequence_number: int):
+        if old_beacon_sequence_number == 0xffffffff:
+            return self.beacon_sequence_number == 0
+        return self.beacon_sequence_number == old_beacon_sequence_number
+
+
+class IPND:
+
+    """
+    for now, we only support broadcast on all interfaces and IPv4 only.
+    todo: extend functionality to filter network interfaces and support IPv6
+    todo: extend functionality to delete nodes after a beacon timeout
+    """
+    def __init__(self, eid_scheme: int, eid_specific_part: str, storage: Storage):
+        self.storage = storage
+
+        # todo: check dynamically for new networks -> also test with changing networks
+        if RUNNING_MICROPYTHON:
+            self.broadcast_addresses, self.own_addresses = IPND.get_micropython_ipv4_broadcast_addresses()
+        else:
+            self.broadcast_addresses, self.own_addresses = IPND.get_cpython_ipv4_broadcast_addresses()
+
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+
+        if not RUNNING_MICROPYTHON:
+            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.sock.settimeout(0)
+
+        self.sock.bind(('', 3003))
+
+        # self.own_beacon = create_minimal_output_beacon(eid_scheme, eid_specific_part)
+        self.own_beacon = Beacon.from_objects(
+            beacon_sequence_number=0,
+            eid_scheme=eid_scheme,
+            eid_specific_part=eid_specific_part,
+            service_block=([(IPND_IDENTIFIER_MTCP, PORT_MTCP)], {})  # todo: extend for all and active clas'
+        )
+
+        self.last_beacon_broadcast = 0
+
+    def update(self):
+        try:
+            # todo: for now it seems one full datagram is returned here, as long as the datagram is smaller than bytes-trying-to-receive
+            raw_data, (address, port) = self.sock.recvfrom(IPND_BEACON_MAX_SIZE)
+        except OSError:
+            pass
+        except MemoryError:
+            warning('MEMORY ERROR DURING BEACON RECEIVE, PASS')
+        else:
+            try:
+                # eid_scheme, eid_specific_part, clas, services = extract_beacon_information_from(raw_data)
+                beacon = Beacon.from_cbor(raw_data)
+            except Exception as e:
+                warning('could not decode beacon. error: {}'.format(e))
+            else:
+                if address not in self.own_addresses:
+                    existing_node = self.storage.get_node(address)
+
+                    if existing_node is None:
+                        debug('received beacon from new node: {}, size: {}'.format(address, len(raw_data)))
+
+                        new_node = Node(address, (beacon.eid_scheme, beacon.eid_specific_part), dict(beacon.service_block[0]), beacon.beacon_sequence_number)
+                        self.storage.add_node(new_node)
+
+                        sequence_number_matches = False
+                    else:
+                        debug('received beacon from known node: {}, size: {}'.format(address, len(raw_data)))
+                        # existing_node.merge_new_info(eid_scheme, eid_specific_part, dict(clas))
+                        existing_node.merge_new_info(beacon.eid_scheme, beacon.eid_specific_part, dict(beacon.service_block[0]))
+
+                        sequence_number_matches = existing_node.advance_sequence_number(beacon.beacon_sequence_number)
+
+                    if not sequence_number_matches:
+                        # send back a uni-cast beacon to a previously unknown node for faster knowledge spread
+                        # ideal case: it never received a beacon from us -> current state (sequence number) is new to the node
+                        # not ideal case: beacons were exchanged concurrently -> state (sequence number) is duplicate, which is unspecified and ideally ignored
+                        # dtn7zero specific detail: we add unicast information to the beacon, so there is no second unicast beacon sent back to us
+
+                        if not (42 in beacon.service_block[1] and beacon.service_block[1][42] == b'unicast'):
+                            self.own_beacon.service_block[1][42] = b'unicast'
+                            self.send_own_beacon_to(address)
+                            del self.own_beacon.service_block[1][42]
+
+        if is_timestamp_older_than_timeout(self.last_beacon_broadcast, IPND_SEND_INTERVAL_MILLISECONDS):
+            for address in self.broadcast_addresses:
+                self.send_own_beacon_to(address)
+            # minimal_output_beacon_increase_counter_by_one(self.own_beacon)
+            self.own_beacon.increment_beacon_sequence_number_by_one()
+            self.last_beacon_broadcast = get_current_clock_millis()
+
+    def send_own_beacon_to(self, address: str):
+        message = self.own_beacon.to_cbor()
+
+        while len(message) > 0:
+            sent_bytes = self.sock.sendto(message, (address, PORT_IPND))
+            message = message[sent_bytes:]
+
+    @staticmethod
+    def get_micropython_ipv4_broadcast_addresses() -> (list, list):
+        address, subnet, _, _ = wlan.ifconfig()
+
+        if address == '0.0.0.0':
+            warning('wlan is not connected, cannot form broadcast address')
+            return []
+
+        address_parts = address.split('.')
+
+        for idx, subnet_part_str in enumerate(subnet.split('.')):
+            subnet_part = int(subnet_part_str)
+            inverse_subnet_part = ~subnet_part & 0xff
+
+            address_parts[idx] = str(int(address_parts[idx]) & subnet_part | inverse_subnet_part)
+
+        return ['.'.join(address_parts)], [address]
+
+    @staticmethod
+    def get_cpython_ipv4_broadcast_addresses() -> (list, list):
+        address_dicts = []
+
+        for interface in netifaces.interfaces():
+            interface_information = netifaces.ifaddresses(interface).get(netifaces.AF_INET, [])
+
+            # linux 'lo' local interface provides 'peer' instead of 'broadcast'
+            # d['peer']=='127.0.0.1' which is no broadcast address
+            # as a hacky solution we hardcode the broadcast address
+            if interface == 'lo':
+                interface_information[0]['broadcast'] = '127.255.255.255'
+
+            address_dicts += interface_information
+
+        return list(map(lambda d: d['broadcast'], address_dicts)), list(map(lambda d: d['addr'], address_dicts))
```

### Comparing `dtn7zero-0.0.4/dtn7zero/routers/__init__.py` & `dtn7zero-0.0.5/dtn7zero/routers/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import time
-from abc import ABC
-from typing import Iterable
-
-from dtn7zero.constants import ATTACH_PREVIOUS_NODE_BLOCK
-from dtn7zero.data import BundleInformation
-from py_dtn7 import Bundle
-from py_dtn7.bundle import PreviousNodeBlock, BlockProcessingControlFlags
-
-
-class Router(ABC):
-
-    def prepare_and_serialize_bundle(self, full_node_uri: str, bundle_information: BundleInformation) -> bytes:
-        """ RFC 9171, 5.4 Bundle Forwarding
-        […]
-        Step 4: For each node selected for forwarding, the BPA MUST invoke the services of the selected CLA(s) in order
-        to effect the sending of the bundle to that node. […] Note that:
-
-        * If the bundle has a Previous Node Block, as defined in Section 4.4.1, then that block MUST be removed from
-        the bundle before the bundle is forwarded.
-
-        * If the BPA is configured to attach Previous Node Blocks to forwarded bundles, then a Previous Node Block
-        containing the node ID of the forwarding node MUST be inserted into the bundle before the bundle is forwarded.
-
-        * If the bundle has a Bundle Age Block, as defined in Section 4.4.2, then at the last possible moment before
-        the CLA initiates conveyance of the bundle via the CL protocol the bundle age value MUST be increased by the
-        difference between the current time and the time at which the bundle was received (or, if the local node is
-        the source of the bundle, created).
-        """
-
-        # copy bundle to not alter the storage instance
-        bundle = Bundle.from_cbor(bundle_information.bundle.to_cbor())
-
-        if bundle.previous_node_block:
-            bundle.remove_block(bundle.previous_node_block)
-
-        if ATTACH_PREVIOUS_NODE_BLOCK:
-            flags = BlockProcessingControlFlags(0)
-            flags.set_flag(4)  # discard block if block cant be processed
-
-            previous_node_block = PreviousNodeBlock.from_objects(full_node_uri, flags)
-
-            bundle.insert_canonical_block(previous_node_block)
-
-        if bundle.bundle_age_block:
-            # todo: assuming no wrap-around on micropython here -> test after which time this happens
-            bundle.bundle_age_block.age_milliseconds += (time.time_ns() // 1000000) - bundle_information.received_at_ms
-
-        """ RFC 9171, 4.4.3 Hop Count
-        […] the hop count value SHOULD initially be zero and SHOULD be increased by 1 on each hop.
-        """
-        if bundle.hop_count_block:
-            bundle.hop_count_block.hop_count += 1
-
-        return bundle.to_cbor()
-
-    def generator_poll_bundles(self) -> Iterable[BundleInformation]:
-        raise NotImplementedError('do not instantiate Router class directly')
-
-    def immediate_forwarding_attempt(self, full_node_uri: str, bundle_information: BundleInformation) -> (bool, int):
-        raise NotImplementedError('do not instantiate Router class directly')
-
-    def send_to_previous_node(self, full_node_uri: str, bundle_information: BundleInformation) -> bool:
-        raise NotImplementedError('do not instantiate Router class directly')
+import time
+from abc import ABC
+from typing import Iterable
+
+from dtn7zero.constants import ATTACH_PREVIOUS_NODE_BLOCK
+from dtn7zero.data import BundleInformation
+from py_dtn7 import Bundle
+from py_dtn7.bundle import PreviousNodeBlock, BlockProcessingControlFlags
+
+
+class Router(ABC):
+
+    def prepare_and_serialize_bundle(self, full_node_uri: str, bundle_information: BundleInformation) -> bytes:
+        """ RFC 9171, 5.4 Bundle Forwarding
+        […]
+        Step 4: For each node selected for forwarding, the BPA MUST invoke the services of the selected CLA(s) in order
+        to effect the sending of the bundle to that node. […] Note that:
+
+        * If the bundle has a Previous Node Block, as defined in Section 4.4.1, then that block MUST be removed from
+        the bundle before the bundle is forwarded.
+
+        * If the BPA is configured to attach Previous Node Blocks to forwarded bundles, then a Previous Node Block
+        containing the node ID of the forwarding node MUST be inserted into the bundle before the bundle is forwarded.
+
+        * If the bundle has a Bundle Age Block, as defined in Section 4.4.2, then at the last possible moment before
+        the CLA initiates conveyance of the bundle via the CL protocol the bundle age value MUST be increased by the
+        difference between the current time and the time at which the bundle was received (or, if the local node is
+        the source of the bundle, created).
+        """
+
+        # copy bundle to not alter the storage instance
+        bundle = Bundle.from_cbor(bundle_information.bundle.to_cbor())
+
+        if bundle.previous_node_block:
+            bundle.remove_block(bundle.previous_node_block)
+
+        if ATTACH_PREVIOUS_NODE_BLOCK:
+            flags = BlockProcessingControlFlags(0)
+            flags.set_flag(4)  # discard block if block cant be processed
+
+            previous_node_block = PreviousNodeBlock.from_objects(full_node_uri, flags)
+
+            bundle.insert_canonical_block(previous_node_block)
+
+        if bundle.bundle_age_block:
+            # todo: assuming no wrap-around on micropython here -> test after which time this happens
+            bundle.bundle_age_block.age_milliseconds += (time.time_ns() // 1000000) - bundle_information.received_at_ms
+
+        """ RFC 9171, 4.4.3 Hop Count
+        […] the hop count value SHOULD initially be zero and SHOULD be increased by 1 on each hop.
+        """
+        if bundle.hop_count_block:
+            bundle.hop_count_block.hop_count += 1
+
+        return bundle.to_cbor()
+
+    def generator_poll_bundles(self) -> Iterable[BundleInformation]:
+        raise NotImplementedError('do not instantiate Router class directly')
+
+    def immediate_forwarding_attempt(self, full_node_uri: str, bundle_information: BundleInformation) -> (bool, int):
+        raise NotImplementedError('do not instantiate Router class directly')
+
+    def send_to_previous_node(self, full_node_uri: str, bundle_information: BundleInformation) -> bool:
+        raise NotImplementedError('do not instantiate Router class directly')
```

### Comparing `dtn7zero-0.0.4/dtn7zero/routers/simple_epidemic_router.py` & `dtn7zero-0.0.5/dtn7zero/routers/simple_epidemic_router.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from typing import Dict, Iterable
-
-from dtn7zero.constants import SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO, IPND_IDENTIFIER_MTCP, IPND_IDENTIFIER_REST
-from dtn7zero.convergence_layer_adapters import CLA
-from dtn7zero.data import BundleInformation, Node, BundleStatusReportReasonCodes
-from dtn7zero.routers import Router
-from dtn7zero.storage import Storage
-from dtn7zero.utility import warning
-
-
-class SimpleEpidemicRouter(Router):
-
-    def __init__(self, convergence_layer_adapters: Dict[str, CLA], storage: Storage):
-        self.clas = convergence_layer_adapters
-        self.storage = storage
-
-    def generator_poll_bundles(self) -> Iterable[BundleInformation]:
-        # Currently there are only two cla types implemented, which are also the only ones supported here.
-
-        for node in self.storage.get_nodes():
-            if IPND_IDENTIFIER_REST in node.clas:
-                for bundle_information in self._generator_poll_advanced(node, self.clas[IPND_IDENTIFIER_REST]):
-                    yield bundle_information
-
-        if IPND_IDENTIFIER_MTCP in self.clas:
-            for bundle_information in self._generator_poll_simple(self.clas[IPND_IDENTIFIER_MTCP]):
-                yield bundle_information
-
-    def _generator_poll_simple(self, cla: CLA):
-        bundle, node_address = cla.poll()
-        while bundle is not None:
-            if not self.storage.was_seen(bundle.bundle_id):
-                self.storage.store_seen(bundle.bundle_id, node_address)
-
-                bundle_information = BundleInformation(bundle)
-
-                node = self.storage.get_node(node_address)
-                if node is not None:  # if node is known, prevent the bundle from being sent back to that same node
-                    bundle_information.forwarded_to_nodes.append(node)
-
-                yield bundle_information
-            bundle, node_address = cla.poll()
-
-    def _generator_poll_advanced(self, node: Node, cla: CLA):
-        bundle_ids = cla.poll_ids(node)
-
-        for bundle_id in bundle_ids:
-            if not self.storage.was_seen(bundle_id):
-                bundle, node_polled_address = cla.poll(bundle_id, node)
-                if bundle is not None:
-                    self.storage.store_seen(bundle_id, node_polled_address)
-
-                    bundle_information = BundleInformation(bundle)
-
-                    node = self.storage.get_node(node_polled_address)
-                    if node is not None:  # if node is known, prevent the bundle from being sent back to that same node
-                        bundle_information.forwarded_to_nodes.append(node)
-
-                    yield bundle_information
-                    break
-
-    def immediate_forwarding_attempt(self, full_node_uri: str, bundle_information: BundleInformation) -> (bool, int):
-        serialized_bundle: bytes = self.prepare_and_serialize_bundle(full_node_uri, bundle_information)
-
-        reason = BundleStatusReportReasonCodes.NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE
-
-        for node in self.storage.get_nodes():
-            if node in bundle_information.forwarded_to_nodes:
-                continue
-
-            for cla in self.clas.values():
-                success = cla.send_to(node, serialized_bundle)
-                if success:
-                    bundle_information.forwarded_to_nodes.append(node)
-                else:
-                    reason = BundleStatusReportReasonCodes.TRAFFIC_PARED
-
-        return len(bundle_information.forwarded_to_nodes) >= SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO, reason
-
-    def send_to_previous_node(self, full_node_uri: str, bundle_information: BundleInformation) -> bool:
-        previous_node_address = self.storage.get_seen(bundle_information.bundle.bundle_id)
-        previous_node = self.storage.get_node(previous_node_address)
-
-        if previous_node_address is None or previous_node is None:
-            warning('Previous node of bundle-id {} is not known (any more). Ignoring request to send to previous node.'.format(bundle_information.bundle.bundle_id))
-            return False
-
-        bundle: bytes = self.prepare_and_serialize_bundle(full_node_uri, bundle_information)
-
-        for cla in self.clas.values():
-            if cla.send_to(previous_node, bundle):
-                return True
-        return False
+from typing import Dict, Iterable
+
+from dtn7zero.constants import SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO, IPND_IDENTIFIER_MTCP, IPND_IDENTIFIER_REST
+from dtn7zero.convergence_layer_adapters import CLA
+from dtn7zero.data import BundleInformation, Node, BundleStatusReportReasonCodes
+from dtn7zero.routers import Router
+from dtn7zero.storage import Storage
+from dtn7zero.utility import warning
+
+
+class SimpleEpidemicRouter(Router):
+
+    def __init__(self, convergence_layer_adapters: Dict[str, CLA], storage: Storage):
+        self.clas = convergence_layer_adapters
+        self.storage = storage
+
+    def generator_poll_bundles(self) -> Iterable[BundleInformation]:
+        # Currently there are only two cla types implemented, which are also the only ones supported here.
+
+        for node in self.storage.get_nodes():
+            if IPND_IDENTIFIER_REST in node.clas:
+                for bundle_information in self._generator_poll_advanced(node, self.clas[IPND_IDENTIFIER_REST]):
+                    yield bundle_information
+
+        if IPND_IDENTIFIER_MTCP in self.clas:
+            for bundle_information in self._generator_poll_simple(self.clas[IPND_IDENTIFIER_MTCP]):
+                yield bundle_information
+
+    def _generator_poll_simple(self, cla: CLA):
+        bundle, node_address = cla.poll()
+        while bundle is not None:
+            if not self.storage.was_seen(bundle.bundle_id):
+                self.storage.store_seen(bundle.bundle_id, node_address)
+
+                bundle_information = BundleInformation(bundle)
+
+                node = self.storage.get_node(node_address)
+                if node is not None:  # if node is known, prevent the bundle from being sent back to that same node
+                    bundle_information.forwarded_to_nodes.append(node)
+
+                yield bundle_information
+            bundle, node_address = cla.poll()
+
+    def _generator_poll_advanced(self, node: Node, cla: CLA):
+        bundle_ids = cla.poll_ids(node)
+
+        for bundle_id in bundle_ids:
+            if not self.storage.was_seen(bundle_id):
+                bundle, node_polled_address = cla.poll(bundle_id, node)
+                if bundle is not None:
+                    self.storage.store_seen(bundle_id, node_polled_address)
+
+                    bundle_information = BundleInformation(bundle)
+
+                    node = self.storage.get_node(node_polled_address)
+                    if node is not None:  # if node is known, prevent the bundle from being sent back to that same node
+                        bundle_information.forwarded_to_nodes.append(node)
+
+                    yield bundle_information
+                    break
+
+    def immediate_forwarding_attempt(self, full_node_uri: str, bundle_information: BundleInformation) -> (bool, int):
+        serialized_bundle: bytes = self.prepare_and_serialize_bundle(full_node_uri, bundle_information)
+
+        reason = BundleStatusReportReasonCodes.NO_TIMELY_CONTACT_WITH_NEXT_NODE_ON_ROUTE
+
+        for node in self.storage.get_nodes():
+            if node in bundle_information.forwarded_to_nodes:
+                continue
+
+            for cla in self.clas.values():
+                success = cla.send_to(node, serialized_bundle)
+                if success:
+                    bundle_information.forwarded_to_nodes.append(node)
+                else:
+                    reason = BundleStatusReportReasonCodes.TRAFFIC_PARED
+
+        return len(bundle_information.forwarded_to_nodes) >= SIMPLE_EPIDEMIC_ROUTER_MIN_NODES_TO_FORWARD_TO, reason
+
+    def send_to_previous_node(self, full_node_uri: str, bundle_information: BundleInformation) -> bool:
+        previous_node_address = self.storage.get_seen(bundle_information.bundle.bundle_id)
+        previous_node = self.storage.get_node(previous_node_address)
+
+        if previous_node_address is None or previous_node is None:
+            warning('Previous node of bundle-id {} is not known (any more). Ignoring request to send to previous node.'.format(bundle_information.bundle.bundle_id))
+            return False
+
+        bundle: bytes = self.prepare_and_serialize_bundle(full_node_uri, bundle_information)
+
+        for cla in self.clas.values():
+            if cla.send_to(previous_node, bundle):
+                return True
+        return False
```

### Comparing `dtn7zero-0.0.4/dtn7zero/storage/__init__.py` & `dtn7zero-0.0.5/dtn7zero/storage/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from abc import ABC
-from typing import List, Tuple, Optional, Iterable
-
-from dtn7zero.data import BundleInformation, Node
-
-
-class Storage(ABC):
-
-    def add_node(self, node: Node):
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def get_node(self, node_address: str) -> Optional[Node]:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def get_nodes(self) -> Iterable[Node]:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def was_seen(self, bundle_id: str) -> bool:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def get_seen(self, bundle_id: str) -> Optional[str]:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def store_seen(self, bundle_id: str, node: Optional[str]):
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def remove_bundle(self, bundle_id: str) -> bool:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
-        raise NotImplementedError('do not instantiate Storage class directly')
-
-    def get_bundles_to_retry(self):
-        raise NotImplementedError('do not instantiate Storage class directly')
+from abc import ABC
+from typing import List, Tuple, Optional, Iterable
+
+from dtn7zero.data import BundleInformation, Node
+
+
+class Storage(ABC):
+
+    def add_node(self, node: Node):
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def get_node(self, node_address: str) -> Optional[Node]:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def get_nodes(self) -> Iterable[Node]:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def was_seen(self, bundle_id: str) -> bool:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def get_seen(self, bundle_id: str) -> Optional[str]:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def store_seen(self, bundle_id: str, node: Optional[str]):
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def remove_bundle(self, bundle_id: str) -> bool:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
+        raise NotImplementedError('do not instantiate Storage class directly')
+
+    def get_bundles_to_retry(self):
+        raise NotImplementedError('do not instantiate Storage class directly')
```

### Comparing `dtn7zero-0.0.4/dtn7zero/storage/simple_in_memory_storage.py` & `dtn7zero-0.0.5/dtn7zero/storage/simple_in_memory_storage.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Dict, Tuple, List, Optional, Iterable
-
-from dtn7zero.constants import SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES, SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS
-from dtn7zero.data import BundleInformation, Node
-from dtn7zero.storage import Storage
-from dtn7zero.utility import get_oldest_bundle, get_oldest_bundle_id
-
-
-class SimpleInMemoryStorage(Storage):
-
-    def __init__(self):
-        self.bundles: Dict[str, BundleInformation] = {}
-        self.bundle_ids: Dict[str, Optional[str]] = {}
-        self.nodes: Dict[str, Node] = {}
-
-    def add_node(self, node: Node):
-        self.nodes[node.address] = node
-
-    def get_node(self, node_address) -> Optional[Node]:
-        return self.nodes.get(node_address)
-
-    def get_nodes(self) -> Iterable[Node]:
-        return self.nodes.values()
-
-    def get_seen(self, bundle_id: str) -> Optional[str]:
-        return self.bundle_ids.get(bundle_id)
-
-    def was_seen(self, bundle_id: str) -> bool:
-        return bundle_id in self.bundle_ids
-
-    def store_seen(self, bundle_id: str, node_address):
-        if node_address is None and self.bundle_ids.get(bundle_id, None) is not None:
-            return  # we do not want to overwrite a valid node with None from an unknown source
-
-        if len(self.bundle_ids) >= SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS:
-            del self.bundle_ids[get_oldest_bundle_id(self.bundle_ids)]
-        self.bundle_ids[bundle_id] = node_address
-
-    def remove_bundle(self, bundle_id: str) -> bool:
-        return self.bundles.pop(bundle_id, False)  # if the bundle exists it is 'truthy'
-
-    def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
-        removed_bundles = []
-
-        if bundle_information.bundle.bundle_id in self.bundles:
-            return True, removed_bundles
-
-        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
-            self.garbage_collect()
-
-        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
-            oldest_bundle = self.bundles.pop(get_oldest_bundle(self.bundles.values()).bundle.bundle_id)
-            removed_bundles.append(oldest_bundle)
-
-        self.store_seen(bundle_information.bundle.bundle_id, None)
-
-        self.bundles[bundle_information.bundle.bundle_id] = bundle_information
-
-        return True, removed_bundles
-
-    def garbage_collect(self):
-        for bundle_id in list(self.bundles):
-            if self.bundles[bundle_id].retention_constraint is None:
-                del self.bundles[bundle_id]
-
-    def get_bundles_to_retry(self):
-        # simply yield all stored bundles
-        # 1. reason: in-memory storage only stores a limited amount of bundles
-        # 2. router only forwards bundles where they have not been forwarded yet -> router filters
-        return (i for i in tuple(self.bundles.values()))
+from typing import Dict, Tuple, List, Optional, Iterable
+
+from dtn7zero.constants import SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES, SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS
+from dtn7zero.data import BundleInformation, Node
+from dtn7zero.storage import Storage
+from dtn7zero.utility import get_oldest_bundle, get_oldest_bundle_id
+
+
+class SimpleInMemoryStorage(Storage):
+
+    def __init__(self):
+        self.bundles: Dict[str, BundleInformation] = {}
+        self.bundle_ids: Dict[str, Optional[str]] = {}
+        self.nodes: Dict[str, Node] = {}
+
+    def add_node(self, node: Node):
+        self.nodes[node.address] = node
+
+    def get_node(self, node_address) -> Optional[Node]:
+        return self.nodes.get(node_address)
+
+    def get_nodes(self) -> Iterable[Node]:
+        return self.nodes.values()
+
+    def get_seen(self, bundle_id: str) -> Optional[str]:
+        return self.bundle_ids.get(bundle_id)
+
+    def was_seen(self, bundle_id: str) -> bool:
+        return bundle_id in self.bundle_ids
+
+    def store_seen(self, bundle_id: str, node_address):
+        if node_address is None and self.bundle_ids.get(bundle_id, None) is not None:
+            return  # we do not want to overwrite a valid node with None from an unknown source
+
+        if len(self.bundle_ids) >= SIMPLE_IN_MEMORY_STORAGE_MAX_KNOWN_BUNDLE_IDS:
+            del self.bundle_ids[get_oldest_bundle_id(self.bundle_ids)]
+        self.bundle_ids[bundle_id] = node_address
+
+    def remove_bundle(self, bundle_id: str) -> bool:
+        return self.bundles.pop(bundle_id, False)  # if the bundle exists it is 'truthy'
+
+    def delay_bundle(self, bundle_information: BundleInformation) -> Tuple[bool, List[BundleInformation]]:
+        removed_bundles = []
+
+        if bundle_information.bundle.bundle_id in self.bundles:
+            return True, removed_bundles
+
+        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
+            self.garbage_collect()
+
+        if len(self.bundles) >= SIMPLE_IN_MEMORY_STORAGE_MAX_STORED_BUNDLES:
+            oldest_bundle = self.bundles.pop(get_oldest_bundle(self.bundles.values()).bundle.bundle_id)
+            removed_bundles.append(oldest_bundle)
+
+        self.store_seen(bundle_information.bundle.bundle_id, None)
+
+        self.bundles[bundle_information.bundle.bundle_id] = bundle_information
+
+        return True, removed_bundles
+
+    def garbage_collect(self):
+        for bundle_id in list(self.bundles):
+            if self.bundles[bundle_id].retention_constraint is None:
+                del self.bundles[bundle_id]
+
+    def get_bundles_to_retry(self):
+        # simply yield all stored bundles
+        # 1. reason: in-memory storage only stores a limited amount of bundles
+        # 2. router only forwards bundles where they have not been forwarded yet -> router filters
+        return (i for i in tuple(self.bundles.values()))
```

### Comparing `dtn7zero-0.0.4/dtn7zero/utility.py` & `dtn7zero-0.0.5/dtn7zero/utility.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import time
-import re
-from typing import Iterable
-
-from dtn7zero.constants import DEBUG, WARNING
-
-NODE_URI_REGEX = re.compile(r'(^dtn://[^~/]+/$)|(^ipn://\d+(\.\d+)*$)')
-ENDPOINT_URI_REGEX = re.compile(r'(^dtn://none$)|(^dtn://[^~/]+/([^~/]+/)*[^~/]+$)|(^ipn://\d+(\.\d+)+$)')
-GROUP_URI_REGEX = re.compile(r'^dtn://[^~/]+/([^~]+/)*~[^/]+$')
-
-
-def get_oldest_bundle_id(bundle_ids: Iterable[str]):
-    """
-    returns the oldest bundle, based on the creation timestamp and sequence number, with inaccurate packages being newer
-    """
-
-    def is_x_older(x_time, x_num, y_time, y_num):
-        if x_time == 0:
-            if y_time == 0:
-                return x_num < y_num
-            else:
-                return False  # prefer packages with no accurate clock -> newer
-        elif y_time == 0:
-            return True  # prefer packages with no accurate clock -> newer
-        elif x_time == y_time:
-            return x_num < y_num
-        else:
-            return x_time < y_time
-
-    oldest, oldest_time, oldest_num = None, None, None
-
-    for bundle_id in bundle_ids:
-        if oldest is None:
-            oldest = bundle_id
-            _, oldest_time, oldest_num = oldest.rsplit('-', 2)  # source-uri might contain unforeseen character
-            oldest_time, oldest_num = int(oldest_time), int(oldest_num)
-        else:
-            _, bundle_time, bundle_num = bundle_id.rsplit('-', 2)  # source-uri might contain unforeseen character
-            bundle_time, bundle_num = int(bundle_time), int(bundle_num)
-
-            if is_x_older(bundle_time, bundle_num, oldest_time, oldest_num):
-                oldest, oldest_time, oldest_num = bundle_id, bundle_time, bundle_num
-
-    return oldest
-
-
-def get_oldest_bundle(bundle_informations):
-    """
-    simplicity -> returns the oldest bundle based on reception time
-
-    This eliminates bundles with extremely long lifetime blocking storage,
-    but it also discriminates packages with low hop count.
-    """
-    oldest = None
-
-    for bundle_information in bundle_informations:
-        if oldest is None:
-            oldest = bundle_information
-        elif bundle_information.received_at_ms < oldest.received_at_ms:
-            oldest = bundle_information
-
-    return oldest
-
-
-def get_current_clock_millis():
-    return time.time_ns() // 1000000
-
-
-def is_timestamp_older_than_timeout(clock_timestamp_millis: int, timeout_millis: int):
-    return time.time_ns() // 1000000 - clock_timestamp_millis >= timeout_millis
-
-
-def debug(*args):
-    if DEBUG:
-        print(*args)
-
-
-def warning(*args):
-    if WARNING:
-        print(*args)
-
-
-def is_correct_node_uri(node_uri: str) -> bool:
-    """ match description:
-    dtn -> starts with "dtn://", then one or more characters (except "~" or "/"), ends with "/"
-    ipn -> starts with "ipn://", then one or more digits, then zero or more "." + one or more digits
-
-    Currently used only on bpa creation to check the supplied node string.
-    """
-    return bool(NODE_URI_REGEX.match(node_uri))
-
-
-def is_correct_endpoint_uri(endpoint_uri: str) -> bool:
-    """ match description:
-    dtn -> one or more characters (except "~" or "/"), then zero or more "/"+one or more characters (except "~" or "/")
-    ipn -> one or more digits
-    special -> "dtn://none" for the anonymous none-endpoint is also supported
-    special -> a correct node uri (example: "dtn://node/") is also a correct endpoint uri
-
-    Currently used only on endpoint registration by the bpa to check the validity of a full-endpoint-uri.
-    As the LocalEndpoint is composed of bpa-node-uri + endpoint-id it is (and should never) be possible to register "dtn://none".
-    """
-    return bool(ENDPOINT_URI_REGEX.match(endpoint_uri)) or is_correct_node_uri(endpoint_uri)
-
-
-def is_correct_group_uri(group_uri: str) -> bool:
-    """match description:
-    dtn -> one or more characters (except "~" or "/"), then zero or more "/"+one or more characters (except "~" or "/"), ending with "/~"+one or more characters (except "~" or "/")
-    ipn -> no group registration
-
-    Currently used only on group-endpoint registration by the bpa to check the validity of a full-group-uri.
-    """
-    return bool(GROUP_URI_REGEX.match(group_uri))
+import time
+import re
+from typing import Iterable
+
+from dtn7zero.constants import DEBUG, WARNING
+
+NODE_URI_REGEX = re.compile(r'(^dtn://[^~/]+/$)|(^ipn://\d+(\.\d+)*$)')
+ENDPOINT_URI_REGEX = re.compile(r'(^dtn://none$)|(^dtn://[^~/]+/([^~/]+/)*[^~/]+$)|(^ipn://\d+(\.\d+)+$)')
+GROUP_URI_REGEX = re.compile(r'^dtn://[^~/]+/([^~]+/)*~[^/]+$')
+
+
+def get_oldest_bundle_id(bundle_ids: Iterable[str]):
+    """
+    returns the oldest bundle, based on the creation timestamp and sequence number, with inaccurate packages being newer
+    """
+
+    def is_x_older(x_time, x_num, y_time, y_num):
+        if x_time == 0:
+            if y_time == 0:
+                return x_num < y_num
+            else:
+                return False  # prefer packages with no accurate clock -> newer
+        elif y_time == 0:
+            return True  # prefer packages with no accurate clock -> newer
+        elif x_time == y_time:
+            return x_num < y_num
+        else:
+            return x_time < y_time
+
+    oldest, oldest_time, oldest_num = None, None, None
+
+    for bundle_id in bundle_ids:
+        if oldest is None:
+            oldest = bundle_id
+            _, oldest_time, oldest_num = oldest.rsplit('-', 2)  # source-uri might contain unforeseen character
+            oldest_time, oldest_num = int(oldest_time), int(oldest_num)
+        else:
+            _, bundle_time, bundle_num = bundle_id.rsplit('-', 2)  # source-uri might contain unforeseen character
+            bundle_time, bundle_num = int(bundle_time), int(bundle_num)
+
+            if is_x_older(bundle_time, bundle_num, oldest_time, oldest_num):
+                oldest, oldest_time, oldest_num = bundle_id, bundle_time, bundle_num
+
+    return oldest
+
+
+def get_oldest_bundle(bundle_informations):
+    """
+    simplicity -> returns the oldest bundle based on reception time
+
+    This eliminates bundles with extremely long lifetime blocking storage,
+    but it also discriminates packages with low hop count.
+    """
+    oldest = None
+
+    for bundle_information in bundle_informations:
+        if oldest is None:
+            oldest = bundle_information
+        elif bundle_information.received_at_ms < oldest.received_at_ms:
+            oldest = bundle_information
+
+    return oldest
+
+
+def get_current_clock_millis():
+    return time.time_ns() // 1000000
+
+
+def is_timestamp_older_than_timeout(clock_timestamp_millis: int, timeout_millis: int):
+    return time.time_ns() // 1000000 - clock_timestamp_millis >= timeout_millis
+
+
+def debug(*args):
+    if DEBUG:
+        print(*args)
+
+
+def warning(*args):
+    if WARNING:
+        print(*args)
+
+
+def is_correct_node_uri(node_uri: str) -> bool:
+    """ match description:
+    dtn -> starts with "dtn://", then one or more characters (except "~" or "/"), ends with "/"
+    ipn -> starts with "ipn://", then one or more digits, then zero or more "." + one or more digits
+
+    Currently used only on bpa creation to check the supplied node string.
+    """
+    return bool(NODE_URI_REGEX.match(node_uri))
+
+
+def is_correct_endpoint_uri(endpoint_uri: str) -> bool:
+    """ match description:
+    dtn -> one or more characters (except "~" or "/"), then zero or more "/"+one or more characters (except "~" or "/")
+    ipn -> one or more digits
+    special -> "dtn://none" for the anonymous none-endpoint is also supported
+    special -> a correct node uri (example: "dtn://node/") is also a correct endpoint uri
+
+    Currently used only on endpoint registration by the bpa to check the validity of a full-endpoint-uri.
+    As the LocalEndpoint is composed of bpa-node-uri + endpoint-id it is (and should never) be possible to register "dtn://none".
+    """
+    return bool(ENDPOINT_URI_REGEX.match(endpoint_uri)) or is_correct_node_uri(endpoint_uri)
+
+
+def is_correct_group_uri(group_uri: str) -> bool:
+    """match description:
+    dtn -> one or more characters (except "~" or "/"), then zero or more "/"+one or more characters (except "~" or "/"), ending with "/~"+one or more characters (except "~" or "/")
+    ipn -> no group registration
+
+    Currently used only on group-endpoint registration by the bpa to check the validity of a full-group-uri.
+    """
+    return bool(GROUP_URI_REGEX.match(group_uri))
```

### Comparing `dtn7zero-0.0.4/dtn7zero.egg-info/PKG-INFO` & `dtn7zero-0.0.5/dtn7zero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -119,15 +119,15 @@
 
 ## Development Information
 
 ### Development Mode
 You can install this project locally to directly reflect code changes in your environment.
 Simply run this in the project root folder (requires at least pip v21.1):
 ```shell
-$ pip install --editable .
+$ python -m pip install --editable .
 ```
 
 ### Build
 To build this project yourself you need the python [build](https://pypi.org/project/build/) tool, as well as [setuptools](https://pypi.org/project/setuptools/):
 ```shell
 $ pip install --upgrade setuptools
 $ pip install --upgrade build
```

### Comparing `dtn7zero-0.0.4/dtn7zero.egg-info/SOURCES.txt` & `dtn7zero-0.0.5/dtn7zero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.4/test/test-api-background.py` & `dtn7zero-0.0.5/test/test-api-background.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import time
-
-from dtn7zero import setup, register, start_background_update_thread
-from py_dtn7.bundle import PrimaryBlock
-
-
-setup("dtn://node1/")
-
-start_background_update_thread(_sleep_time_seconds=0.1)
-
-
-def ping_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-    print("received pong: {}".format(payload))
-
-
-ping = register("ping", ping_callback)
-
-
-def pong_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-    print("sending back pong {}".format(payload))
-    pong.send(payload, full_source_uri)
-
-
-pong = register("pong", pong_callback)
-
-
-counter = 1
-try:
-    while True:
-        time.sleep(2)
-        payload = str(counter).encode()
-        print("sending ping: {}".format(payload))
-        ping.send(payload, "dtn://node1/pong")
-        counter += 1
-except KeyboardInterrupt:
-    pass
-
+import time
+
+from dtn7zero import setup, register, start_background_update_thread
+from py_dtn7.bundle import PrimaryBlock
+
+
+setup("dtn://node1/")
+
+start_background_update_thread(_sleep_time_seconds=0.1)
+
+
+def ping_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+    print("received pong: {}".format(payload))
+
+
+ping = register("ping", ping_callback)
+
+
+def pong_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+    print("sending back pong {}".format(payload))
+    pong.send(payload, full_source_uri)
+
+
+pong = register("pong", pong_callback)
+
+
+counter = 1
+try:
+    while True:
+        time.sleep(2)
+        payload = str(counter).encode()
+        print("sending ping: {}".format(payload))
+        ping.send(payload, "dtn://node1/pong")
+        counter += 1
+except KeyboardInterrupt:
+    pass
+
```

### Comparing `dtn7zero-0.0.4/test/test-api-ping.py` & `dtn7zero-0.0.5/test/test-api-pong.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import time
-
-from dtn7zero import setup, register, start_background_update_thread
-from py_dtn7.bundle import PrimaryBlock
-
-
-setup("dtn://node1/")
-
-start_background_update_thread(_sleep_time_seconds=0.1)
-
-
-def ping_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
-    print("received pong: {}".format(payload))
-
-
-ping = register("ping", ping_callback)
-
-
-counter = 1
-try:
-    while True:
-        time.sleep(2)
-        payload = str(counter).encode()
-        print("sending ping: {}".format(payload))
-        ping.send(payload, "dtn://node2/pong")
-        counter += 1
-except KeyboardInterrupt:
-    pass
-
+import time
+
+from dtn7zero import setup, register, start_background_update_thread
+from py_dtn7.bundle import PrimaryBlock
+
+
+setup("dtn://node2/")
+
+start_background_update_thread(_sleep_time_seconds=0.1)
+
+
+def pong_callback(payload: bytes, full_source_uri: str, full_destination_uri: str, primary_block: PrimaryBlock) -> None:
+    print("sending back pong {}".format(payload))
+    pong.send(payload, full_source_uri)
+
+
+pong = register("pong", pong_callback)
+
+
+try:
+    while True:
+        time.sleep(2)
+except KeyboardInterrupt:
+    pass
+
```

### Comparing `dtn7zero-0.0.4/test/test-bundle-protocol-agent-receiver.py` & `dtn7zero-0.0.5/test/test-bundle-protocol-agent-receiver.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""
-To be run either on CPython or MicroPython.
-
-It must be run in combination with test-bundle-protocol-agent-sender.py, which must be started on another computer.
-"""
-# import gc
-# print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
-# from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-from py_dtn7 import Bundle
-# print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-# gc.collect()
-# print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-
-
-def callback(bundle: Bundle):
-    print('bundle reached receiver endpoint: {}'.format(bundle.payload_block.data))
-
-
-storage = SimpleInMemoryStorage()
-
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://nodeRECEIVE/', storage, router, use_ipnd=True)
-
-receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
-
-bpa.register_endpoint(receiver_endpoint)
-
-# last_garbage_collect = get_current_clock_millis()
-try:
-    while True:
-        bpa.update()
-
-        # if is_timestamp_older_than_timeout(last_garbage_collect, 2000):
-        #     gc.collect()
-        #     print('storage: {}, known-bundles: {}'.format(len(storage.bundles), len(storage.bundle_ids)))
-        #     print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-        #     last_garbage_collect = get_current_clock_millis()
-except KeyboardInterrupt:
-    pass
-
-bpa.unregister_endpoint(receiver_endpoint)
+"""
+To be run either on CPython or MicroPython.
+
+It must be run in combination with test-bundle-protocol-agent-sender.py, which must be started on another computer.
+"""
+# import gc
+# print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+# from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+from py_dtn7 import Bundle
+# print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+# gc.collect()
+# print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+
+
+def callback(bundle: Bundle):
+    print('bundle reached receiver endpoint: {}'.format(bundle.payload_block.data))
+
+
+storage = SimpleInMemoryStorage()
+
+clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://nodeRECEIVE/', storage, router, use_ipnd=True)
+
+receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
+
+bpa.register_endpoint(receiver_endpoint)
+
+# last_garbage_collect = get_current_clock_millis()
+try:
+    while True:
+        bpa.update()
+
+        # if is_timestamp_older_than_timeout(last_garbage_collect, 2000):
+        #     gc.collect()
+        #     print('storage: {}, known-bundles: {}'.format(len(storage.bundles), len(storage.bundle_ids)))
+        #     print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+        #     last_garbage_collect = get_current_clock_millis()
+except KeyboardInterrupt:
+    pass
+
+bpa.unregister_endpoint(receiver_endpoint)
```

### Comparing `dtn7zero-0.0.4/test/test-bundle-protocol-agent-sender.py` & `dtn7zero-0.0.5/test/test-bundle-protocol-agent-sender.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-To be run either on CPython or MicroPython.
-
-It must be run in combination with test-bundle-protocol-agent-receiver.py, which must be started on another computer.
-"""
-
-# import gc
-# print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-# print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-# gc.collect()
-# print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-storage = SimpleInMemoryStorage()
-
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://nodeSEND/', storage, router, use_ipnd=True)
-
-sender_endpoint = LocalEndpoint('sender')
-
-
-bpa.register_endpoint(sender_endpoint)
-
-# print("next free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-
-message_str = 'hello_world {}'
-counter = 1
-
-# print("next free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-
-last_sending_time = get_current_clock_millis()
-try:
-    while True:
-        bpa.update()
-
-        if is_timestamp_older_than_timeout(last_sending_time, 2000):
-            sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://nodeRECEIVE/receiver')
-            counter += 1
-
-            # gc.collect()
-            # print('storage: {}, known-bundles: {}'.format(len(storage.bundles), len(storage.bundle_ids)))
-            # print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-
-            last_sending_time = get_current_clock_millis()
-except KeyboardInterrupt:
-    pass
-
-bpa.unregister_endpoint(sender_endpoint)
+"""
+To be run either on CPython or MicroPython.
+
+It must be run in combination with test-bundle-protocol-agent-receiver.py, which must be started on another computer.
+"""
+
+# import gc
+# print("init free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+# print("after import free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+# gc.collect()
+# print("after import garbage collect free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+storage = SimpleInMemoryStorage()
+
+clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://nodeSEND/', storage, router, use_ipnd=True)
+
+sender_endpoint = LocalEndpoint('sender')
+
+
+bpa.register_endpoint(sender_endpoint)
+
+# print("next free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+
+message_str = 'hello_world {}'
+counter = 1
+
+# print("next free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+
+last_sending_time = get_current_clock_millis()
+try:
+    while True:
+        bpa.update()
+
+        if is_timestamp_older_than_timeout(last_sending_time, 2000):
+            sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://nodeRECEIVE/receiver')
+            counter += 1
+
+            # gc.collect()
+            # print('storage: {}, known-bundles: {}'.format(len(storage.bundles), len(storage.bundle_ids)))
+            # print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+
+            last_sending_time = get_current_clock_millis()
+except KeyboardInterrupt:
+    pass
+
+bpa.unregister_endpoint(sender_endpoint)
```

### Comparing `dtn7zero-0.0.4/test/test-bundle-protocol-agent.py` & `dtn7zero-0.0.5/test/test-bundle-protocol-agent.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""
-To be run either on CPython or MicroPython.
-
-Registers two local endpoints and sends from one to the other.
-"""
-import time
-
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from py_dtn7 import Bundle
-
-
-def callback(bundle: Bundle):
-    print('bundle reached receiver endpoint: {}'.format(bundle))
-
-
-storage = SimpleInMemoryStorage()
-
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
-
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://node2/', storage, router)
-
-sender_endpoint = LocalEndpoint('sender')
-receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
-
-
-bpa.register_endpoint(sender_endpoint)
-bpa.register_endpoint(receiver_endpoint)
-
-message_str = 'hello_world {}'
-counter = 1
-
-try:
-    while True:
-        bpa.update()
-        time.sleep(1)
-        sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://node2/receiver')
-        time.sleep(1)
-        counter += 1
-except KeyboardInterrupt:
-    pass
-
-bpa.unregister_endpoint(sender_endpoint)
-bpa.unregister_endpoint(receiver_endpoint)
-
-
-
+"""
+To be run either on CPython or MicroPython.
+
+Registers two local endpoints and sends from one to the other.
+"""
+import time
+
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from py_dtn7 import Bundle
+
+
+def callback(bundle: Bundle):
+    print('bundle reached receiver endpoint: {}'.format(bundle))
+
+
+storage = SimpleInMemoryStorage()
+
+clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://node2/', storage, router)
+
+sender_endpoint = LocalEndpoint('sender')
+receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
+
+
+bpa.register_endpoint(sender_endpoint)
+bpa.register_endpoint(receiver_endpoint)
+
+message_str = 'hello_world {}'
+counter = 1
+
+try:
+    while True:
+        bpa.update()
+        time.sleep(1)
+        sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://node2/receiver')
+        time.sleep(1)
+        counter += 1
+except KeyboardInterrupt:
+    pass
+
+bpa.unregister_endpoint(sender_endpoint)
+bpa.unregister_endpoint(receiver_endpoint)
+
+
+
```

### Comparing `dtn7zero-0.0.4/test/test-bundle-serialization.py` & `dtn7zero-0.0.5/test/test-bundle-serialization.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-"""
-To be run on CPython or MicroPython.
-
-Tests the correct (de)-serialization of a bundle.
-"""
-from py_dtn7 import Bundle
-
-raw_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00X@LwL2KMBGNgy11Y8Ofa4EYfDultcE7Ulq7b3veSMSKgzvSjDbO0aRVxQYwMInIR4g\xff'
-
-bundle = Bundle.from_cbor(raw_bundle)
-
-print(bundle)
-
-assert raw_bundle == bundle.to_cbor()
-
-flags = bundle.primary_block.bundle_processing_control_flags
-
-print(flags)
-
-assert (flags.is_fragment |
-        flags.payload_is_admin_record << 1 |
-        flags.do_not_fragment << 2 |
-        flags.reserved_3_to_4 << 3 |
-        flags.acknowledgement_is_requested << 5 |
-        flags.status_time_is_requested << 6 |
-        flags.reserved_7_to_13 << 7 |
-        flags.status_of_report_reception_is_requested << 14 |
-        flags.reserved_15 << 15 |
-        flags.status_of_report_forwarding_is_requested << 16 |
-        flags.status_of_report_delivery_is_requested << 17 |
-        flags.status_of_report_deletion_is_requested << 18 |
-        flags.reserved_19_to_20 << 19 |
-        flags.unassigned_21_to_63 << 21 == flags.flags)
-
-flags = bundle.payload_block.block_processing_control_flags
-
-print(flags)
-
-assert (flags.block_must_be_replicated |
-        flags.report_status_if_block_cant_be_processed << 1 |
-        flags.delete_bundle_if_block_cant_be_processed << 2 |
-        flags.reserved_3 << 3 |
-        flags.discard_block_if_block_cant_be_processed << 4 |
-        flags.reserved_5_to_6 << 5 |
-        flags.unassigned_7_to_63 << 7 == flags.flags)
+"""
+To be run on CPython or MicroPython.
+
+Tests the correct (de)-serialization of a bundle.
+"""
+from py_dtn7 import Bundle
+
+raw_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00X@LwL2KMBGNgy11Y8Ofa4EYfDultcE7Ulq7b3veSMSKgzvSjDbO0aRVxQYwMInIR4g\xff'
+
+bundle = Bundle.from_cbor(raw_bundle)
+
+print(bundle)
+
+assert raw_bundle == bundle.to_cbor()
+
+flags = bundle.primary_block.bundle_processing_control_flags
+
+print(flags)
+
+assert (flags.is_fragment |
+        flags.payload_is_admin_record << 1 |
+        flags.do_not_fragment << 2 |
+        flags.reserved_3_to_4 << 3 |
+        flags.acknowledgement_is_requested << 5 |
+        flags.status_time_is_requested << 6 |
+        flags.reserved_7_to_13 << 7 |
+        flags.status_of_report_reception_is_requested << 14 |
+        flags.reserved_15 << 15 |
+        flags.status_of_report_forwarding_is_requested << 16 |
+        flags.status_of_report_delivery_is_requested << 17 |
+        flags.status_of_report_deletion_is_requested << 18 |
+        flags.reserved_19_to_20 << 19 |
+        flags.unassigned_21_to_63 << 21 == flags.flags)
+
+flags = bundle.payload_block.block_processing_control_flags
+
+print(flags)
+
+assert (flags.block_must_be_replicated |
+        flags.report_status_if_block_cant_be_processed << 1 |
+        flags.delete_bundle_if_block_cant_be_processed << 2 |
+        flags.reserved_3 << 3 |
+        flags.discard_block_if_block_cant_be_processed << 4 |
+        flags.reserved_5_to_6 << 5 |
+        flags.unassigned_7_to_63 << 7 == flags.flags)
```

### Comparing `dtn7zero-0.0.4/test/test-bundle-size.py` & `dtn7zero-0.0.5/test/test-bundle-size.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""
-To be run on MicroPython.
-
-Tests RAM usage of (de)-serialization of different payload bundles.
-"""
-import gc
-print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))  # this should always be over 100000
-from py_dtn7 import Bundle
-print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-gc.collect()
-print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
-
-
-raw_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00X@LwL2KMBGNgy11Y8Ofa4EYfDultcE7Ulq7b3veSMSKgzvSjDbO0aRVxQYwMInIR4g\xff'
-
-raw_cat_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00Y\x11\xc8\xff\xd8\xff\xe0\x00\x10JFIF\x00\x01\x01\x00\x00\x01\x00\x01\x00\x00\xff\xdb\x00\x84\x00IIIIMIR[[Rr{m{r\xa8\x9a\x8d\x8d\x9a\xa8\xfe\xb6\xc3\xb6\xc3\xb6\xfe\xff\xf1\xff\xf1\xf1\xff\xf1\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01IIIIMIR[[Rr{m{r\xa8\x9a\x8d\x8d\x9a\xa8\xfe\xb6\xc3\xb6\xc3\xb6\xfe\xff\xf1\xff\xf1\xf1\xff\xf1\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xc2\x00\x11\x08\x01\x94\x02d\x03\x01"\x00\x02\x11\x01\x03\x11\x01\xff\xc4\x00\x18\x00\x01\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\x03\x04\xff\xda\x00\x08\x01\x01\x00\x00\x00\x00\xf4\x01<\xbee\x88/oW@\x00\x14\x02\x06<8\x00:\xfa\xfa\x00\x00\'/\x14\xb1\x01}^\x9a\x00\x05\x10s\xe6N\x18E\x80\xd7\xa7\xb6\xa8\x00\x04\x9e.@\x81zw\xednqu\xaa\x00L\xe71f9\xcc\x10/~\xb7z\xa0\x00\x13\x8f\x88\x00F\xfa\xef-o[\x8bh\x89$\x0c\xf2\xce$\x82\xde\xfa\xbdv\x00\x00\x93\xcd\xe6X\x00\xde\xfb-\xaa\x14\xa9\x10\x99\xd6y\xb1\x9c\xc1\xadw\xeb\xab@\x00\x0c\xe3\xcf\xc0\x02\xe9\xae\xbbZ\xb2*\xe6\xcd\xe36\xa6e\xcc\xces\x98j\xf7\xec\xe9@\x00\x04\xcf\x1e\x1c\xec"\xea\xea\xf4\xd2\xd4.Z\xc6\xf9\xf5\xc4,\xcd\xb9\xces\x9c\x8dk\xbf{\xa0\x00\x01\x13<\xfc\xd2H7n\xf7m\x92h\xcbY\xd6SL\xa2\xd6s0\xc8\xd7n\xba\xdd\xa0\x00\x06d\xce|\xcc\xe4]\xeb[\xd2\xcc\xe3z\xcck\x1a\x99\x9d/;\x96\xac3q2\xba\xed\xd5w@\x00\t\x12q\xf3\xe6\x17z\xdbUf3\xa8]s\xd4\xcbw\x11m\x94\x96jGn\xb1\xaa\x81@\x04&y\xf9\xb1\x17\xae\xf5Hff\x16\xeb\x9e\x99i%\xabi\xabd\xac\xeb\xad\xb6\x02\x80\t$\xc6y\xf2-\xed\xb8\xcce$\x91\xb9*72\xb6\xb4\xd5hF:n\xda\x82\xa8\x00\x893\x9cbt\xb3l\xcc\xc8\x92$\xdc\x84\xbb\xcc\xb6\xb4kMK9o\xd1\xa4\x96!m\x00\x04g\x965\xab*g9\x88\x92I\xa2%\xb2\xe9m\x95\xb5\xaex\xf5u$ [@\x02N9\xce\xb7Q1\x94\x88\x92E\x95)t\xd5\x85j\xd9\x96z\xf6\xd2B\x16\xd5\x00$\xc3\\8\xf5\xe9\x19\x99\x88\x19\xca,k:\xcbV\xea\xc9ih\x93]\xf5\x11\x0b\xab@\x01\x8b\xcb\xcf\xad\xd4\xccDY\x98\x92h\xe9\x9c\xcbkh\xa2\xad\rt\xa4\x16\xea\x80\x04s\xe0\xd5L\xe4%fd\x93[\xdcs\xcd\xa6\xd4\xa4Z\xab7\xb1\r](\x00\xce9\x153\x98\x11fa&\xfa\xeb\x1d|\xa2]\xa2\xd1V\x94\xde\x81\xab\xa5\x00&8\xa93\x99\x0b\x12\xcc\x89:\xf6\xa7\x9a\t\xaa\xaaCM\x06\xf6\r](\x019\xf2X\xced\x02&A\xdf\xb9\x9e\x1c\xd0\xda\x84\x8bm\xa3\xa6\xa8\xb6\xe9@\t\xcb\x08\x99\xceb\xd1\x13!\xae\xfe\x8d\xe2\xf9y`n\x92\xcb\x82\xdbt\xbb\xda\xc5\xb7J\x00N\\\xd13\x9c\x94\xb6D\x90\xbe\xafV\xa6|\\\xa4\xb4]\xeag\x9c\x1a\xd5\xdd\xd6\xb4\x17V\x80\x0c\xf3\xc4fg27l\x98\xa2E\xf6z\xab\x1e?9f\xfa\xe7[q\xc6j]n\xdb\xadQm\xb4\x00\x93\x9efs\x89\x98\xba\xdd\xea\xc7W.\x0c\xd7\xaf\xd9\\\xbc|eu\xef\xa6s\xcac55\xbbn\xb5t\x8bm\xa0\x04\x98\xc4\xcefs,on\xbd\x13\x97,\xc9\xaf_\xa7S\x1eo65\xbbw\xac\xe6s\x90\xb7v\xebwVE\xb6\xd0\x02fba\x9c3\x15\xae\x85\x89\x9c;z\xb7\xa99\xf9\xb8/EFr\x85\xd6\xf4\xd6\xf4\xa8[h\x011\x139\xceq\x05j\x88\xcez\xfa:\xf439\xf8\xf3kQ\x11\x0bwn\xb5\xab\xa4\x96\xd5\x00&s.s\x9cg-b\xdbe\x88\xbe\xae\xd9\xe9S3\x8f\x91\xa1Q\x99Z\xd5\xb7[\xba\xb2-\xaa\x00e\x98\x98\xces\x996\x827\x1d\xbd5FN\x1ex\x85\xd6Ke\xdd\xba\xdd\xa8[h\x00bFfs\x8c\xc2\xead\xd2\xef\xbf@\x89\x8e\xae\x1c\xf3\x99nm\xde&\xadk\xa5T[U@\x132&q&p\x1a\xb9\xd6\xb7\xd7\xad\xc7\x9e\xba1\xcezw\x9c\xe11I*\xe8\xb6\x81h\xe8\x01"Dc13\x08\xdb}\xf7\xb6x\xf2\xc7G=\xf6\xe8\x9a\x87&nu4\xcem\xaa\x82\xa9\xd0\x04\x11\x19\x9c\xf3&b\xed\xad\xf5\xe9\xa5\x939\xe7:n\xdc4g8\xcdi\x0c\xda\xa4\x15N\x80 \x91.s\x8c\xc4j\xed\xbe\x9a\xd4\xb2I\x8c\xefT\xcd\xcb,\xa4\xb6UR\x02\xa9\xd0\x06f\x89\x913\x94\x91W}\xf4&s\x85\x8d\xe94e.\x18\x16\xa8 \xaa\xe8\x02gZ\x93(g9\xcc.\xee\xfa\xd1\x9c\xe7ZI\x9d[br\x90j\x96\xd0\x90Z\xba\x00\xce.\xad\x92I#8:N\x9d4g\x12\xd2\x91\xba\xb9\xe1.u\xbbB\xd31\x0bj\x80\x98\xa5\xa4\x82H\x9c\xf7\xad\xe8\xcf>\x96\xa5&oD\xe7\x9c5v[A\x96b\xd5\xb4\t\x9c\xea\xe8!\x14\x9c\x8c^\xba\x98\xd6\xb4F\xa33Vc,\xddn\xac\x8dY\x98\xc8\xb5t\t\x9eZ\xde\xaaU \x13\x96u5kJ\x8dD$\x91\xb5TT#\x11Kn\x811\xce\xebZ\xdaE!i\x98\x90Y\xa4\xa0\x1a\n\x88T\x92H\x0bv"q\x97{\xdd\x90[\x93U\x04\xcc\x82\xa5)mR\x19J\x96fdJ\xb5\xd0\x93\x1c\xe5\xd6\xf4h\x14Z\x94\x89 \x94\xb5T\x12Y\x99S53\x0b-^\x84\xc7<\xda\xb7z*\xa2\xa9e\t \xd4i(E\x8b1%\x91q\x92\x8b]L\xe3\x9en\x8d][V\x90\x9a\xa0\x12\xc5\x00#P\x98\x913.EYk\xaaLbJ\xd5\xba-n\xc2M\x014Q,"\xa4j\xc8\xe7\x98\xceT\xa0[\xd13\x89"\xdb\xb3y\x97z\x9a\x85\x88F\xa8\xa8!\x05\xa93\xca\x0c\xd6\x90E]i$k\x91\xab\xab%j75\x9d$\x1b\x84\xd1,\x92Z\xaabs\xc4\x03QD/D\xc0\x92\xb5l\xb4\xa5\x15\x81\xabfn\xcc\x8b\x95\xb5d\xc6q\x86\xb1\xa8\xb5\x9dX\x0e\xf9\xc6\x05\xa3B\xaeuP\xb9h\x95\x99\xba\xcbSIm\x96\xf3c\x19Y,\xba\x99\xd6\xb0\x15\xff\xc4\x00\x16\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\xff\xda\x00\x08\x01\x02\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x04P@P\x00\x00@\x00\x94\xa0\x00\x01\x00\x00\x14\x00\x00 \x00\x00\xa0\x00\x08\x00\x00\n\x00\x01\x00\x00\x02\x80\x00@\x00\x00\x14\x00\x08\x00T\x00\x14\x00 \x01D\x00\x05\x00\x80\n\x02\x00\x94\xa0\x10\x14\x8a\x11H\x12\xa8\x02\x01\xa2\x00\xa9\x00P\x04\x00( \x01@\x08\x14\x85\x04\x00\x95@\x10\x01HP P\x02\x00Q\x14\x02\x14\x00 \n\x00\x08P\x00 \x14\x00@\xa0\x00 (\x01\x02\x91@\x8a\x00\x00\x00AB\x14E\x00\x00 \x14\x80\xa0\x00\x01\x00\x15\x00P\x00\x02\x00*\x00\x02\x80\x08\x00X\x00\x01R\x82\x12\x80\xff\xc4\x00\x16\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\xff\xda\x00\x08\x01\x03\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x05@P@\x00\x00P\x00\x08\xb0\x00\x00\xa0\x01a\x16\x00\x00(\x00\x00\x80\x00\x05\x00\x00\x08\x00\x01@\x00\x02\x00\x00P\x00\x00\x10\x00\n\x00\x85\x00\x10\x00(\x01\x05\x00\x10\x00\xa0\x08\x02\x81R\x00\x14\x00\x81H\xa2\xa4\x00(\x12(,\x14S \x05\x00 (\n\x90\x00\xa1\x14EE\x01R\x00\x16\xa0\x02\x99\x02\x84\x00(\x04.\x99\x80)\x00\x02\x80\x85\xa8\x80\xa4\x00\x02\x81\x14\x10\xa0\x80\x00(\x00\x00!`\n\x82\xa0\x00P\x02\x02\x90T\x00\x00\xa0 \xa0\x80\x00\x01@A@AH\x00U@"\x80\x00E\x11T@J)\x00\x00\x05\x08\x0f\xff\xc4\x00/\x10\x00\x02\x02\x01\x03\x03\x03\x02\x06\x02\x03\x01\x00\x00\x00\x00\x00\x01\x02\x11\x10\x12 !01A\x03@Qaq\x13"2BR\x81b\x91#P\xa1\xd1\xff\xda\x00\x08\x01\x01\x00\x01?\x00\xe8z\xd1\xe9&\xd1\x1fY\xa2\x13R\xf7\xf3\x9a\x8999>\xa4\x11\x1fi>P\xd5>\x9am\x10\xf5\x84\xd3\xf6\xf6Jt~#\x1c\xd8\xa6\xe8\x94\xd9&\xdfR*\xd9\x15BK\xda4z\xb1\xa7\xd5\x8f\xa8\xe2/Y\x1a\xd0\xa4\x98\xdaF\xb4?PS\x14\x84\xfa\x966X\xd5\x9aJ\x12\xe0Hq$\x86\xb8\xe9zQCbf\xa1{?V6\x86\xab\xac\x9b\xa2\x13cm\x8a\xd9\xa4HB,\xb2\xcb/e\xf4Q\xe4\x90\xc6\x86\xb9\xde\xb0\x8a\x15\x91^\xd1\xa3\xd4\x80\xd5uZ\xe0\x8a\x1a\xe0\xae\x11Et,\xb2\xf3e\x8cye\x8d\x8d\x8f\xbe\x1f}\xe8K\x92(I\n\xbd\xb3\x898t\xe8H\xf8"<\xac\xb2\xf0\xdf\x04Ye\x8c\xd5\xce\x18\xdf%\x97\x8b/\x08c,l{\x91\x08\n"\x13^\xd9\xb2V\xc9G\x15\xb9lB\x18\xb0\x86\xc6\xf6I\x88b|\xe1\xbeK\xe0\xbc\xa6x\x1e>1\xdd\x92c\xe2\x96\x1e\xe4E\xb15\xe7\xdc\xb4J)\x92\x8d\x08kj\xc2\x16#\x84<X\xde\xe7\xd8\xb2\xc9\x17\xc0\x9d\xb1\x0f\x1e\x19xX\xec.YV\xc6\x86\x9b+j\x8c\x99\x195\xe0R\x8b5P\xa4_\xb6vQ(\xd8\xe2\xe2\xc7\xbda\x0bk\x18\x9e,g\xc6\x1fv!\xf9\x13<\x89\x8b\xb9|\x9e1\xe0]\xb3\xdb\x14\xe4\xc7H\xab\x1b\xf0\x8a(\xa16\x88\xbf\x98\x95\x17\xe0R\xc2\xf6\xed,z\x8a\xd0\xc7\x9a\x12\x12\x14D\x8a\xde\xc4\xc7"\xf1\xe5!\x0c\xec\x86\xcf(}\xc8\xf7\x13\xe3\x16x\xc2\xcf\x92\xac\xbf\x08\xd2}\x10\xa0~\x1a\x1cD\xda\x14\x88\xbbgb\x93;p/p\xc9Y-\x89\xb4E_1\x12^\n;\xad\x8cLom\x96#W\x03,\xf2\'\x84X\xcf(]\xc4,\xa1\xf0\x85\xc1BU\x86T\x98\xa3CQ+\x91M\xa1I1\xa1{m_A\xb9\x1f\x9d\x8e\x0f\xe4pc\x8b(\xd0i\x7f\x02^Q\x17{\x9fEe2\xc7\x85\xdb\x0cX\xf0\xb0\xbc\x88\xbe\xc7\x91,-\x8d\x94\xcam\xf7\x14\x11\xa4M\x8b\xdbP\xceGe1\xc6\xc7\x03D\x84\xda\xee\x87\x18\xb3KYx\xbe\xf9X{o)\xe6\xf1xB\xec,.\xf8]\xcf"y\xef\x86\xcd\\\x91NB\x82Yh^\xe5\x92\x9f\x84&\xfc\x96&\x86\x8a\xf8\x10\xf0\xcb\xdc\xf2\xf0\x9eVP\xdf\x02\xc2\xee!a\xec\xf0!\xe6bDd\xbd\xf4\x9d\xf0\x8a;\nG\x1b,\xb1\xbd\xff\x00;\x90\xc4w\xbc\xc8G\x91y\xfb\x0b\xa3e\x96w\x18\x9bD}AI?w!B\x8aH\x9b\x8e"\xd9x\xbe\x8b\x17m\x8f/\x15P\xfb\xb1\x08x}\xc5\xe7\xed\x84\xac|\xe5l\xb1\xbcV(h\x8b\xa1?u\\\xde\'#\x96\xc4\x84\xb2\xd8\xde^>\x83<\x0fk\xc2\xc5\rp5O\xec-\x8b\xb3\xc7d\xb0\xf0\xb7\xde(\xa5\x84\xc4\xfd\xd4\xe4;b+c{\x13_\'\x08\xfe\xca\xb4.\xd4=\x8f+\xbaBB_\x9d\xb1\xf6+\xf53\xb4^\xcf\x02\x1b\xb7e\x1c\x16\xbe\x11k\xe0\xe0\xe0\xaf\xaa\xc5\x8b\x16-\x89\x97\xed\xd8\xe5Cv%\xb5\x8d\x96\xf7.0\xf7\xc0\xa4\x90\xad\xc5\xfc\xb2Q$\xb8\xa2B\xd8\x8b\xaf\xbe/m\x96^8\xdc\x85\xed\xe4;\xdc\xcb\xdbY\xbe\x8f\xa4\xae\xc6\xb8\x97\xd9\x11\xe2\r\xbf\x04#\xf9\xa3\xf4X\x99\xe1m]\x1b,M\xe1R/6/o!\xe2\xd6/u\xef{\xfd#\xff\x00\xa9\t\\\x17\xd6C\xf3/\x96Sm\xc4\xf5Q\xfbv\xa5\xb1\x97\x86_E\x0b\xdb\xcbs\xd9LI\xee\xad\xe9Y\xe9r\xc4\x96\xa7\xf4hJ\xb4\x92\x8d\xb4\x8f,\xf5\x1f\xe6g\x87\xb5Y\xc1E\x97\x86\x8a\x19e\x96Z/\x0b+\xdb1\xe5\x8b\x0fu\x97\x8a\x1f\x19\xa2\xb6\xfa\x02]\xfe\xaf\x15\xdcg\xab\xfa\xd9\xe1o\xd5BV(\x8a$\xd0\xf8\xcdl\xa6S++\xda\xb1\xedl\xbc\xd8\x844i\xb3H\xd3F\xa6s\xf0Z/j=\r\x92\xecz\xabta)\x9f\x80O\xd2\xe3\x820\xa4Q\xca\x1b\xb6<V)\x89\x0b\x0b\x08\xe0^\xd5\x8f/\x17Lv\xb7.H\xba\xe0\xa3J\x1f\xa5r\xb1Dp\x83\xee\x89z+\xc3\x1cZyH\xf3\xc9\xe9J\x85\x99\x93\xbe\x16P\x93=4\x97tYxct96?\xa6\xe4"\xb2\x8a\xf6\xecxxh\xfa1\xa6\xb6\xa6w\x13q#$\xf2\xd8\xe4;c\x1e\x12\x94\x8fN4\xd8\xb3"V5M\xd7\xce,K\xb3\x1f\x02m\nF\xb1\xb6\xcf\xb8\xda\x1e\xfb\xe0BG\x02e{f1\xa1\xacP\xd0\xcb]\x98\xd3[Q\xe0\xa4\x7fe\xcb\xe5\xe3\xc0\xfbf*\xd9\x06!\x16^%\x1b\'\x1a\x93\xb3\xb3\xc7)\x8d\x8b\x16Yc,\xec\xb3\xc6\x10\xb2\x85\xed\xde\xca\x1a\xc3\x1a\x13\xf0\xfb\r5\xf6\xc53\x8c&\xde\xf6\xf8\xc4\x13\xa20\xa1lx\x9clpj\xf0\xf7<w\x1b\xfaf\x8a\x12\xd8\xb2\xbd\xab\xd8\xc7\x87yM\xa3J\x971\xff\x00G%\xbcY\xcdv9\xc3x\x91\\\x1c\xf1\xc1\x04\xd9\xe0\x88\x9e^\x19\xea.\x07\x1c\'\x9b/\x1c\x8e\x92\xa3\x9d\x8a\x1e_\x08\xfa.\x10\x92Y^\xe6\x8a\xc3\x1a\xc3\xdbj\\K\xfd\x8e\r}Q\xc9e\xbb\x1eP\xf9\x12 \xbcP\xad,%\xc6,\xbc\xd8\xd2d\xe05\xb5<q\x1f\xbe\x17\xdb\n\r\x97\x18\xf6\xe5\x96\xdb\xe7<a{\x87\xba\xd0\xc6=\x89\xca/\x86~I\x7f\x8b\x1aq\xee\xb0\x9a\xec\xfb\r4#\x91&%"\nE\xe2\xcb,\xb2\xcb5P\x9d\x8c\x94G\x1f\xa1\xa0pf\x96(6v\xe2&\x96S\x14d\xfc\x15\x18\xff\x00\x93\x1e\xa9w)\x8a,J\xb1BB\xd9e\xe2\xcb-\x16\x8bE\xae\x9d\xedc\x1eZ\x1d\x1clSk\x8f\x1f\x06\x98K\xf4\xff\x00\xa6U:h_\x0f\xb1\xa6\x85\x14\xc8\xc1/"\x82\xf8O\x12C\x9b\x83\x1f\xab\x1e\x05\xea\xc5\xba,L\x9f\xa8\xa2/UY\xcc\xd9\x08\xb4\x86P\xd2(I\xcb\xb1\xa7\xe1X\xf9\x14[\xec\x8aK\xbc\x8bK\xb2\x1bo\xbb\xc53\x8c%\xff\x00CM\x8e\x1fT\x8a\x8f\xcb-x\x81\xa9\xfcG\xfd\x0f\xd4\xf5>O\xc5\x99\xady\x84O\xf8\xbf\xca&\x86\xfbI1\xa6\x8a/\xc4\x95\x94\xbc1\x11DsVN\x1a\x87\xe8\x8f\xd2\xa3\x9a/\x81CT\x98\xbd\x120HH\x92\xa2)6Ti\xbd&\x85J\xd3dc\xa5\xc9x\xa2:\x12\x95&T\\d\xd2\xe5\x12\x8f\x8f\xf1\x1aQQ\xe1\x15\x05=4/\xa4[e~h\xf8\xb4&\x9a\x93\xd2\x8d\x15KE\x9a+W\x16\xc7\xf4U\xef\xa9|\x9c/\x05\x8e\xc6\x86\xb3[4\x8aR\xfb\xa2\xd7\xd5\x14\xc8\xa5\xf5\x14D\xb3ea\xa1\xa2Q#\x1b\x12)\x1cbD;\x8f\xf3y-4\xb9\xa15o\x914\x9c\x95\x9e\x9f\x13hrNSvK\xf6\xfd\x86\xd6\xbb;\xc6\x84\xb9\x8f\x0e\x92+W\x1a\x87\xa6\\\xea*?$\x9au\xc9^\xe6\xfa\r\x0ck\r%\xe4\xd2\xdfh\xb68O\xf83G\xa9\xfc$(z\xbf\xc5\x9ag\xfc\x18\xa35\xfbYMx\x90\x9f\xd1\x89\x8bm\x97\x86\xc8\xb2-\xd7;$+\xbe\x06\xe5\x96\xbe\x86\xbd<\x16\x8b-\xff\x00\x99\xfd1:|#[\xc7?\x07\xf5\xbe\xd7\xb2{Z\xdc\xd2)\x1c\xae\xd2\x8a\x1a\x93\xee\xff\x00\xf4\xd1\xf5F\x95\xfc\xa2T?\x90\xb4\x7f&q\xfblN_,W\xfc\x88\xad\x8f-\x8eBV8\xa2\xd8\xa4Z\xc4\x84&\x97\x91\xb4Z\xf98\xae\xe3\x94II|\xf1\xc8\xed&\xf5\x1a\xd7\xf25\xd2\xfdV\xc6\xed\xf7-\xfc\xb2\xdfJ\xbd\x8b\xcd\x15\xd2w\x8a(\xa1,-\xcd\x8d\x89\x15\x9aE\x15BeY\xa4\xd2i4\x8d\x15}\x8a~\x1a\x7f\xf8\xce<\xa7\x13O\xc4\x934M~\xd6.Je\x14QE\x14i4\x9a\r&\x92\x8a(\xa2\x8a(\xae\x93\xa3Q\xa8\xd4^\xca+\x15\x8d#C,H\xd0\xeb\x96\x928]\xb9"\x9f\x7f\x02\xcd\x8c\xb3\xbfE<\xde8$\xa8s\xf15bo\xc3\xd4\xbe\x19P~\x1cE\t.S52\xd7\xc1H\xa2\xb7Y\xa8\xb2\xcb\xf6\x0c\xa2\x8d%f\x8a\xcdf\x8d\'\xe1\xbf<#Z\x8f\xe8Cm\xbbdb\xbb\xb1\xc9\x89\x9a\xbf\xd1\xce\x1b9\x93\xc5P\x96h\xac1\xaf"x\xab\xc4\x99k\xcf\xe9c\x8e\x97\xc9K\xc1\xaa\xfb\xab\x14|\xa2\xfey)\x14\xd6-\xe3\x8fn\xd9b\xb2\x8a\xcd\x97\x8a\xdbG\xd8j\xc7\x11*\xe5\x8f\xb5\xc8\xb6\xdd\x96vi|\x1a\xb8\xfe\xc6\xf0\x90\xba\x89\xf6\x1b\xa6<v\xfb\x0e"BX\xac\xb5\xb9\x96_\xb0c\x10\xb6Q[\xab\x15\x9a\x1cm\xdb%\x16\xd9\xa4\x8a\xe5\x1d\xdb<D\xf1\x86,\xbc-\xade\xf2\x8am\x14$\xd1E\x14V\xfb,\xbc\xff\x00^\xc2L\xb1\x08\xb3\xb8\x96\xdb\xdc\xb3CF\x92\xb8e\x0f\xc6|\x9e\x0f\x8e\xa5b\x8a+\xaf}v2\xd6R\x11e\x97\xec\x18\xd1]Z+\xa6\xf6&X\xdb\xd9\xfd\xe6\xbam\x8eO)\x88\xb4j9b^\xce\x8a\xd9X\xa2\x8a\x12(\xa1.\x9b\xd9g\x18N\xcb/\xae\xc6\xf6\xf3\x84^\xd4\x87\xec+uu+(y\xb2\xc7\x85C\x1d\xee}\x16\x87\x9a[\x13\xdc\xb1C[/\xa9E\x15\xd6YC\xc5\xe1\x16\x87X\xf0\xc6\xf1]K\x1b\x1e,\xb2\xf6\xd9\xdf\x16\'\x85\xb1\x89m\xbcX\xbd\xb3\xc3\x18\xcb\x13\xe5\x1f\x98xWh\xe5m\xb3\x81\x8b6\xb0\xda\x1bC\xd9X\xb1Y[\x96.\x90\x9e\xc5\xb2\xf6/od\x99\xa9\xf9G%\x96I\xf2\xcb\xc5!\xa5ef\xf6-\x9ax\x1e\x92\xa3\x7f\xd0\x92hj<\xf1\xd9\x95\x1bf\x8e\xfb;a\x1c"\xf1Yb\xcbbe\xe2\xf1x\xef\xb6\xfa6^\xc5\xb1\xbc6]\x17\x86\xe8k\x96V[|\x17\xd2\xa6r\x87&93S\xaa\x1c\x9b53S\xdd{/,[\xaco\x0b\x17E\x9666"\xf1e\x96_Aa\x8f\x12\x1b\xa5\xb2C\xe1\xb2\xcbX\xf8\xcd\xbcYy\xb2\xf0\xc7\xd2\xf1\xb5t\x9b\x11\xe3,Ce\xf3\x85\x8b\x1btG\xa8\xc6_\x0cL{\x12\x1f-\xe1a\xf6C\xee!\x16\xd8\x87\xb2\x8f\xff\xc4\x00\x16\x11\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x11P\x90\xff\xda\x00\x08\x01\x02\x01\x01?\x00jn\x0f\xff\xc4\x00\x19\x11\x00\x03\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x11P\x80\x90\xff\xda\x00\x08\x01\x03\x01\x01?\x00\xe2\xdc\xc3\xd1\x0c\xba\xe3\xff\xd9\xff'
-
-actual_bundle_size = len(bytearray(raw_cat_bundle))
-print("\nactual bytearray length (actual size of bundle): {}".format(actual_bundle_size))
-
-gc.collect()
-before = gc.mem_free()
-bundle = Bundle.from_cbor(raw_cat_bundle)
-after = gc.mem_free()
-gc.collect()
-after_collect = gc.mem_free()
-
-deserialized_bundle_size = before-after_collect
-print("\ndeserialized bundle:")
-print("free before: {}, object size without collect: {}, object size with collect: {}, garbage collected: {}".format(before, before-after, deserialized_bundle_size, after_collect-after))
-
-gc.collect()
-before = gc.mem_free()
-bundle_bytes = bundle.to_cbor()
-after = gc.mem_free()
-gc.collect()
-after_collect = gc.mem_free()
-
-serialized_bundle_size = before-after_collect
-print("\nbundle bytes:")
-print("free before: {}, object size without collect: {}, object size with collect: {}, garbage collected: {}".format(before, before-after, serialized_bundle_size, after_collect-after))
-
-
-print("\nbundle_bytes length (actual size of again serialized bundle): {}".format(len(bytearray(bundle_bytes))))
-
-
-print("\nthis show (garbage collected) that compared to the actual size that factors are: serialized bundle -> {}, deserialized bundle -> {}\n".format(serialized_bundle_size/actual_bundle_size, deserialized_bundle_size/actual_bundle_size))
-
+"""
+To be run on MicroPython.
+
+Tests RAM usage of (de)-serialization of different payload bundles.
+"""
+import gc
+print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))  # this should always be over 100000
+from py_dtn7 import Bundle
+print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+gc.collect()
+print("free: {}, used: {}".format(gc.mem_free(), gc.mem_alloc()))
+
+
+raw_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00X@LwL2KMBGNgy11Y8Ofa4EYfDultcE7Ulq7b3veSMSKgzvSjDbO0aRVxQYwMInIR4g\xff'
+
+raw_cat_bundle = b'\x9f\x88\x07\x1a\x00\x02\x00\x04\x00\x82\x01l//node1/ping\x82\x01h//node1/\x82\x01h//node1/\x82\x1b\x00\x00\x00\xa8\xb0R\x18\xb8\x00\x1a\x006\xee\x80\x85\n\x02\x00\x00D\x82\x18 \x00\x85\x01\x01\x00\x00Y\x11\xc8\xff\xd8\xff\xe0\x00\x10JFIF\x00\x01\x01\x00\x00\x01\x00\x01\x00\x00\xff\xdb\x00\x84\x00IIIIMIR[[Rr{m{r\xa8\x9a\x8d\x8d\x9a\xa8\xfe\xb6\xc3\xb6\xc3\xb6\xfe\xff\xf1\xff\xf1\xf1\xff\xf1\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01IIIIMIR[[Rr{m{r\xa8\x9a\x8d\x8d\x9a\xa8\xfe\xb6\xc3\xb6\xc3\xb6\xfe\xff\xf1\xff\xf1\xf1\xff\xf1\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xc2\x00\x11\x08\x01\x94\x02d\x03\x01"\x00\x02\x11\x01\x03\x11\x01\xff\xc4\x00\x18\x00\x01\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\x03\x04\xff\xda\x00\x08\x01\x01\x00\x00\x00\x00\xf4\x01<\xbee\x88/oW@\x00\x14\x02\x06<8\x00:\xfa\xfa\x00\x00\'/\x14\xb1\x01}^\x9a\x00\x05\x10s\xe6N\x18E\x80\xd7\xa7\xb6\xa8\x00\x04\x9e.@\x81zw\xednqu\xaa\x00L\xe71f9\xcc\x10/~\xb7z\xa0\x00\x13\x8f\x88\x00F\xfa\xef-o[\x8bh\x89$\x0c\xf2\xce$\x82\xde\xfa\xbdv\x00\x00\x93\xcd\xe6X\x00\xde\xfb-\xaa\x14\xa9\x10\x99\xd6y\xb1\x9c\xc1\xadw\xeb\xab@\x00\x0c\xe3\xcf\xc0\x02\xe9\xae\xbbZ\xb2*\xe6\xcd\xe36\xa6e\xcc\xces\x98j\xf7\xec\xe9@\x00\x04\xcf\x1e\x1c\xec"\xea\xea\xf4\xd2\xd4.Z\xc6\xf9\xf5\xc4,\xcd\xb9\xces\x9c\x8dk\xbf{\xa0\x00\x01\x13<\xfc\xd2H7n\xf7m\x92h\xcbY\xd6SL\xa2\xd6s0\xc8\xd7n\xba\xdd\xa0\x00\x06d\xce|\xcc\xe4]\xeb[\xd2\xcc\xe3z\xcck\x1a\x99\x9d/;\x96\xac3q2\xba\xed\xd5w@\x00\t\x12q\xf3\xe6\x17z\xdbUf3\xa8]s\xd4\xcbw\x11m\x94\x96jGn\xb1\xaa\x81@\x04&y\xf9\xb1\x17\xae\xf5Hff\x16\xeb\x9e\x99i%\xabi\xabd\xac\xeb\xad\xb6\x02\x80\t$\xc6y\xf2-\xed\xb8\xcce$\x91\xb9*72\xb6\xb4\xd5hF:n\xda\x82\xa8\x00\x893\x9cbt\xb3l\xcc\xc8\x92$\xdc\x84\xbb\xcc\xb6\xb4kMK9o\xd1\xa4\x96!m\x00\x04g\x965\xab*g9\x88\x92I\xa2%\xb2\xe9m\x95\xb5\xaex\xf5u$ [@\x02N9\xce\xb7Q1\x94\x88\x92E\x95)t\xd5\x85j\xd9\x96z\xf6\xd2B\x16\xd5\x00$\xc3\\8\xf5\xe9\x19\x99\x88\x19\xca,k:\xcbV\xea\xc9ih\x93]\xf5\x11\x0b\xab@\x01\x8b\xcb\xcf\xad\xd4\xccDY\x98\x92h\xe9\x9c\xcbkh\xa2\xad\rt\xa4\x16\xea\x80\x04s\xe0\xd5L\xe4%fd\x93[\xdcs\xcd\xa6\xd4\xa4Z\xab7\xb1\r](\x00\xce9\x153\x98\x11fa&\xfa\xeb\x1d|\xa2]\xa2\xd1V\x94\xde\x81\xab\xa5\x00&8\xa93\x99\x0b\x12\xcc\x89:\xf6\xa7\x9a\t\xaa\xaaCM\x06\xf6\r](\x019\xf2X\xced\x02&A\xdf\xb9\x9e\x1c\xd0\xda\x84\x8bm\xa3\xa6\xa8\xb6\xe9@\t\xcb\x08\x99\xceb\xd1\x13!\xae\xfe\x8d\xe2\xf9y`n\x92\xcb\x82\xdbt\xbb\xda\xc5\xb7J\x00N\\\xd13\x9c\x94\xb6D\x90\xbe\xafV\xa6|\\\xa4\xb4]\xeag\x9c\x1a\xd5\xdd\xd6\xb4\x17V\x80\x0c\xf3\xc4fg27l\x98\xa2E\xf6z\xab\x1e?9f\xfa\xe7[q\xc6j]n\xdb\xadQm\xb4\x00\x93\x9efs\x89\x98\xba\xdd\xea\xc7W.\x0c\xd7\xaf\xd9\\\xbc|eu\xef\xa6s\xcac55\xbbn\xb5t\x8bm\xa0\x04\x98\xc4\xcefs,on\xbd\x13\x97,\xc9\xaf_\xa7S\x1eo65\xbbw\xac\xe6s\x90\xb7v\xebwVE\xb6\xd0\x02fba\x9c3\x15\xae\x85\x89\x9c;z\xb7\xa99\xf9\xb8/EFr\x85\xd6\xf4\xd6\xf4\xa8[h\x011\x139\xceq\x05j\x88\xcez\xfa:\xf439\xf8\xf3kQ\x11\x0bwn\xb5\xab\xa4\x96\xd5\x00&s.s\x9cg-b\xdbe\x88\xbe\xae\xd9\xe9S3\x8f\x91\xa1Q\x99Z\xd5\xb7[\xba\xb2-\xaa\x00e\x98\x98\xces\x996\x827\x1d\xbd5FN\x1ex\x85\xd6Ke\xdd\xba\xdd\xa8[h\x00bFfs\x8c\xc2\xead\xd2\xef\xbf@\x89\x8e\xae\x1c\xf3\x99nm\xde&\xadk\xa5T[U@\x132&q&p\x1a\xb9\xd6\xb7\xd7\xad\xc7\x9e\xba1\xcezw\x9c\xe11I*\xe8\xb6\x81h\xe8\x01"Dc13\x08\xdb}\xf7\xb6x\xf2\xc7G=\xf6\xe8\x9a\x87&nu4\xcem\xaa\x82\xa9\xd0\x04\x11\x19\x9c\xf3&b\xed\xad\xf5\xe9\xa5\x939\xe7:n\xdc4g8\xcdi\x0c\xda\xa4\x15N\x80 \x91.s\x8c\xc4j\xed\xbe\x9a\xd4\xb2I\x8c\xefT\xcd\xcb,\xa4\xb6UR\x02\xa9\xd0\x06f\x89\x913\x94\x91W}\xf4&s\x85\x8d\xe94e.\x18\x16\xa8 \xaa\xe8\x02gZ\x93(g9\xcc.\xee\xfa\xd1\x9c\xe7ZI\x9d[br\x90j\x96\xd0\x90Z\xba\x00\xce.\xad\x92I#8:N\x9d4g\x12\xd2\x91\xba\xb9\xe1.u\xbbB\xd31\x0bj\x80\x98\xa5\xa4\x82H\x9c\xf7\xad\xe8\xcf>\x96\xa5&oD\xe7\x9c5v[A\x96b\xd5\xb4\t\x9c\xea\xe8!\x14\x9c\x8c^\xba\x98\xd6\xb4F\xa33Vc,\xddn\xac\x8dY\x98\xc8\xb5t\t\x9eZ\xde\xaaU \x13\x96u5kJ\x8dD$\x91\xb5TT#\x11Kn\x811\xce\xebZ\xdaE!i\x98\x90Y\xa4\xa0\x1a\n\x88T\x92H\x0bv"q\x97{\xdd\x90[\x93U\x04\xcc\x82\xa5)mR\x19J\x96fdJ\xb5\xd0\x93\x1c\xe5\xd6\xf4h\x14Z\x94\x89 \x94\xb5T\x12Y\x99S53\x0b-^\x84\xc7<\xda\xb7z*\xa2\xa9e\t \xd4i(E\x8b1%\x91q\x92\x8b]L\xe3\x9en\x8d][V\x90\x9a\xa0\x12\xc5\x00#P\x98\x913.EYk\xaaLbJ\xd5\xba-n\xc2M\x014Q,"\xa4j\xc8\xe7\x98\xceT\xa0[\xd13\x89"\xdb\xb3y\x97z\x9a\x85\x88F\xa8\xa8!\x05\xa93\xca\x0c\xd6\x90E]i$k\x91\xab\xab%j75\x9d$\x1b\x84\xd1,\x92Z\xaabs\xc4\x03QD/D\xc0\x92\xb5l\xb4\xa5\x15\x81\xabfn\xcc\x8b\x95\xb5d\xc6q\x86\xb1\xa8\xb5\x9dX\x0e\xf9\xc6\x05\xa3B\xaeuP\xb9h\x95\x99\xba\xcbSIm\x96\xf3c\x19Y,\xba\x99\xd6\xb0\x15\xff\xc4\x00\x16\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\xff\xda\x00\x08\x01\x02\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x04P@P\x00\x00@\x00\x94\xa0\x00\x01\x00\x00\x14\x00\x00 \x00\x00\xa0\x00\x08\x00\x00\n\x00\x01\x00\x00\x02\x80\x00@\x00\x00\x14\x00\x08\x00T\x00\x14\x00 \x01D\x00\x05\x00\x80\n\x02\x00\x94\xa0\x10\x14\x8a\x11H\x12\xa8\x02\x01\xa2\x00\xa9\x00P\x04\x00( \x01@\x08\x14\x85\x04\x00\x95@\x10\x01HP P\x02\x00Q\x14\x02\x14\x00 \n\x00\x08P\x00 \x14\x00@\xa0\x00 (\x01\x02\x91@\x8a\x00\x00\x00AB\x14E\x00\x00 \x14\x80\xa0\x00\x01\x00\x15\x00P\x00\x02\x00*\x00\x02\x80\x08\x00X\x00\x01R\x82\x12\x80\xff\xc4\x00\x16\x01\x01\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x02\xff\xda\x00\x08\x01\x03\x10\x00\x00\x00\x00\x00\x00\x00\x00\x00\x05@P@\x00\x00P\x00\x08\xb0\x00\x00\xa0\x01a\x16\x00\x00(\x00\x00\x80\x00\x05\x00\x00\x08\x00\x01@\x00\x02\x00\x00P\x00\x00\x10\x00\n\x00\x85\x00\x10\x00(\x01\x05\x00\x10\x00\xa0\x08\x02\x81R\x00\x14\x00\x81H\xa2\xa4\x00(\x12(,\x14S \x05\x00 (\n\x90\x00\xa1\x14EE\x01R\x00\x16\xa0\x02\x99\x02\x84\x00(\x04.\x99\x80)\x00\x02\x80\x85\xa8\x80\xa4\x00\x02\x81\x14\x10\xa0\x80\x00(\x00\x00!`\n\x82\xa0\x00P\x02\x02\x90T\x00\x00\xa0 \xa0\x80\x00\x01@A@AH\x00U@"\x80\x00E\x11T@J)\x00\x00\x05\x08\x0f\xff\xc4\x00/\x10\x00\x02\x02\x01\x03\x03\x03\x02\x06\x02\x03\x01\x00\x00\x00\x00\x00\x01\x02\x11\x10\x12 !01A\x03@Qaq\x13"2BR\x81b\x91#P\xa1\xd1\xff\xda\x00\x08\x01\x01\x00\x01?\x00\xe8z\xd1\xe9&\xd1\x1fY\xa2\x13R\xf7\xf3\x9a\x8999>\xa4\x11\x1fi>P\xd5>\x9am\x10\xf5\x84\xd3\xf6\xf6Jt~#\x1c\xd8\xa6\xe8\x94\xd9&\xdfR*\xd9\x15BK\xda4z\xb1\xa7\xd5\x8f\xa8\xe2/Y\x1a\xd0\xa4\x98\xdaF\xb4?PS\x14\x84\xfa\x966X\xd5\x9aJ\x12\xe0Hq$\x86\xb8\xe9zQCbf\xa1{?V6\x86\xab\xac\x9b\xa2\x13cm\x8a\xd9\xa4HB,\xb2\xcb/e\xf4Q\xe4\x90\xc6\x86\xb9\xde\xb0\x8a\x15\x91^\xd1\xa3\xd4\x80\xd5uZ\xe0\x8a\x1a\xe0\xae\x11Et,\xb2\xf3e\x8cye\x8d\x8d\x8f\xbe\x1f}\xe8K\x92(I\n\xbd\xb3\x898t\xe8H\xf8"<\xac\xb2\xf0\xdf\x04Ye\x8c\xd5\xce\x18\xdf%\x97\x8b/\x08c,l{\x91\x08\n"\x13^\xd9\xb2V\xc9G\x15\xb9lB\x18\xb0\x86\xc6\xf6I\x88b|\xe1\xbeK\xe0\xbc\xa6x\x1e>1\xdd\x92c\xe2\x96\x1e\xe4E\xb15\xe7\xdc\xb4J)\x92\x8d\x08kj\xc2\x16#\x84<X\xde\xe7\xd8\xb2\xc9\x17\xc0\x9d\xb1\x0f\x1e\x19xX\xec.YV\xc6\x86\x9b+j\x8c\x99\x195\xe0R\x8b5P\xa4_\xb6vQ(\xd8\xe2\xe2\xc7\xbda\x0bk\x18\x9e,g\xc6\x1fv!\xf9\x13<\x89\x8b\xb9|\x9e1\xe0]\xb3\xdb\x14\xe4\xc7H\xab\x1b\xf0\x8a(\xa16\x88\xbf\x98\x95\x17\xe0R\xc2\xf6\xed,z\x8a\xd0\xc7\x9a\x12\x12\x14D\x8a\xde\xc4\xc7"\xf1\xe5!\x0c\xec\x86\xcf(}\xc8\xf7\x13\xe3\x16x\xc2\xcf\x92\xac\xbf\x08\xd2}\x10\xa0~\x1a\x1cD\xda\x14\x88\xbbgb\x93;p/p\xc9Y-\x89\xb4E_1\x12^\n;\xad\x8cLom\x96#W\x03,\xf2\'\x84X\xcf(]\xc4,\xa1\xf0\x85\xc1BU\x86T\x98\xa3CQ+\x91M\xa1I1\xa1{m_A\xb9\x1f\x9d\x8e\x0f\xe4pc\x8b(\xd0i\x7f\x02^Q\x17{\x9fEe2\xc7\x85\xdb\x0cX\xf0\xb0\xbc\x88\xbe\xc7\x91,-\x8d\x94\xcam\xf7\x14\x11\xa4M\x8b\xdbP\xceGe1\xc6\xc7\x03D\x84\xda\xee\x87\x18\xb3KYx\xbe\xf9X{o)\xe6\xf1xB\xec,.\xf8]\xcf"y\xef\x86\xcd\\\x91NB\x82Yh^\xe5\x92\x9f\x84&\xfc\x96&\x86\x8a\xf8\x10\xf0\xcb\xdc\xf2\xf0\x9eVP\xdf\x02\xc2\xee!a\xec\xf0!\xe6bDd\xbd\xf4\x9d\xf0\x8a;\nG\x1b,\xb1\xbd\xff\x00;\x90\xc4w\xbc\xc8G\x91y\xfb\x0b\xa3e\x96w\x18\x9bD}AI?w!B\x8aH\x9b\x8e"\xd9x\xbe\x8b\x17m\x8f/\x15P\xfb\xb1\x08x}\xc5\xe7\xed\x84\xac|\xe5l\xb1\xbcV(h\x8b\xa1?u\\\xde\'#\x96\xc4\x84\xb2\xd8\xde^>\x83<\x0fk\xc2\xc5\rp5O\xec-\x8b\xb3\xc7d\xb0\xf0\xb7\xde(\xa5\x84\xc4\xfd\xd4\xe4;b+c{\x13_\'\x08\xfe\xca\xb4.\xd4=\x8f+\xbaBB_\x9d\xb1\xf6+\xf53\xb4^\xcf\x02\x1b\xb7e\x1c\x16\xbe\x11k\xe0\xe0\xe0\xaf\xaa\xc5\x8b\x16-\x89\x97\xed\xd8\xe5Cv%\xb5\x8d\x96\xf7.0\xf7\xc0\xa4\x90\xad\xc5\xfc\xb2Q$\xb8\xa2B\xd8\x8b\xaf\xbe/m\x96^8\xdc\x85\xed\xe4;\xdc\xcb\xdbY\xbe\x8f\xa4\xae\xc6\xb8\x97\xd9\x11\xe2\r\xbf\x04#\xf9\xa3\xf4X\x99\xe1m]\x1b,M\xe1R/6/o!\xe2\xd6/u\xef{\xfd#\xff\x00\xa9\t\\\x17\xd6C\xf3/\x96Sm\xc4\xf5Q\xfbv\xa5\xb1\x97\x86_E\x0b\xdb\xcbs\xd9LI\xee\xad\xe9Y\xe9r\xc4\x96\xa7\xf4hJ\xb4\x92\x8d\xb4\x8f,\xf5\x1f\xe6g\x87\xb5Y\xc1E\x97\x86\x8a\x19e\x96Z/\x0b+\xdb1\xe5\x8b\x0fu\x97\x8a\x1f\x19\xa2\xb6\xfa\x02]\xfe\xaf\x15\xdcg\xab\xfa\xd9\xe1o\xd5BV(\x8a$\xd0\xf8\xcdl\xa6S++\xda\xb1\xedl\xbc\xd8\x844i\xb3H\xd3F\xa6s\xf0Z/j=\r\x92\xecz\xabta)\x9f\x80O\xd2\xe3\x820\xa4Q\xca\x1b\xb6<V)\x89\x0b\x0b\x08\xe0^\xd5\x8f/\x17Lv\xb7.H\xba\xe0\xa3J\x1f\xa5r\xb1Dp\x83\xee\x89z+\xc3\x1cZyH\xf3\xc9\xe9J\x85\x99\x93\xbe\x16P\x93=4\x97tYxct96?\xa6\xe4"\xb2\x8a\xf6\xecxxh\xfa1\xa6\xb6\xa6w\x13q#$\xf2\xd8\xe4;c\x1e\x12\x94\x8fN4\xd8\xb3"V5M\xd7\xce,K\xb3\x1f\x02m\nF\xb1\xb6\xcf\xb8\xda\x1e\xfb\xe0BG\x02e{f1\xa1\xacP\xd0\xcb]\x98\xd3[Q\xe0\xa4\x7fe\xcb\xe5\xe3\xc0\xfbf*\xd9\x06!\x16^%\x1b\'\x1a\x93\xb3\xb3\xc7)\x8d\x8b\x16Yc,\xec\xb3\xc6\x10\xb2\x85\xed\xde\xca\x1a\xc3\x1a\x13\xf0\xfb\r5\xf6\xc53\x8c&\xde\xf6\xf8\xc4\x13\xa20\xa1lx\x9clpj\xf0\xf7<w\x1b\xfaf\x8a\x12\xd8\xb2\xbd\xab\xd8\xc7\x87yM\xa3J\x971\xff\x00G%\xbcY\xcdv9\xc3x\x91\\\x1c\xf1\xc1\x04\xd9\xe0\x88\x9e^\x19\xea.\x07\x1c\'\x9b/\x1c\x8e\x92\xa3\x9d\x8a\x1e_\x08\xfa.\x10\x92Y^\xe6\x8a\xc3\x1a\xc3\xdbj\\K\xfd\x8e\r}Q\xc9e\xbb\x1eP\xf9\x12 \xbcP\xad,%\xc6,\xbc\xd8\xd2d\xe05\xb5<q\x1f\xbe\x17\xdb\n\r\x97\x18\xf6\xe5\x96\xdb\xe7<a{\x87\xba\xd0\xc6=\x89\xca/\x86~I\x7f\x8b\x1aq\xee\xb0\x9a\xec\xfb\r4#\x91&%"\nE\xe2\xcb,\xb2\xcb5P\x9d\x8c\x94G\x1f\xa1\xa0pf\x96(6v\xe2&\x96S\x14d\xfc\x15\x18\xff\x00\x93\x1e\xa9w)\x8a,J\xb1BB\xd9e\xe2\xcb-\x16\x8bE\xae\x9d\xedc\x1eZ\x1d\x1clSk\x8f\x1f\x06\x98K\xf4\xff\x00\xa6U:h_\x0f\xb1\xa6\x85\x14\xc8\xc1/"\x82\xf8O\x12C\x9b\x83\x1f\xab\x1e\x05\xea\xc5\xba,L\x9f\xa8\xa2/UY\xcc\xd9\x08\xb4\x86P\xd2(I\xcb\xb1\xa7\xe1X\xf9\x14[\xec\x8aK\xbc\x8bK\xb2\x1bo\xbb\xc53\x8c%\xff\x00CM\x8e\x1fT\x8a\x8f\xcb-x\x81\xa9\xfcG\xfd\x0f\xd4\xf5>O\xc5\x99\xady\x84O\xf8\xbf\xca&\x86\xfbI1\xa6\x8a/\xc4\x95\x94\xbc1\x11DsVN\x1a\x87\xe8\x8f\xd2\xa3\x9a/\x81CT\x98\xbd\x120HH\x92\xa2)6Ti\xbd&\x85J\xd3dc\xa5\xc9x\xa2:\x12\x95&T\\d\xd2\xe5\x12\x8f\x8f\xf1\x1aQQ\xe1\x15\x05=4/\xa4[e~h\xf8\xb4&\x9a\x93\xd2\x8d\x15KE\x9a+W\x16\xc7\xf4U\xef\xa9|\x9c/\x05\x8e\xc6\x86\xb3[4\x8aR\xfb\xa2\xd7\xd5\x14\xc8\xa5\xf5\x14D\xb3ea\xa1\xa2Q#\x1b\x12)\x1cbD;\x8f\xf3y-4\xb9\xa15o\x914\x9c\x95\x9e\x9f\x13hrNSvK\xf6\xfd\x86\xd6\xbb;\xc6\x84\xb9\x8f\x0e\x92+W\x1a\x87\xa6\\\xea*?$\x9au\xc9^\xe6\xfa\r\x0ck\r%\xe4\xd2\xdfh\xb68O\xf83G\xa9\xfc$(z\xbf\xc5\x9ag\xfc\x18\xa35\xfbYMx\x90\x9f\xd1\x89\x8bm\x97\x86\xc8\xb2-\xd7;$+\xbe\x06\xe5\x96\xbe\x86\xbd<\x16\x8b-\xff\x00\x99\xfd1:|#[\xc7?\x07\xf5\xbe\xd7\xb2{Z\xdc\xd2)\x1c\xae\xd2\x8a\x1a\x93\xee\xff\x00\xf4\xd1\xf5F\x95\xfc\xa2T?\x90\xb4\x7f&q\xfblN_,W\xfc\x88\xad\x8f-\x8eBV8\xa2\xd8\xa4Z\xc4\x84&\x97\x91\xb4Z\xf98\xae\xe3\x94II|\xf1\xc8\xed&\xf5\x1a\xd7\xf25\xd2\xfdV\xc6\xed\xf7-\xfc\xb2\xdfJ\xbd\x8b\xcd\x15\xd2w\x8a(\xa1,-\xcd\x8d\x89\x15\x9aE\x15BeY\xa4\xd2i4\x8d\x15}\x8a~\x1a\x7f\xf8\xce<\xa7\x13O\xc4\x934M~\xd6.Je\x14QE\x14i4\x9a\r&\x92\x8a(\xa2\x8a(\xae\x93\xa3Q\xa8\xd4^\xca+\x15\x8d#C,H\xd0\xeb\x96\x928]\xb9"\x9f\x7f\x02\xcd\x8c\xb3\xbfE<\xde8$\xa8s\xf15bo\xc3\xd4\xbe\x19P~\x1cE\t.S52\xd7\xc1H\xa2\xb7Y\xa8\xb2\xcb\xf6\x0c\xa2\x8d%f\x8a\xcdf\x8d\'\xe1\xbf<#Z\x8f\xe8Cm\xbbdb\xbb\xb1\xc9\x89\x9a\xbf\xd1\xce\x1b9\x93\xc5P\x96h\xac1\xaf"x\xab\xc4\x99k\xcf\xe9c\x8e\x97\xc9K\xc1\xaa\xfb\xab\x14|\xa2\xfey)\x14\xd6-\xe3\x8fn\xd9b\xb2\x8a\xcd\x97\x8a\xdbG\xd8j\xc7\x11*\xe5\x8f\xb5\xc8\xb6\xdd\x96vi|\x1a\xb8\xfe\xc6\xf0\x90\xba\x89\xf6\x1b\xa6<v\xfb\x0e"BX\xac\xb5\xb9\x96_\xb0c\x10\xb6Q[\xab\x15\x9a\x1cm\xdb%\x16\xd9\xa4\x8a\xe5\x1d\xdb<D\xf1\x86,\xbc-\xade\xf2\x8am\x14$\xd1E\x14V\xfb,\xbc\xff\x00^\xc2L\xb1\x08\xb3\xb8\x96\xdb\xdc\xb3CF\x92\xb8e\x0f\xc6|\x9e\x0f\x8e\xa5b\x8a+\xaf}v2\xd6R\x11e\x97\xec\x18\xd1]Z+\xa6\xf6&X\xdb\xd9\xfd\xe6\xbam\x8eO)\x88\xb4j9b^\xce\x8a\xd9X\xa2\x8a\x12(\xa1.\x9b\xd9g\x18N\xcb/\xae\xc6\xf6\xf3\x84^\xd4\x87\xec+uu+(y\xb2\xc7\x85C\x1d\xee}\x16\x87\x9a[\x13\xdc\xb1C[/\xa9E\x15\xd6YC\xc5\xe1\x16\x87X\xf0\xc6\xf1]K\x1b\x1e,\xb2\xf6\xd9\xdf\x16\'\x85\xb1\x89m\xbcX\xbd\xb3\xc3\x18\xcb\x13\xe5\x1f\x98xWh\xe5m\xb3\x81\x8b6\xb0\xda\x1bC\xd9X\xb1Y[\x96.\x90\x9e\xc5\xb2\xf6/od\x99\xa9\xf9G%\x96I\xf2\xcb\xc5!\xa5ef\xf6-\x9ax\x1e\x92\xa3\x7f\xd0\x92hj<\xf1\xd9\x95\x1bf\x8e\xfb;a\x1c"\xf1Yb\xcbbe\xe2\xf1x\xef\xb6\xfa6^\xc5\xb1\xbc6]\x17\x86\xe8k\x96V[|\x17\xd2\xa6r\x87&93S\xaa\x1c\x9b53S\xdd{/,[\xaco\x0b\x17E\x9666"\xf1e\x96_Aa\x8f\x12\x1b\xa5\xb2C\xe1\xb2\xcbX\xf8\xcd\xbcYy\xb2\xf0\xc7\xd2\xf1\xb5t\x9b\x11\xe3,Ce\xf3\x85\x8b\x1btG\xa8\xc6_\x0cL{\x12\x1f-\xe1a\xf6C\xee!\x16\xd8\x87\xb2\x8f\xff\xc4\x00\x16\x11\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x11P\x90\xff\xda\x00\x08\x01\x02\x01\x01?\x00jn\x0f\xff\xc4\x00\x19\x11\x00\x03\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x11P\x80\x90\xff\xda\x00\x08\x01\x03\x01\x01?\x00\xe2\xdc\xc3\xd1\x0c\xba\xe3\xff\xd9\xff'
+
+actual_bundle_size = len(bytearray(raw_cat_bundle))
+print("\nactual bytearray length (actual size of bundle): {}".format(actual_bundle_size))
+
+gc.collect()
+before = gc.mem_free()
+bundle = Bundle.from_cbor(raw_cat_bundle)
+after = gc.mem_free()
+gc.collect()
+after_collect = gc.mem_free()
+
+deserialized_bundle_size = before-after_collect
+print("\ndeserialized bundle:")
+print("free before: {}, object size without collect: {}, object size with collect: {}, garbage collected: {}".format(before, before-after, deserialized_bundle_size, after_collect-after))
+
+gc.collect()
+before = gc.mem_free()
+bundle_bytes = bundle.to_cbor()
+after = gc.mem_free()
+gc.collect()
+after_collect = gc.mem_free()
+
+serialized_bundle_size = before-after_collect
+print("\nbundle bytes:")
+print("free before: {}, object size without collect: {}, object size with collect: {}, garbage collected: {}".format(before, before-after, serialized_bundle_size, after_collect-after))
+
+
+print("\nbundle_bytes length (actual size of again serialized bundle): {}".format(len(bytearray(bundle_bytes))))
+
+
+print("\nthis show (garbage collected) that compared to the actual size that factors are: serialized bundle -> {}, deserialized bundle -> {}\n".format(serialized_bundle_size/actual_bundle_size, deserialized_bundle_size/actual_bundle_size))
+
```

### Comparing `dtn7zero-0.0.4/test/test-dtn7rs-rest-cla.py` & `dtn7zero-0.0.5/test/test-dtn7rs-rest-cla.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""
-This can be run on CPython or MicroPython.
-
-It tests the rest-cla against a running dtn7rs on the specified IP with the following generic start command:
-dtnd -n node1 -r epidemic -C mtcp -e incoming
-
-Note on MicroPython:
-The current configuration of maximum in-memory stored bundles collides with the memory intensive urequests library.
-It therefore will likely crash after a few exchanged bundles.
-This is an open end topic to investigate.
-"""
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.constants import IPND_IDENTIFIER_REST, PORT_REST
-from dtn7zero.convergence_layer_adapters.dtn7rs_rest import Dtn7RsRestCLA
-from dtn7zero.data import Node
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-
-dtn7rs = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_REST: PORT_REST})
-
-storage = SimpleInMemoryStorage()
-storage.add_node(dtn7rs)
-
-clas = {IPND_IDENTIFIER_REST: Dtn7RsRestCLA()}
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://node2/', storage, router, use_ipnd=False)
-
-endpoint = LocalEndpoint('hello')
-bpa.register_endpoint(endpoint)
-
-last_send = get_current_clock_millis()
-try:
-    while True:
-        bpa.update()
-
-        if is_timestamp_older_than_timeout(last_send, 2000):
-            endpoint.start_transmission(b'world', 'dtn://node1/incoming')
-
-            last_send = get_current_clock_millis()
-except KeyboardInterrupt:
-    pass
+"""
+This can be run on CPython or MicroPython.
+
+It tests the rest-cla against a running dtn7rs on the specified IP with the following generic start command:
+dtnd -n node1 -r epidemic -C mtcp -e incoming
+
+Note on MicroPython:
+The current configuration of maximum in-memory stored bundles collides with the memory intensive urequests library.
+It therefore will likely crash after a few exchanged bundles.
+This is an open end topic to investigate.
+"""
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.constants import IPND_IDENTIFIER_REST, PORT_REST
+from dtn7zero.convergence_layer_adapters.dtn7rs_rest import Dtn7RsRestCLA
+from dtn7zero.data import Node
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+
+dtn7rs = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_REST: PORT_REST})
+
+storage = SimpleInMemoryStorage()
+storage.add_node(dtn7rs)
+
+clas = {IPND_IDENTIFIER_REST: Dtn7RsRestCLA()}
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://node2/', storage, router, use_ipnd=False)
+
+endpoint = LocalEndpoint('hello')
+bpa.register_endpoint(endpoint)
+
+last_send = get_current_clock_millis()
+try:
+    while True:
+        bpa.update()
+
+        if is_timestamp_older_than_timeout(last_send, 2000):
+            endpoint.start_transmission(b'world', 'dtn://node1/incoming')
+
+            last_send = get_current_clock_millis()
+except KeyboardInterrupt:
+    pass
```

### Comparing `dtn7zero-0.0.4/test/test-ipnd.py` & `dtn7zero-0.0.5/test/test-ipnd.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""
-To be run either on CPython or MicroPython.
-
-If started on two or more different computers in your lokal network,
-they should find each other immediately after startup.
-
-To test against the dtn7rs, we can use a generic start command (make sure to set the correct broadcast IP):
-dtnd -n node1 -r epidemic -C mtcp -e incoming -E 192.168.2.255:3003
-
-important note: because the beacon-services are not defined clearly and we do not know the expected format of the dtn7rs,
-the unicast-beacon will fail to deserialize on the dtn7rs, which is not pretty but cannot be helped at the moment.
-"""
-from dtn7zero.ipnd import IPND
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-
-
-storage = SimpleInMemoryStorage()
-
-discovery = IPND(eid_scheme=1, eid_specific_part='//test-node/', storage=storage)
-
-
-last_print = get_current_clock_millis()
-
-try:
-    while True:
-        discovery.update()
-        if is_timestamp_older_than_timeout(last_print, 2000):
-            print('known nodes: {}'.format(storage.nodes))
-            last_print = get_current_clock_millis()
-except KeyboardInterrupt:
-    pass
+"""
+To be run either on CPython or MicroPython.
+
+If started on two or more different computers in your lokal network,
+they should find each other immediately after startup.
+
+To test against the dtn7rs, we can use a generic start command (make sure to set the correct broadcast IP):
+dtnd -n node1 -r epidemic -C mtcp -e incoming -E 192.168.2.255:3003
+
+important note: because the beacon-services are not defined clearly and we do not know the expected format of the dtn7rs,
+the unicast-beacon will fail to deserialize on the dtn7rs, which is not pretty but cannot be helped at the moment.
+"""
+from dtn7zero.ipnd import IPND
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+
+
+storage = SimpleInMemoryStorage()
+
+discovery = IPND(eid_scheme=1, eid_specific_part='//test-node/', storage=storage)
+
+
+last_print = get_current_clock_millis()
+
+try:
+    while True:
+        discovery.update()
+        if is_timestamp_older_than_timeout(last_print, 2000):
+            print('known nodes: {}'.format(storage.nodes))
+            last_print = get_current_clock_millis()
+except KeyboardInterrupt:
+    pass
```

### Comparing `dtn7zero-0.0.4/test/test-mtcp-receiver.py` & `dtn7zero-0.0.5/test/test-mtcp-receiver.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-This test consists of test-mtcp-intermediate.py, test-mtcp-receiver.py, and test-mtcp-sender.py .
-
-To test the daisy-chain correctly, ipnd is disabled and the nodes are added manually.
-
---> PLEASE CHECK AND SET THE CORRECT IP ADDRESSES
---> THIS TEST WAS DESIGNED FOR SENDER AND RECEIVER TO BE RUN ON AN ESP32
---> THE INTERMEDIATE NODE SHOULD BE RUNNING ON A COMPUTER
---> THE INTERMEDIATE NODE CAN BE REPLACED BY THE dtn7rs
-
-start-command for the dtn7rs intermediate node:
-dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.182:16162/ESP32-6 -s mtcp://192.168.2.162:16162/ESP32-4
-
-
-additional notes on the ESP32 sender:
-
-As only one ESP32 can be accessed to start a script on one computer, it may be useful to set the sender-script as main-script on one ESP32:
-mpremote fs cp test/test-mtcp-sender.py :main.py
-
-The script may be stopped when entering 'mpremote' shell and pressing 'Ctrl + C' as it is an endless loop.
-Afterwards, subsequent mpremote calls will not start it again until a soft reset or power reset is performed.
-The script may then be removed using:
-mpremote fs rm :main.py
-"""
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.data import Node
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
-from py_dtn7 import Bundle
-
-
-dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
-
-storage = SimpleInMemoryStorage()
-storage.add_node(dtn7rs_node)
-
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://ESP32-4/', storage, router, use_ipnd=False)
-
-
-def callback(bundle: Bundle):
-    print('received: {}'.format(bundle.payload_block.data))
-
-
-receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
-bpa.register_endpoint(receiver_endpoint)
-
-
-try:
-    while True:
-        bpa.update()
-except KeyboardInterrupt:
-    pass
-
-bpa.unregister_endpoint(receiver_endpoint)
+"""
+This test consists of test-mtcp-intermediate.py, test-mtcp-receiver.py, and test-mtcp-sender.py .
+
+To test the daisy-chain correctly, ipnd is disabled and the nodes are added manually.
+
+--> PLEASE CHECK AND SET THE CORRECT IP ADDRESSES
+--> THIS TEST WAS DESIGNED FOR SENDER AND RECEIVER TO BE RUN ON AN ESP32
+--> THE INTERMEDIATE NODE SHOULD BE RUNNING ON A COMPUTER
+--> THE INTERMEDIATE NODE CAN BE REPLACED BY THE dtn7rs
+
+start-command for the dtn7rs intermediate node:
+dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.182:16162/ESP32-6 -s mtcp://192.168.2.162:16162/ESP32-4
+
+
+additional notes on the ESP32 sender:
+
+As only one ESP32 can be accessed to start a script on one computer, it may be useful to set the sender-script as main-script on one ESP32:
+mpremote fs cp test/test-mtcp-sender.py :main.py
+
+The script may be stopped when entering 'mpremote' shell and pressing 'Ctrl + C' as it is an endless loop.
+Afterwards, subsequent mpremote calls will not start it again until a soft reset or power reset is performed.
+The script may then be removed using:
+mpremote fs rm :main.py
+"""
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.data import Node
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
+from py_dtn7 import Bundle
+
+
+dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
+
+storage = SimpleInMemoryStorage()
+storage.add_node(dtn7rs_node)
+
+clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://ESP32-4/', storage, router, use_ipnd=False)
+
+
+def callback(bundle: Bundle):
+    print('received: {}'.format(bundle.payload_block.data))
+
+
+receiver_endpoint = LocalEndpoint('receiver', receive_callback=callback)
+bpa.register_endpoint(receiver_endpoint)
+
+
+try:
+    while True:
+        bpa.update()
+except KeyboardInterrupt:
+    pass
+
+bpa.unregister_endpoint(receiver_endpoint)
```

### Comparing `dtn7zero-0.0.4/test/test-mtcp-sender.py` & `dtn7zero-0.0.5/test/test-mtcp-sender.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-This test consists of test-mtcp-intermediate.py, test-mtcp-receiver.py, and test-mtcp-sender.py .
-
-To test the daisy-chain correctly, ipnd is disabled and the nodes are added manually.
-
---> PLEASE CHECK AND SET THE CORRECT IP ADDRESSES
---> THIS TEST WAS DESIGNED FOR SENDER AND RECEIVER TO BE RUN ON AN ESP32
---> THE INTERMEDIATE NODE SHOULD BE RUNNING ON A COMPUTER
---> THE INTERMEDIATE NODE CAN BE REPLACED BY THE dtn7rs
-
-start-command for the dtn7rs intermediate node:
-dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.182:16162/ESP32-6 -s mtcp://192.168.2.162:16162/ESP32-4
-
-
-additional notes on the ESP32 sender:
-
-As only one ESP32 can be accessed to start a script on one computer, it may be useful to set the sender-script as main-script on one ESP32:
-mpremote fs cp test/test-mtcp-sender.py :main.py
-
-The script may be stopped when entering 'mpremote' shell and pressing 'Ctrl + C' as it is an endless loop.
-Afterwards, subsequent mpremote calls will not start it again until a soft reset or power reset is performed.
-The script may then be removed using:
-mpremote fs rm :main.py
-"""
-from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
-from dtn7zero.endpoints import LocalEndpoint
-from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
-from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
-from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
-from dtn7zero.data import Node
-from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
-from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
-
-
-dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
-
-storage = SimpleInMemoryStorage()
-storage.add_node(dtn7rs_node)
-
-clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
-router = SimpleEpidemicRouter(clas, storage)
-bpa = BundleProtocolAgent('dtn://ESP32-6/', storage, router, use_ipnd=False)
-
-sender_endpoint = LocalEndpoint('sender')
-
-
-bpa.register_endpoint(sender_endpoint)
-
-message_str = 'hello_world {}'
-counter = 0
-
-last_transmission = get_current_clock_millis()
-try:
-    while True:
-        bpa.update()
-
-        if is_timestamp_older_than_timeout(last_transmission, 2000):
-            sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://ESP32-4/receiver')
-            counter += 1
-
-            last_transmission = get_current_clock_millis()
-except KeyboardInterrupt:
-    pass
-
-bpa.unregister_endpoint(sender_endpoint)
+"""
+This test consists of test-mtcp-intermediate.py, test-mtcp-receiver.py, and test-mtcp-sender.py .
+
+To test the daisy-chain correctly, ipnd is disabled and the nodes are added manually.
+
+--> PLEASE CHECK AND SET THE CORRECT IP ADDRESSES
+--> THIS TEST WAS DESIGNED FOR SENDER AND RECEIVER TO BE RUN ON AN ESP32
+--> THE INTERMEDIATE NODE SHOULD BE RUNNING ON A COMPUTER
+--> THE INTERMEDIATE NODE CAN BE REPLACED BY THE dtn7rs
+
+start-command for the dtn7rs intermediate node:
+dtnd -n node1 -r epidemic -C mtcp -e incoming -s mtcp://192.168.2.182:16162/ESP32-6 -s mtcp://192.168.2.162:16162/ESP32-4
+
+
+additional notes on the ESP32 sender:
+
+As only one ESP32 can be accessed to start a script on one computer, it may be useful to set the sender-script as main-script on one ESP32:
+mpremote fs cp test/test-mtcp-sender.py :main.py
+
+The script may be stopped when entering 'mpremote' shell and pressing 'Ctrl + C' as it is an endless loop.
+Afterwards, subsequent mpremote calls will not start it again until a soft reset or power reset is performed.
+The script may then be removed using:
+mpremote fs rm :main.py
+"""
+from dtn7zero.bundle_protocol_agent import BundleProtocolAgent
+from dtn7zero.endpoints import LocalEndpoint
+from dtn7zero.convergence_layer_adapters.mtcp import MTcpCLA
+from dtn7zero.storage.simple_in_memory_storage import SimpleInMemoryStorage
+from dtn7zero.routers.simple_epidemic_router import SimpleEpidemicRouter
+from dtn7zero.data import Node
+from dtn7zero.constants import IPND_IDENTIFIER_MTCP, PORT_MTCP
+from dtn7zero.utility import get_current_clock_millis, is_timestamp_older_than_timeout
+
+
+dtn7rs_node = Node('192.168.2.163', (1, '//node1/'), {IPND_IDENTIFIER_MTCP: PORT_MTCP})
+
+storage = SimpleInMemoryStorage()
+storage.add_node(dtn7rs_node)
+
+clas = {IPND_IDENTIFIER_MTCP: MTcpCLA()}
+router = SimpleEpidemicRouter(clas, storage)
+bpa = BundleProtocolAgent('dtn://ESP32-6/', storage, router, use_ipnd=False)
+
+sender_endpoint = LocalEndpoint('sender')
+
+
+bpa.register_endpoint(sender_endpoint)
+
+message_str = 'hello_world {}'
+counter = 0
+
+last_transmission = get_current_clock_millis()
+try:
+    while True:
+        bpa.update()
+
+        if is_timestamp_older_than_timeout(last_transmission, 2000):
+            sender_endpoint.start_transmission(message_str.format(counter).encode('utf-8'), 'dtn://ESP32-4/receiver')
+            counter += 1
+
+            last_transmission = get_current_clock_millis()
+except KeyboardInterrupt:
+    pass
+
+bpa.unregister_endpoint(sender_endpoint)
```

### Comparing `dtn7zero-0.0.4/test/test-py-dtn7-functionality.py` & `dtn7zero-0.0.5/test/test-py-dtn7-functionality.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-#!/usr/bin/env python3
-
-# tests and documents the (http-)functionality of the py_dtn7 library against a dtn-rs server
-import time
-import json
-import sys
-
-from py_dtn7 import DTNRESTClient, Bundle
-
-# connection to the dtn-rs client is made and the node_id gets fetched
-dtn = DTNRESTClient(host='http://192.168.2.163', port=3000)
-# dtn = DTNRESTClient(host='http://localhost', port=3000)
-
-# the 'name' of the server. A registered service gets a subname in the servers namespace
-print('connected to dtn node: {}\n'.format(dtn.node_id))
-
-# I do not know if there is a better way to get this.
-# But, the node_id includes the naming identifier, which is left out in bundles, but needs to be included when sending through the send endpoint
-USING_IPN_NAMING = dtn.node_id.startswith('ipn')
-
-# echo service definition
-# there are two naming schemes: dtn and ipn
-service = 'echo'
-if USING_IPN_NAMING:
-    service = 7
-
-# fetches all bundles via the public status/bundles and download endpoint
-# deserializes them into the bundle class
-pretty_bundles = '\n'.join(str(bundle) for bundle in dtn.get_all_bundles())
-print('all bundles currently stored on the server: \n{}\n'.format(pretty_bundles))
-
-# fetches a raw bundle from the public download endpoint
-# bundle_id or time and seq must be provided
-# bundle can be deserialized through Bundle.from_cbor(...)
-bundle_id = 'dtn://node1/-724512676024-0'
-raw_bundle_bytes = dtn.download(bundle_id=bundle_id)
-if raw_bundle_bytes == b'Bundle not found':
-    deserialized_bundle = raw_bundle_bytes.decode()
-else:
-    deserialized_bundle = Bundle.from_cbor(raw_bundle_bytes)
-print('this a download response for bundle-id "{}": \nraw: {}\ndeserialized: {}\n'.format(bundle_id, raw_bundle_bytes, deserialized_bundle))
-
-# fetches a list of all endpoints(str) currently registered at this server
-pretty_endpoints = '\n'.join(dtn.endpoints)
-print('all endpoints currently registered at this endpoint: \n{}\n'.format(pretty_endpoints))
-
-# fetches a list of all bundle-ids(str) of the bundles currently stored on the server
-pretty_bundle_ids = '\n'.join(dtn.bundles)
-print('all bundle-ids of the bundles currently on the server: \n{}\n'.format(pretty_bundle_ids))
-
-# fetches a list of all bundle-ids(str) of the bundles currently stored on the server matching the filter.
-# no wildcards possible, but generalizations or parts, examples: dtn://node1/ping, node1/ping, node1, ping
-address_part_criteria = 'ping'
-pretty_filtered_bundle_ids = '\n'.join(dtn.get_filtered_bundles(address_part_criteria))
-print('all bundle-ids of the bundles currently on the server matching the filter "{}": \n{}\n'.format(address_part_criteria, pretty_filtered_bundle_ids))
-
-# fetches a list of all bundle-ids with the current status (concatenated string)
-pretty_stored_bundles = '\n'.join(dtn.store)
-print('all bundle-ids of the bundles currently on the server and their constraints: \n{}\n'.format(pretty_stored_bundles))
-
-# fetches a list of all known peers -> dictionary structure
-pretty_peers = '\n'.join(json.dumps(peer, indent=4) for peer in dtn.peers)
-print('all peers known by the server: \n{}\n'.format(pretty_peers))
-
-# fetches general info about the server instance
-if sys.implementation.name == 'micropython':
-    pretty_info = json.dumps(dtn.info)
-else:
-    pretty_info = json.dumps(dtn.info, indent=4)
-print('info about the server instance: \n{}\n'.format(pretty_info))
-
-# the following public endpoints are not supported by this library:
-# /download.hex
-# /push
-# /status/bundles/digest
-# /status/bundles/verbose
-# /status/bundles/filtered/digest?addr=<address_part_criteria>
-
-"""
-LOCAL ONLY API
-This is only available via localhost, or, on other network interfaces with the -U option
-"""
-
-# registers a service for message reception
-# this may be a singleton endpoint: mailbox or echo
-# this may be a group endpoint: dtn://global/~news
-# So, this can either be in the server-namespace, or, you define your own (global) one
-print(dtn.register(service).content)
-
-try:
-    while True:
-        # fetches from the internal 'endpoint' endpoint a single bundle
-        # if not bundle is available the string 'Nothing to receive' is returned
-        raw_bundle = dtn.fetch_endpoint(service)
-        if b'Nothing to receive' in raw_bundle:
-            print('no bundle was available at endpoint "{}", returned: {}'.format(service, raw_bundle))
-        else:
-            deserialized_bundle = Bundle.from_cbor(raw_bundle)
-            print('a bundle fetched from the endpoint "{}":\n  raw: {}\n  deserialized: {}'.format(service, raw_bundle, deserialized_bundle))
-
-            # sends an echo-reply back to the origin via the send endpoint
-            response = dtn.send(
-                payload=deserialized_bundle.payload_block.data,
-                destination=deserialized_bundle.primary_block.full_source_uri,
-                lifetime=3600*24*1000
-            )
-            print('  echo reply was sent back to server, response was: {}, {}, {}'.format(response.status_code, response.content, response.headers))
-
-        time.sleep(1)
-except KeyboardInterrupt:
-    pass
-
-# unregisters a previously registered service
-print(dtn.unregister(service).content)
+#!/usr/bin/env python3
+
+# tests and documents the (http-)functionality of the py_dtn7 library against a dtn-rs server
+import time
+import json
+import sys
+
+from py_dtn7 import DTNRESTClient, Bundle
+
+# connection to the dtn-rs client is made and the node_id gets fetched
+dtn = DTNRESTClient(host='http://192.168.2.163', port=3000)
+# dtn = DTNRESTClient(host='http://localhost', port=3000)
+
+# the 'name' of the server. A registered service gets a subname in the servers namespace
+print('connected to dtn node: {}\n'.format(dtn.node_id))
+
+# I do not know if there is a better way to get this.
+# But, the node_id includes the naming identifier, which is left out in bundles, but needs to be included when sending through the send endpoint
+USING_IPN_NAMING = dtn.node_id.startswith('ipn')
+
+# echo service definition
+# there are two naming schemes: dtn and ipn
+service = 'echo'
+if USING_IPN_NAMING:
+    service = 7
+
+# fetches all bundles via the public status/bundles and download endpoint
+# deserializes them into the bundle class
+pretty_bundles = '\n'.join(str(bundle) for bundle in dtn.get_all_bundles())
+print('all bundles currently stored on the server: \n{}\n'.format(pretty_bundles))
+
+# fetches a raw bundle from the public download endpoint
+# bundle_id or time and seq must be provided
+# bundle can be deserialized through Bundle.from_cbor(...)
+bundle_id = 'dtn://node1/-724512676024-0'
+raw_bundle_bytes = dtn.download(bundle_id=bundle_id)
+if raw_bundle_bytes == b'Bundle not found':
+    deserialized_bundle = raw_bundle_bytes.decode()
+else:
+    deserialized_bundle = Bundle.from_cbor(raw_bundle_bytes)
+print('this a download response for bundle-id "{}": \nraw: {}\ndeserialized: {}\n'.format(bundle_id, raw_bundle_bytes, deserialized_bundle))
+
+# fetches a list of all endpoints(str) currently registered at this server
+pretty_endpoints = '\n'.join(dtn.endpoints)
+print('all endpoints currently registered at this endpoint: \n{}\n'.format(pretty_endpoints))
+
+# fetches a list of all bundle-ids(str) of the bundles currently stored on the server
+pretty_bundle_ids = '\n'.join(dtn.bundles)
+print('all bundle-ids of the bundles currently on the server: \n{}\n'.format(pretty_bundle_ids))
+
+# fetches a list of all bundle-ids(str) of the bundles currently stored on the server matching the filter.
+# no wildcards possible, but generalizations or parts, examples: dtn://node1/ping, node1/ping, node1, ping
+address_part_criteria = 'ping'
+pretty_filtered_bundle_ids = '\n'.join(dtn.get_filtered_bundles(address_part_criteria))
+print('all bundle-ids of the bundles currently on the server matching the filter "{}": \n{}\n'.format(address_part_criteria, pretty_filtered_bundle_ids))
+
+# fetches a list of all bundle-ids with the current status (concatenated string)
+pretty_stored_bundles = '\n'.join(dtn.store)
+print('all bundle-ids of the bundles currently on the server and their constraints: \n{}\n'.format(pretty_stored_bundles))
+
+# fetches a list of all known peers -> dictionary structure
+pretty_peers = '\n'.join(json.dumps(peer, indent=4) for peer in dtn.peers)
+print('all peers known by the server: \n{}\n'.format(pretty_peers))
+
+# fetches general info about the server instance
+if sys.implementation.name == 'micropython':
+    pretty_info = json.dumps(dtn.info)
+else:
+    pretty_info = json.dumps(dtn.info, indent=4)
+print('info about the server instance: \n{}\n'.format(pretty_info))
+
+# the following public endpoints are not supported by this library:
+# /download.hex
+# /push
+# /status/bundles/digest
+# /status/bundles/verbose
+# /status/bundles/filtered/digest?addr=<address_part_criteria>
+
+"""
+LOCAL ONLY API
+This is only available via localhost, or, on other network interfaces with the -U option
+"""
+
+# registers a service for message reception
+# this may be a singleton endpoint: mailbox or echo
+# this may be a group endpoint: dtn://global/~news
+# So, this can either be in the server-namespace, or, you define your own (global) one
+print(dtn.register(service).content)
+
+try:
+    while True:
+        # fetches from the internal 'endpoint' endpoint a single bundle
+        # if not bundle is available the string 'Nothing to receive' is returned
+        raw_bundle = dtn.fetch_endpoint(service)
+        if b'Nothing to receive' in raw_bundle:
+            print('no bundle was available at endpoint "{}", returned: {}'.format(service, raw_bundle))
+        else:
+            deserialized_bundle = Bundle.from_cbor(raw_bundle)
+            print('a bundle fetched from the endpoint "{}":\n  raw: {}\n  deserialized: {}'.format(service, raw_bundle, deserialized_bundle))
+
+            # sends an echo-reply back to the origin via the send endpoint
+            response = dtn.send(
+                payload=deserialized_bundle.payload_block.data,
+                destination=deserialized_bundle.primary_block.full_source_uri,
+                lifetime=3600*24*1000
+            )
+            print('  echo reply was sent back to server, response was: {}, {}, {}'.format(response.status_code, response.content, response.headers))
+
+        time.sleep(1)
+except KeyboardInterrupt:
+    pass
+
+# unregisters a previously registered service
+print(dtn.unregister(service).content)
```

