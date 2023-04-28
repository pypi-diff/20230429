# Comparing `tmp/data_pipeline_api-0.7.8.tar.gz` & `tmp/data_pipeline_api-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_pipeline_api-0.7.8.tar", max compression
+gzip compressed data, was "data_pipeline_api-0.7.9.tar", max compression
```

## Comparing `data_pipeline_api-0.7.8.tar` & `data_pipeline_api-0.7.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-03-29 17:03:22.347493 data_pipeline_api-0.7.8/LICENSE
--rw-r--r--   0        0        0     1826 2022-03-29 17:03:22.347733 data_pipeline_api-0.7.8/README.md
--rw-r--r--   0        0        0      752 2022-10-25 17:38:08.574844 data_pipeline_api-0.7.8/data_pipeline_api/__init__.py
--rw-r--r--   0        0        0     1366 2022-03-29 17:03:22.348146 data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSModelRun.py
--rw-r--r--   0        0        0      959 2022-03-29 17:03:22.348250 data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSconfig.yaml
--rw-r--r--   0        0        0      958 2022-03-29 17:03:22.348338 data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSconfigWindows.yaml
--rw-r--r--   0        0        0        0 2022-03-29 17:03:22.348377 data_pipeline_api-0.7.8/data_pipeline_api/ext/__init__.py
--rw-r--r--   0        0        0      100 2022-03-29 17:03:22.348489 data_pipeline_api-0.7.8/data_pipeline_api/ext/static_params_SEIRS.csv
--rw-r--r--   0        0        0    16122 2022-10-25 17:38:16.159783 data_pipeline_api-0.7.8/data_pipeline_api/fdp_utils.py
--rw-r--r--   0        0        0     6628 2022-10-25 17:38:08.575161 data_pipeline_api-0.7.8/data_pipeline_api/link.py
--rw-r--r--   0        0        0    20844 2022-10-25 17:47:25.878525 data_pipeline_api-0.7.8/data_pipeline_api/pipeline.py
--rw-r--r--   0        0        0     7799 2022-10-25 17:38:08.575300 data_pipeline_api-0.7.8/data_pipeline_api/raise_issue.py
--rw-r--r--   0        0        0     1951 2022-10-27 20:25:07.485442 data_pipeline_api-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     2690 2022-10-27 20:25:25.451479 data_pipeline_api-0.7.8/setup.py
--rw-r--r--   0        0        0     2781 2022-10-27 20:25:25.451683 data_pipeline_api-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      779 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/ext/__init__.py
+-rw-r--r--   0        0        0      990 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSconfig.yaml
+-rw-r--r--   0        0        0      989 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSconfigWindows.yaml
+-rw-r--r--   0        0        0     1409 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSModelRun.py
+-rw-r--r--   0        0        0      108 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/ext/static_params_SEIRS.csv
+-rw-r--r--   0        0        0    16638 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/fdp_utils.py
+-rw-r--r--   0        0        0     6844 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/link.py
+-rw-r--r--   0        0        0    21457 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/pipeline.py
+-rw-r--r--   0        0        0     8054 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/data_pipeline_api/raise_issue.py
+-rw-r--r--   0        0        0    35823 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/LICENSE
+-rw-r--r--   0        0        0     2041 2023-04-27 23:37:27.850922 data_pipeline_api-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1875 2023-04-27 12:30:19.227240 data_pipeline_api-0.7.9/README.md
+-rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 data_pipeline_api-0.7.9/PKG-INFO
```

### Comparing `data_pipeline_api-0.7.8/LICENSE` & `data_pipeline_api-0.7.9/LICENSE`

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

### Comparing `data_pipeline_api-0.7.8/README.md` & `data_pipeline_api-0.7.9/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# pyDataPipeline
-
-[![pyDataPipeline](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml/badge.svg?branch=dev)](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml)
-[![codecov](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline/branch/dev/graph/badge.svg?token=Eax5AmrDxx)](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5562602.svg)](https://doi.org/10.5281/zenodo.5562602)
-[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5461/badge)](https://bestpractices.coreinfrastructure.org/projects/5461)
-
-Welcome to pyDataPipeline a Python api to interact with the Fair Data Pipeline.
-
-Full documention of the pyDataPipeline is avaialable at [https://www.fairdatapipeline.org/pyDataPipeline/](https://www.fairdatapipeline.org/pyDataPipeline/)
-
-## Installation
-pyDataPipeline can be installed from PyPi:
-```
-pip3 install data-pipeline-api
-```
-
-Or from the Repository:
-```
-git clone https://github.com/FAIRDataPipeline/pythonFDP.git
-
-git checkout dev
-
-pip3 install -e .
-```
-**NB. PyDataPipeline requires Python3.**
-
-## Example submission_script
-
-Assume FDP_CONFIG_DIR, storage_locations and objects have been set by CLI tool
-
-```
-import os
-import fairdatapipeline as pipeline
-
-token = os.environ['FDP_LOCAL_TOKEN']
-config_dir = os.environ['FDP_CONFIG_DIR']
-config_path = os.path.join(config_dir, 'config.yaml')
-script_path = os.path.join(config_dir, 'script.sh')
-
-handle = pipeline.initialise(token, config_path, script_path)
-
-pipeline.finalise(token, handle)
-
-```
-
-## SEIRS Model Example
-
-The SEIRS Model Example is available at: [https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html](https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html)
+# pyDataPipeline
+
+[![pyDataPipeline](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml/badge.svg?branch=dev)](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml)
+[![codecov](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline/branch/dev/graph/badge.svg?token=Eax5AmrDxx)](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5562602.svg)](https://doi.org/10.5281/zenodo.5562602)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5461/badge)](https://bestpractices.coreinfrastructure.org/projects/5461)
+
+Welcome to pyDataPipeline a Python api to interact with the Fair Data Pipeline.
+
+Full documention of the pyDataPipeline is avaialable at [https://www.fairdatapipeline.org/pyDataPipeline/](https://www.fairdatapipeline.org/pyDataPipeline/)
+
+## Installation
+pyDataPipeline can be installed from PyPi:
+```
+pip3 install data-pipeline-api
+```
+
+Or from the Repository:
+```
+git clone https://github.com/FAIRDataPipeline/pythonFDP.git
+
+git checkout dev
+
+pip3 install -e .
+```
+**NB. PyDataPipeline requires Python3.**
+
+## Example submission_script
+
+Assume FDP_CONFIG_DIR, storage_locations and objects have been set by CLI tool
+
+```
+import os
+import fairdatapipeline as pipeline
+
+token = os.environ['FDP_LOCAL_TOKEN']
+config_dir = os.environ['FDP_CONFIG_DIR']
+config_path = os.path.join(config_dir, 'config.yaml')
+script_path = os.path.join(config_dir, 'script.sh')
+
+handle = pipeline.initialise(token, config_path, script_path)
+
+pipeline.finalise(token, handle)
+
+```
+
+## SEIRS Model Example
+
+The SEIRS Model Example is available at: [https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html](https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html)
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/__init__.py` & `data_pipeline_api-0.7.9/data_pipeline_api/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-__all__ = [
-    "initialise",
-    "link_read",
-    "link_write",
-    "finalise",
-    "raise_issue_by_data_product",
-    "raise_issue_by_index",
-    "raise_issue_with_config",
-    "raise_issue_by_type",
-    "raise_issue_by_existing_data_product",
-    "raise_issue_with_submission_script",
-    "raise_issue_with_github_repo",
-    "get_handle_index_from_path",
-]
-
-from .fdp_utils import get_handle_index_from_path
-from .link import link_read, link_write
-from .pipeline import finalise, initialise
-from .raise_issue import (
-    raise_issue_by_data_product,
-    raise_issue_by_existing_data_product,
-    raise_issue_by_index,
-    raise_issue_by_type,
-    raise_issue_with_config,
-    raise_issue_with_github_repo,
-    raise_issue_with_submission_script,
-)
+__all__ = [
+    "initialise",
+    "link_read",
+    "link_write",
+    "finalise",
+    "raise_issue_by_data_product",
+    "raise_issue_by_index",
+    "raise_issue_with_config",
+    "raise_issue_by_type",
+    "raise_issue_by_existing_data_product",
+    "raise_issue_with_submission_script",
+    "raise_issue_with_github_repo",
+    "get_handle_index_from_path",
+]
+
+from .fdp_utils import get_handle_index_from_path
+from .link import link_read, link_write
+from .pipeline import finalise, initialise
+from .raise_issue import (
+    raise_issue_by_data_product,
+    raise_issue_by_existing_data_product,
+    raise_issue_by_index,
+    raise_issue_by_type,
+    raise_issue_with_config,
+    raise_issue_with_github_repo,
+    raise_issue_with_submission_script,
+)
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSModelRun.py` & `data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSModelRun.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import os
-import platform
-import sys
-
-sys.path.append(str(os.getcwd()))
-import data_pipeline_api as pipeline  # noqa: E402
-import simpleModel as simpleModel  # noqa: E402
-
-token = str(os.environ.get("FDP_LOCAL_TOKEN"))
-script = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "script.sh")
-if platform.system() == "Windows":
-    script = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "script.bat")
-config = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "config.yaml")
-handle = pipeline.initialise(token, config, script)
-
-initial_parameters = pipeline.link_read(handle, "SEIRS_model/parameters")
-model_output = pipeline.link_write(
-    handle, "SEIRS_model/results/model_output/python"
-)
-model_plot = pipeline.link_write(handle, "SEIRS_model/results/figure/python")
-
-# Model Code
-states = {"s": 0.999, "e": 0.001, "i": 0, "r": 0}
-
-init_params = simpleModel.readInitialParameters(initial_parameters)
-
-alpha = init_params["alpha"]
-beta = init_params["beta"]
-inv_gamma = init_params["inv_gamma"]
-inv_omega = init_params["inv_omega"]
-inv_mu = init_params["inv_mu"]
-inv_sigma = init_params["inv_sigma"]
-R0 = init_params["R0"]
-
-sm = simpleModel.SEIRS_Model(
-    states, 1000, 5, alpha, beta, inv_gamma, inv_omega, inv_mu, inv_sigma
-)
-
-simpleModel.SEIRS_Plot(sm, model_plot)
-
-simpleModel.write_model_to_csv(sm, model_output)
-
-pipeline.finalise(token, handle)
+import os
+import platform
+import sys
+
+sys.path.append(str(os.getcwd()))
+import data_pipeline_api as pipeline  # noqa: E402
+import simpleModel as simpleModel  # noqa: E402
+
+token = str(os.environ.get("FDP_LOCAL_TOKEN"))
+script = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "script.sh")
+if platform.system() == "Windows":
+    script = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "script.bat")
+config = os.path.join(str(os.environ.get("FDP_CONFIG_DIR")), "config.yaml")
+handle = pipeline.initialise(token, config, script)
+
+initial_parameters = pipeline.link_read(handle, "SEIRS_model/parameters")
+model_output = pipeline.link_write(
+    handle, "SEIRS_model/results/model_output/python"
+)
+model_plot = pipeline.link_write(handle, "SEIRS_model/results/figure/python")
+
+# Model Code
+states = {"s": 0.999, "e": 0.001, "i": 0, "r": 0}
+
+init_params = simpleModel.readInitialParameters(initial_parameters)
+
+alpha = init_params["alpha"]
+beta = init_params["beta"]
+inv_gamma = init_params["inv_gamma"]
+inv_omega = init_params["inv_omega"]
+inv_mu = init_params["inv_mu"]
+inv_sigma = init_params["inv_sigma"]
+R0 = init_params["R0"]
+
+sm = simpleModel.SEIRS_Model(
+    states, 1000, 5, alpha, beta, inv_gamma, inv_omega, inv_mu, inv_sigma
+)
+
+simpleModel.SEIRS_Plot(sm, model_plot)
+
+simpleModel.write_model_to_csv(sm, model_output)
+
+pipeline.finalise(token, handle)
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSconfig.yaml` & `data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSconfigWindows.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-run_metadata:
-  default_input_namespace: rfield
-  description: SEIRS Model python
-  script: python3 data_pipeline_api/ext/SEIRSModelRun.py
-  remote_repo: https://github.com/FAIRDataPipeline/pyDataPipeline.git
-
-register:
-- namespace: PSU
-  full_name: Pennsylvania State University
-  website: https://ror.org/04p491231
-
-- external_object: SEIRS_model/parameters
-  namespace_name: PSU
-  root: https://raw.githubusercontent.com/
-  path: FAIRDataPipeline/pyDataPipeline/dev/data_pipeline_api/ext/static_params_SEIRS.csv
-  title: Static parameters of the model
-  description: Static parameters of the model
-  identifier: https://doi.org/10.1038/s41592-020-0856-2
-  file_type: csv
-  release_date: 2021-09-20T12:00
-  version: "1.0.0"
-  primary: True
-
-write:
-- data_product: SEIRS_model/results/model_output/python
-  description: SEIRS model results
-  file_type: csv
-
-- data_product: SEIRS_model/results/figure/python
-  description: SEIRS output plot
-  file_type: png
+run_metadata:
+  default_input_namespace: rfield
+  description: SEIRS Model python
+  script: python data_pipeline_api/ext/SEIRSModelRun.py
+  remote_repo: https://github.com/FAIRDataPipeline/pyDataPipeline.git
+
+register:
+- namespace: PSU
+  full_name: Pennsylvania State University
+  website: https://ror.org/04p491231
+
+- external_object: SEIRS_model/parameters
+  namespace_name: PSU
+  root: https://raw.githubusercontent.com/
+  path: FAIRDataPipeline/pyDataPipeline/dev/data_pipeline_api/ext/static_params_SEIRS.csv
+  title: Static parameters of the model
+  description: Static parameters of the model
+  identifier: https://doi.org/10.1038/s41592-020-0856-2
+  file_type: csv
+  release_date: 2021-09-20T12:00
+  version: "1.0.0"
+  primary: True
+
+write:
+- data_product: SEIRS_model/results/model_output/python
+  description: SEIRS model results
+  file_type: csv
+
+- data_product: SEIRS_model/results/figure/python
+  description: SEIRS output plot
+  file_type: png
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/ext/SEIRSconfigWindows.yaml` & `data_pipeline_api-0.7.9/data_pipeline_api/ext/SEIRSconfig.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-run_metadata:
-  default_input_namespace: rfield
-  description: SEIRS Model python
-  script: python data_pipeline_api/ext/SEIRSModelRun.py
-  remote_repo: https://github.com/FAIRDataPipeline/pyDataPipeline.git
-
-register:
-- namespace: PSU
-  full_name: Pennsylvania State University
-  website: https://ror.org/04p491231
-
-- external_object: SEIRS_model/parameters
-  namespace_name: PSU
-  root: https://raw.githubusercontent.com/
-  path: FAIRDataPipeline/pyDataPipeline/dev/data_pipeline_api/ext/static_params_SEIRS.csv
-  title: Static parameters of the model
-  description: Static parameters of the model
-  identifier: https://doi.org/10.1038/s41592-020-0856-2
-  file_type: csv
-  release_date: 2021-09-20T12:00
-  version: "1.0.0"
-  primary: True
-
-write:
-- data_product: SEIRS_model/results/model_output/python
-  description: SEIRS model results
-  file_type: csv
-
-- data_product: SEIRS_model/results/figure/python
-  description: SEIRS output plot
-  file_type: png
+run_metadata:
+  default_input_namespace: rfield
+  description: SEIRS Model python
+  script: python3 data_pipeline_api/ext/SEIRSModelRun.py
+  remote_repo: https://github.com/FAIRDataPipeline/pyDataPipeline.git
+
+register:
+- namespace: PSU
+  full_name: Pennsylvania State University
+  website: https://ror.org/04p491231
+
+- external_object: SEIRS_model/parameters
+  namespace_name: PSU
+  root: https://raw.githubusercontent.com/
+  path: FAIRDataPipeline/pyDataPipeline/dev/data_pipeline_api/ext/static_params_SEIRS.csv
+  title: Static parameters of the model
+  description: Static parameters of the model
+  identifier: https://doi.org/10.1038/s41592-020-0856-2
+  file_type: csv
+  release_date: 2021-09-20T12:00
+  version: "1.0.0"
+  primary: True
+
+write:
+- data_product: SEIRS_model/results/model_output/python
+  description: SEIRS model results
+  file_type: csv
+
+- data_product: SEIRS_model/results/figure/python
+  description: SEIRS output plot
+  file_type: png
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/fdp_utils.py` & `data_pipeline_api-0.7.9/data_pipeline_api/fdp_utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,516 +1,516 @@
-import hashlib
-import json
-import logging
-import os
-import random
-import uuid
-from datetime import datetime
-from typing import Any, Optional
-
-# from typing import BinaryIO, Union
-from urllib.parse import urlsplit
-
-import requests
-import yaml
-
-
-def get_first_entry(entries: list) -> dict:
-    """
-    get_first_entry helper function for get_entry that return first element
-
-    exception handling is done in the main code
-
-    Parameters
-    ----------
-    entries : list
-        [response list from api]
-
-    Returns
-    -------
-    dict
-        [dictionary output from api]
-    """
-    return entries[0]
-
-
-def get_entry(
-    url: str,
-    endpoint: str,
-    query: dict,
-    token: str = None,
-    api_version: str = "1.0.0",
-) -> list:
-    """
-    Internal function to retreive and item from the registry using a query
-    Args:
-        |   url: str of the registry url
-        |   endpoint: endpoint (table)
-        |   query: dict forming a query
-        |   token: (optional) str of the registry token
-    Returns:
-        |   dict: responce from registry
-    """
-    headers = get_headers(token=token, api_version=api_version)
-
-    # Remove api address from query
-    for key in query:
-        if isinstance(query[key], str):
-            if url in query[key]:
-                query[key] = extract_id(query[key])
-        elif isinstance(query[key], dict):
-            for _key in query[key]:
-                if url in query[key][_key]:
-                    query[key][_key] = extract_id(query[key][_key])
-        elif isinstance(query[key], list):
-            for i in range(len(query[key])):
-                if url in query[key][i]:
-                    query[key][i] = extract_id(query[key][i])
-
-    if url[-1] != "/":
-        url += "/"
-    url += endpoint + "/?"
-    _query = [f"{k}={v}" for k, v in query.items()]
-    url += "&".join(_query)
-    response = requests.get(url, headers=headers)
-    if response.status_code != 200:
-        raise ValueError(
-            "Server responded with: "
-            + str(response.status_code)
-            + " Query = "
-            + url
-        )
-    return response.json()["results"]
-
-
-def get_entity(
-    url: str,
-    endpoint: str,
-    id: int,
-    token: str = None,
-    api_version: str = "1.0.0",
-) -> dict:
-    """
-    Internal function to get an item from the registry using it's id
-    Args:
-        |   url: str of the registry url
-        |   enpoint: endpoint (table)
-        |   id: id of the item
-        |   token: (optional) str of the registry token
-    Returns:
-        |   dict: responce from registry
-    """
-    headers = get_headers(token=token, api_version=api_version)
-
-    if url[-1] != "/":
-        url += "/"
-    url += endpoint + "/" + str(id)
-    response = requests.get(url, headers=headers)
-    if response.status_code != 200:
-        raise ValueError(
-            "Server responded with: "
-            + str(response.status_code)
-            + " Query = "
-            + url
-        )
-    return response.json()
-
-
-def extract_id(url: str) -> str:
-    """
-    Internal function to return the id from an api url
-    Args:
-        |   url: str of the api url
-    Returns:
-        |   str: id derrived from the url
-    """
-
-    split_url_path = urlsplit(url).path.split("/")
-    if not split_url_path:
-        raise IndexError(f"Unable to extract ID from registry URL: {url}")
-    return [s for s in split_url_path if s != ""][-1]
-
-
-def post_entry(
-    url: str, endpoint: str, data: dict, token: str, api_version: str = "1.0.0"
-) -> dict:
-    """
-    Internal function to post and entry on the registry
-    Args:
-        |   url: str of the registry url
-        |   enpoint: str of the endpoint (table)
-        |   data: a dictionary containing the data to be posted
-        |   token: str of the registry token
-    Returns:
-        |   dict: responce from registry
-    """
-    headers = get_headers(
-        request_type="post", token=token, api_version=api_version
-    )
-
-    if url[-1] != "/":
-        url += "/"
-    _url = url + endpoint + "/"
-    _data = json.dumps(data)
-
-    response = requests.post(_url, _data, headers=headers)
-
-    if response.status_code == 409:
-        logging.info("Entry Exists: Attempting to return Existing Entry")
-        existing_entry = get_entry(url, endpoint, data)
-        if not existing_entry:
-            raise ValueError("Could not return existing Entry")
-        return existing_entry[0]
-
-    if response.status_code != 201:
-        raise ValueError("Server responded with: " + str(response.status_code))
-
-    return response.json()
-
-
-def patch_entry(
-    url: str, data: dict, token: str, api_version: str = "1.0.0"
-) -> dict:
-    """
-    Internal function to patch and entry on the registry
-    Args:
-        |   url: str of the url of what to be patched
-        |   data: a dictionary containing the data to be patched
-        |   token: str of the registry token
-    Returns:
-        |   dict: responce from registry
-    """
-    headers = get_headers(
-        request_type="post", token=token, api_version=api_version
-    )
-
-    data_json = json.dumps(data)
-
-    response = requests.patch(url, data_json, headers=headers)
-    if response.status_code != 200:
-        raise ValueError("Server responded with: " + str(response.status_code))
-
-    return response.json()
-
-
-def get_headers(
-    request_type: str = "get", token: str = None, api_version: str = "1.0.0"
-) -> dict:
-    """
-    Internal function to return headers to be added to a request
-    Args:
-        |   request_type: (optional) type of request e.g. 'post' or 'get' defaults to 'get'
-        |   token: (optional) token, if a token is supplied this will be added to the headers
-        |   api_version: (optional) the version of the data registy to interact with, defaults to '1.0.0'
-    Returns:
-        |   dict: a dictionary of appropriate headers to be added to a request
-    """
-    headers = {"Accept": "application/json; version=" + api_version}
-    if token:
-        headers["Authorization"] = "token " + token
-    if request_type == "post":
-        headers["Content-Type"] = "application/json"
-    return headers
-
-
-def post_storage_root(
-    url: str, data: dict, token: str, api_version: str = "1.0.0"
-) -> dict:
-    """
-    Internal function to post a storage root to the registry
-    the function first adds file:// if the root is local
-    Args:
-        |   url: str the url for the storage root e.g. https://github.com/
-    Returns:
-        |   dict: repsonse from the local registy
-    """
-    if "local" in data and data["local"]:
-        data["root"] = "file://" + data["root"]
-        if data["root"][-1] != os.sep:
-            data["root"] = data["root"] + os.sep
-    elif data["root"][-1] != "/":
-        data["root"] = data["root"] + "/"
-    return post_entry(url, "storage_root", data, token, api_version)
-
-def post_file_type(
-    url: str, data: dict, token: str, api_version: str = "1.0.0"
-) -> dict:
-    """
-    Internal wrapper function to return check if a file_type already exists and return it.
-    """
-    if not "extension" in data and data["extension"]:
-        raise ValueError("error file_type name not specified")
-    file_type_exists = get_entry(url= url, 
-        endpoint= "file_type", 
-        query= {"extension": data["extension"]}, 
-        api_version= api_version)
-    if file_type_exists : return file_type_exists[0]
-    return post_entry(url= url,
-        endpoint= "file_type",
-        data= data,
-        token= token,
-        api_version= api_version)
-
-def remove_local_from_root(root: str) -> str:
-    """
-    Internal function to remove prepending file:// from a given root
-    Args:
-        |   root: the root
-    Returns:
-        |   str: the root without file://
-    """
-    if "file://" in root:
-        root = root.replace("file://", "")
-
-    return root
-
-
-def random_hash() -> str:
-    """
-    Internal function to generate a random unique hash
-
-    Returns:
-        |   str: 40 character randomly generated hash.
-    """
-    seed = datetime.now().timestamp() * random.uniform(1, 1000000)
-    seed_encoded = str(seed).encode("utf-8")
-    hashed = hashlib.sha1(seed_encoded)
-
-    return hashed.hexdigest()
-
-
-def get_file_hash(
-    path: str,
-) -> str:
-    """
-    Internal function to return a files sha1 hash
-    Args:
-        |   path: str file path
-    Returns:
-        |   str: sha1 hash
-    """
-    with open(path, "rb") as data:
-        _data = data.read()
-    # data = data.encode('utf-8')
-    hashed = hashlib.sha1(_data)
-
-    return hashed.hexdigest()
-
-
-def read_token(token_path: str) -> str:
-    """
-    Internal function read a token from a given file
-    Args:
-        |   token_path: path to token
-    Returns:
-        |   str: token
-    """
-    with open(token_path) as token:
-        _token = token.readline().strip()
-    return _token
-
-
-def get_token(token_path: str) -> str:
-    """
-    Internal function alias for read_token()
-    Args:
-        |   token_path: path to token
-    Returns:
-        |   str: token
-    """
-    return read_token(token_path)
-
-
-def is_file(filename: str) -> bool:
-    """
-    Internal function to check whether a file exists
-    Args:
-        |   filename: file to check
-    Returns:
-        |   boolean: whether the file exists
-    """
-    return os.path.isfile(filename)
-
-
-def is_yaml(filename: str) -> bool:
-    """
-    Internal function to check whether a file can be opened as a YAML file
-    ! warning returns True if the file can be coerced into yaml format
-    Args:
-        |   filename: path to the yaml file
-    Returns:
-        |   boolean: can the file be coerced into a yaml format?
-    """
-    try:
-        with open(filename, "r") as data:
-            yaml.safe_load(data)
-    except Exception as err:
-        print(f"{type(err).__name__} was raised: {err}")
-        return False
-    return True
-
-
-def is_valid_yaml(filename: str) -> bool:
-    """
-    Internal function validate whether a file exists and can be coerced into a yaml format
-    Args:
-        |   filename: path to the yaml file
-    Returns:
-        |   boolean: does the file exist and can it be coerced into a yaml format
-    """
-    return is_file(filename) & is_yaml(filename)
-
-
-def generate_uuid() -> str:
-    """
-    Internal function similar to random hash
-    Returns:
-        |   str: a random unique identifier
-    """
-    return datetime.now().strftime("%Y%m-%d%H-%M%S-") + str(uuid.uuid4())
-
-
-def get_handle_index_from_path(handle: dict, path: str) -> Optional[Any]:
-    """
-    Get an input or output handle index from a path
-    usually generated by link_read or link_write
-
-    Args:
-        |   handle: the handle containing the index
-        |   path: path as generated by link_read or link_write
-    """
-    tmp = None
-    if "output" in handle:
-        for output in handle["output"]:
-            if handle["output"][output]["path"] == path:
-                tmp = output
-    if "input" in handle:
-        for input in handle["input"]:
-            if handle["input"][input]["path"] == path:
-                tmp = input
-    return tmp
-
-
-# flake8: noqa C901
-def register_issues(token: str, handle: dict) -> dict:  # sourcery no-metrics
-    """
-    Internal function, should only be called from finalise.
-    """
-
-    api_url = handle["yaml"]["run_metadata"]["local_data_registry_url"]
-    issues = handle["issues"]
-    groups = {handle["issues"][i]["group"] for i in handle["issues"]}
-    api_version = handle["yaml"]["run_metadata"]["api_version"]
-
-    for group in groups:
-        component_list = []
-        issue = None
-        severity = None
-        for i in issues:
-            if issues[i]["group"] == group:
-                type = issues[i]["type"]
-                issue = issues[i]["issue"]
-                severity = issues[i]["severity"]
-                index = issues[i]["index"]
-                data_product = issues[i]["use_data_product"]
-                component = issues[i]["use_component"]
-                version = issues[i]["version"]
-                namespace = issues[i]["use_namespace"]
-
-                component_url = None
-                object_id = None
-                if type == "config":
-                    object_id = handle["model_config"]
-                elif type == "github_repo":
-                    object_id = handle["code_repo"]
-
-                elif type == "submission_script":
-                    object_id = handle["submission_script"]
-                if object_id:
-                    component_url = get_entry(
-                        url=api_url,
-                        endpoint="object_component",
-                        query={
-                            "object": extract_id(object_id),
-                            "whole_object": True,
-                        },
-                        api_version=api_version,
-                    )[0]["url"]
-
-                if index:
-                    if "output" in handle:
-                        for ii in handle["output"]:
-                            if handle["output"][ii] == index:
-                                if (
-                                    "component_url"
-                                    in handle["output"][ii].keys()
-                                ):
-                                    component_url = handle["output"][ii][
-                                        "component_url"
-                                    ]
-                                else:
-                                    logging.warning("No Component Found")
-                    if "input" in handle:
-                        for ii in handle["input"]:
-                            if handle["input"][ii] == index:
-                                if (
-                                    "component_url"
-                                    in handle["input"][ii].keys()
-                                ):
-                                    component_url = handle["input"][ii][
-                                        "component_url"
-                                    ]
-                                else:
-                                    logging.warning("No Component Found")
-
-                if data_product:
-                    current_namespace = get_entry(
-                        url=api_url,
-                        endpoint="namespace",
-                        query={"name": namespace},
-                        api_version=api_version,
-                    )[0]["url"]
-
-                    object = get_entry(
-                        url=api_url,
-                        endpoint="data_product",
-                        query={
-                            "name": data_product,
-                            "version": version,
-                            "namespace": extract_id(current_namespace),
-                        },
-                        api_version=api_version,
-                    )[0]["object"]
-                    object_id = extract_id(object)
-                    if component:
-                        component_url = get_entry(
-                            url=api_url,
-                            endpoint="object_component",
-                            query={"name": component, "object": object_id},
-                            api_version=api_version,
-                        )
-                    else:
-                        component_obj = get_entry(
-                            url=api_url,
-                            endpoint="object_component",
-                            query={"object": object_id, "whole_object": True},
-                            api_version=api_version,
-                        )
-                        component_url = component_obj[0]["url"]
-
-                if component_url:
-                    component_list.append(component_url)
-
-        # Register the issue:
-        logging.info("Registering issue: {}".format(group))
-        current_issue = post_entry(
-            url=api_url,
-            endpoint="issue",
-            data={
-                "severity": severity,
-                "description": issue,
-                "component_issues": component_list,
-            },
-            token=token,
-            api_version=api_version,
-        )
-    return current_issue
+import hashlib
+import json
+import logging
+import os
+import random
+import uuid
+from datetime import datetime
+from typing import Any, Optional
+
+# from typing import BinaryIO, Union
+from urllib.parse import urlsplit
+
+import requests
+import yaml
+
+
+def get_first_entry(entries: list) -> dict:
+    """
+    get_first_entry helper function for get_entry that return first element
+
+    exception handling is done in the main code
+
+    Parameters
+    ----------
+    entries : list
+        [response list from api]
+
+    Returns
+    -------
+    dict
+        [dictionary output from api]
+    """
+    return entries[0]
+
+
+def get_entry(
+    url: str,
+    endpoint: str,
+    query: dict,
+    token: str = None,
+    api_version: str = "1.0.0",
+) -> list:
+    """
+    Internal function to retreive and item from the registry using a query
+    Args:
+        |   url: str of the registry url
+        |   endpoint: endpoint (table)
+        |   query: dict forming a query
+        |   token: (optional) str of the registry token
+    Returns:
+        |   dict: responce from registry
+    """
+    headers = get_headers(token=token, api_version=api_version)
+
+    # Remove api address from query
+    for key in query:
+        if isinstance(query[key], str):
+            if url in query[key]:
+                query[key] = extract_id(query[key])
+        elif isinstance(query[key], dict):
+            for _key in query[key]:
+                if url in query[key][_key]:
+                    query[key][_key] = extract_id(query[key][_key])
+        elif isinstance(query[key], list):
+            for i in range(len(query[key])):
+                if url in query[key][i]:
+                    query[key][i] = extract_id(query[key][i])
+
+    if url[-1] != "/":
+        url += "/"
+    url += endpoint + "/?"
+    _query = [f"{k}={v}" for k, v in query.items()]
+    url += "&".join(_query)
+    response = requests.get(url, headers=headers)
+    if response.status_code != 200:
+        raise ValueError(
+            "Server responded with: "
+            + str(response.status_code)
+            + " Query = "
+            + url
+        )
+    return response.json()["results"]
+
+
+def get_entity(
+    url: str,
+    endpoint: str,
+    id: int,
+    token: str = None,
+    api_version: str = "1.0.0",
+) -> dict:
+    """
+    Internal function to get an item from the registry using it's id
+    Args:
+        |   url: str of the registry url
+        |   enpoint: endpoint (table)
+        |   id: id of the item
+        |   token: (optional) str of the registry token
+    Returns:
+        |   dict: responce from registry
+    """
+    headers = get_headers(token=token, api_version=api_version)
+
+    if url[-1] != "/":
+        url += "/"
+    url += endpoint + "/" + str(id)
+    response = requests.get(url, headers=headers)
+    if response.status_code != 200:
+        raise ValueError(
+            "Server responded with: "
+            + str(response.status_code)
+            + " Query = "
+            + url
+        )
+    return response.json()
+
+
+def extract_id(url: str) -> str:
+    """
+    Internal function to return the id from an api url
+    Args:
+        |   url: str of the api url
+    Returns:
+        |   str: id derrived from the url
+    """
+
+    split_url_path = urlsplit(url).path.split("/")
+    if not split_url_path:
+        raise IndexError(f"Unable to extract ID from registry URL: {url}")
+    return [s for s in split_url_path if s != ""][-1]
+
+
+def post_entry(
+    url: str, endpoint: str, data: dict, token: str, api_version: str = "1.0.0"
+) -> dict:
+    """
+    Internal function to post and entry on the registry
+    Args:
+        |   url: str of the registry url
+        |   enpoint: str of the endpoint (table)
+        |   data: a dictionary containing the data to be posted
+        |   token: str of the registry token
+    Returns:
+        |   dict: responce from registry
+    """
+    headers = get_headers(
+        request_type="post", token=token, api_version=api_version
+    )
+
+    if url[-1] != "/":
+        url += "/"
+    _url = url + endpoint + "/"
+    _data = json.dumps(data)
+
+    response = requests.post(_url, _data, headers=headers)
+
+    if response.status_code == 409:
+        logging.info("Entry Exists: Attempting to return Existing Entry")
+        existing_entry = get_entry(url, endpoint, data)
+        if not existing_entry:
+            raise ValueError("Could not return existing Entry")
+        return existing_entry[0]
+
+    if response.status_code != 201:
+        raise ValueError("Server responded with: " + str(response.status_code))
+
+    return response.json()
+
+
+def patch_entry(
+    url: str, data: dict, token: str, api_version: str = "1.0.0"
+) -> dict:
+    """
+    Internal function to patch and entry on the registry
+    Args:
+        |   url: str of the url of what to be patched
+        |   data: a dictionary containing the data to be patched
+        |   token: str of the registry token
+    Returns:
+        |   dict: responce from registry
+    """
+    headers = get_headers(
+        request_type="post", token=token, api_version=api_version
+    )
+
+    data_json = json.dumps(data)
+
+    response = requests.patch(url, data_json, headers=headers)
+    if response.status_code != 200:
+        raise ValueError("Server responded with: " + str(response.status_code))
+
+    return response.json()
+
+
+def get_headers(
+    request_type: str = "get", token: str = None, api_version: str = "1.0.0"
+) -> dict:
+    """
+    Internal function to return headers to be added to a request
+    Args:
+        |   request_type: (optional) type of request e.g. 'post' or 'get' defaults to 'get'
+        |   token: (optional) token, if a token is supplied this will be added to the headers
+        |   api_version: (optional) the version of the data registy to interact with, defaults to '1.0.0'
+    Returns:
+        |   dict: a dictionary of appropriate headers to be added to a request
+    """
+    headers = {"Accept": "application/json; version=" + api_version}
+    if token:
+        headers["Authorization"] = "token " + token
+    if request_type == "post":
+        headers["Content-Type"] = "application/json"
+    return headers
+
+
+def post_storage_root(
+    url: str, data: dict, token: str, api_version: str = "1.0.0"
+) -> dict:
+    """
+    Internal function to post a storage root to the registry
+    the function first adds file:// if the root is local
+    Args:
+        |   url: str the url for the storage root e.g. https://github.com/
+    Returns:
+        |   dict: repsonse from the local registy
+    """
+    if "local" in data and data["local"]:
+        data["root"] = "file://" + data["root"]
+        if data["root"][-1] != os.sep:
+            data["root"] = data["root"] + os.sep
+    elif data["root"][-1] != "/":
+        data["root"] = data["root"] + "/"
+    return post_entry(url, "storage_root", data, token, api_version)
+
+def post_file_type(
+    url: str, data: dict, token: str, api_version: str = "1.0.0"
+) -> dict:
+    """
+    Internal wrapper function to return check if a file_type already exists and return it.
+    """
+    if not "extension" in data and data["extension"]:
+        raise ValueError("error file_type name not specified")
+    file_type_exists = get_entry(url= url, 
+        endpoint= "file_type", 
+        query= {"extension": data["extension"]}, 
+        api_version= api_version)
+    if file_type_exists : return file_type_exists[0]
+    return post_entry(url= url,
+        endpoint= "file_type",
+        data= data,
+        token= token,
+        api_version= api_version)
+
+def remove_local_from_root(root: str) -> str:
+    """
+    Internal function to remove prepending file:// from a given root
+    Args:
+        |   root: the root
+    Returns:
+        |   str: the root without file://
+    """
+    if "file://" in root:
+        root = root.replace("file://", "")
+
+    return root
+
+
+def random_hash() -> str:
+    """
+    Internal function to generate a random unique hash
+
+    Returns:
+        |   str: 40 character randomly generated hash.
+    """
+    seed = datetime.now().timestamp() * random.uniform(1, 1000000)
+    seed_encoded = str(seed).encode("utf-8")
+    hashed = hashlib.sha1(seed_encoded)
+
+    return hashed.hexdigest()
+
+
+def get_file_hash(
+    path: str,
+) -> str:
+    """
+    Internal function to return a files sha1 hash
+    Args:
+        |   path: str file path
+    Returns:
+        |   str: sha1 hash
+    """
+    with open(path, "rb") as data:
+        _data = data.read()
+    # data = data.encode('utf-8')
+    hashed = hashlib.sha1(_data)
+
+    return hashed.hexdigest()
+
+
+def read_token(token_path: str) -> str:
+    """
+    Internal function read a token from a given file
+    Args:
+        |   token_path: path to token
+    Returns:
+        |   str: token
+    """
+    with open(token_path) as token:
+        _token = token.readline().strip()
+    return _token
+
+
+def get_token(token_path: str) -> str:
+    """
+    Internal function alias for read_token()
+    Args:
+        |   token_path: path to token
+    Returns:
+        |   str: token
+    """
+    return read_token(token_path)
+
+
+def is_file(filename: str) -> bool:
+    """
+    Internal function to check whether a file exists
+    Args:
+        |   filename: file to check
+    Returns:
+        |   boolean: whether the file exists
+    """
+    return os.path.isfile(filename)
+
+
+def is_yaml(filename: str) -> bool:
+    """
+    Internal function to check whether a file can be opened as a YAML file
+    ! warning returns True if the file can be coerced into yaml format
+    Args:
+        |   filename: path to the yaml file
+    Returns:
+        |   boolean: can the file be coerced into a yaml format?
+    """
+    try:
+        with open(filename, "r") as data:
+            yaml.safe_load(data)
+    except Exception as err:
+        print(f"{type(err).__name__} was raised: {err}")
+        return False
+    return True
+
+
+def is_valid_yaml(filename: str) -> bool:
+    """
+    Internal function validate whether a file exists and can be coerced into a yaml format
+    Args:
+        |   filename: path to the yaml file
+    Returns:
+        |   boolean: does the file exist and can it be coerced into a yaml format
+    """
+    return is_file(filename) & is_yaml(filename)
+
+
+def generate_uuid() -> str:
+    """
+    Internal function similar to random hash
+    Returns:
+        |   str: a random unique identifier
+    """
+    return datetime.now().strftime("%Y%m-%d%H-%M%S-") + str(uuid.uuid4())
+
+
+def get_handle_index_from_path(handle: dict, path: str) -> Optional[Any]:
+    """
+    Get an input or output handle index from a path
+    usually generated by link_read or link_write
+
+    Args:
+        |   handle: the handle containing the index
+        |   path: path as generated by link_read or link_write
+    """
+    tmp = None
+    if "output" in handle:
+        for output in handle["output"]:
+            if handle["output"][output]["path"] == path:
+                tmp = output
+    if "input" in handle:
+        for input in handle["input"]:
+            if handle["input"][input]["path"] == path:
+                tmp = input
+    return tmp
+
+
+# flake8: noqa C901
+def register_issues(token: str, handle: dict) -> dict:  # sourcery no-metrics
+    """
+    Internal function, should only be called from finalise.
+    """
+
+    api_url = handle["yaml"]["run_metadata"]["local_data_registry_url"]
+    issues = handle["issues"]
+    groups = {handle["issues"][i]["group"] for i in handle["issues"]}
+    api_version = handle["yaml"]["run_metadata"]["api_version"]
+
+    for group in groups:
+        component_list = []
+        issue = None
+        severity = None
+        for i in issues:
+            if issues[i]["group"] == group:
+                type = issues[i]["type"]
+                issue = issues[i]["issue"]
+                severity = issues[i]["severity"]
+                index = issues[i]["index"]
+                data_product = issues[i]["use_data_product"]
+                component = issues[i]["use_component"]
+                version = issues[i]["version"]
+                namespace = issues[i]["use_namespace"]
+
+                component_url = None
+                object_id = None
+                if type == "config":
+                    object_id = handle["model_config"]
+                elif type == "github_repo":
+                    object_id = handle["code_repo"]
+
+                elif type == "submission_script":
+                    object_id = handle["submission_script"]
+                if object_id:
+                    component_url = get_entry(
+                        url=api_url,
+                        endpoint="object_component",
+                        query={
+                            "object": extract_id(object_id),
+                            "whole_object": True,
+                        },
+                        api_version=api_version,
+                    )[0]["url"]
+
+                if index:
+                    if "output" in handle:
+                        for ii in handle["output"]:
+                            if handle["output"][ii] == index:
+                                if (
+                                    "component_url"
+                                    in handle["output"][ii].keys()
+                                ):
+                                    component_url = handle["output"][ii][
+                                        "component_url"
+                                    ]
+                                else:
+                                    logging.warning("No Component Found")
+                    if "input" in handle:
+                        for ii in handle["input"]:
+                            if handle["input"][ii] == index:
+                                if (
+                                    "component_url"
+                                    in handle["input"][ii].keys()
+                                ):
+                                    component_url = handle["input"][ii][
+                                        "component_url"
+                                    ]
+                                else:
+                                    logging.warning("No Component Found")
+
+                if data_product:
+                    current_namespace = get_entry(
+                        url=api_url,
+                        endpoint="namespace",
+                        query={"name": namespace},
+                        api_version=api_version,
+                    )[0]["url"]
+
+                    object = get_entry(
+                        url=api_url,
+                        endpoint="data_product",
+                        query={
+                            "name": data_product,
+                            "version": version,
+                            "namespace": extract_id(current_namespace),
+                        },
+                        api_version=api_version,
+                    )[0]["object"]
+                    object_id = extract_id(object)
+                    if component:
+                        component_url = get_entry(
+                            url=api_url,
+                            endpoint="object_component",
+                            query={"name": component, "object": object_id},
+                            api_version=api_version,
+                        )
+                    else:
+                        component_obj = get_entry(
+                            url=api_url,
+                            endpoint="object_component",
+                            query={"object": object_id, "whole_object": True},
+                            api_version=api_version,
+                        )
+                        component_url = component_obj[0]["url"]
+
+                if component_url:
+                    component_list.append(component_url)
+
+        # Register the issue:
+        logging.info("Registering issue: {}".format(group))
+        current_issue = post_entry(
+            url=api_url,
+            endpoint="issue",
+            data={
+                "severity": severity,
+                "description": issue,
+                "component_issues": component_list,
+            },
+            token=token,
+            api_version=api_version,
+        )
+    return current_issue
```

### Comparing `data_pipeline_api-0.7.8/data_pipeline_api/pipeline.py` & `data_pipeline_api-0.7.9/data_pipeline_api/pipeline.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,613 +1,613 @@
-import datetime
-import logging
-import os
-
-import yaml
-
-from data_pipeline_api import fdp_utils
-
-
-def initialise(token: str, config: str, script: str) -> dict:
-    """Reads in token, config file and script, creates necessary registry items
-    and creates new code run.
-
-    Args:
-        |   token: registry token
-        |   config: Path to config file
-        |   script: Path to script file
-
-    Returns:
-        |   dict: a dictionary containing the following keys:
-        |       'yaml': config_yaml path,
-        |       'fdp_config_dir': config dir path,
-        |       'model_config': model config url,
-        |       'submission_script': submission script object url,
-        |       'code_repo': code repo object url,
-        |       'code_run': coderun url,
-        |       'code_run_uuid': coderun uuid,
-        |       'author': author url
-    """
-
-    # Validate Yamls
-    if not fdp_utils.is_valid_yaml(config):
-        raise ValueError("Config is not a valid YAML file")
-    if not fdp_utils.is_file(script):
-        raise ValueError("Script does not exist")
-
-    # Read config file and extract run metadata
-    with open(config, "r") as data:
-        config_yaml = yaml.safe_load(data)
-    run_metadata = config_yaml["run_metadata"]
-    registry_url = run_metadata["local_data_registry_url"]
-    if registry_url[-1] != "/":
-        registry_url += "/"
-    filename = os.path.basename(config)
-
-    # @todo to be set from config
-    if "api_version" not in config_yaml["run_metadata"].keys():
-        config_yaml["run_metadata"]["api_version"] = "1.0.0"
-
-    api_version = config_yaml["run_metadata"]["api_version"]
-
-    logging.info("Reading {} from local filestore".format(filename))
-
-    # Configure storage root for config
-    config_storageroot_response = fdp_utils.post_storage_root(
-        token=token,
-        url=registry_url,
-        data={"root": run_metadata["write_data_store"], "local": True},
-        api_version=api_version,
-    )
-
-    config_storageroot_url = config_storageroot_response["url"]
-    config_storageroot_id = fdp_utils.extract_id(config_storageroot_url)
-    config_hash = fdp_utils.get_file_hash(config)
-
-    # Configure Storage Location for config
-    config_storage_data = {
-        "path": config.replace(run_metadata["write_data_store"], ""),
-        "hash": config_hash,
-        "public": True,
-        "storage_root": config_storageroot_url,
-    }
-
-    config_location_response = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="storage_location",
-        data=config_storage_data,
-        api_version=api_version,
-    )
-
-    config_location_url = config_location_response["url"]
-
-    # Configure Yaml File Type
-    config_filetype_response = fdp_utils.post_file_type(
-        token=token,
-        url=registry_url,
-        data={"name": "YAML Document", "extension": "yaml"},
-        api_version=api_version,
-    )
-    config_filetype_url = config_filetype_response["url"]
-
-    # Get user for registry admin account
-    results = fdp_utils.get_entry(
-        url=registry_url,
-        endpoint="users",
-        query={"username": "admin"},
-        token=token,
-        api_version=api_version,
-    )
-
-    if not results:
-        raise IndexError(f"list {results} empty")
-    else:
-        user = fdp_utils.get_first_entry(results)
-    # Check users exists
-    if not user:
-        raise ValueError(
-            "Error: Admin user not found\
-        \nDid you run fair init?"
-        )
-
-    user_url = user["url"]
-    user_id = fdp_utils.extract_id(user_url)
-    # Get author(s)
-    results = fdp_utils.get_entry(
-        url=registry_url,
-        endpoint="user_author",
-        query={"user": user_id},
-        api_version=api_version,
-    )
-    if not results:
-        raise IndexError(f"list {results} empty")
-    else:
-        author = fdp_utils.get_first_entry(results)
-    # Check user author exists
-    if not author:
-        raise ValueError(
-            "Error: user_author not found\
-            \nDid you run fair init?"
-        )
-
-    author_url = author["author"]
-
-    # Create new object for config file
-
-    config_object = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="object",
-        data={
-            "description": "Working config.yaml location in datastore",
-            "storage_location": config_location_url,
-            "authors": [author_url],
-            "file_type": config_filetype_url,
-        },
-        api_version=api_version,
-    )
-
-    config_object_url = config_object["url"]
-
-    logging.info("Writing {} to local registry".format(filename))
-
-    # Check if script exists in storage_location
-    script_storageroot_url = config_storageroot_url
-    _ = config_storageroot_id
-    script_hash = fdp_utils.get_file_hash(script)
-
-    script_location_exists = fdp_utils.get_entry(
-        registry_url,
-        "storage_location",
-        query={
-            "hash": script_hash
-        }
-    )
-    if script_location_exists:
-        script_location_url = script_location_exists[0]["url"]
-    else:
-        # Create Script Storage Location
-        script_storage_data = {
-            "path": script.replace(run_metadata["write_data_store"], ""),
-            "hash": script_hash,
-            "public": True,
-            "storage_root": script_storageroot_url,
-        }
-
-        script_location_response = fdp_utils.post_entry(
-            token=token,
-            url=registry_url,
-            endpoint="storage_location",
-            data=script_storage_data,
-            api_version=api_version,
-        )
-
-        script_location_url = script_location_response["url"]
-    script_file_type = os.path.basename(script).split(".")[-1]
-
-    # TODO: Change to Batch?
-    # Create Script File Type
-    script_filetype_response = fdp_utils.post_file_type(
-        token=token,
-        url=registry_url,
-        data={"name": "python submission script", "extension": script_file_type},
-        api_version=api_version,
-    )
-
-    script_filetype_url = script_filetype_response["url"]
-
-    # Create new registry object for script
-    script_object = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="object",
-        data={
-            "description": "Working script location in datastore",
-            "storage_location": script_location_url,
-            "authors": [author_url],
-            "file_type": script_filetype_url,
-        },
-        api_version=api_version,
-    )
-
-    script_object_url = script_object["url"]
-
-    logging.info("Writing {} to local registry".format(script))
-
-    # Create new remote storage root
-    repo_storageroot_url = fdp_utils.post_storage_root(
-        token=token,
-        url=registry_url,
-        data={"root": "https://github.com", "local": False},
-        api_version=api_version,
-    )["url"]
-
-    repo_storageroot_id = fdp_utils.extract_id(repo_storageroot_url)
-
-    sha = run_metadata["latest_commit"]
-    repo_name = run_metadata["remote_repo"]
-
-    # Check if code repo entry exists for given hash
-
-    _ = fdp_utils.get_entry(
-        url=registry_url,
-        endpoint="storage_location",
-        query={
-            "hash": sha,
-            "public": True,
-            "storage_root": repo_storageroot_id,
-        },
-        api_version=api_version,
-    )
-
-    # Configure Code Repo Location
-    coderepo_location_response = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="storage_location",
-        data={
-            "path": repo_name,
-            "hash": sha,
-            "public": True,
-            "storage_root": repo_storageroot_url,
-        },
-        api_version=api_version,
-    )
-
-    coderepo_location_url = coderepo_location_response["url"]
-
-    # Configure Code Repo Object
-    coderepo_object_response = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="object",
-        data={
-            "description": "Analysis / processing script location",
-            "storage_location": coderepo_location_url,
-            "authors": [author_url],
-        },
-        api_version=api_version,
-    )
-
-    coderepo_object_url = coderepo_object_response["url"]
-
-    logging.info("Writing {} to local registry".format(repo_name))
-
-    # Register new code run
-
-    coderun_response = fdp_utils.post_entry(
-        token=token,
-        url=registry_url,
-        endpoint="code_run",
-        data={
-            "run_date": str(datetime.datetime.now()),
-            "description": run_metadata["description"],
-            "code_repo": coderepo_object_url,
-            "model_config": config_object_url,
-            "submission_script": script_object_url,
-            "input_urls": [],
-            "output_urls": [],
-        },
-        api_version=api_version,
-    )
-
-    coderun_url = coderun_response["url"]
-    coderun_uuid = coderun_response["uuid"]
-
-    logging.info("Writing new code_run to local registry")
-
-    # Write code run and object info to handle
-
-    return {
-        "yaml": config_yaml,
-        "fdp_config_dir": os.path.dirname(config),
-        "model_config": config_object_url,
-        "submission_script": script_object_url,
-        "code_repo": coderepo_object_url,
-        "code_run": coderun_url,
-        "code_run_uuid": coderun_uuid,
-        "author": author_url,
-    }
-
-
-# flake8: noqa C901
-def finalise(token: str, handle: dict) -> None:
-    """
-    Renames files with their hash, updates data_product names and records
-    metadata in the registry
-
-    Args:
-        |   token: registry token
-        |   config: Path to config file
-        |   script: Path to script file
-
-    Returns:
-        |   dict: a dictionary containing the following keys:
-        |       'yaml': config_yaml path
-        |       'fdp_config_dir': config dir path
-        |       'model_config': model config url
-        |       'submission_script': submission script object url
-        |       'code_repo': code repo object url
-        |       'code_run': coderun url
-        |       'code_run_uuid': coderun uuid
-        |       'author': author url
-        |       'inputs':
-        |           'data_product': data product
-        |           'use_data_product': data product
-        |           'use_component': component
-        |           'use_version': version
-        |           'use_namespace': namespace
-        |           'path': path
-        |           'component_url': component url
-        |       'outputs':
-        |           component_url: component url
-        |           data_product_url: data product url
-    """
-    # token = fdp_utils.read_token(token)
-    registry_url = handle["yaml"]["run_metadata"]["local_data_registry_url"]
-    datastore = handle["yaml"]["run_metadata"]["write_data_store"]
-    api_version = handle["yaml"]["run_metadata"]["api_version"]
-
-    datastore = fdp_utils.remove_local_from_root(datastore)
-    datastore_root = fdp_utils.get_entry(
-        url=registry_url,
-        endpoint="storage_root",
-        query={"root": datastore},
-        api_version=api_version,
-    )
-    datastore_root_url = None
-
-    # Check datastore is in registry
-    if datastore_root:
-        datastore_root_dict = fdp_utils.get_first_entry(datastore_root)
-        datastore_root_url = datastore_root_dict["url"]
-    else:
-        datastore_root_url = fdp_utils.post_storage_root(
-            token=token,
-            url=registry_url,
-            data={"root": datastore, "local": True},
-            api_version=api_version,
-        )["url"]
-
-    datastore_root_id = fdp_utils.extract_id(datastore_root_url)
-
-    if "output" in handle:
-        for output in handle["output"]:
-
-            if "${RUN_ID}" in handle["output"][output]["use_data_product"]:
-                handle["output"][output]["use_data_product"] = handle[
-                    "output"
-                ][output]["use_data_product"].replace(
-                    "${RUN_ID}", handle["code_run_uuid"]
-                )
-            write_namespace = fdp_utils.get_entry(
-                url=registry_url,
-                endpoint="namespace",
-                query={"name": handle["output"][output]["use_namespace"]},
-                api_version=api_version,
-            )
-            write_namespace_url = None
-            if write_namespace:
-                entry = fdp_utils.get_first_entry(write_namespace)
-                write_namespace_url = entry["url"]
-            else:
-                write_namespace_url = fdp_utils.post_entry(
-                    token=token,
-                    url=registry_url,
-                    endpoint="namespace",
-                    data={"name": handle["output"][output]["use_namespace"]},
-                    api_version=api_version,
-                )["url"]
-
-            hash = fdp_utils.get_file_hash(handle["output"][output]["path"])
-
-            storage_exists = fdp_utils.get_entry(
-                url=registry_url,
-                endpoint="storage_location",
-                query={
-                    "hash": hash,
-                    "public": handle["output"][output]["public"],
-                    "storage_root": datastore_root_id,
-                },
-                api_version=api_version,
-            )
-
-            storage_location_url = None
-
-            if storage_exists:
-                storage_exists_dict = fdp_utils.get_first_entry(storage_exists)
-                storage_location_url = storage_exists_dict["url"]
-
-                os.remove(handle["output"][output]["path"])
-
-                directory = os.path.dirname(handle["output"][output]["path"])
-                i = 0
-                while os.path.normpath(directory) != os.path.normpath(
-                    datastore
-                ):
-                    try:
-                        os.rmdir(directory)
-                    except Exception:
-                        logging.warning(
-                            "Ignoring Directory: {} as it is not empty".format(
-                                directory
-                            )
-                        )
-                        pass
-                    directory = os.path.split(directory)[0]
-                    i += 1
-                    if i > 4:
-                        break
-
-                existing_path = storage_exists_dict["path"]
-
-                existing_root = fdp_utils.get_entity(
-                    url=registry_url,
-                    endpoint="storage_root",
-                    id=int(
-                        fdp_utils.extract_id(
-                            storage_exists_dict["storage_root"]
-                        )
-                    ),
-                    api_version=api_version,
-                )["root"]
-
-                existing_root = fdp_utils.remove_local_from_root(existing_root)
-
-                new_path = os.path.join(existing_root, existing_path)
-
-            else:
-                tmp_filename = os.path.basename(
-                    handle["output"][output]["path"]
-                )
-                extension = tmp_filename.split(sep=".")[-1]
-                new_filename = ".".join([hash, extension])
-                data_product = handle["output"][output]["data_product"]
-                namespace = handle["output"][output]["use_namespace"]
-                new_path = os.path.join(
-                    datastore, namespace, data_product, new_filename
-                ).replace("\\", "/")
-                os.rename(handle["output"][output]["path"], new_path)
-                new_storage_location = os.path.join(
-                    namespace, data_product, new_filename
-                ).replace("\\", "/")
-
-                storage_location_url = fdp_utils.post_entry(
-                    token=token,
-                    url=registry_url,
-                    endpoint="storage_location",
-                    data={
-                        "path": new_storage_location,
-                        "hash": hash,
-                        "public": handle["output"][output]["public"],
-                        "storage_root": datastore_root_url,
-                    },
-                    api_version=api_version,
-                )["url"]
-
-            file_type = os.path.basename(new_path).split(".")[-1]
-
-            file_type_url = fdp_utils.post_file_type(
-                token=token,
-                url=registry_url,
-                data={"name": file_type, "extension": file_type},
-                api_version=api_version,
-                )["url"]
-
-            data_product_exists = fdp_utils.get_entry(
-                url=registry_url,
-                endpoint="data_product",
-                query={
-                    "name": handle["output"][output]["use_data_product"],
-                    "version": handle["output"][output]["use_version"],
-                    "namespace": write_namespace_url,
-                },
-                api_version=api_version,
-            )
-
-            if data_product_exists:
-                data_product_exists_dict = fdp_utils.get_first_entry(
-                    data_product_exists
-                )
-                data_product_url = data_product_exists_dict["url"]
-                object_url = data_product_exists_dict["object"]
-                obj = fdp_utils.get_entity(
-                    url=registry_url,
-                    endpoint="object",
-                    id=int(fdp_utils.extract_id(object_url)),
-                    api_version=api_version,
-                )
-                component_url = obj["components"][0]
-
-            else:
-                object_url = fdp_utils.post_entry(
-                    token=token,
-                    url=registry_url,
-                    endpoint="object",
-                    data={
-                        "description": handle["output"][output][
-                            "data_product_description"
-                        ],
-                        "storage_location": storage_location_url,
-                        "authors": [handle["author"]],
-                        "file_type": file_type_url,
-                    },
-                    api_version=api_version,
-                )["url"]
-
-                component_url = None
-
-                if handle["output"][output]["use_component"]:
-                    component_url = fdp_utils.post_entry(
-                        token=token,
-                        url=registry_url,
-                        endpoint="object_component",
-                        data={
-                            "object": object_url,
-                            "name": handle["output"][output]["use_component"],
-                        },
-                        api_version=api_version,
-                    )["url"]
-                else:
-                    component_url = fdp_utils.get_entry(
-                        url=registry_url,
-                        endpoint="object_component",
-                        query={
-                            "object": fdp_utils.extract_id(object_url),
-                        },
-                        api_version=api_version,
-                    )[0]["url"]
-
-                data_product_url = fdp_utils.post_entry(
-                    token=token,
-                    url=registry_url,
-                    endpoint="data_product",
-                    data={
-                        "name": handle["output"][output]["use_data_product"],
-                        "version": handle["output"][output]["use_version"],
-                        "object": object_url,
-                        "namespace": write_namespace_url,
-                    },
-                    api_version=api_version,
-                )["url"]
-
-            handle["output"][output]["component_url"] = component_url
-            handle["output"][output]["data_product_url"] = data_product_url
-
-            logging.info(
-                "Writing {} to local registry".format(
-                    handle["output"][output]["use_data_product"]
-                )
-            )
-
-    output_components = []
-    input_components = []
-
-    if "output" in handle.keys():
-        for output in handle["output"]:
-            output_components.append(handle["output"][output]["component_url"])
-
-    if "input" in handle.keys():
-        for input in handle["input"]:
-            input_components.append(handle["input"][input]["component_url"])
-
-    if "issues" in handle.keys():
-        fdp_utils.register_issues(token, handle)
-
-    fdp_utils.patch_entry(
-        token=token,
-        url=handle["code_run"],
-        data={"inputs": input_components, "outputs": output_components},
-        api_version=api_version,
-    )
-
-    coderuns_path = os.path.join(
-        handle["fdp_config_dir"], "coderuns.txt"
-    ).replace("\\", "/")
-
-    with open(coderuns_path, "a+") as coderun_file:
-        coderun_file.seek(0)
-        data = coderun_file.read(100)
-        if len(data) > 0:
-            coderun_file.write("\n")
-        coderun_file.write(handle["code_run_uuid"])
+import datetime
+import logging
+import os
+
+import yaml
+
+from data_pipeline_api import fdp_utils
+
+
+def initialise(token: str, config: str, script: str) -> dict:
+    """Reads in token, config file and script, creates necessary registry items
+    and creates new code run.
+
+    Args:
+        |   token: registry token
+        |   config: Path to config file
+        |   script: Path to script file
+
+    Returns:
+        |   dict: a dictionary containing the following keys:
+        |       'yaml': config_yaml path,
+        |       'fdp_config_dir': config dir path,
+        |       'model_config': model config url,
+        |       'submission_script': submission script object url,
+        |       'code_repo': code repo object url,
+        |       'code_run': coderun url,
+        |       'code_run_uuid': coderun uuid,
+        |       'author': author url
+    """
+
+    # Validate Yamls
+    if not fdp_utils.is_valid_yaml(config):
+        raise ValueError("Config is not a valid YAML file")
+    if not fdp_utils.is_file(script):
+        raise ValueError("Script does not exist")
+
+    # Read config file and extract run metadata
+    with open(config, "r") as data:
+        config_yaml = yaml.safe_load(data)
+    run_metadata = config_yaml["run_metadata"]
+    registry_url = run_metadata["local_data_registry_url"]
+    if registry_url[-1] != "/":
+        registry_url += "/"
+    filename = os.path.basename(config)
+
+    # @todo to be set from config
+    if "api_version" not in config_yaml["run_metadata"].keys():
+        config_yaml["run_metadata"]["api_version"] = "1.0.0"
+
+    api_version = config_yaml["run_metadata"]["api_version"]
+
+    logging.info("Reading {} from local filestore".format(filename))
+
+    # Configure storage root for config
+    config_storageroot_response = fdp_utils.post_storage_root(
+        token=token,
+        url=registry_url,
+        data={"root": run_metadata["write_data_store"], "local": True},
+        api_version=api_version,
+    )
+
+    config_storageroot_url = config_storageroot_response["url"]
+    config_storageroot_id = fdp_utils.extract_id(config_storageroot_url)
+    config_hash = fdp_utils.get_file_hash(config)
+
+    # Configure Storage Location for config
+    config_storage_data = {
+        "path": config.replace(run_metadata["write_data_store"], ""),
+        "hash": config_hash,
+        "public": True,
+        "storage_root": config_storageroot_url,
+    }
+
+    config_location_response = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="storage_location",
+        data=config_storage_data,
+        api_version=api_version,
+    )
+
+    config_location_url = config_location_response["url"]
+
+    # Configure Yaml File Type
+    config_filetype_response = fdp_utils.post_file_type(
+        token=token,
+        url=registry_url,
+        data={"name": "YAML Document", "extension": "yaml"},
+        api_version=api_version,
+    )
+    config_filetype_url = config_filetype_response["url"]
+
+    # Get user for registry admin account
+    results = fdp_utils.get_entry(
+        url=registry_url,
+        endpoint="users",
+        query={"username": "admin"},
+        token=token,
+        api_version=api_version,
+    )
+
+    if not results:
+        raise IndexError(f"list {results} empty")
+    else:
+        user = fdp_utils.get_first_entry(results)
+    # Check users exists
+    if not user:
+        raise ValueError(
+            "Error: Admin user not found\
+        \nDid you run fair init?"
+        )
+
+    user_url = user["url"]
+    user_id = fdp_utils.extract_id(user_url)
+    # Get author(s)
+    results = fdp_utils.get_entry(
+        url=registry_url,
+        endpoint="user_author",
+        query={"user": user_id},
+        api_version=api_version,
+    )
+    if not results:
+        raise IndexError(f"list {results} empty")
+    else:
+        author = fdp_utils.get_first_entry(results)
+    # Check user author exists
+    if not author:
+        raise ValueError(
+            "Error: user_author not found\
+            \nDid you run fair init?"
+        )
+
+    author_url = author["author"]
+
+    # Create new object for config file
+
+    config_object = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="object",
+        data={
+            "description": "Working config.yaml location in datastore",
+            "storage_location": config_location_url,
+            "authors": [author_url],
+            "file_type": config_filetype_url,
+        },
+        api_version=api_version,
+    )
+
+    config_object_url = config_object["url"]
+
+    logging.info("Writing {} to local registry".format(filename))
+
+    # Check if script exists in storage_location
+    script_storageroot_url = config_storageroot_url
+    _ = config_storageroot_id
+    script_hash = fdp_utils.get_file_hash(script)
+
+    script_location_exists = fdp_utils.get_entry(
+        registry_url,
+        "storage_location",
+        query={
+            "hash": script_hash
+        }
+    )
+    if script_location_exists:
+        script_location_url = script_location_exists[0]["url"]
+    else:
+        # Create Script Storage Location
+        script_storage_data = {
+            "path": script.replace(run_metadata["write_data_store"], ""),
+            "hash": script_hash,
+            "public": True,
+            "storage_root": script_storageroot_url,
+        }
+
+        script_location_response = fdp_utils.post_entry(
+            token=token,
+            url=registry_url,
+            endpoint="storage_location",
+            data=script_storage_data,
+            api_version=api_version,
+        )
+
+        script_location_url = script_location_response["url"]
+    script_file_type = os.path.basename(script).split(".")[-1]
+
+    # TODO: Change to Batch?
+    # Create Script File Type
+    script_filetype_response = fdp_utils.post_file_type(
+        token=token,
+        url=registry_url,
+        data={"name": "python submission script", "extension": script_file_type},
+        api_version=api_version,
+    )
+
+    script_filetype_url = script_filetype_response["url"]
+
+    # Create new registry object for script
+    script_object = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="object",
+        data={
+            "description": "Working script location in datastore",
+            "storage_location": script_location_url,
+            "authors": [author_url],
+            "file_type": script_filetype_url,
+        },
+        api_version=api_version,
+    )
+
+    script_object_url = script_object["url"]
+
+    logging.info("Writing {} to local registry".format(script))
+
+    # Create new remote storage root
+    repo_storageroot_url = fdp_utils.post_storage_root(
+        token=token,
+        url=registry_url,
+        data={"root": "https://github.com", "local": False},
+        api_version=api_version,
+    )["url"]
+
+    repo_storageroot_id = fdp_utils.extract_id(repo_storageroot_url)
+
+    sha = run_metadata["latest_commit"]
+    repo_name = run_metadata["remote_repo"]
+
+    # Check if code repo entry exists for given hash
+
+    _ = fdp_utils.get_entry(
+        url=registry_url,
+        endpoint="storage_location",
+        query={
+            "hash": sha,
+            "public": True,
+            "storage_root": repo_storageroot_id,
+        },
+        api_version=api_version,
+    )
+
+    # Configure Code Repo Location
+    coderepo_location_response = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="storage_location",
+        data={
+            "path": repo_name,
+            "hash": sha,
+            "public": True,
+            "storage_root": repo_storageroot_url,
+        },
+        api_version=api_version,
+    )
+
+    coderepo_location_url = coderepo_location_response["url"]
+
+    # Configure Code Repo Object
+    coderepo_object_response = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="object",
+        data={
+            "description": "Analysis / processing script location",
+            "storage_location": coderepo_location_url,
+            "authors": [author_url],
+        },
+        api_version=api_version,
+    )
+
+    coderepo_object_url = coderepo_object_response["url"]
+
+    logging.info("Writing {} to local registry".format(repo_name))
+
+    # Register new code run
+
+    coderun_response = fdp_utils.post_entry(
+        token=token,
+        url=registry_url,
+        endpoint="code_run",
+        data={
+            "run_date": str(datetime.datetime.now()),
+            "description": run_metadata["description"],
+            "code_repo": coderepo_object_url,
+            "model_config": config_object_url,
+            "submission_script": script_object_url,
+            "input_urls": [],
+            "output_urls": [],
+        },
+        api_version=api_version,
+    )
+
+    coderun_url = coderun_response["url"]
+    coderun_uuid = coderun_response["uuid"]
+
+    logging.info("Writing new code_run to local registry")
+
+    # Write code run and object info to handle
+
+    return {
+        "yaml": config_yaml,
+        "fdp_config_dir": os.path.dirname(config),
+        "model_config": config_object_url,
+        "submission_script": script_object_url,
+        "code_repo": coderepo_object_url,
+        "code_run": coderun_url,
+        "code_run_uuid": coderun_uuid,
+        "author": author_url,
+    }
+
+
+# flake8: noqa C901
+def finalise(token: str, handle: dict) -> None:
+    """
+    Renames files with their hash, updates data_product names and records
+    metadata in the registry
+
+    Args:
+        |   token: registry token
+        |   config: Path to config file
+        |   script: Path to script file
+
+    Returns:
+        |   dict: a dictionary containing the following keys:
+        |       'yaml': config_yaml path
+        |       'fdp_config_dir': config dir path
+        |       'model_config': model config url
+        |       'submission_script': submission script object url
+        |       'code_repo': code repo object url
+        |       'code_run': coderun url
+        |       'code_run_uuid': coderun uuid
+        |       'author': author url
+        |       'inputs':
+        |           'data_product': data product
+        |           'use_data_product': data product
+        |           'use_component': component
+        |           'use_version': version
+        |           'use_namespace': namespace
+        |           'path': path
+        |           'component_url': component url
+        |       'outputs':
+        |           component_url: component url
+        |           data_product_url: data product url
+    """
+    # token = fdp_utils.read_token(token)
+    registry_url = handle["yaml"]["run_metadata"]["local_data_registry_url"]
+    datastore = handle["yaml"]["run_metadata"]["write_data_store"]
+    api_version = handle["yaml"]["run_metadata"]["api_version"]
+
+    datastore = fdp_utils.remove_local_from_root(datastore)
+    datastore_root = fdp_utils.get_entry(
+        url=registry_url,
+        endpoint="storage_root",
+        query={"root": datastore},
+        api_version=api_version,
+    )
+    datastore_root_url = None
+
+    # Check datastore is in registry
+    if datastore_root:
+        datastore_root_dict = fdp_utils.get_first_entry(datastore_root)
+        datastore_root_url = datastore_root_dict["url"]
+    else:
+        datastore_root_url = fdp_utils.post_storage_root(
+            token=token,
+            url=registry_url,
+            data={"root": datastore, "local": True},
+            api_version=api_version,
+        )["url"]
+
+    datastore_root_id = fdp_utils.extract_id(datastore_root_url)
+
+    if "output" in handle:
+        for output in handle["output"]:
+
+            if "${RUN_ID}" in handle["output"][output]["use_data_product"]:
+                handle["output"][output]["use_data_product"] = handle[
+                    "output"
+                ][output]["use_data_product"].replace(
+                    "${RUN_ID}", handle["code_run_uuid"]
+                )
+            write_namespace = fdp_utils.get_entry(
+                url=registry_url,
+                endpoint="namespace",
+                query={"name": handle["output"][output]["use_namespace"]},
+                api_version=api_version,
+            )
+            write_namespace_url = None
+            if write_namespace:
+                entry = fdp_utils.get_first_entry(write_namespace)
+                write_namespace_url = entry["url"]
+            else:
+                write_namespace_url = fdp_utils.post_entry(
+                    token=token,
+                    url=registry_url,
+                    endpoint="namespace",
+                    data={"name": handle["output"][output]["use_namespace"]},
+                    api_version=api_version,
+                )["url"]
+
+            hash = fdp_utils.get_file_hash(handle["output"][output]["path"])
+
+            storage_exists = fdp_utils.get_entry(
+                url=registry_url,
+                endpoint="storage_location",
+                query={
+                    "hash": hash,
+                    "public": handle["output"][output]["public"],
+                    "storage_root": datastore_root_id,
+                },
+                api_version=api_version,
+            )
+
+            storage_location_url = None
+
+            if storage_exists:
+                storage_exists_dict = fdp_utils.get_first_entry(storage_exists)
+                storage_location_url = storage_exists_dict["url"]
+
+                os.remove(handle["output"][output]["path"])
+
+                directory = os.path.dirname(handle["output"][output]["path"])
+                i = 0
+                while os.path.normpath(directory) != os.path.normpath(
+                    datastore
+                ):
+                    try:
+                        os.rmdir(directory)
+                    except Exception:
+                        logging.warning(
+                            "Ignoring Directory: {} as it is not empty".format(
+                                directory
+                            )
+                        )
+                        pass
+                    directory = os.path.split(directory)[0]
+                    i += 1
+                    if i > 4:
+                        break
+
+                existing_path = storage_exists_dict["path"]
+
+                existing_root = fdp_utils.get_entity(
+                    url=registry_url,
+                    endpoint="storage_root",
+                    id=int(
+                        fdp_utils.extract_id(
+                            storage_exists_dict["storage_root"]
+                        )
+                    ),
+                    api_version=api_version,
+                )["root"]
+
+                existing_root = fdp_utils.remove_local_from_root(existing_root)
+
+                new_path = os.path.join(existing_root, existing_path)
+
+            else:
+                tmp_filename = os.path.basename(
+                    handle["output"][output]["path"]
+                )
+                extension = tmp_filename.split(sep=".")[-1]
+                new_filename = ".".join([hash, extension])
+                data_product = handle["output"][output]["data_product"]
+                namespace = handle["output"][output]["use_namespace"]
+                new_path = os.path.join(
+                    datastore, namespace, data_product, new_filename
+                ).replace("\\", "/")
+                os.rename(handle["output"][output]["path"], new_path)
+                new_storage_location = os.path.join(
+                    namespace, data_product, new_filename
+                ).replace("\\", "/")
+
+                storage_location_url = fdp_utils.post_entry(
+                    token=token,
+                    url=registry_url,
+                    endpoint="storage_location",
+                    data={
+                        "path": new_storage_location,
+                        "hash": hash,
+                        "public": handle["output"][output]["public"],
+                        "storage_root": datastore_root_url,
+                    },
+                    api_version=api_version,
+                )["url"]
+
+            file_type = os.path.basename(new_path).split(".")[-1]
+
+            file_type_url = fdp_utils.post_file_type(
+                token=token,
+                url=registry_url,
+                data={"name": file_type, "extension": file_type},
+                api_version=api_version,
+                )["url"]
+
+            data_product_exists = fdp_utils.get_entry(
+                url=registry_url,
+                endpoint="data_product",
+                query={
+                    "name": handle["output"][output]["use_data_product"],
+                    "version": handle["output"][output]["use_version"],
+                    "namespace": write_namespace_url,
+                },
+                api_version=api_version,
+            )
+
+            if data_product_exists:
+                data_product_exists_dict = fdp_utils.get_first_entry(
+                    data_product_exists
+                )
+                data_product_url = data_product_exists_dict["url"]
+                object_url = data_product_exists_dict["object"]
+                obj = fdp_utils.get_entity(
+                    url=registry_url,
+                    endpoint="object",
+                    id=int(fdp_utils.extract_id(object_url)),
+                    api_version=api_version,
+                )
+                component_url = obj["components"][0]
+
+            else:
+                object_url = fdp_utils.post_entry(
+                    token=token,
+                    url=registry_url,
+                    endpoint="object",
+                    data={
+                        "description": handle["output"][output][
+                            "data_product_description"
+                        ],
+                        "storage_location": storage_location_url,
+                        "authors": [handle["author"]],
+                        "file_type": file_type_url,
+                    },
+                    api_version=api_version,
+                )["url"]
+
+                component_url = None
+
+                if handle["output"][output]["use_component"]:
+                    component_url = fdp_utils.post_entry(
+                        token=token,
+                        url=registry_url,
+                        endpoint="object_component",
+                        data={
+                            "object": object_url,
+                            "name": handle["output"][output]["use_component"],
+                        },
+                        api_version=api_version,
+                    )["url"]
+                else:
+                    component_url = fdp_utils.get_entry(
+                        url=registry_url,
+                        endpoint="object_component",
+                        query={
+                            "object": fdp_utils.extract_id(object_url),
+                        },
+                        api_version=api_version,
+                    )[0]["url"]
+
+                data_product_url = fdp_utils.post_entry(
+                    token=token,
+                    url=registry_url,
+                    endpoint="data_product",
+                    data={
+                        "name": handle["output"][output]["use_data_product"],
+                        "version": handle["output"][output]["use_version"],
+                        "object": object_url,
+                        "namespace": write_namespace_url,
+                    },
+                    api_version=api_version,
+                )["url"]
+
+            handle["output"][output]["component_url"] = component_url
+            handle["output"][output]["data_product_url"] = data_product_url
+
+            logging.info(
+                "Writing {} to local registry".format(
+                    handle["output"][output]["use_data_product"]
+                )
+            )
+
+    output_components = []
+    input_components = []
+
+    if "output" in handle.keys():
+        for output in handle["output"]:
+            output_components.append(handle["output"][output]["component_url"])
+
+    if "input" in handle.keys():
+        for input in handle["input"]:
+            input_components.append(handle["input"][input]["component_url"])
+
+    if "issues" in handle.keys():
+        fdp_utils.register_issues(token, handle)
+
+    fdp_utils.patch_entry(
+        token=token,
+        url=handle["code_run"],
+        data={"inputs": input_components, "outputs": output_components},
+        api_version=api_version,
+    )
+
+    coderuns_path = os.path.join(
+        handle["fdp_config_dir"], "coderuns.txt"
+    ).replace("\\", "/")
+
+    with open(coderuns_path, "a+") as coderun_file:
+        coderun_file.seek(0)
+        data = coderun_file.read(100)
+        if len(data) > 0:
+            coderun_file.write("\n")
+        coderun_file.write(handle["code_run_uuid"])
```

### Comparing `data_pipeline_api-0.7.8/setup.py` & `data_pipeline_api-0.7.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,75 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: data-pipeline-api
+Version: 0.7.9
+Summary: Python api to interact with the Fair Data Pipeline
+Home-page: https://www.fairdatapipeline.org/
+License: GNU General Public License v3.0
+Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
+Author: Ryan J Field
+Author-email: ryan.field@glasgow.ac.uk
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: h5py (>=3.6.0,<4.0.0)
+Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Project-URL: Issue Tracker, https://github.com/FAIRDataPipeline/pyDataPipeline/issues
+Project-URL: Repository, https://github.com/FAIRDataPipeline/pyDataPipeline
+Description-Content-Type: text/markdown
+
+# pyDataPipeline
+
+[![pyDataPipeline](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml/badge.svg?branch=dev)](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml)
+[![codecov](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline/branch/dev/graph/badge.svg?token=Eax5AmrDxx)](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5562602.svg)](https://doi.org/10.5281/zenodo.5562602)
+[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5461/badge)](https://bestpractices.coreinfrastructure.org/projects/5461)
+
+Welcome to pyDataPipeline a Python api to interact with the Fair Data Pipeline.
+
+Full documention of the pyDataPipeline is avaialable at [https://www.fairdatapipeline.org/pyDataPipeline/](https://www.fairdatapipeline.org/pyDataPipeline/)
+
+## Installation
+pyDataPipeline can be installed from PyPi:
+```
+pip3 install data-pipeline-api
+```
+
+Or from the Repository:
+```
+git clone https://github.com/FAIRDataPipeline/pythonFDP.git
+
+git checkout dev
+
+pip3 install -e .
+```
+**NB. PyDataPipeline requires Python3.**
+
+## Example submission_script
+
+Assume FDP_CONFIG_DIR, storage_locations and objects have been set by CLI tool
+
+```
+import os
+import fairdatapipeline as pipeline
+
+token = os.environ['FDP_LOCAL_TOKEN']
+config_dir = os.environ['FDP_CONFIG_DIR']
+config_path = os.path.join(config_dir, 'config.yaml')
+script_path = os.path.join(config_dir, 'script.sh')
+
+handle = pipeline.initialise(token, config_path, script_path)
 
-packages = \
-['data_pipeline_api', 'data_pipeline_api.ext']
+pipeline.finalise(token, handle)
 
-package_data = \
-{'': ['*']}
+```
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'h5py>=3.6.0,<4.0.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'scipy>=1.7.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'data-pipeline-api',
-    'version': '0.7.8',
-    'description': 'Python api to interact with the Fair Data Pipeline',
-    'long_description': "# pyDataPipeline\n\n[![pyDataPipeline](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml/badge.svg?branch=dev)](https://github.com/FAIRDataPipeline/pyDataPipeline/actions/workflows/pyDataPipeline.yaml)\n[![codecov](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline/branch/dev/graph/badge.svg?token=Eax5AmrDxx)](https://codecov.io/gh/FAIRDataPipeline/pyDataPipeline)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5562602.svg)](https://doi.org/10.5281/zenodo.5562602)\n[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5461/badge)](https://bestpractices.coreinfrastructure.org/projects/5461)\n\nWelcome to pyDataPipeline a Python api to interact with the Fair Data Pipeline.\n\nFull documention of the pyDataPipeline is avaialable at [https://www.fairdatapipeline.org/pyDataPipeline/](https://www.fairdatapipeline.org/pyDataPipeline/)\n\n## Installation\npyDataPipeline can be installed from PyPi:\n```\npip3 install data-pipeline-api\n```\n\nOr from the Repository:\n```\ngit clone https://github.com/FAIRDataPipeline/pythonFDP.git\n\ngit checkout dev\n\npip3 install -e .\n```\n**NB. PyDataPipeline requires Python3.**\n\n## Example submission_script\n\nAssume FDP_CONFIG_DIR, storage_locations and objects have been set by CLI tool\n\n```\nimport os\nimport fairdatapipeline as pipeline\n\ntoken = os.environ['FDP_LOCAL_TOKEN']\nconfig_dir = os.environ['FDP_CONFIG_DIR']\nconfig_path = os.path.join(config_dir, 'config.yaml')\nscript_path = os.path.join(config_dir, 'script.sh')\n\nhandle = pipeline.initialise(token, config_path, script_path)\n\npipeline.finalise(token, handle)\n\n```\n\n## SEIRS Model Example\n\nThe SEIRS Model Example is available at: [https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html](https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html)\n",
-    'author': 'Ryan J Field',
-    'author_email': 'ryan.field@glasgow.ac.uk',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://www.fairdatapipeline.org/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
-}
+## SEIRS Model Example
 
+The SEIRS Model Example is available at: [https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html](https://www.fairdatapipeline.org/pyDataPipeline/examples/SEIRS.html)
 
-setup(**setup_kwargs)
```

