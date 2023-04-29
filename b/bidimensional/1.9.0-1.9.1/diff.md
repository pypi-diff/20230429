# Comparing `tmp/bidimensional-1.9.0.tar.gz` & `tmp/bidimensional-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bidimensional-1.9.0.tar", last modified: Thu Feb 16 12:23:20 2023, max compression
+gzip compressed data, was "bidimensional-1.9.1.tar", last modified: Sat Apr 29 21:20:36 2023, max compression
```

## Comparing `bidimensional-1.9.0.tar` & `bidimensional-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.612491 bidimensional-1.9.0/
--rw-rw-rw-   0        0        0    35184 2022-12-12 00:00:22.000000 bidimensional-1.9.0/LICENSE
--rw-rw-rw-   0        0        0    44812 2023-02-16 12:23:20.611584 bidimensional-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3615 2022-12-19 10:42:38.000000 bidimensional-1.9.0/README.md
--rw-rw-rw-   0        0        0      884 2023-02-16 12:22:39.000000 bidimensional-1.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-16 12:23:20.613491 bidimensional-1.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.044615 bidimensional-1.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.052137 bidimensional-1.9.0/src/bidimensional/
--rw-rw-rw-   0        0        0      110 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.432488 bidimensional-1.9.0/src/bidimensional/core/
--rw-rw-rw-   0        0        0        0 2022-12-19 10:42:44.000000 bidimensional-1.9.0/src/bidimensional/core/__init__.py
--rw-rw-rw-   0        0        0    13528 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/core/coordinate.py
--rw-rw-rw-   0        0        0    13562 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/core/lines.py
--rw-rw-rw-   0        0        0     3181 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/core/operations.py
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.529490 bidimensional-1.9.0/src/bidimensional/functions/
--rw-rw-rw-   0        0        0       28 2022-12-19 10:42:38.000000 bidimensional-1.9.0/src/bidimensional/functions/__init__.py
--rw-rw-rw-   0        0        0    16554 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/functions/spline.py
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.608490 bidimensional-1.9.0/src/bidimensional/polygons/
--rw-rw-rw-   0        0        0       62 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/polygons/__init__.py
--rw-rw-rw-   0        0        0     9316 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/polygons/polygon.py
--rw-rw-rw-   0        0        0    18466 2023-02-16 12:22:39.000000 bidimensional-1.9.0/src/bidimensional/polygons/triangle.py
-drwxrwxrwx   0        0        0        0 2023-02-16 12:23:20.362489 bidimensional-1.9.0/src/bidimensional.egg-info/
--rw-rw-rw-   0        0        0    44812 2023-02-16 12:23:19.000000 bidimensional-1.9.0/src/bidimensional.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-02-16 12:23:20.000000 bidimensional-1.9.0/src/bidimensional.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 12:23:19.000000 bidimensional-1.9.0/src/bidimensional.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-16 12:23:19.000000 bidimensional-1.9.0/src/bidimensional.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.929924 bidimensional-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-29 21:20:22.000000 bidimensional-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44056 2023-04-29 21:20:36.929924 bidimensional-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-29 21:20:22.000000 bidimensional-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-29 21:20:22.000000 bidimensional-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:20:36.929924 bidimensional-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.925923 bidimensional-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.925923 bidimensional-1.9.1/src/bidimensional/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.929924 bidimensional-1.9.1/src/bidimensional/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/core/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/core/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/core/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.929924 bidimensional-1.9.1/src/bidimensional/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/functions/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.929924 bidimensional-1.9.1/src/bidimensional/polygons/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/polygons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/polygons/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17850 2023-04-29 21:20:22.000000 bidimensional-1.9.1/src/bidimensional/polygons/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:20:36.929924 bidimensional-1.9.1/src/bidimensional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44056 2023-04-29 21:20:36.000000 bidimensional-1.9.1/src/bidimensional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-29 21:20:36.000000 bidimensional-1.9.1/src/bidimensional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:20:36.000000 bidimensional-1.9.1/src/bidimensional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 21:20:36.000000 bidimensional-1.9.1/src/bidimensional.egg-info/top_level.txt
```

### Comparing `bidimensional-1.9.0/LICENSE` & `bidimensional-1.9.1/LICENSE`

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
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
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
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
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

### Comparing `bidimensional-1.9.0/PKG-INFO` & `bidimensional-1.9.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,756 +1,756 @@
-Metadata-Version: 2.1
-Name: bidimensional
-Version: 1.9.0
-Summary: A collection of 2D utilities for coordinate representation and manipulation.
-Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
-Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Project-URL: Homepage, https://github.com/erlete/bidimensional
-Project-URL: Bug Tracker, https://github.com/erlete/bidimensional/issues
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.13
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Bidimensional
-
-[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
-
-This package contains a collection of useful classes and functions for working with 2D geometry in Python.
-
-## Objectives and contributions
-
-This package has three fundamental bases:
-
-* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
-* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
-* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
-
-Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
-
-## Features
-
-The following features are currently implemented:
-
-* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
-* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
-* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
-* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
-
-## Installation
-
-The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
-
-```bash
-pip install bidimensional
-```
-
-_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
-
-## Usage
-
-Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
-
-## Examples
-
-Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
-
-```python
-import bidimensional.operations as op
-import matplotlib.pyplot as plt
-
-from bidimensional import Coordinate
-from bidimensional.polygons import Triangle
-
-
-outer_triangle = Triangle(
-    Coordinate(0, 0),
-    Coordinate(1, 0),
-    Coordinate(0, 1)
-)
-
-inner_triangle = Triangle(
-    op.midpoint(outer_triangle.a, outer_triangle.b),
-    op.midpoint(outer_triangle.b, outer_triangle.c),
-    op.midpoint(outer_triangle.c, outer_triangle.a)
-)
-
-outer_triangle.plot(color="darkorange", lw=2)
-inner_triangle.plot()
-
-plt.gca().add_patch(plt.Circle(
-    inner_triangle.circumcenter,
-    inner_triangle.circumradius,
-    color="darkblue",
-    fill=False,
-    lw=2
-))
-
-plt.axis("equal")
-plt.grid()
-plt.show()
-```
+Metadata-Version: 2.1
+Name: bidimensional
+Version: 1.9.1
+Summary: A collection of 2D utilities for coordinate representation and manipulation.
+Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
+Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
+License:                     GNU AFFERO GENERAL PUBLIC LICENSE
+                               Version 3, 19 November 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU Affero General Public License is a free, copyleft license for
+        software and other kinds of works, specifically designed to ensure
+        cooperation with the community in the case of network server software.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        our General Public Licenses are intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          Developers that use our General Public Licenses protect your rights
+        with two steps: (1) assert copyright on the software, and (2) offer
+        you this License which gives you legal permission to copy, distribute
+        and/or modify the software.
+        
+          A secondary benefit of defending all users' freedom is that
+        improvements made in alternate versions of the program, if they
+        receive widespread use, become available for other developers to
+        incorporate.  Many developers of free software are heartened and
+        encouraged by the resulting cooperation.  However, in the case of
+        software used on network servers, this result may fail to come about.
+        The GNU General Public License permits making a modified version and
+        letting the public access it on a server without ever releasing its
+        source code to the public.
+        
+          The GNU Affero General Public License is designed specifically to
+        ensure that, in such cases, the modified source code becomes available
+        to the community.  It requires the operator of a network server to
+        provide the source code of the modified version running there to the
+        users of that server.  Therefore, public use of a modified version, on
+        a publicly accessible server, gives the public access to the source
+        code of the modified version.
+        
+          An older license, called the Affero General Public License and
+        published by Affero, was designed to accomplish similar goals.  This is
+        a different license, not a version of the Affero GPL, but Affero has
+        released a new version of the Affero GPL which permits relicensing under
+        this license.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU Affero General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Remote Network Interaction; Use with the GNU General Public License.
+        
+          Notwithstanding any other provision of this License, if you modify the
+        Program, your modified version must prominently offer all users
+        interacting with it remotely through a computer network (if your version
+        supports such interaction) an opportunity to receive the Corresponding
+        Source of your version by providing access to the Corresponding Source
+        from a network server at no charge, through some standard or customary
+        means of facilitating copying of software.  This Corresponding Source
+        shall include the Corresponding Source for any work covered by version 3
+        of the GNU General Public License that is incorporated pursuant to the
+        following paragraph.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the work with which it is combined will remain governed by version
+        3 of the GNU General Public License.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU Affero General Public License from time to time.  Such new versions
+        will be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU Affero General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU Affero General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU Affero General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU Affero General Public License for more details.
+        
+            You should have received a copy of the GNU Affero General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If your software can interact with users remotely through a computer
+        network, you should also make sure that it provides a way for users to
+        get its source.  For example, if your program is a web application, its
+        interface could display a "Source" link that leads users to an archive
+        of the code.  There are many ways you could offer source, and different
+        solutions will be better for different programs; see section 13 for the
+        specific requirements.
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU AGPL, see
+        <https://www.gnu.org/licenses/>.
+        
+Project-URL: Homepage, https://github.com/erlete/bidimensional
+Project-URL: Bug Tracker, https://github.com/erlete/bidimensional/issues
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.13
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bidimensional
+
+[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
+
+This package contains a collection of useful classes and functions for working with 2D geometry in Python.
+
+## Objectives and contributions
+
+This package has three fundamental bases:
+
+* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
+* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
+* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
+
+Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
+
+## Features
+
+The following features are currently implemented:
+
+* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
+* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
+* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
+* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
+
+## Installation
+
+The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
+
+```bash
+pip install bidimensional
+```
+
+_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
+
+## Usage
+
+Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
+
+## Examples
+
+Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
+
+```python
+import bidimensional.operations as op
+import matplotlib.pyplot as plt
+
+from bidimensional import Coordinate
+from bidimensional.polygons import Triangle
+
+
+outer_triangle = Triangle(
+    Coordinate(0, 0),
+    Coordinate(1, 0),
+    Coordinate(0, 1)
+)
+
+inner_triangle = Triangle(
+    op.midpoint(outer_triangle.a, outer_triangle.b),
+    op.midpoint(outer_triangle.b, outer_triangle.c),
+    op.midpoint(outer_triangle.c, outer_triangle.a)
+)
+
+outer_triangle.plot(color="darkorange", lw=2)
+inner_triangle.plot()
+
+plt.gca().add_patch(plt.Circle(
+    inner_triangle.circumcenter,
+    inner_triangle.circumradius,
+    color="darkblue",
+    fill=False,
+    lw=2
+))
+
+plt.axis("equal")
+plt.grid()
+plt.show()
+```
```

### Comparing `bidimensional-1.9.0/README.md` & `bidimensional-1.9.1/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# Bidimensional
-
-[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
-
-This package contains a collection of useful classes and functions for working with 2D geometry in Python.
-
-## Objectives and contributions
-
-This package has three fundamental bases:
-
-* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
-* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
-* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
-
-Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
-
-## Features
-
-The following features are currently implemented:
-
-* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
-* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
-* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
-* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
-
-## Installation
-
-The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
-
-```bash
-pip install bidimensional
-```
-
-_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
-
-## Usage
-
-Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
-
-## Examples
-
-Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
-
-```python
-import bidimensional.operations as op
-import matplotlib.pyplot as plt
-
-from bidimensional import Coordinate
-from bidimensional.polygons import Triangle
-
-
-outer_triangle = Triangle(
-    Coordinate(0, 0),
-    Coordinate(1, 0),
-    Coordinate(0, 1)
-)
-
-inner_triangle = Triangle(
-    op.midpoint(outer_triangle.a, outer_triangle.b),
-    op.midpoint(outer_triangle.b, outer_triangle.c),
-    op.midpoint(outer_triangle.c, outer_triangle.a)
-)
-
-outer_triangle.plot(color="darkorange", lw=2)
-inner_triangle.plot()
-
-plt.gca().add_patch(plt.Circle(
-    inner_triangle.circumcenter,
-    inner_triangle.circumradius,
-    color="darkblue",
-    fill=False,
-    lw=2
-))
-
-plt.axis("equal")
-plt.grid()
-plt.show()
-```
+# Bidimensional
+
+[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
+
+This package contains a collection of useful classes and functions for working with 2D geometry in Python.
+
+## Objectives and contributions
+
+This package has three fundamental bases:
+
+* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
+* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
+* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
+
+Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
+
+## Features
+
+The following features are currently implemented:
+
+* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
+* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
+* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
+* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
+
+## Installation
+
+The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
+
+```bash
+pip install bidimensional
+```
+
+_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
+
+## Usage
+
+Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
+
+## Examples
+
+Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
+
+```python
+import bidimensional.operations as op
+import matplotlib.pyplot as plt
+
+from bidimensional import Coordinate
+from bidimensional.polygons import Triangle
+
+
+outer_triangle = Triangle(
+    Coordinate(0, 0),
+    Coordinate(1, 0),
+    Coordinate(0, 1)
+)
+
+inner_triangle = Triangle(
+    op.midpoint(outer_triangle.a, outer_triangle.b),
+    op.midpoint(outer_triangle.b, outer_triangle.c),
+    op.midpoint(outer_triangle.c, outer_triangle.a)
+)
+
+outer_triangle.plot(color="darkorange", lw=2)
+inner_triangle.plot()
+
+plt.gca().add_patch(plt.Circle(
+    inner_triangle.circumcenter,
+    inner_triangle.circumradius,
+    color="darkblue",
+    fill=False,
+    lw=2
+))
+
+plt.axis("equal")
+plt.grid()
+plt.show()
+```
```

### Comparing `bidimensional-1.9.0/pyproject.toml` & `bidimensional-1.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[build-system]
-requires = [
-    "setuptools",
-    "matplotlib",
-    "numpy"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "bidimensional"
-version = "1.9.0"
-description = "A collection of 2D utilities for coordinate representation and manipulation."
-readme = "README.md"
-license = {file = "LICENSE"}
-requires-python = ">=3.7.13"
-authors = [
-    {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
-]
-maintainers = [
-    {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
-]
-classifiers = [
-    "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/erlete/bidimensional"
-"Bug Tracker" = "https://github.com/erlete/bidimensional/issues"
+[build-system]
+requires = [
+    "setuptools",
+    "matplotlib",
+    "numpy"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "bidimensional"
+version = "1.9.1"
+description = "A collection of 2D utilities for coordinate representation and manipulation."
+readme = "README.md"
+license = {file = "LICENSE"}
+requires-python = ">=3.7.13"
+authors = [
+    {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
+]
+maintainers = [
+    {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
+]
+classifiers = [
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/erlete/bidimensional"
+"Bug Tracker" = "https://github.com/erlete/bidimensional/issues"
```

### Comparing `bidimensional-1.9.0/src/bidimensional/core/lines.py` & `bidimensional-1.9.1/src/bidimensional/core/coordinate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,463 +1,446 @@
-"""Container module for linear classes.
-
-This module contains both `Segment` and `Line` classes, used to represent
-linear sequences of coordinates, delimited and (mathematically) unlimited.
-
-Author:
-    Paulo Sanchez (@erlete)
-"""
-
-
-from __future__ import annotations
-
-from typing import Generator, Optional
-
-import matplotlib
-import matplotlib.pyplot as plt
-
-from . import operations as op
-from .coordinate import Coordinate
-
-
-class Line:
-    """A class to represent a line in 2D space.
-
-    This class provides a way to represent a line in 2D space. It must be
-    composed by two Coordinate objects.
-
-    Attributes:
-        a (Coordinate): the first coordinate.
-        b (Coordinate): the second coordinate.
-        slope (float): the slope of the line.
-    """
-
-    STYLES = {
-        "color": "#7d4e11",
-        "lw": 1.25,
-        "alpha": .3,
-        "linestyle": (5, (10, 3))
-    }
-
-    _ERROR_MSGS = {
-        "TypeError1": "value must be a Coordinate object.",
-        "TypeError2": "value must be a Line object."
-    }
-
-    def __init__(self, a: Coordinate, b: Coordinate) -> None:
-        """Initialize a line instance.
-
-        Args:
-            a (Coordinate): the first coordinate.
-            b (Coordinate): the second coordinate.
-        """
-        self._properties = {}
-
-        self.a = a
-        self.b = b
-
-    @property
-    def a(self) -> Coordinate:
-        """Get the first coordinate of the line definition.
-
-        Returns:
-            Coordinate: the first coordinate of the line definition.
-        """
-        return self._a
-
-    @a.setter
-    def a(self, value: Coordinate) -> None:
-        """Set the first coordinate of the line definition.
-
-        Args:
-            value (Coordinate): the first coordinate of the line definition.
-
-        Raises:
-            TypeError: if `value` is not a type Coordinate.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError(self._ERROR_MSGS.get("TypeError1"))
-
-        self._a = value
-        self._properties.clear()
-
-    @property
-    def b(self) -> Coordinate:
-        """Get the second coordinate of the line definition.
-
-        Returns:
-            Coordinate: the second coordinate of the line definition.
-        """
-        return self._b
-
-    @b.setter
-    def b(self, value: Coordinate) -> None:
-        """Set the second coordinate of the line definition.
-
-        Args:
-            value (Coordinate): the second coordinate of the line definition.
-
-        Raises:
-            TypeError: if `value` is not a type Coordinate.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError(self._ERROR_MSGS.get("TypeError1"))
-
-        self._b = value
-        self._properties.clear()
-
-    @property
-    def slope(self) -> float:
-        """Get the slope of the line.
-
-        Returns:
-            float: the slope of the line.
-        """
-        if self._properties.get("slope") is None:
-
-            if self.b.x - self.a.x == 0:
-                print("Warning: slope has an infinite value.")
-
-                self._properties["slope"] = (
-                    (self.b.y - self.a.y)
-                    / 1e-14
-                )
-
-            else:
-                self._properties["slope"] = (
-                    (self.b.y - self.a.y)
-                    / (self.b.x - self.a.x)
-                )
-
-        return self._properties["slope"]
-
-    def intersect(self, line: Line) -> Optional[Coordinate]:
-        """Determine the intersection between two lines.
-
-        Args:
-            line (Line): the line to determine the intersection with.
-
-        Returns:
-            Optional[Coordinate]: the intersection between the two lines (if it
-                exists, otherwise None).
-
-        Raises:
-            TypeError: if line is not a Line object.
-
-        Notes:
-            This method is also implemented as `__mul__`, accessible using the
-            `*` operator between `Line` instances.
-        """
-        if not isinstance(line, Line):
-            raise TypeError(f"Expected Line, got {type(line)}")
-
-        if self.slope == line.slope:
-            return None
-
-        x = (
-            line.b.y - self.b.y + self.slope
-            * self.b.x - line.slope * line.b.x
-        ) / (self.slope - line.slope)
-        y = self.slope * (x - self.b.x) + self.b.y
-
-        return Coordinate(x, y)
-
-    def plot(self, ax: matplotlib.axes.Axes = None, **kwargs) -> None:
-        """Plot the line.
-
-        Args:
-            ax (matplotlib.axes.Axes, optional): The axes to plot on. Defaults
-                to None (if None, the current axes will be used).
-            **kwargs: Keyword arguments to pass to the plot
-        """
-        styles = self.STYLES.copy()
-        styles.update(kwargs)
-        ax = plt.gca() if ax is None else ax
-
-        ax.axline(self.a, self.b, **styles)
-
-    def __mul__(self, line: Line) -> Optional[Coordinate]:
-        """Determine the intersection between two lines.
-
-        Args:
-            line (Line): the line to determine the intersection with.
-
-        Returns:
-            Optional[Coordinate]: the intersection between the two lines (if it
-                exists, otherwise None).
-
-        Notes:
-            This is an alternative representation of the `intersect` method.
-        """
-        return self.intersect(line)
-
-    def __eq__(self, value: object) -> bool:
-        """Compare the equality of two objects.
-
-        Args:
-            value (object): the other object to compare.
-
-        Returns:
-            bool: the result of the operation.
-        """
-        if not isinstance(value, Line):
-            raise TypeError(self._ERROR_MSGS.get("TypeError2"))
-
-        return {self.a, self.b} == {value.a, value.b}
-
-    def __ne__(self, value: object) -> bool:
-        """Compare the inequality of two objects.
-
-        Args:
-            value (object): the other object to compare.
-
-        Returns:
-            bool: the result of the operation.
-        """
-        if not isinstance(value, Line):
-            raise TypeError(self._ERROR_MSGS.get("TypeError2"))
-
-        return {self.a, self.b} != {value.a, value.b}
-
-    def __hash__(self) -> int:
-        """Obtain the hash of the line.
-
-        Returns:
-            int: the hash of the line.
-        """
-        return hash((self.a, self.b))
-
-    def __getitem__(self, index: int) -> Coordinate:
-        """Get the coordinates of the line through indices.
-
-        Args:
-            index (int): the index of the coordinate.
-
-        Returns:
-            Coordinate: the value of the coordinate.
-
-        Raises:
-            IndexError: if the index of the coordinate is not 0 or 1.
-        """
-        if index == 0:
-            return self.a
-        elif index == 1:
-            return self.b
-        else:
-            raise IndexError("index must be 0 or 1")
-
-    def __setitem__(self, index: int, value: Coordinate) -> None:
-        """Set the coordinates of the line through indices.
-
-        Args:
-            index (int): the index of the coordinate.
-            value (Coordinate): the new value of the coordinate.
-
-        Raises:
-            IndexError: if the index of the coordinate is not 0 or 1.
-        """
-        if index == 0:
-            self.a = value
-        elif index == 1:
-            self.b = value
-        else:
-            raise IndexError("index must be 0 or 1")
-
-    def __iter__(self) -> Generator[Coordinate, None, None]:
-        """Obtain the iterable of the line.
-
-        Returns:
-            Generator[float, None, None]: the iterable of the line.
-        """
-        yield self.a
-        yield self.b
-
-    def __reversed__(self) -> Generator[Coordinate, None, None]:
-        """Obtain the reversed iterable of the line.
-
-        Returns:
-            Generator[float, None, None]: the reversed iterable of the line.
-        """
-        yield self.b
-        yield self.a
-
-    def __str__(self) -> str:
-        """Convert the line to a string.
-
-        Returns:
-            str: the line as a string.
-        """
-        return f"Line({self.a}, {self.b})"
-
-    def __repr__(self) -> str:
-        """Obtain the string representation of the line.
-
-        Returns:
-            str: the string representation of the line.
-        """
-        return f"Line({self.a}, {self.b})"
-
-
-class Segment(Line):
-    """A class to represent a segment in 2D space.
-
-    This class provides a way to represent a segment in 2D space. It must be
-    composed by two Coordinate objects.
-
-    Attributes:
-        a (Coordinate): the first coordinate.
-        b (Coordinate): the second coordinate.
-        slope (float): the slope of the segment.
-    """
-
-    STYLES = {
-        "color": "#396fe3",
-        "lw": 1.5,
-        "alpha": .9
-    }
-
-    def __init__(self, a: Coordinate, b: Coordinate) -> None:
-        """Initialize a segment instance.
-
-        Args:
-            a (Coordinate): the first coordinate.
-            b (Coordinate): the second coordinate.
-        """
-        super().__init__(a, b)
-
-    @property
-    def x(self) -> float:
-        """Get the x difference between the two coordinates.
-
-        Returns:
-            float: The x difference between the two coordinates.
-        """
-        return self.b.x - self.a.x
-
-    @property
-    def y(self) -> float:
-        """Get the y difference between the two coordinates.
-
-        Returns:
-            float: The y difference between the two coordinates.
-        """
-        return self.b.y - self.a.y
-
-    @property
-    def distance(self) -> float:
-        """Get the cartesian distance between the two coordinates.
-
-        Returns:
-            float: The y difference between the two coordinates.
-        """
-        if self._properties.get("distance") is None:
-            self._properties["distance"] = op.distance(self._a, self._b)
-
-        return self._properties["distance"]
-
-    def intersect(self, line: Line) -> Optional[Coordinate]:
-        """Determine the intersection between two segments.
-
-        Args:
-            line (Line): the line to determine the intersection with.
-
-        Raises:
-            TypeError: if line is not a Line object.
-
-        Returns:
-            Optional[Coordinate]: the intersection between the two segments (if it
-                exists, otherwise None).
-        """
-        if not isinstance(line, Line):
-            raise TypeError(f"Expected Line, got {type(line)}")
-
-        intersection = super().intersect(line)
-        if intersection is None:
-            return None
-
-        if (
-            self.a.x <= intersection.x <= self.b.x
-            or self.b.x <= intersection.x <= self.a.x
-        ) and (
-            self.a.y <= intersection.y <= self.b.y
-            or self.b.y <= intersection.y <= self.a.y
-        ) and (
-            line.a.x <= intersection.x <= line.b.x
-            or line.b.x <= intersection.x <= line.a.x
-        ) and (
-            line.a.y <= intersection.y <= line.b.y
-            or line.b.y <= intersection.y <= line.a.y
-        ):
-            return intersection
-
-        return None
-
-    def plot(self, *args, ax: matplotlib.axes.Axes = None, **kwargs) -> None:
-        """Plot the segment.
-
-        Args:
-            *args: Arguments to pass to the plot function.
-            ax (matplotlib.axes.Axes, optional): The axes to plot on. Defaults
-                to None (if None, the current axes will be used).
-            **kwargs: Keyword arguments to pass to the plot
-        """
-        styles = self.STYLES.copy()
-        styles.update(kwargs)
-        shape = args[0] if args else '-'
-        ax = plt.gca() if ax is None else ax
-
-        ax.plot(
-            (self._a.x, self._b.x), (self._a.y, self._b.y),
-            shape, **styles
-        )
-
-    def __eq__(self, value: object) -> bool:
-        """Compare the equality of two objects.
-
-        Args:
-            value (object): the other object to compare.
-
-        Returns:
-            bool: the result of the operation.
-        """
-        if not isinstance(value, Segment):
-            raise TypeError("value must be a Segment object.")
-
-        return {self.a, self.b} == {value.a, value.b}
-
-    def __ne__(self, value: object) -> bool:
-        """Compare the inequality of two objects.
-
-        Args:
-            value (object): the other object to compare.
-
-        Returns:
-            bool: the result of the operation.
-        """
-        if not isinstance(value, Line):
-            raise TypeError(self._ERROR_MSGS.get("TypeError2"))
-
-        return {self.a, self.b} != {value.a, value.b}
-
-    def __hash__(self) -> int:
-        """Obtain the hash of the segment.
-
-        Returns:
-            int: the hash of the segment.
-        """
-        return hash(hash(self.a) + hash(self.b))
-
-    def __str__(self) -> str:
-        """Convert the segment to a string.
-
-        Returns:
-            str: the segment as a string.
-        """
-        return f"Segment({self.a}, {self.b})"
-
-    def __repr__(self) -> str:
-        """Obtain the string representation of the segment.
-
-        Returns:
-            str: the string representation of the segment.
-        """
-        return f"Segment({self.a}, {self.b})"
+"""Coordinate class container module.
+
+This module contains the Coordinate class, which is used to represent a 2D
+coordinate. It is used by all classes in the `bidimensional` package and
+presents many similarities to the builtin `tuple` class.
+
+Author:
+    Paulo Sanchez (@erlete)
+"""
+
+
+from __future__ import annotations
+
+from math import ceil, floor, trunc
+from typing import Any, Dict, Generator, Sequence, Union
+
+import matplotlib.pyplot as plt
+
+
+class Coordinate(Sequence):
+    """Real-value, bidimensional coordinate.
+
+    This class represents a two-dimensional coordinate. Its main purpose is to
+    serve as a normalized conversion format for data going in and out of the
+    scripts contained in the project.
+
+    Args:
+        x (float): the x value of the coordinate.
+        y (float): the y value of the coordinate.
+        STYLES (Dict[str, Any]): the dictionary containing default matplotlib
+            styles for coordinate plotting.
+    """
+
+    __slots__ = ("_x", "_y")
+
+    STYLES: Dict[str, Any] = {
+        "color": "#396fe3",
+        "ms": 10
+    }
+
+    def __init__(self, x: Union[int, float], y: Union[int, float]) -> None:
+        """Initialize a coordinate instance.
+
+        Args:
+            x (Union[int, float]): the X component of the coordinate.
+            y (Union[int, float]): the Y component of the coordinate.
+        """
+        self.x: float = x
+        self.y: float = y
+
+    @property
+    def x(self) -> float:
+        """Get the X component of the coordinate.
+
+        Returns:
+            float: the X component of the coordinate.
+        """
+        return self._x
+
+    @x.setter
+    def x(self, value: Union[int, float]) -> None:
+        """Set the X component of the coordinate.
+
+        Args:
+            value (Union[int, float]): the X component of the coordinate.
+
+        Raises:
+            TypeError: if `value` is not a type `int` or `float`.
+        """
+        if not isinstance(value, (int, float)):
+            raise TypeError(
+                "expected \"int\" or \"float\", "
+                + f"got \"{value.__class__.__name__}\""
+            )
+
+        self._x = float(value)
+
+    @property
+    def y(self) -> float:
+        """Get the Y component of the coordinate.
+
+        Returns:
+            float: the Y component of the coordinate.
+        """
+        return self._y
+
+    @y.setter
+    def y(self, value: Union[int, float]) -> None:
+        """Set the X component of the coordinate.
+
+        Args:
+            value (Union[int, float]): the X component of the coordinate.
+
+        Raises:
+            TypeError: if `value` is not a type `int` or `float`.
+        """
+        if not isinstance(value, (int, float)):
+            raise TypeError(
+                "expected \"int\" or \"float\", "
+                + f"got \"{value.__class__.__name__}\""
+            )
+
+        self._y = float(value)
+
+    def plot(self, *args, ax=None, annotate=False, **kwargs) -> None:
+        """Plot the coordinate.
+
+        Args:
+            *args (tuple): Arguments to pass to the plot function.
+            ax (matplotlib.axes.Axes, optional): The axes to plot on. Defaults
+                to None (if None, the current axes will be used).
+            annotate (bool, optional): Whether to annotate the coordinate.
+            **kwargs (dict): Keyword arguments to pass to the plot
+        """
+        styles = self.STYLES.copy()
+        styles.update(kwargs)
+        shape = args[0] if args else '.'
+        ax = plt.gca() if ax is None else ax
+
+        if annotate:
+            ax.annotate(f"({self._x:.4f}, {self._y:.4f})", (self._x, self._y))
+
+        ax.plot(self._x, self._y, shape, **styles)
+
+    def __add__(self, value: Coordinate) -> Coordinate:
+        """Add two coordinates.
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            return Coordinate(self._x + value.x, self._y + value.y)
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __sub__(self, value: Coordinate) -> Coordinate:
+        """Subtract two coordinates.
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            return Coordinate(self._x - value.x, self._y - value.y)
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __mul__(self, value: Coordinate) -> Coordinate:
+        """Multiply two coordinates.
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            return Coordinate(self._x * value.x, self._y * value.y)
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __truediv__(self, value: Coordinate) -> Coordinate:
+        """Divide two coordinates (floating point).
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            return Coordinate(self._x * value.x, self._y * -value.y)
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __floordiv__(self, value: Coordinate) -> Coordinate:
+        """Divide two coordinates (floor result).
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            temp = floor(self / value)
+            return Coordinate(temp.x, temp.y)
+        self.__class__.__name__
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __mod__(self, value: Coordinate) -> Coordinate:
+        """Modulus of two coordinates.
+
+        Args:
+            value (Coordinate): the other coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if isinstance(value, Coordinate):
+            temp = (self / value - self // value) * value
+            return Coordinate(temp.x, temp.y)
+
+        raise TypeError(
+            f"expected \"{self.__class__.__name__}\", "
+            + f"got \"{value.__class__.__name__}\""
+        )
+
+    def __neg__(self) -> Coordinate:
+        """Negate a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(-self._x, -self._y)
+
+    def __pos__(self) -> Coordinate:
+        """Positivize a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(+self._x, +self._y)
+
+    def __abs__(self) -> Coordinate:
+        """Return the absolute value of a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(abs(self._x), abs(self._y))
+
+    def __round__(self, n: int = 0) -> Coordinate:
+        """Round a coordinate.
+
+        Args:
+            n (int, optional): the digits of precission for the rounding
+                operation. Defaults to 0.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        if not isinstance(n, int):
+            raise TypeError("n must be an int.")
+
+        return Coordinate(round(self._x, n), round(self._y, n))
+
+    def __floor__(self) -> Coordinate:
+        """Floor a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(floor(self._x), floor(self._y))
+
+    def __ceil__(self) -> Coordinate:
+        """Ceil a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(ceil(self._x), ceil(self._y))
+
+    def __trunc__(self) -> Coordinate:
+        """Truncate a coordinate.
+
+        Returns:
+            Coordinate: the result of the operation.
+        """
+        return Coordinate(trunc(self._x), trunc(self._y))
+
+    def __eq__(self, value: object) -> bool:
+        """Compare the equality of two objects.
+
+        Args:
+            value (object): the other coordinate.
+
+        Returns:
+            bool: the result of the operation.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError(
+                f"expected \"{self.__class__.__name__}\", "
+                + f"got \"{value.__class__.__name__}\""
+            )
+
+        return self._x == value.x and self._y == value.y
+
+    def __ne__(self, value: object) -> bool:
+        """Compare the inequality of two objects.
+
+        Args:
+            value (object): the other coordinate.
+
+        Returns:
+            bool: the result of the operation.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError(
+                f"expected \"{self.__class__.__name__}\", "
+                + f"got \"{value.__class__.__name__}\""
+            )
+
+        return self._x != value.x or self._y != value.y
+
+    def __str__(self) -> str:
+        """Convert the coordinate to a string.
+
+        Returns:
+            str: the coordinate as a string.
+        """
+        return f"Coordinate({self._x}, {self._y})"
+
+    def __repr__(self) -> str:
+        """Obtain the string representation of the coordinate.
+
+        Returns:
+            str: the string representation of the coordinate.
+        """
+        return f"Coordinate({self._x}, {self._y})"
+
+    def __hash__(self) -> int:
+        """Obtain the hash of the coordinate.
+
+        Returns:
+            int: the hash of the coordinate.
+        """
+        return hash((self._x, self._y))
+
+    def __bool__(self) -> bool:
+        """Obtain the boolean value of the coordinate.
+
+        Returns:
+            bool: the boolean value of the coordinate.
+        """
+        return self._x != 0 or self._y != 0
+
+    def __len__(self) -> int:
+        """Obtain the amount of terms in the coordinate.
+
+        Returns:
+            int: the amount of terms in the coordinate.
+        """
+        return 2
+
+    def __getitem__(self, index: Union[int, slice]) -> Any:
+        """Get the X, Y coordinate components via index or slice.
+
+        Args:
+            index (Union[int, slice]): the index or slice of the component(s).
+
+        Returns:
+            Any: the value(s) of the component(s).
+
+        Raises:
+            IndexError: if the index of the component is not 0 or 1.
+            TypeError: if the index is not an int or a slice.
+        """
+        if isinstance(index, int):
+            if index == 0:
+                return self._x
+            elif index == 1:
+                return self._y
+            else:
+                raise IndexError("index must be 0 (x) or 1 (y)")
+
+        elif isinstance(index, slice):
+            return (self._x, self._y)[index]
+
+        else:
+            raise TypeError("index must be an int or a slice.")
+
+    def __setitem__(self, index: Union[int, slice], value: Union[int, float]) -> None:
+        """Set the X or Y coordinate components via index or slice.
+
+        Args:
+            index (Union[int, slice]): the index or slice of the component(s).
+            value (Union[int, float]): the new value(s) of the component(s).
+
+        Raises:
+            IndexError: if the index of the component is not 0 or 1.
+            NotImplementedError: if the index is a slice.
+        """
+        if isinstance(index, int):
+            if index == 0:
+                self.x = value
+            elif index == 1:
+                self.y = value
+            else:
+                raise IndexError("index must be 0 (x) or 1 (y)")
+
+        elif isinstance(index, slice):
+            raise NotImplementedError(
+                "slice attribute assignment is not supported"
+            )
+
+        else:
+            raise TypeError("index must be an int or a slice.")
+
+    def __iter__(self) -> Generator[float, None, None]:
+        """Obtain the iterable of the coordinate.
+
+        Returns:
+            Generator[float, None, None]: the iterable of the coordinate.
+        """
+        yield self._x
+        yield self._y
+
+    def __reversed__(self) -> Generator[float, None, None]:
+        """Obtain the reversed iterable of the coordinate.
+
+        Returns:
+            Generator[float, None, None]: the reversed iterable of the
+                coordinate.
+        """
+        yield self._y
+        yield self._x
+
+    def __copy__(self) -> Coordinate:
+        """Copy the coordinate.
+
+        Returns:
+            Coordinate: the copy of the coordinate.
+        """
+        return self.__class__(self._x, self._y)
```

### Comparing `bidimensional-1.9.0/src/bidimensional/core/operations.py` & `bidimensional-1.9.1/src/bidimensional/core/operations.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-"""2D operations module.
-
-This module contains methods used to perform operations on 2D coordinates, such
-as calculating distances and angles between them.
-
-Author:
-    Paulo Sanchez (@erlete)
-"""
-
-
-import math
-from itertools import combinations
-
-from .coordinate import Coordinate
-
-
-def distance(a: Coordinate, b: Coordinate) -> float:
-    """Calculate the distance between two coordinates.
-
-    Args:
-        a (Coordinate): first coordinate.
-        b (Coordinate): second coordinate.
-
-    Raises:
-        TypeError: if a or b are not Coordinate objects.
-
-    Returns:
-        float: distance between the two coordinates.
-    """
-    if not all(isinstance(x, Coordinate) for x in (a, b)):
-        raise TypeError("a and b must be Coordinate instances")
-
-    return math.sqrt((a.x - b.x) ** 2 + (a.y - b.y) ** 2)
-
-
-def angle(a: Coordinate, b: Coordinate, c: Coordinate) -> float:
-    """Calculate the angle between three coordinates.
-
-    Args:
-        a (Coordinate): first coordinate.
-        b (Coordinate): second coordinate.
-        c (Coordinate): third coordinate.
-
-    Raises:
-        TypeError: if a, b or c are not Coordinate objects.
-
-    Returns:
-        float: angle between the three coordinates.
-    """
-    if not all(isinstance(x, Coordinate) for x in (a, b, c)):
-        raise TypeError("a, b and c must be Coordinate instances")
-
-    e1 = distance(b, c)
-    e2 = distance(a, c)
-    e3 = distance(a, b)
-
-    return math.degrees(math.acos(
-        (math.pow(e2, 2) + math.pow(e3, 2) - math.pow(e1, 2)) / (2 * e2 * e3)
-    ))
-
-
-def midpoint(a: Coordinate, b: Coordinate) -> Coordinate:
-    """Calculate the midpoint between two coordinates.
-
-    Args:
-        a (Coordinate): first coordinate.
-        b (Coordinate): second coordinate.
-
-    Raises:
-        TypeError: if a or b are not Coordinate objects.
-
-    Returns:
-        Coordinate: midpoint between the two coordinates.
-    """
-    if not all(isinstance(x, Coordinate) for x in (a, b)):
-        raise TypeError("a and b must be Coordinate instances")
-
-    return Coordinate((a.x + b.x) / 2, (a.y + b.y) / 2)
-
-
-def area(*vertices: Coordinate) -> float:
-    """Calculate the area of a polygon.
-
-    Args:
-        *vertices (Coordinate): vertices of the polygon.
-
-    Returns:
-        float: area of the polygon.
-    """
-    x = [vertex.x for vertex in vertices]
-    y = [vertex.y for vertex in vertices]
-
-    area: float = 0
-
-    j = -1
-    for i in range(len(vertices)):
-        area += (x[j] + x[i]) * (y[j] - y[i])
-        j = i
-
-    return abs(area / 2)
-
-
-def perimeter(*coordinates: Coordinate) -> float:
-    """Calculate the perimeter of a polygon.
-
-    Args:
-        *coordinates (Coordinate): coordinates of the polygon.
-
-    Raises:
-        TypeError: if any of the coordinates are not Coordinate objects.
-
-    Returns:
-        float: perimeter of the polygon.
-    """
-    if not all(isinstance(x, Coordinate) for x in coordinates):
-        raise TypeError("All coordinates must be Coordinate instances")
-
-    return sum(distance(*pair) for pair in combinations(coordinates, 2))
+"""2D operations module.
+
+This module contains methods used to perform operations on 2D coordinates, such
+as calculating distances and angles between them.
+
+Author:
+    Paulo Sanchez (@erlete)
+"""
+
+
+import math
+from itertools import combinations
+
+from .coordinate import Coordinate
+
+
+def distance(a: Coordinate, b: Coordinate) -> float:
+    """Calculate the distance between two coordinates.
+
+    Args:
+        a (Coordinate): first coordinate.
+        b (Coordinate): second coordinate.
+
+    Raises:
+        TypeError: if a or b are not Coordinate objects.
+
+    Returns:
+        float: distance between the two coordinates.
+    """
+    if not all(isinstance(x, Coordinate) for x in (a, b)):
+        raise TypeError("a and b must be Coordinate instances")
+
+    return math.sqrt((a.x - b.x) ** 2 + (a.y - b.y) ** 2)
+
+
+def angle(a: Coordinate, b: Coordinate, c: Coordinate) -> float:
+    """Calculate the angle between three coordinates.
+
+    Args:
+        a (Coordinate): first coordinate.
+        b (Coordinate): second coordinate.
+        c (Coordinate): third coordinate.
+
+    Raises:
+        TypeError: if a, b or c are not Coordinate objects.
+
+    Returns:
+        float: angle between the three coordinates.
+    """
+    if not all(isinstance(x, Coordinate) for x in (a, b, c)):
+        raise TypeError("a, b and c must be Coordinate instances")
+
+    e1 = distance(b, c)
+    e2 = distance(a, c)
+    e3 = distance(a, b)
+
+    return math.degrees(math.acos(
+        (math.pow(e2, 2) + math.pow(e3, 2) - math.pow(e1, 2)) / (2 * e2 * e3)
+    ))
+
+
+def midpoint(a: Coordinate, b: Coordinate) -> Coordinate:
+    """Calculate the midpoint between two coordinates.
+
+    Args:
+        a (Coordinate): first coordinate.
+        b (Coordinate): second coordinate.
+
+    Raises:
+        TypeError: if a or b are not Coordinate objects.
+
+    Returns:
+        Coordinate: midpoint between the two coordinates.
+    """
+    if not all(isinstance(x, Coordinate) for x in (a, b)):
+        raise TypeError("a and b must be Coordinate instances")
+
+    return Coordinate((a.x + b.x) / 2, (a.y + b.y) / 2)
+
+
+def area(*vertices: Coordinate) -> float:
+    """Calculate the area of a polygon.
+
+    Args:
+        *vertices (Coordinate): vertices of the polygon.
+
+    Returns:
+        float: area of the polygon.
+    """
+    x = [vertex.x for vertex in vertices]
+    y = [vertex.y for vertex in vertices]
+
+    area: float = 0
+
+    j = -1
+    for i in range(len(vertices)):
+        area += (x[j] + x[i]) * (y[j] - y[i])
+        j = i
+
+    return abs(area / 2)
+
+
+def perimeter(*coordinates: Coordinate) -> float:
+    """Calculate the perimeter of a polygon.
+
+    Args:
+        *coordinates (Coordinate): coordinates of the polygon.
+
+    Raises:
+        TypeError: if any of the coordinates are not Coordinate objects.
+
+    Returns:
+        float: perimeter of the polygon.
+    """
+    if not all(isinstance(x, Coordinate) for x in coordinates):
+        raise TypeError("All coordinates must be Coordinate instances")
+
+    return sum(distance(*pair) for pair in combinations(coordinates, 2))
```

### Comparing `bidimensional-1.9.0/src/bidimensional/polygons/polygon.py` & `bidimensional-1.9.1/src/bidimensional/polygons/polygon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,311 +1,311 @@
-"""Container module for the Polygon class.
-
-Author:
-    Paulo Sanchez (@erlete)
-"""
-
-from __future__ import annotations
-
-from itertools import combinations_with_replacement as cr
-from math import ceil, log
-from string import ascii_lowercase, ascii_uppercase
-from typing import Dict, Sequence
-
-import matplotlib
-import matplotlib.pyplot as plt
-
-from ..core import operations as op
-from ..core.coordinate import Coordinate
-from ..core.lines import Segment
-
-
-class Polygon:
-    """Generic polygon class.
-
-    This class represents a generic polygon in the bidimensional plane. It is
-    composed of a set of vertices, which are instances of the Coordinate class.
-
-    Attributes:
-        ANNOTATIONS (Dict[str, str]): annotations for the vertices and sides of
-            the polygon.
-        vertices (Dict[str, Coordinate]): vertices of the polygon.
-        sides (Dict[str, Segment]): sides of the polygon.
-        area (float): area of the polygon.
-        perimeter (float): perimeter of the polygon.
-    """
-
-    ANNOTATIONS: Dict[str, str] = {
-        "vertices": ascii_uppercase,
-        "sides": ascii_lowercase
-    }
-
-    def __init__(self, *vertices: Coordinate):
-        """Initialize a polygon instance.
-
-        Args:
-            *vertices (Coordinate): vertices of the polygon.
-
-        Notes:
-            Duplicate vertices are removed from the list of vertices upon
-            polygon instantiation.
-        """
-        vertices = [  # type: ignore
-            vertex for i, vertex in enumerate(vertices)
-            if vertex not in vertices[:i]
-        ]
-        self.vertices = vertices  # type: ignore
-        self.sides = [  # type: ignore
-            Segment(vertices[i], vertices[i + 1])
-            for i in range(len(vertices) - 1)
-        ] + [Segment(vertices[-1], vertices[0])]
-
-    @property
-    def vertices(self) -> Dict[str, Coordinate]:
-        """Get the vertices of the polygon.
-
-        Returns:
-            Dict[str, Coordinate]: vertices of the polygon.
-        """
-        return self._vertices
-
-    @vertices.setter
-    def vertices(self, vertices: Sequence[Coordinate]) -> None:
-        """Set the vertices of the polygon.
-
-        Args:
-            vertices (Sequence[Coordinate]): vertices of the polygon.
-
-        Raises:
-            TypeError: if any of the vertices is not of type Coordinate.
-            ValueError: if the number of vertices is less than 3.
-        """
-        if len(vertices) < 3:
-            raise ValueError("a polygon must have at least 3 vertices")
-
-        if any(not isinstance(vertex, Coordinate) for vertex in vertices):
-            raise TypeError("all vertices must be of type Coordinate")
-
-        characters = self.ANNOTATIONS["vertices"]
-        padding = ceil(log(len(vertices), len(characters)))
-
-        annotations = [
-            ''.join(letters)
-            for letters in sorted(
-                set(
-                    list(cr(characters, padding))
-                    + list(cr(reversed(characters), padding))
-                )
-            )
-        ]
-
-        self._vertices = {
-            annotation: vertex
-            for annotation, vertex in zip(annotations, vertices)
-        }
-
-    @property
-    def sides(self) -> Dict[str, Segment]:
-        """Get the sides of the polygon.
-
-        Returns:
-            Dict[str, Segment]: sides of the polygon.
-        """
-        return self._sides
-
-    @sides.setter
-    def sides(self, sides: Sequence[Segment]) -> None:
-        """Set the sides of the polygon.
-
-        Args:
-            sides (Sequence[Segment]): sides of the polygon.
-
-        Raises:
-            TypeError: if any of the sides is not of type Segment.
-        """
-        if any(not isinstance(vertex, Segment) for vertex in sides):
-            raise TypeError("all sides must be of type Segment")
-
-        characters = self.ANNOTATIONS["sides"]
-        padding = ceil(log(len(sides), len(characters)))
-
-        annotations = [
-            ''.join(letters)
-            for letters in sorted(
-                set(
-                    list(cr(characters, padding))
-                    + list(cr(reversed(characters), padding))
-                )
-            )
-        ]
-
-        self._sides = {
-            annotation: side
-            for annotation, side in zip(annotations, sides)
-        }
-
-    @property
-    def area(self) -> float:
-        """Get the area of the polygon.
-
-        Returns:
-            float: area of the polygon.
-        """
-        return op.area(*self.vertices.values())
-
-    @property
-    def perimeter(self) -> float:
-        """Get the perimeter of the polygon.
-
-        Returns:
-            float: perimeter of the polygon.
-        """
-        return sum(side.distance for side in self.sides.values())
-
-    def plot(self, ax: matplotlib.axes.Axes = None,
-             annotate: bool = True, **kwargs) -> None:
-        """Plot the polygon.
-
-        Args:
-            ax (matplotlib.axes.Axes, optional): axes to plot on. Defaults to
-                None.
-            annotate (bool, optional): whether to annotate the vertices.
-                Defaults to True.
-            **kwargs: keyword arguments for `matplotlib.pyplot.plot`.
-        """
-        if ax is None:
-            ax = plt.gca()
-
-        for label, vertex in self._vertices.items():
-            vertex.plot(ax=ax)
-            if annotate:
-                ax.annotate(label, vertex, fontsize=10, fontweight="bold")
-
-        for label, side in self._sides.items():
-            side.plot(ax=ax)
-            if annotate:
-                ax.annotate(label, op.midpoint(*side), fontsize=10)
-
-    def __repr__(self) -> str:
-        """Get the raw representation of the polygon.
-
-        Returns:
-            str: raw representation of the polygon.
-        """
-        return f"Polygon({len(self.vertices)} vertices)"
-
-    def __str__(self) -> str:
-        """Get the string representation of the polygon.
-
-        Returns:
-            str: string representation of the polygon.
-        """
-        return (
-            "Polygon(\n    "
-            + ",\n    ".join(map(str, self.vertices.values()))
-            + "\n)"
-        )
-
-    def __eq__(self, other: object) -> bool:
-        """Determine if the polygon is equal to another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is equal to the other object.
-        """
-        if not isinstance(other, Polygon):
-            return False
-
-        return set(self.vertices.values()) == set(other.vertices.values())
-
-    def __ne__(self, other: object) -> bool:
-        """Determine if the polygon is not equal to another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is not equal to the other object.
-        """
-        return not self == other
-
-    def __gt__(self, other: object) -> bool:
-        """Determine if the polygon is greater than another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is greater than the other object.
-        """
-        if not isinstance(other, Polygon):
-            return False
-
-        return self.area > other.area
-
-    def __ge__(self, other: object) -> bool:
-        """Determine if the polygon is greater than or equal to another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is greater than or equal to the other object.
-        """
-        if not isinstance(other, Polygon):
-            return False
-
-        return self.area >= other.area
-
-    def __lt__(self, other: object) -> bool:
-        """Determine if the polygon is less than another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is less than the other object.
-        """
-        if not isinstance(other, Polygon):
-            return False
-
-        return self.area < other.area
-
-    def __le__(self, other: object) -> bool:
-        """Determine if the polygon is less than or equal to another object.
-
-        Args:
-            other (object): object to compare to.
-
-        Returns:
-            bool: if the polygon is less than or equal to the other object.
-        """
-        if not isinstance(other, Polygon):
-            return False
-
-        return self.area <= other.area
-
-    def __bool__(self) -> bool:
-        """Determine the boolean state of the polygon.
-
-        Returns:
-            bool: the boolean state of the polygon.
-        """
-        return bool(self.vertices)
-
-    def __len__(self) -> int:
-        """Get the number of vertices of the polygon.
-
-        Returns:
-            int: number of vertices of the polygon.
-        """
-        return len(self.vertices)
-
-    def __hash__(self) -> int:
-        """Get the hash of the polygon.
-
-        Returns:
-            int: hash of the polygon.
-        """
-        return hash(set(self.vertices.values()))
+"""Container module for the Polygon class.
+
+Author:
+    Paulo Sanchez (@erlete)
+"""
+
+from __future__ import annotations
+
+from itertools import combinations_with_replacement as cr
+from math import ceil, log
+from string import ascii_lowercase, ascii_uppercase
+from typing import Dict, Sequence
+
+import matplotlib
+import matplotlib.pyplot as plt
+
+from ..core import operations as op
+from ..core.coordinate import Coordinate
+from ..core.lines import Segment
+
+
+class Polygon:
+    """Generic polygon class.
+
+    This class represents a generic polygon in the bidimensional plane. It is
+    composed of a set of vertices, which are instances of the Coordinate class.
+
+    Attributes:
+        ANNOTATIONS (Dict[str, str]): annotations for the vertices and sides of
+            the polygon.
+        vertices (Dict[str, Coordinate]): vertices of the polygon.
+        sides (Dict[str, Segment]): sides of the polygon.
+        area (float): area of the polygon.
+        perimeter (float): perimeter of the polygon.
+    """
+
+    ANNOTATIONS: Dict[str, str] = {
+        "vertices": ascii_uppercase,
+        "sides": ascii_lowercase
+    }
+
+    def __init__(self, *vertices: Coordinate):
+        """Initialize a polygon instance.
+
+        Args:
+            *vertices (Coordinate): vertices of the polygon.
+
+        Notes:
+            Duplicate vertices are removed from the list of vertices upon
+            polygon instantiation.
+        """
+        vertices = [  # type: ignore
+            vertex for i, vertex in enumerate(vertices)
+            if vertex not in vertices[:i]
+        ]
+        self.vertices = vertices  # type: ignore
+        self.sides = [  # type: ignore
+            Segment(vertices[i], vertices[i + 1])
+            for i in range(len(vertices) - 1)
+        ] + [Segment(vertices[-1], vertices[0])]
+
+    @property
+    def vertices(self) -> Dict[str, Coordinate]:
+        """Get the vertices of the polygon.
+
+        Returns:
+            Dict[str, Coordinate]: vertices of the polygon.
+        """
+        return self._vertices
+
+    @vertices.setter
+    def vertices(self, vertices: Sequence[Coordinate]) -> None:
+        """Set the vertices of the polygon.
+
+        Args:
+            vertices (Sequence[Coordinate]): vertices of the polygon.
+
+        Raises:
+            TypeError: if any of the vertices is not of type Coordinate.
+            ValueError: if the number of vertices is less than 3.
+        """
+        if len(vertices) < 3:
+            raise ValueError("a polygon must have at least 3 vertices")
+
+        if any(not isinstance(vertex, Coordinate) for vertex in vertices):
+            raise TypeError("all vertices must be of type Coordinate")
+
+        characters = self.ANNOTATIONS["vertices"]
+        padding = ceil(log(len(vertices), len(characters)))
+
+        annotations = [
+            ''.join(letters)
+            for letters in sorted(
+                set(
+                    list(cr(characters, padding))
+                    + list(cr(reversed(characters), padding))
+                )
+            )
+        ]
+
+        self._vertices = {
+            annotation: vertex
+            for annotation, vertex in zip(annotations, vertices)
+        }
+
+    @property
+    def sides(self) -> Dict[str, Segment]:
+        """Get the sides of the polygon.
+
+        Returns:
+            Dict[str, Segment]: sides of the polygon.
+        """
+        return self._sides
+
+    @sides.setter
+    def sides(self, sides: Sequence[Segment]) -> None:
+        """Set the sides of the polygon.
+
+        Args:
+            sides (Sequence[Segment]): sides of the polygon.
+
+        Raises:
+            TypeError: if any of the sides is not of type Segment.
+        """
+        if any(not isinstance(vertex, Segment) for vertex in sides):
+            raise TypeError("all sides must be of type Segment")
+
+        characters = self.ANNOTATIONS["sides"]
+        padding = ceil(log(len(sides), len(characters)))
+
+        annotations = [
+            ''.join(letters)
+            for letters in sorted(
+                set(
+                    list(cr(characters, padding))
+                    + list(cr(reversed(characters), padding))
+                )
+            )
+        ]
+
+        self._sides = {
+            annotation: side
+            for annotation, side in zip(annotations, sides)
+        }
+
+    @property
+    def area(self) -> float:
+        """Get the area of the polygon.
+
+        Returns:
+            float: area of the polygon.
+        """
+        return op.area(*self.vertices.values())
+
+    @property
+    def perimeter(self) -> float:
+        """Get the perimeter of the polygon.
+
+        Returns:
+            float: perimeter of the polygon.
+        """
+        return sum(side.distance for side in self.sides.values())
+
+    def plot(self, ax: matplotlib.axes.Axes = None,
+             annotate: bool = True, **kwargs) -> None:
+        """Plot the polygon.
+
+        Args:
+            ax (matplotlib.axes.Axes, optional): axes to plot on. Defaults to
+                None.
+            annotate (bool, optional): whether to annotate the vertices.
+                Defaults to True.
+            **kwargs: keyword arguments for `matplotlib.pyplot.plot`.
+        """
+        if ax is None:
+            ax = plt.gca()
+
+        for label, vertex in self._vertices.items():
+            vertex.plot(ax=ax, **kwargs)
+            if annotate:
+                ax.annotate(label, vertex, fontsize=10, fontweight="bold")
+
+        for label, side in self._sides.items():
+            side.plot(ax=ax, **kwargs)
+            if annotate:
+                ax.annotate(label, op.midpoint(*side), fontsize=10)
+
+    def __repr__(self) -> str:
+        """Get the raw representation of the polygon.
+
+        Returns:
+            str: raw representation of the polygon.
+        """
+        return f"Polygon({len(self.vertices)} vertices)"
+
+    def __str__(self) -> str:
+        """Get the string representation of the polygon.
+
+        Returns:
+            str: string representation of the polygon.
+        """
+        return (
+            "Polygon(\n    "
+            + ",\n    ".join(map(str, self.vertices.values()))
+            + "\n)"
+        )
+
+    def __eq__(self, other: object) -> bool:
+        """Determine if the polygon is equal to another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is equal to the other object.
+        """
+        if not isinstance(other, Polygon):
+            return False
+
+        return set(self.vertices.values()) == set(other.vertices.values())
+
+    def __ne__(self, other: object) -> bool:
+        """Determine if the polygon is not equal to another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is not equal to the other object.
+        """
+        return not self == other
+
+    def __gt__(self, other: object) -> bool:
+        """Determine if the polygon is greater than another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is greater than the other object.
+        """
+        if not isinstance(other, Polygon):
+            return False
+
+        return self.area > other.area
+
+    def __ge__(self, other: object) -> bool:
+        """Determine if the polygon is greater than or equal to another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is greater than or equal to the other object.
+        """
+        if not isinstance(other, Polygon):
+            return False
+
+        return self.area >= other.area
+
+    def __lt__(self, other: object) -> bool:
+        """Determine if the polygon is less than another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is less than the other object.
+        """
+        if not isinstance(other, Polygon):
+            return False
+
+        return self.area < other.area
+
+    def __le__(self, other: object) -> bool:
+        """Determine if the polygon is less than or equal to another object.
+
+        Args:
+            other (object): object to compare to.
+
+        Returns:
+            bool: if the polygon is less than or equal to the other object.
+        """
+        if not isinstance(other, Polygon):
+            return False
+
+        return self.area <= other.area
+
+    def __bool__(self) -> bool:
+        """Determine the boolean state of the polygon.
+
+        Returns:
+            bool: the boolean state of the polygon.
+        """
+        return bool(self.vertices)
+
+    def __len__(self) -> int:
+        """Get the number of vertices of the polygon.
+
+        Returns:
+            int: number of vertices of the polygon.
+        """
+        return len(self.vertices)
+
+    def __hash__(self) -> int:
+        """Get the hash of the polygon.
+
+        Returns:
+            int: hash of the polygon.
+        """
+        return hash(set(self.vertices.values()))
```

### Comparing `bidimensional-1.9.0/src/bidimensional/polygons/triangle.py` & `bidimensional-1.9.1/src/bidimensional/polygons/triangle.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,616 +1,616 @@
-"""Triangle polygon utilities module.
-
-This module contains all utilities related to the triangle polygon, such as
-calculating the area, perimeter, circumcenter and circumradius, etc.
-
-Author:
-    Paulo Sanchez (@erlete)
-"""
-
-from __future__ import annotations
-
-from itertools import combinations
-from math import sqrt
-from typing import Any, Dict
-
-from ..core import operations as op
-from ..core.coordinate import Coordinate
-from .polygon import Polygon
-
-
-class Circumcircle:
-    """Circumcirle calculation utility.
-
-    This class is used to calculate the circumcenter and circumradius of a
-    triangle, given its three vertices as 2D coordinates.
-
-    Attributes:
-        a (Coordinate): first vertex of the triangle.
-        b (Coordinate): second vertex of the triangle.
-        c (Coordinate): third vertex of the triangle.
-        center (Coordinate): center of the circumcircle.
-        radius (float): radius of the circumcircle.
-    """
-
-    def __init__(self, a: Coordinate, b: Coordinate, c: Coordinate) -> None:
-        """Initialize a circumcircle instance.
-
-        Args:
-            a (Coordinate): first vertex of the triangle.
-            b (Coordinate): second vertex of the triangle.
-            c (Coordinate): third vertex of the triangle.
-        """
-        self._a = a
-        self._b = b
-        self.c = c  # Automatically calls `Circumcircle._calculate` method.
-
-    @property
-    def a(self) -> Coordinate:
-        """First vertex of the triangle.
-
-        Returns:
-            Coordinate: first vertex of the triangle.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        return self._a
-
-    @a.setter
-    def a(self, value: Coordinate) -> None:
-        """First vertex of the triangle.
-
-        Args:
-            value (Coordinate): first vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("a must be a Coordinate instance")
-
-        self._a = value
-        self._calculate()
-
-    @property
-    def b(self) -> Coordinate:
-        """Second vertex of the triangle.
-
-        Returns:
-            Coordinate: second vertex of the triangle.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        return self._b
-
-    @b.setter
-    def b(self, value: Coordinate) -> None:
-        """Second vertex of the triangle.
-
-        Args:
-            value (Coordinate): second vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("b must be a Coordinate instance")
-
-        self._b = value
-        self._calculate()
-
-    @property
-    def c(self) -> Coordinate:
-        """Third vertex of the triangle.
-
-        Returns:
-            Coordinate: third vertex of the triangle.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        return self._c
-
-    @c.setter
-    def c(self, value: Coordinate) -> None:
-        """Third vertex of the triangle.
-
-        Args:
-            value (Coordinate): third vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-
-        Note:
-            If the value of the vertex is changed, the circumcenter and
-            circumradius are recalculated.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("c must be a Coordinate instance")
-
-        self._c = value
-        self._calculate()
-
-    @property
-    def center(self) -> Coordinate:
-        """Center of the circumcircle.
-
-        Returns:
-            Coordinate: center of the circumcircle.
-        """
-        return self._center
-
-    @property
-    def radius(self) -> float:
-        """Radius of the circumcircle.
-
-        Returns:
-            float: radius of the circumcircle.
-        """
-        return self._radius
-
-    def _ensure_non_collinear(self) -> None:
-        """Ensure that the triangle is not collinear.
-
-        Raises:
-            ValueError: if the triangle is collinear.
-        """
-        x_displacements = {
-            "ab": self.b.x - self.a.x,
-            "bc": self.c.x - self.b.x,
-            "ac": self.c.x - self.a.x
-        }
-
-        y_displacements = {
-            "ab": self.b.y - self.a.y,
-            "bc": self.c.y - self.b.y,
-            "ac": self.c.y - self.a.y
-        }
-
-        if (self.a.x == self.b.x == self.c.x
-                or self.a.y == self.b.y == self.c.y):
-
-            raise ValueError("The triangle is collinear")
-
-        slopes = []
-
-        if x_displacements["ab"] != 0:
-            slopes.append(y_displacements["ab"] / x_displacements["ab"])
-
-        if x_displacements["bc"] != 0:
-            slopes.append(y_displacements["bc"] / x_displacements["bc"])
-
-        if x_displacements["ac"] != 0:
-            slopes.append(y_displacements["ac"] / x_displacements["ac"])
-
-        if any(slope[0] == slope[1]
-               for slope in combinations(slopes, 2)):
-
-            raise ValueError("The triangle is collinear")
-
-    def _calculate(self) -> None:
-        """Calculate the center and radius of the circumcircle."""
-        self._ensure_non_collinear()
-
-        if any(v[1] - v[0] for v in combinations(
-                (self._a, self._b, self._c), 2)):
-
-            # Vertical alignment prevention:
-
-            if not (self._b - self._a).x:
-                self._a, self._c = self._c, self._a
-
-            if not (self._c - self._a).x:
-                self._a, self._b = self._b, self._a
-
-        # Segment displacement:
-
-        displacement = {
-            "ab": Coordinate(
-                self.b.x - self.a.x,
-                self.b.y - self.a.y
-            ),
-            "ac": Coordinate(
-                self.c.x - self.a.x,
-                self.c.y - self.a.y
-            )
-        }
-
-        # Unitary vectors:
-
-        unitary = {
-            "ab": Coordinate(
-                displacement["ab"].y / sqrt(
-                    displacement["ab"].x ** 2 + displacement["ab"].y ** 2
-                ),
-                -displacement["ab"].x / sqrt(
-                    displacement["ab"].x ** 2 + displacement["ab"].y ** 2
-                )
-            ),
-            "ac": Coordinate(
-                displacement["ac"].y / sqrt(
-                    displacement["ac"].x ** 2 + displacement["ac"].y ** 2
-                ),
-                -displacement["ac"].x / sqrt(
-                    displacement["ac"].x ** 2 + displacement["ac"].y ** 2
-                )
-            )
-        }
-
-        # V-vector for vertical intersection:
-
-        vertical = {
-            "ab": Coordinate(
-                unitary["ab"].x / unitary["ab"].y,
-                1
-            ),
-            "ac": Coordinate(
-                -(unitary["ac"].x / unitary["ac"].y),
-                1
-            )
-        }
-
-        # Midpoint setting:
-
-        midpoint = {
-            "ab": Coordinate(
-                displacement["ab"].x / 2 + self.a.x,
-                displacement["ab"].y / 2 + self.a.y
-            ),
-            "ac": Coordinate(
-                displacement["ac"].x / 2 + self.a.x,
-                displacement["ac"].y / 2 + self.a.y
-            )
-        }
-
-        # Midpoint height equivalence:
-
-        intersection = Coordinate(
-            midpoint["ab"].x + (
-                (midpoint["ac"].y - midpoint["ab"].y) / unitary["ab"].y
-            ) * unitary["ab"].x,
-            midpoint["ac"].y
-        )
-
-        # Circumcenter calculation:
-
-        self._center = Coordinate(
-            intersection.x + (
-                (midpoint["ac"].x - intersection.x)
-                / (vertical["ab"].x + vertical["ac"].x)
-            ) * vertical["ab"].x,
-            intersection.y + (
-                midpoint["ac"].x - intersection.x
-            ) / (
-                vertical["ab"].x + vertical["ac"].x
-            )
-        )
-
-        # Circumradius calculation:
-
-        self._radius = sqrt(
-            (self.a.x - self._center.x) ** 2
-            + (self.a.y - self._center.y) ** 2
-        )
-
-
-class Triangle(Polygon):
-    """Triangle class.
-
-    This class represents a triangle in the 2D plane. It is defined by three
-    vertices, a, b and c (Coordinate objects). The class provides methods to
-    compute the angles of the triangle, the circumcenter and the circumradius.
-    It also provides methods used to determine special properties of the
-    triangle, such as if it is equilateral, isosceles, scalene, right, obtuse
-    or acute.
-
-    Attributes:
-        a (Coordinate): first vertex of the triangle.
-        b (Coordinate): second vertex of the triangle.
-        c (Coordinate): third vertex of the triangle.
-        circumcenter (Coordinate): circumcenter of the triangle.
-        circumradius (float): circumradius of the triangle.
-    """
-
-    TOL_DIGITS = 10
-
-    def __init__(self, a: Coordinate, b: Coordinate, c: Coordinate) -> None:
-        """Initialize a triangle instance.
-
-        Args:
-            a (Coordinate): first vertex of the triangle.
-            b (Coordinate): second vertex of the triangle.
-            c (Coordinate): third vertex of the triangle.
-        """
-        super().__init__(a, b, c)
-        self._properties: Dict[str, Any] = {}
-
-        self.a = a
-        self.b = b
-        self.c = c
-
-    @property
-    def a(self) -> Coordinate:
-        """First vertex of the triangle.
-
-        Returns:
-            Coordinate: first vertex of the triangle.
-        """
-        return self._a
-
-    @a.setter
-    def a(self, value: Coordinate) -> None:
-        """First vertex of the triangle.
-
-        Args:
-            value (Coordinate): first vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("a must be a Coordinate instance")
-
-        self._a = value
-        self._properties.clear()
-
-    @property
-    def b(self) -> Coordinate:
-        """Second vertex of the triangle.
-
-        Returns:
-            Coordinate: second vertex of the triangle.
-        """
-        return self._b
-
-    @b.setter
-    def b(self, value: Coordinate) -> None:
-        """Second vertex of the triangle.
-
-        Args:
-            value (Coordinate): second vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("b must be a Coordinate instance")
-
-        self._b = value
-        self._properties.clear()
-
-    @property
-    def c(self) -> Coordinate:
-        """Third vertex of the triangle.
-
-        Returns:
-            Coordinate: third vertex of the triangle.
-        """
-        return self._c
-
-    @c.setter
-    def c(self, value: Coordinate) -> None:
-        """Third vertex of the triangle.
-
-        Args:
-            value (Coordinate): third vertex of the triangle.
-
-        Raises:
-            TypeError: if the value is not a Coordinate object.
-        """
-        if not isinstance(value, Coordinate):
-            raise TypeError("c must be a Coordinate instance")
-
-        self._c = value
-        self._properties.clear()
-
-    @property
-    def angles(self) -> Dict[str, float]:
-        """Inner angles of the triangle.
-
-        Returns:
-            Dict[str, float]: Angles of the triangle.
-        """
-        if self._properties.get("angles") is None:
-            self._properties["angles"] = {
-                'a': round(op.angle(self.b, self.c, self.a), self.TOL_DIGITS),
-                'b': round(op.angle(self.c, self.a, self.b), self.TOL_DIGITS),
-                'c': round(op.angle(self.a, self.b, self.c), self.TOL_DIGITS)
-            }
-
-        return self._properties["angles"]
-
-    @property
-    def circumcenter(self) -> Coordinate:
-        """Circumcenter of the triangle.
-
-        Returns:
-            Coordinate: Circumcenter of the triangle.
-        """
-        if self._properties.get("circumcircle") is None:
-            self._properties["circumcircle"] = Circumcircle(
-                self.a, self.b, self.c
-            )
-
-        return self._properties["circumcircle"].center
-
-    @property
-    def circumradius(self) -> float:
-        """Circumradius of the triangle.
-
-        Returns:
-            float: Circumradius of the triangle.
-        """
-        if self._properties.get("circumcircle") is None:
-            self._properties["circumcircle"] = Circumcircle(
-                self.a, self.b, self.c
-            )
-
-        return self._properties["circumcircle"].radius
-
-    def is_right(self) -> bool:
-        """Check whether the triangle has a right angle.
-
-        Returns:
-            bool: `True` if the triangle has a right angle, `False` otherwise.
-        """
-        return any(
-            round(angle_, self.TOL_DIGITS) == 90
-            for angle_ in self.angles.values()
-        )
-
-    def is_obtuse(self) -> bool:
-        """Check whether the triangle has an obtuse angle.
-
-        Returns:
-            bool: `True` if the triangle has an obtuse angle, `False`
-                otherwise.
-        """
-        return any(
-            angle_ > 90
-            for angle_ in self.angles.values()
-        )
-
-    def is_acute(self) -> bool:
-        """Check whether every angle in the triangle is an acute angle.
-
-        Returns:
-            bool: `True` if the triangle has an acute angle, `False` otherwise.
-        """
-        return all(
-            angle_ < 90
-            for angle_ in self.angles.values()
-        )
-
-    def is_equilateral(self) -> bool:
-        """Check whether the triangle is equilateral.
-
-        Returns:
-            bool: `True` if the triangle is equilateral, `False` otherwise.
-        """
-        return len(set(self.angles.values())) == 1
-
-    def is_isosceles(self) -> bool:
-        """Check whether the triangle is isosceles.
-
-        Returns:
-            bool: `True` if the triangle is isosceles, `False` otherwise.
-        """
-        return len(set(self.angles.values())) == 2
-
-    def is_scalene(self) -> bool:
-        """Check whether the triangle is scalene.
-
-        Returns:
-            bool: `True` if the triangle is scalene, `False` otherwise.
-        """
-        return len(set(self.angles.values())) == 3
-
-    def is_collinear(self) -> bool:
-        """Check whether the triangle is collinear.
-
-        Returns:
-            bool: `True` if the triangle is collinear, `False` otherwise.
-        """
-        x_displacements = {
-            "ab": self.b.x - self.a.x,
-            "bc": self.c.x - self.b.x,
-            "ac": self.c.x - self.a.x
-        }
-
-        y_displacements = {
-            "ab": self.b.y - self.a.y,
-            "bc": self.c.y - self.b.y,
-            "ac": self.c.y - self.a.y
-        }
-
-        if (self.a.x == self.b.x == self.c.x
-                or self.a.y == self.b.y == self.c.y):
-
-            return True
-
-        slopes = []
-
-        if x_displacements["ab"] != 0:
-            slopes.append(y_displacements["ab"] / x_displacements["ab"])
-
-        if x_displacements["bc"] != 0:
-            slopes.append(y_displacements["bc"] / x_displacements["bc"])
-
-        if x_displacements["ac"] != 0:
-            slopes.append(y_displacements["ac"] / x_displacements["ac"])
-
-        if any(slope[0] == slope[1]
-               for slope in combinations(slopes, 2)):
-
-            return True
-
-        return False
-
-    def __repr__(self) -> str:
-        """Return the string representation of the triangle.
-
-        Returns:
-            str: string representation of the triangle.
-        """
-        return f"Triangle({self.a}, {self.b}, {self.c})"
-
-    def __str__(self) -> str:
-        """Return the raw representation of the triangle.
-
-        Returns:
-            str: raw representation of the triangle.
-        """
-        return f"Triangle({self.a}, {self.b}, {self.c})"
-
-    def __contains__(self, value: Coordinate) -> bool:
-        """Check whether a point is inside the triangle.
-
-        Args:
-            point (Coordinate): Point to check.
-
-        Returns:
-            bool: `True` if the point is inside the triangle, `False`
-                otherwise.
-
-        Note:
-            This method excludes points on the edges of the triangle up to a
-            tolerance of 1e-14. This means that if the point is located exacly
-            at the edge of the triangle, it will be considered outside the
-            figure, but if it is located 1e-14 units towards the baricenter of
-            the triangle, it will be considered inside the figure.
-
-        Reference:
-            http://totologic.blogspot.com/2014/01/accurate-point-in-triangle-test.html
-        """
-        a = (
-            (self._b.y - self._c.y) * (value.x - self._c.x)
-            + (self._c.x - self._b.x) * (value.y - self._c.y)
-        ) / (
-            (self._b.y - self._c.y) * (self._a.x - self._c.x)
-            + (self._c.x - self._b.x) * (self._a.y - self._c.y)
-        )
-
-        b = (
-            (self._c.y - self._a.y) * (value.x - self._c.x)
-            + (self._a.x - self._c.x) * (value.y - self._c.y)
-        ) / (
-            (self._b.y - self._c.y) * (self._a.x - self._c.x)
-            + (self._c.x - self._b.x) * (self._a.y - self._c.y)
-        )
-
-        c = 1 - a - b
-
-        return 0 <= a <= 1 and 0 <= b <= 1 and 0 <= c <= 1
+"""Triangle polygon utilities module.
+
+This module contains all utilities related to the triangle polygon, such as
+calculating the area, perimeter, circumcenter and circumradius, etc.
+
+Author:
+    Paulo Sanchez (@erlete)
+"""
+
+from __future__ import annotations
+
+from itertools import combinations
+from math import sqrt
+from typing import Any, Dict
+
+from ..core import operations as op
+from ..core.coordinate import Coordinate
+from .polygon import Polygon
+
+
+class Circumcircle:
+    """Circumcirle calculation utility.
+
+    This class is used to calculate the circumcenter and circumradius of a
+    triangle, given its three vertices as 2D coordinates.
+
+    Attributes:
+        a (Coordinate): first vertex of the triangle.
+        b (Coordinate): second vertex of the triangle.
+        c (Coordinate): third vertex of the triangle.
+        center (Coordinate): center of the circumcircle.
+        radius (float): radius of the circumcircle.
+    """
+
+    def __init__(self, a: Coordinate, b: Coordinate, c: Coordinate) -> None:
+        """Initialize a circumcircle instance.
+
+        Args:
+            a (Coordinate): first vertex of the triangle.
+            b (Coordinate): second vertex of the triangle.
+            c (Coordinate): third vertex of the triangle.
+        """
+        self._a = a
+        self._b = b
+        self.c = c  # Automatically calls `Circumcircle._calculate` method.
+
+    @property
+    def a(self) -> Coordinate:
+        """First vertex of the triangle.
+
+        Returns:
+            Coordinate: first vertex of the triangle.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        return self._a
+
+    @a.setter
+    def a(self, value: Coordinate) -> None:
+        """First vertex of the triangle.
+
+        Args:
+            value (Coordinate): first vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("a must be a Coordinate instance")
+
+        self._a = value
+        self._calculate()
+
+    @property
+    def b(self) -> Coordinate:
+        """Second vertex of the triangle.
+
+        Returns:
+            Coordinate: second vertex of the triangle.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        return self._b
+
+    @b.setter
+    def b(self, value: Coordinate) -> None:
+        """Second vertex of the triangle.
+
+        Args:
+            value (Coordinate): second vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("b must be a Coordinate instance")
+
+        self._b = value
+        self._calculate()
+
+    @property
+    def c(self) -> Coordinate:
+        """Third vertex of the triangle.
+
+        Returns:
+            Coordinate: third vertex of the triangle.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        return self._c
+
+    @c.setter
+    def c(self, value: Coordinate) -> None:
+        """Third vertex of the triangle.
+
+        Args:
+            value (Coordinate): third vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+
+        Note:
+            If the value of the vertex is changed, the circumcenter and
+            circumradius are recalculated.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("c must be a Coordinate instance")
+
+        self._c = value
+        self._calculate()
+
+    @property
+    def center(self) -> Coordinate:
+        """Center of the circumcircle.
+
+        Returns:
+            Coordinate: center of the circumcircle.
+        """
+        return self._center
+
+    @property
+    def radius(self) -> float:
+        """Radius of the circumcircle.
+
+        Returns:
+            float: radius of the circumcircle.
+        """
+        return self._radius
+
+    def _ensure_non_collinear(self) -> None:
+        """Ensure that the triangle is not collinear.
+
+        Raises:
+            ValueError: if the triangle is collinear.
+        """
+        x_displacements = {
+            "ab": self.b.x - self.a.x,
+            "bc": self.c.x - self.b.x,
+            "ac": self.c.x - self.a.x
+        }
+
+        y_displacements = {
+            "ab": self.b.y - self.a.y,
+            "bc": self.c.y - self.b.y,
+            "ac": self.c.y - self.a.y
+        }
+
+        if (self.a.x == self.b.x == self.c.x
+                or self.a.y == self.b.y == self.c.y):
+
+            raise ValueError("The triangle is collinear")
+
+        slopes = []
+
+        if x_displacements["ab"] != 0:
+            slopes.append(y_displacements["ab"] / x_displacements["ab"])
+
+        if x_displacements["bc"] != 0:
+            slopes.append(y_displacements["bc"] / x_displacements["bc"])
+
+        if x_displacements["ac"] != 0:
+            slopes.append(y_displacements["ac"] / x_displacements["ac"])
+
+        if any(slope[0] == slope[1]
+               for slope in combinations(slopes, 2)):
+
+            raise ValueError("The triangle is collinear")
+
+    def _calculate(self) -> None:
+        """Calculate the center and radius of the circumcircle."""
+        self._ensure_non_collinear()
+
+        if any(v[1] - v[0] for v in combinations(
+                (self._a, self._b, self._c), 2)):
+
+            # Vertical alignment prevention:
+
+            if not (self._b - self._a).x:
+                self._a, self._c = self._c, self._a
+
+            if not (self._c - self._a).x:
+                self._a, self._b = self._b, self._a
+
+        # Segment displacement:
+
+        displacement = {
+            "ab": Coordinate(
+                self.b.x - self.a.x,
+                self.b.y - self.a.y
+            ),
+            "ac": Coordinate(
+                self.c.x - self.a.x,
+                self.c.y - self.a.y
+            )
+        }
+
+        # Unitary vectors:
+
+        unitary = {
+            "ab": Coordinate(
+                displacement["ab"].y / sqrt(
+                    displacement["ab"].x ** 2 + displacement["ab"].y ** 2
+                ),
+                -displacement["ab"].x / sqrt(
+                    displacement["ab"].x ** 2 + displacement["ab"].y ** 2
+                )
+            ),
+            "ac": Coordinate(
+                displacement["ac"].y / sqrt(
+                    displacement["ac"].x ** 2 + displacement["ac"].y ** 2
+                ),
+                -displacement["ac"].x / sqrt(
+                    displacement["ac"].x ** 2 + displacement["ac"].y ** 2
+                )
+            )
+        }
+
+        # V-vector for vertical intersection:
+
+        vertical = {
+            "ab": Coordinate(
+                unitary["ab"].x / unitary["ab"].y,
+                1
+            ),
+            "ac": Coordinate(
+                -(unitary["ac"].x / unitary["ac"].y),
+                1
+            )
+        }
+
+        # Midpoint setting:
+
+        midpoint = {
+            "ab": Coordinate(
+                displacement["ab"].x / 2 + self.a.x,
+                displacement["ab"].y / 2 + self.a.y
+            ),
+            "ac": Coordinate(
+                displacement["ac"].x / 2 + self.a.x,
+                displacement["ac"].y / 2 + self.a.y
+            )
+        }
+
+        # Midpoint height equivalence:
+
+        intersection = Coordinate(
+            midpoint["ab"].x + (
+                (midpoint["ac"].y - midpoint["ab"].y) / unitary["ab"].y
+            ) * unitary["ab"].x,
+            midpoint["ac"].y
+        )
+
+        # Circumcenter calculation:
+
+        self._center = Coordinate(
+            intersection.x + (
+                (midpoint["ac"].x - intersection.x)
+                / (vertical["ab"].x + vertical["ac"].x)
+            ) * vertical["ab"].x,
+            intersection.y + (
+                midpoint["ac"].x - intersection.x
+            ) / (
+                vertical["ab"].x + vertical["ac"].x
+            )
+        )
+
+        # Circumradius calculation:
+
+        self._radius = sqrt(
+            (self.a.x - self._center.x) ** 2
+            + (self.a.y - self._center.y) ** 2
+        )
+
+
+class Triangle(Polygon):
+    """Triangle class.
+
+    This class represents a triangle in the 2D plane. It is defined by three
+    vertices, a, b and c (Coordinate objects). The class provides methods to
+    compute the angles of the triangle, the circumcenter and the circumradius.
+    It also provides methods used to determine special properties of the
+    triangle, such as if it is equilateral, isosceles, scalene, right, obtuse
+    or acute.
+
+    Attributes:
+        a (Coordinate): first vertex of the triangle.
+        b (Coordinate): second vertex of the triangle.
+        c (Coordinate): third vertex of the triangle.
+        circumcenter (Coordinate): circumcenter of the triangle.
+        circumradius (float): circumradius of the triangle.
+    """
+
+    TOL_DIGITS = 10
+
+    def __init__(self, a: Coordinate, b: Coordinate, c: Coordinate) -> None:
+        """Initialize a triangle instance.
+
+        Args:
+            a (Coordinate): first vertex of the triangle.
+            b (Coordinate): second vertex of the triangle.
+            c (Coordinate): third vertex of the triangle.
+        """
+        super().__init__(a, b, c)
+        self._properties: Dict[str, Any] = {}
+
+        self.a = a
+        self.b = b
+        self.c = c
+
+    @property
+    def a(self) -> Coordinate:
+        """First vertex of the triangle.
+
+        Returns:
+            Coordinate: first vertex of the triangle.
+        """
+        return self._a
+
+    @a.setter
+    def a(self, value: Coordinate) -> None:
+        """First vertex of the triangle.
+
+        Args:
+            value (Coordinate): first vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("a must be a Coordinate instance")
+
+        self._a = value
+        self._properties.clear()
+
+    @property
+    def b(self) -> Coordinate:
+        """Second vertex of the triangle.
+
+        Returns:
+            Coordinate: second vertex of the triangle.
+        """
+        return self._b
+
+    @b.setter
+    def b(self, value: Coordinate) -> None:
+        """Second vertex of the triangle.
+
+        Args:
+            value (Coordinate): second vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("b must be a Coordinate instance")
+
+        self._b = value
+        self._properties.clear()
+
+    @property
+    def c(self) -> Coordinate:
+        """Third vertex of the triangle.
+
+        Returns:
+            Coordinate: third vertex of the triangle.
+        """
+        return self._c
+
+    @c.setter
+    def c(self, value: Coordinate) -> None:
+        """Third vertex of the triangle.
+
+        Args:
+            value (Coordinate): third vertex of the triangle.
+
+        Raises:
+            TypeError: if the value is not a Coordinate object.
+        """
+        if not isinstance(value, Coordinate):
+            raise TypeError("c must be a Coordinate instance")
+
+        self._c = value
+        self._properties.clear()
+
+    @property
+    def angles(self) -> Dict[str, float]:
+        """Inner angles of the triangle.
+
+        Returns:
+            Dict[str, float]: Angles of the triangle.
+        """
+        if self._properties.get("angles") is None:
+            self._properties["angles"] = {
+                'a': round(op.angle(self.b, self.c, self.a), self.TOL_DIGITS),
+                'b': round(op.angle(self.c, self.a, self.b), self.TOL_DIGITS),
+                'c': round(op.angle(self.a, self.b, self.c), self.TOL_DIGITS)
+            }
+
+        return self._properties["angles"]
+
+    @property
+    def circumcenter(self) -> Coordinate:
+        """Circumcenter of the triangle.
+
+        Returns:
+            Coordinate: Circumcenter of the triangle.
+        """
+        if self._properties.get("circumcircle") is None:
+            self._properties["circumcircle"] = Circumcircle(
+                self.a, self.b, self.c
+            )
+
+        return self._properties["circumcircle"].center
+
+    @property
+    def circumradius(self) -> float:
+        """Circumradius of the triangle.
+
+        Returns:
+            float: Circumradius of the triangle.
+        """
+        if self._properties.get("circumcircle") is None:
+            self._properties["circumcircle"] = Circumcircle(
+                self.a, self.b, self.c
+            )
+
+        return self._properties["circumcircle"].radius
+
+    def is_right(self) -> bool:
+        """Check whether the triangle has a right angle.
+
+        Returns:
+            bool: `True` if the triangle has a right angle, `False` otherwise.
+        """
+        return any(
+            round(angle_, self.TOL_DIGITS) == 90
+            for angle_ in self.angles.values()
+        )
+
+    def is_obtuse(self) -> bool:
+        """Check whether the triangle has an obtuse angle.
+
+        Returns:
+            bool: `True` if the triangle has an obtuse angle, `False`
+                otherwise.
+        """
+        return any(
+            angle_ > 90
+            for angle_ in self.angles.values()
+        )
+
+    def is_acute(self) -> bool:
+        """Check whether every angle in the triangle is an acute angle.
+
+        Returns:
+            bool: `True` if the triangle has an acute angle, `False` otherwise.
+        """
+        return all(
+            angle_ < 90
+            for angle_ in self.angles.values()
+        )
+
+    def is_equilateral(self) -> bool:
+        """Check whether the triangle is equilateral.
+
+        Returns:
+            bool: `True` if the triangle is equilateral, `False` otherwise.
+        """
+        return len(set(self.angles.values())) == 1
+
+    def is_isosceles(self) -> bool:
+        """Check whether the triangle is isosceles.
+
+        Returns:
+            bool: `True` if the triangle is isosceles, `False` otherwise.
+        """
+        return len(set(self.angles.values())) == 2
+
+    def is_scalene(self) -> bool:
+        """Check whether the triangle is scalene.
+
+        Returns:
+            bool: `True` if the triangle is scalene, `False` otherwise.
+        """
+        return len(set(self.angles.values())) == 3
+
+    def is_collinear(self) -> bool:
+        """Check whether the triangle is collinear.
+
+        Returns:
+            bool: `True` if the triangle is collinear, `False` otherwise.
+        """
+        x_displacements = {
+            "ab": self.b.x - self.a.x,
+            "bc": self.c.x - self.b.x,
+            "ac": self.c.x - self.a.x
+        }
+
+        y_displacements = {
+            "ab": self.b.y - self.a.y,
+            "bc": self.c.y - self.b.y,
+            "ac": self.c.y - self.a.y
+        }
+
+        if (self.a.x == self.b.x == self.c.x
+                or self.a.y == self.b.y == self.c.y):
+
+            return True
+
+        slopes = []
+
+        if x_displacements["ab"] != 0:
+            slopes.append(y_displacements["ab"] / x_displacements["ab"])
+
+        if x_displacements["bc"] != 0:
+            slopes.append(y_displacements["bc"] / x_displacements["bc"])
+
+        if x_displacements["ac"] != 0:
+            slopes.append(y_displacements["ac"] / x_displacements["ac"])
+
+        if any(slope[0] == slope[1]
+               for slope in combinations(slopes, 2)):
+
+            return True
+
+        return False
+
+    def __repr__(self) -> str:
+        """Return the string representation of the triangle.
+
+        Returns:
+            str: string representation of the triangle.
+        """
+        return f"Triangle({self.a}, {self.b}, {self.c})"
+
+    def __str__(self) -> str:
+        """Return the raw representation of the triangle.
+
+        Returns:
+            str: raw representation of the triangle.
+        """
+        return f"Triangle({self.a}, {self.b}, {self.c})"
+
+    def __contains__(self, value: Coordinate) -> bool:
+        """Check whether a point is inside the triangle.
+
+        Args:
+            point (Coordinate): Point to check.
+
+        Returns:
+            bool: `True` if the point is inside the triangle, `False`
+                otherwise.
+
+        Note:
+            This method excludes points on the edges of the triangle up to a
+            tolerance of 1e-14. This means that if the point is located exacly
+            at the edge of the triangle, it will be considered outside the
+            figure, but if it is located 1e-14 units towards the baricenter of
+            the triangle, it will be considered inside the figure.
+
+        Reference:
+            http://totologic.blogspot.com/2014/01/accurate-point-in-triangle-test.html
+        """
+        a = (
+            (self._b.y - self._c.y) * (value.x - self._c.x)
+            + (self._c.x - self._b.x) * (value.y - self._c.y)
+        ) / (
+            (self._b.y - self._c.y) * (self._a.x - self._c.x)
+            + (self._c.x - self._b.x) * (self._a.y - self._c.y)
+        )
+
+        b = (
+            (self._c.y - self._a.y) * (value.x - self._c.x)
+            + (self._a.x - self._c.x) * (value.y - self._c.y)
+        ) / (
+            (self._b.y - self._c.y) * (self._a.x - self._c.x)
+            + (self._c.x - self._b.x) * (self._a.y - self._c.y)
+        )
+
+        c = 1 - a - b
+
+        return 0 <= a <= 1 and 0 <= b <= 1 and 0 <= c <= 1
```

### Comparing `bidimensional-1.9.0/src/bidimensional.egg-info/PKG-INFO` & `bidimensional-1.9.1/src/bidimensional.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,756 +1,756 @@
-Metadata-Version: 2.1
-Name: bidimensional
-Version: 1.9.0
-Summary: A collection of 2D utilities for coordinate representation and manipulation.
-Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
-Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Project-URL: Homepage, https://github.com/erlete/bidimensional
-Project-URL: Bug Tracker, https://github.com/erlete/bidimensional/issues
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.13
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Bidimensional
-
-[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
-
-This package contains a collection of useful classes and functions for working with 2D geometry in Python.
-
-## Objectives and contributions
-
-This package has three fundamental bases:
-
-* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
-* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
-* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
-
-Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
-
-## Features
-
-The following features are currently implemented:
-
-* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
-* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
-* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
-* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
-
-## Installation
-
-The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
-
-```bash
-pip install bidimensional
-```
-
-_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
-
-## Usage
-
-Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
-
-## Examples
-
-Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
-
-```python
-import bidimensional.operations as op
-import matplotlib.pyplot as plt
-
-from bidimensional import Coordinate
-from bidimensional.polygons import Triangle
-
-
-outer_triangle = Triangle(
-    Coordinate(0, 0),
-    Coordinate(1, 0),
-    Coordinate(0, 1)
-)
-
-inner_triangle = Triangle(
-    op.midpoint(outer_triangle.a, outer_triangle.b),
-    op.midpoint(outer_triangle.b, outer_triangle.c),
-    op.midpoint(outer_triangle.c, outer_triangle.a)
-)
-
-outer_triangle.plot(color="darkorange", lw=2)
-inner_triangle.plot()
-
-plt.gca().add_patch(plt.Circle(
-    inner_triangle.circumcenter,
-    inner_triangle.circumradius,
-    color="darkblue",
-    fill=False,
-    lw=2
-))
-
-plt.axis("equal")
-plt.grid()
-plt.show()
-```
+Metadata-Version: 2.1
+Name: bidimensional
+Version: 1.9.1
+Summary: A collection of 2D utilities for coordinate representation and manipulation.
+Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
+Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
+License:                     GNU AFFERO GENERAL PUBLIC LICENSE
+                               Version 3, 19 November 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU Affero General Public License is a free, copyleft license for
+        software and other kinds of works, specifically designed to ensure
+        cooperation with the community in the case of network server software.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        our General Public Licenses are intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          Developers that use our General Public Licenses protect your rights
+        with two steps: (1) assert copyright on the software, and (2) offer
+        you this License which gives you legal permission to copy, distribute
+        and/or modify the software.
+        
+          A secondary benefit of defending all users' freedom is that
+        improvements made in alternate versions of the program, if they
+        receive widespread use, become available for other developers to
+        incorporate.  Many developers of free software are heartened and
+        encouraged by the resulting cooperation.  However, in the case of
+        software used on network servers, this result may fail to come about.
+        The GNU General Public License permits making a modified version and
+        letting the public access it on a server without ever releasing its
+        source code to the public.
+        
+          The GNU Affero General Public License is designed specifically to
+        ensure that, in such cases, the modified source code becomes available
+        to the community.  It requires the operator of a network server to
+        provide the source code of the modified version running there to the
+        users of that server.  Therefore, public use of a modified version, on
+        a publicly accessible server, gives the public access to the source
+        code of the modified version.
+        
+          An older license, called the Affero General Public License and
+        published by Affero, was designed to accomplish similar goals.  This is
+        a different license, not a version of the Affero GPL, but Affero has
+        released a new version of the Affero GPL which permits relicensing under
+        this license.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU Affero General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Remote Network Interaction; Use with the GNU General Public License.
+        
+          Notwithstanding any other provision of this License, if you modify the
+        Program, your modified version must prominently offer all users
+        interacting with it remotely through a computer network (if your version
+        supports such interaction) an opportunity to receive the Corresponding
+        Source of your version by providing access to the Corresponding Source
+        from a network server at no charge, through some standard or customary
+        means of facilitating copying of software.  This Corresponding Source
+        shall include the Corresponding Source for any work covered by version 3
+        of the GNU General Public License that is incorporated pursuant to the
+        following paragraph.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the work with which it is combined will remain governed by version
+        3 of the GNU General Public License.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU Affero General Public License from time to time.  Such new versions
+        will be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU Affero General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU Affero General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU Affero General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU Affero General Public License as published
+            by the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU Affero General Public License for more details.
+        
+            You should have received a copy of the GNU Affero General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If your software can interact with users remotely through a computer
+        network, you should also make sure that it provides a way for users to
+        get its source.  For example, if your program is a web application, its
+        interface could display a "Source" link that leads users to an archive
+        of the code.  There are many ways you could offer source, and different
+        solutions will be better for different programs; see section 13 for the
+        specific requirements.
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU AGPL, see
+        <https://www.gnu.org/licenses/>.
+        
+Project-URL: Homepage, https://github.com/erlete/bidimensional
+Project-URL: Bug Tracker, https://github.com/erlete/bidimensional/issues
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.13
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bidimensional
+
+[![PyPI release](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-publish.yml) [![Python Test Execution](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml/badge.svg)](https://github.com/erlete/bidimensional/actions/workflows/python-tests.yml)
+
+This package contains a collection of useful classes and functions for working with 2D geometry in Python.
+
+## Objectives and contributions
+
+This package has three fundamental bases:
+
+* **Simplicity** - The package is designed to be simple and easy to use, with a minimalistic approach to the implementation of its features.
+* **Rich documentation** - The package is fully documented, with a detailed description of its features and their usage.
+* **Performance** - The package is designed to be as fast as possible, mainly using simple algebraic operations instead of complex calculations.
+
+Any contribution is welcome as long as it follows the objectives of the package. For more information, refer to the [contributing guidelines](CONTRIBUTING.md).
+
+## Features
+
+The following features are currently implemented:
+
+* `Coordinate` - A class for representing a 2D coordinate. It can be used to represent a point in the plane, or a vector from the origin. It provides with multiple access methods, as well as a set of useful methods for performing operations with other coordinates.
+* `polygons.Triangle` - A class for representing a triangle in the plane. Contains several methods that can be used to compute its area, perimeter and relevant centers, as well as determining relevant properties of triangles (e.g. if they are equilateral, isosceles, etc.).
+* `functions.Spline` - A class for representing a spline function. It can be used to interpolate a set of points in the plane and to compute the value of the function at any given point in between.
+* `operations` - A module that contains relevant functions for performing operations with coordinates and triangles. It provides with functions for computing the distance between two points, the area of a triangle, the midpoint of a segment, etc.
+
+## Installation
+
+The installation process is performed via PyPI (Python Package Index), so the package can be installed using the `pip` command.
+
+```bash
+pip install bidimensional
+```
+
+_Refer to the [PyPI release](https://pypi.org/project/bidimensional) for more information about how to install the package in your system._
+
+## Usage
+
+Once the package has been installed, its modules can be easily imported into custom programs via the `import` statement.
+
+## Examples
+
+Composition of a small triangle out of the midpoints of the sides of a larger triangle, computation of the circumcircle of the inner triangle and figure plotting.
+
+```python
+import bidimensional.operations as op
+import matplotlib.pyplot as plt
+
+from bidimensional import Coordinate
+from bidimensional.polygons import Triangle
+
+
+outer_triangle = Triangle(
+    Coordinate(0, 0),
+    Coordinate(1, 0),
+    Coordinate(0, 1)
+)
+
+inner_triangle = Triangle(
+    op.midpoint(outer_triangle.a, outer_triangle.b),
+    op.midpoint(outer_triangle.b, outer_triangle.c),
+    op.midpoint(outer_triangle.c, outer_triangle.a)
+)
+
+outer_triangle.plot(color="darkorange", lw=2)
+inner_triangle.plot()
+
+plt.gca().add_patch(plt.Circle(
+    inner_triangle.circumcenter,
+    inner_triangle.circumradius,
+    color="darkblue",
+    fill=False,
+    lw=2
+))
+
+plt.axis("equal")
+plt.grid()
+plt.show()
+```
```

### Comparing `bidimensional-1.9.0/src/bidimensional.egg-info/SOURCES.txt` & `bidimensional-1.9.1/src/bidimensional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

