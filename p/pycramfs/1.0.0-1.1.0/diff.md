# Comparing `tmp/pycramfs-1.0.0.tar.gz` & `tmp/pycramfs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycramfs-1.0.0.tar", last modified: Thu Apr 27 17:55:43 2023, max compression
+gzip compressed data, was "pycramfs-1.1.0.tar", last modified: Sat Jul  1 13:11:58 2023, max compression
```

## Comparing `pycramfs-1.0.0.tar` & `pycramfs-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:55:43.248649 pycramfs-1.0.0/
--rw-rw-rw-   0        0        0    35821 2023-04-27 15:05:06.000000 pycramfs-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9032 2023-04-27 17:55:43.246651 pycramfs-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7804 2023-04-27 16:16:33.000000 pycramfs-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 17:55:43.221649 pycramfs-1.0.0/pycramfs/
--rw-rw-rw-   0        0        0     3044 2023-04-27 15:10:34.000000 pycramfs-1.0.0/pycramfs/__init__.py
--rw-rw-rw-   0        0        0     7344 2023-04-27 17:49:47.000000 pycramfs-1.0.0/pycramfs/__main__.py
--rw-rw-rw-   0        0        0     1065 2023-04-25 16:42:21.000000 pycramfs-1.0.0/pycramfs/const.py
--rw-rw-rw-   0        0        0       41 2023-04-22 09:13:45.000000 pycramfs-1.0.0/pycramfs/exception.py
--rw-rw-rw-   0        0        0     3127 2023-04-26 17:16:30.000000 pycramfs-1.0.0/pycramfs/extract.py
--rw-rw-rw-   0        0        0     8599 2023-04-26 13:58:13.000000 pycramfs-1.0.0/pycramfs/file.py
--rw-rw-rw-   0        0        0     3674 2023-04-26 11:17:54.000000 pycramfs-1.0.0/pycramfs/structure.py
--rw-rw-rw-   0        0        0     4069 2023-04-26 11:15:10.000000 pycramfs-1.0.0/pycramfs/util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:55:43.243647 pycramfs-1.0.0/pycramfs.egg-info/
--rw-rw-rw-   0        0        0     9032 2023-04-27 17:55:43.000000 pycramfs-1.0.0/pycramfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-27 17:55:43.000000 pycramfs-1.0.0/pycramfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:55:43.000000 pycramfs-1.0.0/pycramfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-27 17:55:43.000000 pycramfs-1.0.0/pycramfs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 17:55:43.000000 pycramfs-1.0.0/pycramfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1430 2023-04-27 17:50:12.000000 pycramfs-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 17:55:43.248649 pycramfs-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:11:58.133241 pycramfs-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-01 13:11:47.000000 pycramfs-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-01 13:11:58.133241 pycramfs-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-01 13:11:47.000000 pycramfs-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:11:58.133241 pycramfs-1.1.0/pycramfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pycramfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 13:11:58.133241 pycramfs-1.1.0/pycramfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-01 13:11:58.000000 pycramfs-1.1.0/pycramfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-01 13:11:58.000000 pycramfs-1.1.0/pycramfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 13:11:58.000000 pycramfs-1.1.0/pycramfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 13:11:58.000000 pycramfs-1.1.0/pycramfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 13:11:58.000000 pycramfs-1.1.0/pycramfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-01 13:11:47.000000 pycramfs-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 13:11:58.133241 pycramfs-1.1.0/setup.cfg
```

### Comparing `pycramfs-1.0.0/LICENSE` & `pycramfs-1.1.0/LICENSE`

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
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pycramfs-1.0.0/PKG-INFO` & `pycramfs-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,257 +1,258 @@
-Metadata-Version: 2.1
-Name: pycramfs
-Version: 1.0.0
-Summary: Read and extract cramfs images.
-Author-email: AT0myks <at0myks.dev@gmail.com>
-Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
-Project-URL: Source, https://github.com/AT0myks/pycramfs
-Keywords: cramfs,filesystem
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Filesystems
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pycramfs
-
-<p align="left">
-<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
-<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
-<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
-</p>
-
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Usage](#usage)
-* [References](#references)
-
-A library and tool to read and extract cramfs images.
-
-It is far from being as complete as the tools it's based on,
-but should be enough for simple images.
-For example, as of right now it only supports contiguous data layout.
-Only little endian images are supported.
-
-It also provides ways to extract data from an image,
-although you might prefer using
-[`cramfsck`](https://github.com/npitre/cramfs-tools)
-on Linux and 7-Zip on Windows for better compatibility.
-
-## Requirements
-
-Python 3.8+.
-
-## Installation
-
-```
-pip install pycramfs
-```
-
-## Usage
-
-### API
-
-Here's an overview of what you can do:
-```py
-from pycramfs import Cramfs
-from pycramfs.extract import extract_dir, extract_file
-from pycramfs.util import find_superblocks
-
-fsimage = "cramfs.bin"
-superblocks = find_superblocks(fsimage)
-
-with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
-    # Optional offset for start of file system.
-    # You can also create Cramfs instances from bytes or a file descriptor.
-
-    sblock = cramfs.super  # Access the file system's superblock
-    print(sblock.name)
-    print(dict(sblock))  # Superblock as a dictionary
-    assert cramfs.calculate_crc() == sblock.fsid.crc
-
-    rootdir = cramfs.rootdir  # root directory
-    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
-    # Number of files in the whole file system (shortcut to sblock.fsid.files).
-    print(len(cramfs))
-    print("/etc/passwd" in cramfs)  # Check if path exists
-
-    # Iterate over the whole file system.
-    for file in cramfs:
-        print(file.parent)  # Instance of Directory (None for the root directory)
-        print(file in cramfs)  # Check if file belongs to this image
-        if file.is_symlink:  # Check the file's type
-            print(file.readlink())  # Symlink target
-
-    etc = cramfs.select("/etc")  # Select a specific file or directory
-    etc = cramfs.select("etc")  # Can also be a relative path
-    rootdir = etc.select("..")  # And a special entry
-    assert rootdir == rootdir.select('.')
-    print(etc)  # print the file or directory's name
-    # The file or directory's absolute path (an instance of PurePosixPath).
-    print(etc.path)
-    print(etc.files)  # A dictionary mapping file names to File instances
-    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
-    print(etc.total)  # Number of entries in this whole subtree
-    # A list of this directory's children (shortcut to list(etc.files.values())).
-    print(list(etc))
-
-    # Find the first file in this subtree that has this name.
-    passwd = cramfs.find("passwd")
-    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
-    passwd = etc["passwd"]
-    print("passwd" in etc)  # Check if directory contains this file
-    print(passwd in etc)  # Also works with instances of File
-
-    # Iterate over this directory's files.
-    for file in etc:
-        print(file.inode)  # Access inode information
-        # These attributes are shortcuts to file.inode.<attr>
-        print(file.mode)
-        print(file.uid)
-        print(file.size)
-        print(file.gid)
-
-    # Iterate over this whole subtree.
-    for file in etc.riter():
-        print(file.name)  # File name, equivalent to file.path.name
-        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
-    
-    # Iterate over files in the subtree that match a pattern.
-    for config_file in etc.itermatch("*.conf"):
-        print(config_file.read_bytes())  # Read the file's raw content
-        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
-
-    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
-
-    # You can use absolute paths from any directory.
-    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
-    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
-
-    # Calling find(), select() and itermatch() on cramfs
-    # is the same as calling them on cramfs.rootdir.
-
-    extract_dir(etc, "extract/etc")  # Extract a directory tree
-    extract_file(passwd, "extract/passwd")  # Extract a single file
-```
-
-### Command line
-
-pycramfs comes with a command-line interface that consists of 4 sub-commands.
-
-#### Info
-
-```
-usage: pycramfs info [-h] file
-
-Show information about all the superblocks that can be found in a file
-
-positional arguments:
-  file
-```
-
-Example output:
-```
-$ pycramfs info cramfs.bin
-Superblock #1
-Magic:     0x28CD3D45
-Size:      282,624
-Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
-Future:    0
-Signature: Compressed ROMFS
-Name:      Compressed
-CRC:       0xDEADBEEF
-Edition:   0
-Blocks:    6,926
-Files:     420
-Offset:    8157
-```
-
-#### List
-
-```
-usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
-
-List the contents of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
-  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
-  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
-                                  filter by file type with f, d, l, p, s, b, c
-```
-
-Example that lists only directories and symlinks that match a pattern:
-```
-$ pycramfs list cramfs.bin -t d l -p "*bin*"
-drwxrwxr-x      256   123:0   /bin 
-lrwxrwxrwx        7   123:0   /bin/ash -> busybox
-lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
-3 file(s) found
-```
-
-#### Extract
-
-```
-usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
-
-Extract files from the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-  -d DEST, --dest DEST         destination directory. Default: next to file
-  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
-  -f, --force                  overwrite files that already exist. Default: False
-  -q, --quiet                  don't print extraction status. Default: False
-```
-
-On Linux, just like `cramfsck -x` you need to run as root
-if you want to preserve file mode, owner and group.
-
-On Windows, the only reason to run as a privileged user is to be able to create
-symlinks.
-Unprivileged accounts can create symlinks if Developer Mode is enabled.
-Otherwise, a regular file containing the target will be created.
-Special files will always just be empty files.
-
-#### Check
-
-This command is similar to running `cramfsck -c file` but is not as thorough.
-
-```
-usage: pycramfs check [-h] [-o OFFSET] file
-
-Make a few superficial checks of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-```
-
-## References
-
-- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
-- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
-- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
-- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
+Metadata-Version: 2.1
+Name: pycramfs
+Version: 1.1.0
+Summary: Read and extract cramfs images.
+Author-email: AT0myks <at0myks.dev@gmail.com>
+Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
+Project-URL: Source, https://github.com/AT0myks/pycramfs
+Keywords: cramfs,filesystem
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Filesystems
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pycramfs
+
+<p align="left">
+<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
+<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
+<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
+</p>
+
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Usage](#usage)
+* [References](#references)
+
+A library and tool to read and extract cramfs images.
+
+It is far from being as complete as the tools it's based on,
+but should be enough for simple images.
+For example, as of right now it only supports contiguous data layout.
+Only little endian images are supported.
+
+It also provides ways to extract data from an image,
+although you might prefer using
+[`cramfsck`](https://github.com/npitre/cramfs-tools)
+on Linux and 7-Zip on Windows for better compatibility.
+
+## Requirements
+
+Python 3.8+.
+
+## Installation
+
+```
+pip install pycramfs
+```
+
+## Usage
+
+### API
+
+Here's an overview of what you can do:
+```py
+from pycramfs import Cramfs
+from pycramfs.extract import extract_dir, extract_file
+from pycramfs.util import find_superblocks
+
+fsimage = "cramfs.bin"
+superblocks = find_superblocks(fsimage)
+
+with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
+    # Optional offset for start of file system.
+    # You can also create Cramfs instances from bytes or a file descriptor.
+
+    sblock = cramfs.super  # Access the file system's superblock
+    print(sblock.name)
+    print(dict(sblock))  # Superblock as a dictionary
+    assert cramfs.calculate_crc() == sblock.fsid.crc
+
+    rootdir = cramfs.rootdir  # root directory
+    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
+    # Number of files in the whole file system (shortcut to sblock.fsid.files).
+    print(len(cramfs))
+    print("/etc/passwd" in cramfs)  # Check if path exists
+
+    # Iterate over the whole file system.
+    for file in cramfs:
+        print(file.parent)  # Instance of Directory (None for the root directory)
+        print(file in cramfs)  # Check if file belongs to this image
+        if file.is_symlink:  # Check the file's type
+            print(file.readlink())  # Symlink target
+
+    etc = cramfs.select("/etc")  # Select a specific file or directory
+    etc = cramfs.select("etc")  # Can also be a relative path
+    rootdir = etc.select("..")  # And a special entry
+    assert rootdir == rootdir.select('.')
+    print(etc)  # print the file or directory's name
+    # The file or directory's absolute path (an instance of PurePosixPath).
+    print(etc.path)
+    print(etc.files)  # A dictionary mapping file names to File instances
+    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
+    print(etc.total)  # Number of entries in this whole subtree
+    # A list of this directory's children (shortcut to list(etc.files.values())).
+    print(list(etc))
+
+    # Find the first file in this subtree that has this name.
+    passwd = cramfs.find("passwd")
+    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
+    passwd = etc["passwd"]
+    print("passwd" in etc)  # Check if directory contains this file
+    print(passwd in etc)  # Also works with instances of File
+
+    # Iterate over this directory's files.
+    for file in etc:
+        print(file.inode)  # Access inode information
+        # These attributes are shortcuts to file.inode.<attr>
+        print(file.mode)
+        print(file.uid)
+        print(file.size)
+        print(file.gid)
+
+    # Iterate over this whole subtree.
+    for file in etc.riter():
+        print(file.name)  # File name, equivalent to file.path.name
+        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
+    
+    # Iterate over files in the subtree that match a pattern.
+    for config_file in etc.itermatch("*.conf"):
+        print(config_file.read_bytes())  # Read the file's raw content
+        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
+
+    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
+
+    # You can use absolute paths from any directory.
+    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
+    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
+
+    # Calling find(), select() and itermatch() on cramfs
+    # is the same as calling them on cramfs.rootdir.
+
+    extract_dir(etc, "extract/etc")  # Extract a directory tree
+    extract_file(passwd, "extract/passwd")  # Extract a single file
+```
+
+### Command line
+
+pycramfs comes with a command-line interface that consists of 4 sub-commands.
+
+#### Info
+
+```
+usage: pycramfs info [-h] file
+
+Show information about all the superblocks that can be found in a file
+
+positional arguments:
+  file
+```
+
+Example output:
+```
+$ pycramfs info cramfs.bin
+Superblock #1
+Magic:     0x28CD3D45
+Size:      282,624
+Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
+Future:    0
+Signature: Compressed ROMFS
+Name:      Compressed
+CRC:       0xDEADBEEF
+Edition:   0
+Blocks:    6,926
+Files:     420
+Offset:    8157
+```
+
+#### List
+
+```
+usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
+
+List the contents of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
+  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
+  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
+                                  filter by file type with f, d, l, p, s, b, c
+```
+
+Example that lists only directories and symlinks that match a pattern:
+```
+$ pycramfs list cramfs.bin -t d l -p "*bin*"
+drwxrwxr-x      256   123:0   /bin 
+lrwxrwxrwx        7   123:0   /bin/ash -> busybox
+lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
+3 file(s) found
+```
+
+#### Extract
+
+```
+usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
+
+Extract files from the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+  -d DEST, --dest DEST         destination directory. Default: next to file
+  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
+  -f, --force                  overwrite files that already exist. Default: False
+  -q, --quiet                  don't print extraction status. Default: False
+```
+
+On Linux, just like `cramfsck -x` you need to run as root
+if you want to preserve file mode, owner and group.
+
+On Windows, the only reason to run as a privileged user is to be able to create
+symlinks.
+Unprivileged accounts can create symlinks if Developer Mode is enabled.
+Otherwise, a regular file containing the target will be created.
+Special files will always just be empty files.
+
+#### Check
+
+This command is similar to running `cramfsck -c file` but is not as thorough.
+
+```
+usage: pycramfs check [-h] [-o OFFSET] file
+
+Make a few superficial checks of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+```
+
+## References
+
+- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
+- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
+- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
+- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pycramfs Version: 1.0.0 Summary: Read and extract
+Metadata-Version: 2.1 Name: pycramfs Version: 1.1.0 Summary: Read and extract
 cramfs images. Author-email: AT0myks
 dev@gmail.com> Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
 Project-URL: Source, https://github.com/AT0myks/pycramfs Keywords:
 cramfs,filesystem Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 End Users/Desktop Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: System :: Filesystems Classifier: Topic ::
-Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE # pycramfs
+Utilities Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # pycramfs
 [Python versions] [PyPI] [License]
 * [Requirements](#requirements) * [Installation](#installation) * [Usage]
 (#usage) * [References](#references) A library and tool to read and extract
 cramfs images. It is far from being as complete as the tools it's based on, but
 should be enough for simple images. For example, as of right now it only
 supports contiguous data layout. Only little endian images are supported. It
 also provides ways to extract data from an image, although you might prefer
```

### Comparing `pycramfs-1.0.0/README.md` & `pycramfs-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-# pycramfs
-
-<p align="left">
-<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
-<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
-<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
-</p>
-
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Usage](#usage)
-* [References](#references)
-
-A library and tool to read and extract cramfs images.
-
-It is far from being as complete as the tools it's based on,
-but should be enough for simple images.
-For example, as of right now it only supports contiguous data layout.
-Only little endian images are supported.
-
-It also provides ways to extract data from an image,
-although you might prefer using
-[`cramfsck`](https://github.com/npitre/cramfs-tools)
-on Linux and 7-Zip on Windows for better compatibility.
-
-## Requirements
-
-Python 3.8+.
-
-## Installation
-
-```
-pip install pycramfs
-```
-
-## Usage
-
-### API
-
-Here's an overview of what you can do:
-```py
-from pycramfs import Cramfs
-from pycramfs.extract import extract_dir, extract_file
-from pycramfs.util import find_superblocks
-
-fsimage = "cramfs.bin"
-superblocks = find_superblocks(fsimage)
-
-with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
-    # Optional offset for start of file system.
-    # You can also create Cramfs instances from bytes or a file descriptor.
-
-    sblock = cramfs.super  # Access the file system's superblock
-    print(sblock.name)
-    print(dict(sblock))  # Superblock as a dictionary
-    assert cramfs.calculate_crc() == sblock.fsid.crc
-
-    rootdir = cramfs.rootdir  # root directory
-    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
-    # Number of files in the whole file system (shortcut to sblock.fsid.files).
-    print(len(cramfs))
-    print("/etc/passwd" in cramfs)  # Check if path exists
-
-    # Iterate over the whole file system.
-    for file in cramfs:
-        print(file.parent)  # Instance of Directory (None for the root directory)
-        print(file in cramfs)  # Check if file belongs to this image
-        if file.is_symlink:  # Check the file's type
-            print(file.readlink())  # Symlink target
-
-    etc = cramfs.select("/etc")  # Select a specific file or directory
-    etc = cramfs.select("etc")  # Can also be a relative path
-    rootdir = etc.select("..")  # And a special entry
-    assert rootdir == rootdir.select('.')
-    print(etc)  # print the file or directory's name
-    # The file or directory's absolute path (an instance of PurePosixPath).
-    print(etc.path)
-    print(etc.files)  # A dictionary mapping file names to File instances
-    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
-    print(etc.total)  # Number of entries in this whole subtree
-    # A list of this directory's children (shortcut to list(etc.files.values())).
-    print(list(etc))
-
-    # Find the first file in this subtree that has this name.
-    passwd = cramfs.find("passwd")
-    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
-    passwd = etc["passwd"]
-    print("passwd" in etc)  # Check if directory contains this file
-    print(passwd in etc)  # Also works with instances of File
-
-    # Iterate over this directory's files.
-    for file in etc:
-        print(file.inode)  # Access inode information
-        # These attributes are shortcuts to file.inode.<attr>
-        print(file.mode)
-        print(file.uid)
-        print(file.size)
-        print(file.gid)
-
-    # Iterate over this whole subtree.
-    for file in etc.riter():
-        print(file.name)  # File name, equivalent to file.path.name
-        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
-    
-    # Iterate over files in the subtree that match a pattern.
-    for config_file in etc.itermatch("*.conf"):
-        print(config_file.read_bytes())  # Read the file's raw content
-        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
-
-    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
-
-    # You can use absolute paths from any directory.
-    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
-    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
-
-    # Calling find(), select() and itermatch() on cramfs
-    # is the same as calling them on cramfs.rootdir.
-
-    extract_dir(etc, "extract/etc")  # Extract a directory tree
-    extract_file(passwd, "extract/passwd")  # Extract a single file
-```
-
-### Command line
-
-pycramfs comes with a command-line interface that consists of 4 sub-commands.
-
-#### Info
-
-```
-usage: pycramfs info [-h] file
-
-Show information about all the superblocks that can be found in a file
-
-positional arguments:
-  file
-```
-
-Example output:
-```
-$ pycramfs info cramfs.bin
-Superblock #1
-Magic:     0x28CD3D45
-Size:      282,624
-Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
-Future:    0
-Signature: Compressed ROMFS
-Name:      Compressed
-CRC:       0xDEADBEEF
-Edition:   0
-Blocks:    6,926
-Files:     420
-Offset:    8157
-```
-
-#### List
-
-```
-usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
-
-List the contents of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
-  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
-  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
-                                  filter by file type with f, d, l, p, s, b, c
-```
-
-Example that lists only directories and symlinks that match a pattern:
-```
-$ pycramfs list cramfs.bin -t d l -p "*bin*"
-drwxrwxr-x      256   123:0   /bin 
-lrwxrwxrwx        7   123:0   /bin/ash -> busybox
-lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
-3 file(s) found
-```
-
-#### Extract
-
-```
-usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
-
-Extract files from the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-  -d DEST, --dest DEST         destination directory. Default: next to file
-  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
-  -f, --force                  overwrite files that already exist. Default: False
-  -q, --quiet                  don't print extraction status. Default: False
-```
-
-On Linux, just like `cramfsck -x` you need to run as root
-if you want to preserve file mode, owner and group.
-
-On Windows, the only reason to run as a privileged user is to be able to create
-symlinks.
-Unprivileged accounts can create symlinks if Developer Mode is enabled.
-Otherwise, a regular file containing the target will be created.
-Special files will always just be empty files.
-
-#### Check
-
-This command is similar to running `cramfsck -c file` but is not as thorough.
-
-```
-usage: pycramfs check [-h] [-o OFFSET] file
-
-Make a few superficial checks of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-```
-
-## References
-
-- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
-- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
-- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
-- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
+# pycramfs
+
+<p align="left">
+<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
+<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
+<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
+</p>
+
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Usage](#usage)
+* [References](#references)
+
+A library and tool to read and extract cramfs images.
+
+It is far from being as complete as the tools it's based on,
+but should be enough for simple images.
+For example, as of right now it only supports contiguous data layout.
+Only little endian images are supported.
+
+It also provides ways to extract data from an image,
+although you might prefer using
+[`cramfsck`](https://github.com/npitre/cramfs-tools)
+on Linux and 7-Zip on Windows for better compatibility.
+
+## Requirements
+
+Python 3.8+.
+
+## Installation
+
+```
+pip install pycramfs
+```
+
+## Usage
+
+### API
+
+Here's an overview of what you can do:
+```py
+from pycramfs import Cramfs
+from pycramfs.extract import extract_dir, extract_file
+from pycramfs.util import find_superblocks
+
+fsimage = "cramfs.bin"
+superblocks = find_superblocks(fsimage)
+
+with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
+    # Optional offset for start of file system.
+    # You can also create Cramfs instances from bytes or a file descriptor.
+
+    sblock = cramfs.super  # Access the file system's superblock
+    print(sblock.name)
+    print(dict(sblock))  # Superblock as a dictionary
+    assert cramfs.calculate_crc() == sblock.fsid.crc
+
+    rootdir = cramfs.rootdir  # root directory
+    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
+    # Number of files in the whole file system (shortcut to sblock.fsid.files).
+    print(len(cramfs))
+    print("/etc/passwd" in cramfs)  # Check if path exists
+
+    # Iterate over the whole file system.
+    for file in cramfs:
+        print(file.parent)  # Instance of Directory (None for the root directory)
+        print(file in cramfs)  # Check if file belongs to this image
+        if file.is_symlink:  # Check the file's type
+            print(file.readlink())  # Symlink target
+
+    etc = cramfs.select("/etc")  # Select a specific file or directory
+    etc = cramfs.select("etc")  # Can also be a relative path
+    rootdir = etc.select("..")  # And a special entry
+    assert rootdir == rootdir.select('.')
+    print(etc)  # print the file or directory's name
+    # The file or directory's absolute path (an instance of PurePosixPath).
+    print(etc.path)
+    print(etc.files)  # A dictionary mapping file names to File instances
+    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
+    print(etc.total)  # Number of entries in this whole subtree
+    # A list of this directory's children (shortcut to list(etc.files.values())).
+    print(list(etc))
+
+    # Find the first file in this subtree that has this name.
+    passwd = cramfs.find("passwd")
+    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
+    passwd = etc["passwd"]
+    print("passwd" in etc)  # Check if directory contains this file
+    print(passwd in etc)  # Also works with instances of File
+
+    # Iterate over this directory's files.
+    for file in etc:
+        print(file.inode)  # Access inode information
+        # These attributes are shortcuts to file.inode.<attr>
+        print(file.mode)
+        print(file.uid)
+        print(file.size)
+        print(file.gid)
+
+    # Iterate over this whole subtree.
+    for file in etc.riter():
+        print(file.name)  # File name, equivalent to file.path.name
+        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
+    
+    # Iterate over files in the subtree that match a pattern.
+    for config_file in etc.itermatch("*.conf"):
+        print(config_file.read_bytes())  # Read the file's raw content
+        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
+
+    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
+
+    # You can use absolute paths from any directory.
+    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
+    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
+
+    # Calling find(), select() and itermatch() on cramfs
+    # is the same as calling them on cramfs.rootdir.
+
+    extract_dir(etc, "extract/etc")  # Extract a directory tree
+    extract_file(passwd, "extract/passwd")  # Extract a single file
+```
+
+### Command line
+
+pycramfs comes with a command-line interface that consists of 4 sub-commands.
+
+#### Info
+
+```
+usage: pycramfs info [-h] file
+
+Show information about all the superblocks that can be found in a file
+
+positional arguments:
+  file
+```
+
+Example output:
+```
+$ pycramfs info cramfs.bin
+Superblock #1
+Magic:     0x28CD3D45
+Size:      282,624
+Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
+Future:    0
+Signature: Compressed ROMFS
+Name:      Compressed
+CRC:       0xDEADBEEF
+Edition:   0
+Blocks:    6,926
+Files:     420
+Offset:    8157
+```
+
+#### List
+
+```
+usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
+
+List the contents of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
+  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
+  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
+                                  filter by file type with f, d, l, p, s, b, c
+```
+
+Example that lists only directories and symlinks that match a pattern:
+```
+$ pycramfs list cramfs.bin -t d l -p "*bin*"
+drwxrwxr-x      256   123:0   /bin 
+lrwxrwxrwx        7   123:0   /bin/ash -> busybox
+lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
+3 file(s) found
+```
+
+#### Extract
+
+```
+usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
+
+Extract files from the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+  -d DEST, --dest DEST         destination directory. Default: next to file
+  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
+  -f, --force                  overwrite files that already exist. Default: False
+  -q, --quiet                  don't print extraction status. Default: False
+```
+
+On Linux, just like `cramfsck -x` you need to run as root
+if you want to preserve file mode, owner and group.
+
+On Windows, the only reason to run as a privileged user is to be able to create
+symlinks.
+Unprivileged accounts can create symlinks if Developer Mode is enabled.
+Otherwise, a regular file containing the target will be created.
+Special files will always just be empty files.
+
+#### Check
+
+This command is similar to running `cramfsck -c file` but is not as thorough.
+
+```
+usage: pycramfs check [-h] [-o OFFSET] file
+
+Make a few superficial checks of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+```
+
+## References
+
+- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
+- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
+- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
+- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
```

### Comparing `pycramfs-1.0.0/pycramfs/__main__.py` & `pycramfs-1.1.0/pycramfs/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import argparse
-from pathlib import Path, PurePosixPath
-
-from pycramfs import Cramfs, __version__
-from pycramfs.const import PAGE_SIZE
-from pycramfs.exception import CramfsError
-from pycramfs.extract import extract_dir, extract_file
-from pycramfs.file import filetype
-from pycramfs.util import _print, find_superblocks
-
-
-def print_file(file):
-    # Max file size is 2**24-1 or 16777215 -> 8 characters.
-    # Max UID is 2**16-1 or 65535 -> 5 characters.
-    # Max GID is 2**8-1 or 255 -> 3 characters.
-    link = f"-> {file.readlink()}" if file.is_symlink else ''
-    print(file.filemode, f"{file.size:8} {file.uid:5}:{file.gid:<3}", file.path, link)
-
-
-def list_(args):
-    if (types := args.type) is not None:
-        types = set(''.join(types).replace('f', '-'))
-    count = 0
-    with Cramfs.from_file(args.file, args.offset) as cramfs:
-        if args.pattern is None:
-            it = cramfs
-        else:
-            it = cramfs.itermatch(args.pattern)
-        if types is None:
-            for file in it:
-                print_file(file)
-                count += 1
-        else:
-            for file in it:
-                if file.filemode[0] in types:
-                    print_file(file)
-                    count += 1
-    print(f"{count} file(s) found")
-
-
-def info(args):
-    width = 10
-    superblocks = find_superblocks(args.file)
-    if not superblocks:
-        print("No superblock found")
-        return
-    for idx, superblock in enumerate(superblocks):
-        super = argparse.Namespace(**superblock)
-        fsid = argparse.Namespace(**super.fsid)
-        print(f"Superblock #{idx + 1}")
-        print(f"{'Magic:':{width}} 0x{super.magic:X}")
-        print(f"{'Size:':{width}} {super.size:,}")
-        print(f"{'Flags:':{width}} {super.flags!r}")
-        print(f"{'Future:':{width}} {super.future}")
-        print(f"{'Signature:':{width}} {super.signature}")
-        print(f"{'Name:':{width}} {super.name}")
-        print(f"{'CRC:':{width}} 0x{fsid.crc:08X}")
-        print(f"{'Edition:':{width}} {fsid.edition}")
-        print(f"{'Blocks:':{width}} {fsid.blocks:,}")
-        print(f"{'Files:':{width}} {fsid.files:,}")
-        print(f"{'Offset:':{width}} {super.offset}")
-        if idx != len(superblocks) - 1:
-            print()
-
-
-def extract(args):
-    dest = args.dest
-    with Cramfs.from_file(args.file, args.offset) as cramfs:
-        file = cramfs.select(args.path)
-        if file is None:
-            raise CramfsError(f"{args.path} not found")
-        elif file.is_dir:
-            if dest is None:
-                dest = args.file.with_name(args.file.stem)
-            amount = extract_dir(file, dest, args.force, args.quiet)
-        else:
-            if dest is None:
-                dest = args.file.parent / file.name
-            amount = extract_file(file, dest, args.force, args.quiet)
-    _print(f"{int(amount)} file(s) extracted to {dest.resolve()}", quiet=args.quiet)
-
-
-def check(args):
-    with Cramfs.from_file(args.file, args.offset) as cramfs:
-        for file in cramfs:
-            if file.inode.namelen == 0 and str(file.path) != '/':
-                print("filename length is zero", file.path)
-            offset = file.inode.offset
-            if file.is_dir:
-                if offset == 0 and file.size != 0:
-                    print("directory inode has zero offset and non-zero size:", file.path)
-            elif file.is_file:
-                if offset == 0 and file.size != 0:
-                    print("file inode has zero offset and non-zero size", file.path)
-                if file.size == 0 and offset != 0:
-                    print("file inode has zero size and non-zero offset", file.path)
-            elif file.is_symlink:
-                if offset == 0:
-                    print("symbolic link has zero offset", file.path)
-                if file.size == 0:
-                    print("symbolic link has zero size", file.path)
-            else:
-                if offset != 0:
-                    print("special file has non-zero offset:", file.path)
-                if file.is_char_device or file.is_block_device:
-                    pass
-                elif file.is_fifo or file.is_socket:
-                    typ = "fifo" if file.is_fifo else "socket"
-                    if file.size != 0:
-                        print(f"{typ} has non-zero size: {file.path}")
-                else:
-                    print(f"bogus mode: {file.path} ({file.mode:o})")
-
-
-def main():
-    filetypes = list(''.join(filetype).replace('-', 'f'))
-
-    pfile = argparse.ArgumentParser(add_help=False)
-    pfile.add_argument("file", type=Path)
-
-    poffset = argparse.ArgumentParser(add_help=False)
-    poffset.add_argument("-o", "--offset", type=int, default=0, help="absolute position of file system's start. Default: %(default)s")
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {__version__}")
-    subparsers = parser.add_subparsers(required=True, dest="command")  # dest is only here to avoid a TypeError in Python 3.8 (see bpo-29298)
-
-    helplist = "List the contents of the file system"
-    parser_l = subparsers.add_parser("list", parents=[pfile, poffset], help=helplist.lower(), description=helplist)
-    parser_l.add_argument("-p", "--pattern", help="filter by file name pattern with fnmatch")
-    parser_l.add_argument("-t", "--type", nargs='+', metavar="TYPE", choices=filetypes, help="filter by file type with %(choices)s")
-    parser_l.set_defaults(func=list_)
-
-    helpinfo = "Show information about all the superblocks that can be found in a file"
-    parser_i = subparsers.add_parser("info", parents=[pfile], help=helpinfo.lower(), description=helpinfo)
-    parser_i.set_defaults(func=info)
-
-    helpextr = "Extract files from the file system"
-    parser_e = subparsers.add_parser("extract", parents=[pfile, poffset], help=helpextr.lower(), description=helpextr)
-    parser_e.add_argument("-d", "--dest", type=Path, help="destination directory. Default: next to file")
-    parser_e.add_argument("-p", "--path", type=PurePosixPath, default='/', help="absolute path of directory or file to extract. Default: %(default)r")
-    parser_e.add_argument("-f", "--force", action="store_true", help="overwrite files that already exist. Default: %(default)s")
-    parser_e.add_argument("-q", "--quiet", action="store_true", help="don't print extraction status. Default: %(default)s")
-    parser_e.set_defaults(func=extract)
-
-    helpchck = "Make a few superficial checks of the file system"
-    parser_c = subparsers.add_parser("check", parents=[pfile, poffset], help=helpchck.lower(), description=helpchck)
-    parser_c.set_defaults(func=check)
-
-    args = parser.parse_args()
-    if not args.file.exists():
-        parser.error("file does not exist")
-    if "offset" in args and args.offset is not None:
-        if args.offset < 0:
-            parser.error("offset cannot be negative")
-        if (args.file.stat().st_size - args.offset) < PAGE_SIZE:
-            parser.error("a cramfs image can't fit at this offset")
-    try:
-        args.func(args)
-    except Exception as e:
-        parser.error(repr(e))
-
-
-if __name__ == "__main__":
-    main()
+from argparse import ArgumentParser, Namespace
+from pathlib import Path, PurePosixPath
+
+from pycramfs import Cramfs, __version__
+from pycramfs.const import PAGE_SIZE
+from pycramfs.exception import CramfsError
+from pycramfs.extract import extract_dir, extract_file
+from pycramfs.file import Directory, File, Symlink, filetype
+from pycramfs.util import find_superblocks, printq
+
+
+def print_file(file: File) -> None:
+    # Max file size is 2**24-1 or 16777215 -> 8 characters.
+    # Max UID is 2**16-1 or 65535 -> 5 characters.
+    # Max GID is 2**8-1 or 255 -> 3 characters.
+    link = f"-> {file.readlink()}" if isinstance(file, Symlink) else ''
+    print(file.filemode, f"{file.size:8} {file.uid:5}:{file.gid:<3}", file.path, link)
+
+
+def list_(args: Namespace) -> None:
+    if (types := args.type) is not None:
+        types = set(''.join(types).replace('f', '-'))
+    count = 0
+    with Cramfs.from_file(args.file, args.offset) as cramfs:
+        if args.pattern is None:
+            it = cramfs
+        else:
+            it = cramfs.itermatch(args.pattern)
+        if types is None:
+            for file in it:
+                print_file(file)
+                count += 1
+        else:
+            for file in it:
+                if file.filemode[0] in types:
+                    print_file(file)
+                    count += 1
+    print(f"{count} file(s) found")
+
+
+def info(args: Namespace) -> None:
+    width = 10
+    superblocks = find_superblocks(args.file)
+    if not superblocks:
+        print("No superblock found")
+        return
+    for idx, superblock in enumerate(superblocks):
+        super = Namespace(**superblock)
+        fsid = Namespace(**super.fsid)
+        print(f"Superblock #{idx + 1}")
+        print(f"{'Magic:':{width}} 0x{super.magic:X}")
+        print(f"{'Size:':{width}} {super.size:,}")
+        print(f"{'Flags:':{width}} {super.flags!r}")
+        print(f"{'Future:':{width}} {super.future}")
+        print(f"{'Signature:':{width}} {super.signature}")
+        print(f"{'Name:':{width}} {super.name}")
+        print(f"{'CRC:':{width}} 0x{fsid.crc:08X}")
+        print(f"{'Edition:':{width}} {fsid.edition}")
+        print(f"{'Blocks:':{width}} {fsid.blocks:,}")
+        print(f"{'Files:':{width}} {fsid.files:,}")
+        print(f"{'Offset:':{width}} {super.offset}")
+        if idx != len(superblocks) - 1:
+            print()
+
+
+def extract(args: Namespace) -> None:
+    dest = args.dest
+    with Cramfs.from_file(args.file, args.offset) as cramfs:
+        file = cramfs.select(args.path)
+        if file is None:
+            raise CramfsError(f"{args.path} not found")
+        elif isinstance(file, Directory):
+            if dest is None:
+                dest = args.file.with_name(args.file.stem)
+            amount = extract_dir(file, dest, args.force, args.quiet)
+        else:
+            if dest is None:
+                dest = args.file.parent / file.name
+            amount = extract_file(file, dest, args.force, args.quiet)
+    printq(f"{int(amount)} file(s) extracted to {dest.resolve()}", quiet=args.quiet)
+
+
+def check(args: Namespace) -> None:
+    with Cramfs.from_file(args.file, args.offset) as cramfs:
+        for file in cramfs:
+            if file.inode.namelen == 0 and str(file.path) != '/':
+                print("filename length is zero", file.path)
+            offset = file.inode.offset
+            if file.is_dir:
+                if offset == 0 and file.size != 0:
+                    print("directory inode has zero offset and non-zero size:", file.path)
+            elif file.is_file:
+                if offset == 0 and file.size != 0:
+                    print("file inode has zero offset and non-zero size", file.path)
+                if file.size == 0 and offset != 0:
+                    print("file inode has zero size and non-zero offset", file.path)
+            elif file.is_symlink:
+                if offset == 0:
+                    print("symbolic link has zero offset", file.path)
+                if file.size == 0:
+                    print("symbolic link has zero size", file.path)
+            else:
+                if offset != 0:
+                    print("special file has non-zero offset:", file.path)
+                if file.is_char_device or file.is_block_device:
+                    pass
+                elif file.is_fifo or file.is_socket:
+                    typ = "fifo" if file.is_fifo else "socket"
+                    if file.size != 0:
+                        print(f"{typ} has non-zero size: {file.path}")
+                else:
+                    print(f"bogus mode: {file.path} ({file.mode:o})")
+
+
+def main():
+    filetypes = list(''.join(filetype).replace('-', 'f'))
+
+    pfile = ArgumentParser(add_help=False)
+    pfile.add_argument("file", type=Path)
+
+    poffset = ArgumentParser(add_help=False)
+    poffset.add_argument("-o", "--offset", type=int, default=0, help="absolute position of file system's start. Default: %(default)s")
+
+    parser = ArgumentParser()
+    parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {__version__}")
+    subparsers = parser.add_subparsers(required=True, dest="command")  # dest is only here to avoid a TypeError in Python 3.8 (see bpo-29298)
+
+    helplist = "List the contents of the file system"
+    parser_l = subparsers.add_parser("list", parents=[pfile, poffset], help=helplist.lower(), description=helplist)
+    parser_l.add_argument("-p", "--pattern", help="filter by file name pattern with fnmatch")
+    parser_l.add_argument("-t", "--type", nargs='+', metavar="TYPE", choices=filetypes, help="filter by file type with %(choices)s")
+    parser_l.set_defaults(func=list_)
+
+    helpinfo = "Show information about all the superblocks that can be found in a file"
+    parser_i = subparsers.add_parser("info", parents=[pfile], help=helpinfo.lower(), description=helpinfo)
+    parser_i.set_defaults(func=info)
+
+    helpextr = "Extract files from the file system"
+    parser_e = subparsers.add_parser("extract", parents=[pfile, poffset], help=helpextr.lower(), description=helpextr)
+    parser_e.add_argument("-d", "--dest", type=Path, help="destination directory. Default: next to file")
+    parser_e.add_argument("-p", "--path", type=PurePosixPath, default='/', help="absolute path of directory or file to extract. Default: %(default)r")
+    parser_e.add_argument("-f", "--force", action="store_true", help="overwrite files that already exist. Default: %(default)s")
+    parser_e.add_argument("-q", "--quiet", action="store_true", help="don't print extraction status. Default: %(default)s")
+    parser_e.set_defaults(func=extract)
+
+    helpchck = "Make a few superficial checks of the file system"
+    parser_c = subparsers.add_parser("check", parents=[pfile, poffset], help=helpchck.lower(), description=helpchck)
+    parser_c.set_defaults(func=check)
+
+    args = parser.parse_args()
+    if not args.file.exists():
+        parser.error("file does not exist")
+    if "offset" in args and args.offset is not None:
+        if args.offset < 0:
+            parser.error("offset cannot be negative")
+        if (args.file.stat().st_size - args.offset) < PAGE_SIZE:
+            parser.error("a cramfs image can't fit at this offset")
+    try:
+        args.func(args)
+    except Exception as e:
+        parser.error(repr(e))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pycramfs-1.0.0/pycramfs/file.py` & `pycramfs-1.1.0/pycramfs/file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,316 +1,337 @@
-import fnmatch
-import struct
-import zlib
-from pathlib import PurePosixPath
-
-from pycramfs.const import BLK_FLAGS, BLK_PTR_FMT, PAGE_SIZE, BlockFlag
-from pycramfs.exception import CramfsError
-from pycramfs.structure import Inode
-
-
-class File:
-    """Abstract base class for files."""
-
-    def __init__(self, fd, image, inode: Inode, name: bytes, parent=None):
-        self._fd = fd
-        self._image = image
-        self._inode = inode
-        self._name = name
-        self._parent = parent
-
-    def __str__(self):
-        return self.name
-
-    def __repr__(self):
-        return f"{self.__class__.__qualname__}({self.name!r})"
-
-    def __lt__(self, other):
-        if not isinstance(other, File):
-            return NotImplemented
-        return self._name < other._name
-
-    def __le__(self, other):
-        if not isinstance(other, File):
-            return NotImplemented
-        return self._name <= other._name
-
-    @property
-    def image(self):
-        return self._image
-
-    @property
-    def inode(self) -> Inode:
-        return self._inode
-
-    @property
-    def name(self) -> str:
-        return self._name.decode()
-
-    @property
-    def parent(self):
-        return self._parent
-
-    @property
-    def path(self) -> PurePosixPath:
-        """Return the file's absolute path."""
-        if self._parent is None:
-            return PurePosixPath('/')
-        return self._parent.path / self.name
-
-    @property
-    def mode(self) -> int:
-        return self._inode.mode
-
-    @property
-    def uid(self) -> int:
-        return self._inode.uid
-
-    @property
-    def size(self) -> int:
-        """Return the size attribute of this file's inode.
-
-        - regular file: uncompressed file size in bytes
-        - directory: sum(inode.namelen + sizeof(Inode) for each child inode)
-        - symlink: uncompressed target path size in bytes
-        - device file: i_rdev (device number, major and minor)
-        - FIFO and socket should be 0
-        """
-        return self._inode.size
-
-    @property
-    def gid(self) -> int:
-        return self._inode.gid
-
-    @property
-    def filemode(self) -> str:
-        return self._inode.filemode
-
-    @property
-    def is_dir(self):
-        return False
-
-    @property
-    def is_file(self):
-        return False
-
-    @property
-    def is_symlink(self):
-        return False
-
-    @property
-    def is_block_device(self):
-        return False
-
-    @property
-    def is_char_device(self):
-        return False
-
-    @property
-    def is_fifo(self):
-        return False
-
-    @property
-    def is_socket(self):
-        return False
-
-
-class Directory(File):
-
-    def __init__(self, fd, image, inode: Inode, name: bytes = b'', parent=None, files=None):
-        super().__init__(fd, image, inode, name, parent)
-        self._files = files if files is not None else {}
-        self._total = None
-
-    def __len__(self):
-        return len(self._files)
-
-    def __iter__(self):
-        return self.iterdir()
-
-    def __getitem__(self, key):
-        return self._files[key]
-
-    def __contains__(self, item):
-        if isinstance(item, str):
-            return item in self._files
-        elif isinstance(item, File):
-            return item in self._files.values()
-        return False
-
-    def __reversed__(self):
-        for filename in reversed(self._files):
-            yield self._files[filename]
-
-    @property
-    def is_dir(self):
-        return True
-
-    @property
-    def files(self):
-        return self._files
-
-    @property
-    def total(self):
-        """Return the total amount of files in this subtree."""
-        if self._total is None:
-            self._total = len(self) + sum(child.total for child in self._files.values() if child.is_dir)
-        return self._total
-
-    def iterdir(self):
-        for file in self._files.values():
-            yield file
-
-    def riter(self):
-        """Iterate over this directory recursively."""
-        yield self
-        for file in self._files.values():
-            if file.is_dir:
-                for f in file.riter():
-                    yield f
-            else:
-                yield file
-
-    def find(self, filename):
-        """Find a file of any kind anywhere under this directory."""
-        filename = PurePosixPath(filename).name
-        for file in self.riter():
-            if file.name == filename:
-                return file
-        return None
-
-    def select(self, path):
-        """Select a file of any kind by path.
-
-        The path can be absolute or relative.
-        Special entries `'.'` and `'..'` are supported.
-        """
-        path = PurePosixPath(path)
-        if str(path) == "..":
-            return self.parent if self.parent is not None else self
-        if path.root == '/':
-            if str(self.path) == '/':
-                path = path.relative_to('/')
-            else:
-                return self._image.rootdir.select(path)
-        if str(path) == '.':
-            return self
-        child, *descendants = path.parts
-        if (file := self._files.get(child, None)) is not None:
-            if file.is_dir and descendants:
-                return file.select(PurePosixPath(*descendants))
-            else:
-                return file
-        return None
-
-    def itermatch(self, pattern):
-        """Iterate over files in this subtree that (fn)match the pattern."""
-        # We must use str() here because filter doesn't call normcase on Posix.
-        if str(self.path) == '/':
-            paths = (str(file.path) for file in self.riter())
-        else:
-            paths = (str(file.path.relative_to(self.path)) for file in self.riter())
-        for path in fnmatch.filter(paths, pattern):
-            yield self.select(path)
-
-    @classmethod
-    def from_fd(cls, fd, image, inode: Inode, name: bytes = b''):
-        self = cls(fd, image, inode, name)
-        if inode.offset == 0:  # Empty dir
-            return self
-        fd.seek(inode.offset)
-        end = inode.size + inode.offset
-        children = []
-        while fd.tell() != end:
-            ino = Inode.from_fd(fd)
-            name = fd.read(ino.namelen).rstrip(b'\x00')
-            children.append((ino, name))
-        for ino, name in children:
-            if ino.is_dir:
-                file = Directory.from_fd(fd, image, ino, name)
-                file._parent = self
-            else:
-                cls = filetype[ino.filemode[0]]
-                file = cls(fd, image, ino, name, self)
-            self._files[name.decode()] = file
-        return self
-
-
-class DataFile(File):
-
-    def read_bytes(self) -> bytes:
-        """Read blocks and decompress them if necessary."""
-        maxblock = (self._inode.size + PAGE_SIZE - 1) // PAGE_SIZE
-        self._fd.seek(self._inode.offset)
-        block_pointers = self._fd.read(struct.calcsize(BLK_PTR_FMT) * maxblock)
-        content = b''
-        for block_ptr, *_ in struct.iter_unpack(BLK_PTR_FMT, block_pointers):
-            uncompressed = block_ptr & BlockFlag.UNCOMPRESSED
-            direct = block_ptr & BlockFlag.DIRECT_PTR
-            if direct:
-                raise CramfsError("Only contiguous data layout supported")
-            block_ptr &= ~BLK_FLAGS  # Remove potential block pointer flags
-            block_len = block_ptr - self._fd.tell()
-            data = self._fd.read(block_len)
-            if not uncompressed:
-                data = zlib.decompress(data)
-            content += data
-        return content
-
-    def read_text(self, encoding="utf8", errors="strict") -> str:
-        return self.read_bytes().decode(encoding, errors)
-
-
-class RegularFile(DataFile):
-
-    @property
-    def is_file(self):
-        return True
-
-
-class Symlink(DataFile):
-
-    @property
-    def is_symlink(self):
-        return True
-
-    def readlink(self):
-        return PurePosixPath(self.read_text())
-
-
-class FIFO(File):
-
-    @property
-    def is_fifo(self):
-        return True
-
-
-class Socket(File):
-
-    @property
-    def is_socket(self):
-        return True
-
-
-class CharacterDevice(File):
-
-    @property
-    def is_char_device(self):
-        return True
-
-
-class BlockDevice(File):
-
-    @property
-    def is_block_device(self):
-        return True
-
-
-filetype = {
-    '-': RegularFile,
-    'd': Directory,
-    'l': Symlink,
-    'p': FIFO,
-    's': Socket,
-    'b': BlockDevice,
-    'c': CharacterDevice
-}
+from __future__ import annotations
+
+import fnmatch
+import struct
+import zlib
+from pathlib import PurePosixPath
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Optional, Tuple
+
+from pycramfs.const import BLK_FLAGS, BLK_PTR_FMT, PAGE_SIZE, BlockFlag
+from pycramfs.exception import CramfsError
+from pycramfs.structure import Inode
+
+if TYPE_CHECKING:
+    from pycramfs import Cramfs
+    from pycramfs.types import ByteStream, StrPath
+
+
+class File:
+    """Abstract base class for files."""
+
+    def __init__(
+        self,
+        fd: ByteStream,
+        image: Cramfs,
+        inode: Inode,
+        name: bytes,
+        parent: Optional[Directory] = None
+    ) -> None:
+        self._fd = fd
+        self._image = image
+        self._inode = inode
+        self._name = name
+        self._parent = parent
+
+    def __str__(self) -> str:
+        return self.name
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__qualname__}({self.name!r})"
+
+    def __lt__(self, other: Any) -> bool:
+        if not isinstance(other, File):
+            return NotImplemented
+        return self._name < other._name
+
+    def __le__(self, other: Any) -> bool:
+        if not isinstance(other, File):
+            return NotImplemented
+        return self._name <= other._name
+
+    @property
+    def image(self) -> Cramfs:
+        return self._image
+
+    @property
+    def inode(self) -> Inode:
+        return self._inode
+
+    @property
+    def name(self) -> str:
+        return self._name.decode()
+
+    @property
+    def parent(self) -> Optional[Directory]:
+        return self._parent
+
+    @property
+    def path(self) -> PurePosixPath:
+        """Return the file's absolute path."""
+        if self._parent is None:
+            return PurePosixPath('/')
+        return self._parent.path / self.name
+
+    @property
+    def mode(self) -> int:
+        return self._inode.mode
+
+    @property
+    def uid(self) -> int:
+        return self._inode.uid
+
+    @property
+    def size(self) -> int:
+        """Return the size attribute of this file's inode.
+
+        - regular file: uncompressed file size in bytes
+        - directory: sum(inode.namelen + sizeof(Inode) for each child inode)
+        - symlink: uncompressed target path size in bytes
+        - device file: i_rdev (device number, major and minor)
+        - FIFO and socket should be 0
+        """
+        return self._inode.size
+
+    @property
+    def gid(self) -> int:
+        return self._inode.gid
+
+    @property
+    def filemode(self) -> str:
+        return self._inode.filemode
+
+    @property
+    def is_dir(self) -> bool:
+        return False
+
+    @property
+    def is_file(self) -> bool:
+        return False
+
+    @property
+    def is_symlink(self) -> bool:
+        return False
+
+    @property
+    def is_block_device(self) -> bool:
+        return False
+
+    @property
+    def is_char_device(self) -> bool:
+        return False
+
+    @property
+    def is_fifo(self) -> bool:
+        return False
+
+    @property
+    def is_socket(self) -> bool:
+        return False
+
+
+class Directory(File):
+
+    def __init__(
+        self,
+        fd: ByteStream,
+        image: Cramfs,
+        inode: Inode,
+        name: bytes = b'',
+        parent: Optional[Directory] = None,
+        files: Optional[Dict[str, File]] = None
+    ) -> None:
+        super().__init__(fd, image, inode, name, parent)
+        self._files = files if files is not None else {}
+        self._total = None
+
+    def __len__(self) -> int:
+        return len(self._files)
+
+    def __iter__(self) -> Iterator[File]:
+        yield from self.iterdir()
+
+    def __getitem__(self, key: str) -> File:
+        return self._files[key]
+
+    def __contains__(self, item: Any) -> bool:
+        if isinstance(item, str):
+            return item in self._files
+        elif isinstance(item, File):
+            return item in self._files.values()
+        return False
+
+    def __reversed__(self) -> Iterator[File]:
+        for filename in reversed(self._files):
+            yield self._files[filename]
+
+    @property
+    def is_dir(self) -> Literal[True]:
+        return True
+
+    @property
+    def files(self) -> Dict[str, File]:
+        return self._files
+
+    @property
+    def total(self) -> int:
+        """Return the total amount of files in this subtree."""
+        if self._total is None:
+            self._total = len(self) + sum(child.total for child in self._files.values() if isinstance(child, Directory))
+        return self._total
+
+    def iterdir(self) -> Iterator[File]:
+        yield from self._files.values()
+
+    def riter(self) -> Iterator[File]:
+        """Iterate over this directory recursively."""
+        yield self
+        for file in self._files.values():
+            if isinstance(file, Directory):
+                yield from file.riter()
+            else:
+                yield file
+
+    def find(self, filename: StrPath) -> Optional[File]:
+        """Find a file of any kind anywhere under this directory."""
+        filename = PurePosixPath(filename).name
+        for file in self.riter():
+            if file.name == filename:
+                return file
+        return None
+
+    def select(self, path: StrPath) -> Optional[File]:
+        """Select a file of any kind by path.
+
+        The path can be absolute or relative.
+        Special entries `'.'` and `'..'` are supported.
+        """
+        path = PurePosixPath(path)
+        if str(path) == "..":
+            return self.parent if self.parent is not None else self
+        if path.root == '/':
+            if str(self.path) == '/':
+                path = path.relative_to('/')
+            else:
+                return self._image.rootdir.select(path)
+        if str(path) == '.':
+            return self
+        child, *descendants = path.parts
+        if (file := self._files.get(child, None)) is not None:
+            if isinstance(file, Directory) and descendants:
+                return file.select(PurePosixPath(*descendants))
+            elif not descendants:
+                return file
+        return None
+
+    def itermatch(self, pattern: str) -> Iterator[File]:
+        """Iterate over files in this subtree that (fn)match the pattern."""
+        # We must use str() here because filter doesn't call normcase on Posix.
+        if str(self.path) == '/':
+            paths = (str(file.path) for file in self.riter())
+        else:
+            paths = (str(file.path.relative_to(self.path)) for file in self.riter())
+        for path in fnmatch.filter(paths, pattern):
+            yield self.select(path)  # type: ignore
+
+    @classmethod
+    def from_fd(cls, fd: ByteStream, image: Cramfs, inode: Inode, name: bytes = b'') -> Directory:
+        self = cls(fd, image, inode, name)
+        if inode.offset == 0:  # Empty dir
+            return self
+        fd.seek(inode.offset)
+        end = inode.size + inode.offset
+        children: List[Tuple[Inode, bytes]] = []
+        while fd.tell() != end:
+            ino = Inode.from_fd(fd)
+            name = fd.read(ino.namelen).rstrip(b'\x00')
+            children.append((ino, name))
+        for ino, name in children:
+            if ino.is_dir:
+                file = Directory.from_fd(fd, image, ino, name)
+                file._parent = self
+            else:
+                cls = filetype[ino.filemode[0]]
+                file = cls(fd, image, ino, name, self)
+            self._files[name.decode()] = file
+        return self
+
+
+class DataFile(File):
+
+    def iter_bytes(self) -> Iterator[bytes]:
+        """Read blocks and decompress them if necessary."""
+        maxblock = (self._inode.size + PAGE_SIZE - 1) // PAGE_SIZE
+        self._fd.seek(self._inode.offset)
+        block_pointers = self._fd.read(struct.calcsize(BLK_PTR_FMT) * maxblock)
+        for block_ptr, *_ in struct.iter_unpack(BLK_PTR_FMT, block_pointers):
+            uncompressed = block_ptr & BlockFlag.UNCOMPRESSED
+            direct = block_ptr & BlockFlag.DIRECT_PTR
+            if direct:
+                raise CramfsError("Only contiguous data layout supported")
+            block_ptr &= ~BLK_FLAGS  # Remove potential block pointer flags
+            block_len = block_ptr - self._fd.tell()
+            data = self._fd.read(block_len)
+            if not uncompressed:
+                data = zlib.decompress(data)
+            yield data
+
+    def read_bytes(self) -> bytes:
+        return b''.join(self.iter_bytes())
+
+    def read_text(self, encoding: str = "utf8", errors: str = "strict") -> str:
+        return self.read_bytes().decode(encoding, errors)
+
+
+class RegularFile(DataFile):
+
+    @property
+    def is_file(self) -> Literal[True]:
+        return True
+
+
+class Symlink(DataFile):
+
+    @property
+    def is_symlink(self) -> Literal[True]:
+        return True
+
+    def readlink(self) -> PurePosixPath:
+        return PurePosixPath(self.read_text())
+
+
+class FIFO(File):
+
+    @property
+    def is_fifo(self) -> Literal[True]:
+        return True
+
+
+class Socket(File):
+
+    @property
+    def is_socket(self) -> Literal[True]:
+        return True
+
+
+class CharacterDevice(File):
+
+    @property
+    def is_char_device(self) -> Literal[True]:
+        return True
+
+
+class BlockDevice(File):
+
+    @property
+    def is_block_device(self) -> Literal[True]:
+        return True
+
+
+filetype = {
+    '-': RegularFile,
+    'd': Directory,
+    'l': Symlink,
+    'p': FIFO,
+    's': Socket,
+    'b': BlockDevice,
+    'c': CharacterDevice
+}
```

### Comparing `pycramfs-1.0.0/pycramfs.egg-info/PKG-INFO` & `pycramfs-1.1.0/pycramfs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,257 +1,258 @@
-Metadata-Version: 2.1
-Name: pycramfs
-Version: 1.0.0
-Summary: Read and extract cramfs images.
-Author-email: AT0myks <at0myks.dev@gmail.com>
-Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
-Project-URL: Source, https://github.com/AT0myks/pycramfs
-Keywords: cramfs,filesystem
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Filesystems
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pycramfs
-
-<p align="left">
-<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
-<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
-<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
-</p>
-
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Usage](#usage)
-* [References](#references)
-
-A library and tool to read and extract cramfs images.
-
-It is far from being as complete as the tools it's based on,
-but should be enough for simple images.
-For example, as of right now it only supports contiguous data layout.
-Only little endian images are supported.
-
-It also provides ways to extract data from an image,
-although you might prefer using
-[`cramfsck`](https://github.com/npitre/cramfs-tools)
-on Linux and 7-Zip on Windows for better compatibility.
-
-## Requirements
-
-Python 3.8+.
-
-## Installation
-
-```
-pip install pycramfs
-```
-
-## Usage
-
-### API
-
-Here's an overview of what you can do:
-```py
-from pycramfs import Cramfs
-from pycramfs.extract import extract_dir, extract_file
-from pycramfs.util import find_superblocks
-
-fsimage = "cramfs.bin"
-superblocks = find_superblocks(fsimage)
-
-with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
-    # Optional offset for start of file system.
-    # You can also create Cramfs instances from bytes or a file descriptor.
-
-    sblock = cramfs.super  # Access the file system's superblock
-    print(sblock.name)
-    print(dict(sblock))  # Superblock as a dictionary
-    assert cramfs.calculate_crc() == sblock.fsid.crc
-
-    rootdir = cramfs.rootdir  # root directory
-    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
-    # Number of files in the whole file system (shortcut to sblock.fsid.files).
-    print(len(cramfs))
-    print("/etc/passwd" in cramfs)  # Check if path exists
-
-    # Iterate over the whole file system.
-    for file in cramfs:
-        print(file.parent)  # Instance of Directory (None for the root directory)
-        print(file in cramfs)  # Check if file belongs to this image
-        if file.is_symlink:  # Check the file's type
-            print(file.readlink())  # Symlink target
-
-    etc = cramfs.select("/etc")  # Select a specific file or directory
-    etc = cramfs.select("etc")  # Can also be a relative path
-    rootdir = etc.select("..")  # And a special entry
-    assert rootdir == rootdir.select('.')
-    print(etc)  # print the file or directory's name
-    # The file or directory's absolute path (an instance of PurePosixPath).
-    print(etc.path)
-    print(etc.files)  # A dictionary mapping file names to File instances
-    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
-    print(etc.total)  # Number of entries in this whole subtree
-    # A list of this directory's children (shortcut to list(etc.files.values())).
-    print(list(etc))
-
-    # Find the first file in this subtree that has this name.
-    passwd = cramfs.find("passwd")
-    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
-    passwd = etc["passwd"]
-    print("passwd" in etc)  # Check if directory contains this file
-    print(passwd in etc)  # Also works with instances of File
-
-    # Iterate over this directory's files.
-    for file in etc:
-        print(file.inode)  # Access inode information
-        # These attributes are shortcuts to file.inode.<attr>
-        print(file.mode)
-        print(file.uid)
-        print(file.size)
-        print(file.gid)
-
-    # Iterate over this whole subtree.
-    for file in etc.riter():
-        print(file.name)  # File name, equivalent to file.path.name
-        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
-    
-    # Iterate over files in the subtree that match a pattern.
-    for config_file in etc.itermatch("*.conf"):
-        print(config_file.read_bytes())  # Read the file's raw content
-        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
-
-    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
-
-    # You can use absolute paths from any directory.
-    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
-    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
-
-    # Calling find(), select() and itermatch() on cramfs
-    # is the same as calling them on cramfs.rootdir.
-
-    extract_dir(etc, "extract/etc")  # Extract a directory tree
-    extract_file(passwd, "extract/passwd")  # Extract a single file
-```
-
-### Command line
-
-pycramfs comes with a command-line interface that consists of 4 sub-commands.
-
-#### Info
-
-```
-usage: pycramfs info [-h] file
-
-Show information about all the superblocks that can be found in a file
-
-positional arguments:
-  file
-```
-
-Example output:
-```
-$ pycramfs info cramfs.bin
-Superblock #1
-Magic:     0x28CD3D45
-Size:      282,624
-Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
-Future:    0
-Signature: Compressed ROMFS
-Name:      Compressed
-CRC:       0xDEADBEEF
-Edition:   0
-Blocks:    6,926
-Files:     420
-Offset:    8157
-```
-
-#### List
-
-```
-usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
-
-List the contents of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
-  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
-  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
-                                  filter by file type with f, d, l, p, s, b, c
-```
-
-Example that lists only directories and symlinks that match a pattern:
-```
-$ pycramfs list cramfs.bin -t d l -p "*bin*"
-drwxrwxr-x      256   123:0   /bin 
-lrwxrwxrwx        7   123:0   /bin/ash -> busybox
-lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
-3 file(s) found
-```
-
-#### Extract
-
-```
-usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
-
-Extract files from the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-  -d DEST, --dest DEST         destination directory. Default: next to file
-  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
-  -f, --force                  overwrite files that already exist. Default: False
-  -q, --quiet                  don't print extraction status. Default: False
-```
-
-On Linux, just like `cramfsck -x` you need to run as root
-if you want to preserve file mode, owner and group.
-
-On Windows, the only reason to run as a privileged user is to be able to create
-symlinks.
-Unprivileged accounts can create symlinks if Developer Mode is enabled.
-Otherwise, a regular file containing the target will be created.
-Special files will always just be empty files.
-
-#### Check
-
-This command is similar to running `cramfsck -c file` but is not as thorough.
-
-```
-usage: pycramfs check [-h] [-o OFFSET] file
-
-Make a few superficial checks of the file system
-
-positional arguments:
-  file
-
-options:
-  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
-```
-
-## References
-
-- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
-- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
-- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
-- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
+Metadata-Version: 2.1
+Name: pycramfs
+Version: 1.1.0
+Summary: Read and extract cramfs images.
+Author-email: AT0myks <at0myks.dev@gmail.com>
+Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
+Project-URL: Source, https://github.com/AT0myks/pycramfs
+Keywords: cramfs,filesystem
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Filesystems
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pycramfs
+
+<p align="left">
+<a><img alt="Python versions" src="https://img.shields.io/pypi/pyversions/pycramfs"></a>
+<a href="https://pypi.org/project/pycramfs/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pycramfs"></a>
+<a href="https://github.com/AT0myks/pycramfs/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pycramfs"></a>
+</p>
+
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Usage](#usage)
+* [References](#references)
+
+A library and tool to read and extract cramfs images.
+
+It is far from being as complete as the tools it's based on,
+but should be enough for simple images.
+For example, as of right now it only supports contiguous data layout.
+Only little endian images are supported.
+
+It also provides ways to extract data from an image,
+although you might prefer using
+[`cramfsck`](https://github.com/npitre/cramfs-tools)
+on Linux and 7-Zip on Windows for better compatibility.
+
+## Requirements
+
+Python 3.8+.
+
+## Installation
+
+```
+pip install pycramfs
+```
+
+## Usage
+
+### API
+
+Here's an overview of what you can do:
+```py
+from pycramfs import Cramfs
+from pycramfs.extract import extract_dir, extract_file
+from pycramfs.util import find_superblocks
+
+fsimage = "cramfs.bin"
+superblocks = find_superblocks(fsimage)
+
+with Cramfs.from_file(fsimage, offset=superblocks[0]["offset"]) as cramfs:
+    # Optional offset for start of file system.
+    # You can also create Cramfs instances from bytes or a file descriptor.
+
+    sblock = cramfs.super  # Access the file system's superblock
+    print(sblock.name)
+    print(dict(sblock))  # Superblock as a dictionary
+    assert cramfs.calculate_crc() == sblock.fsid.crc
+
+    rootdir = cramfs.rootdir  # root directory
+    print(cramfs.size)  # File system size in bytes (shortcut to sblock.size)
+    # Number of files in the whole file system (shortcut to sblock.fsid.files).
+    print(len(cramfs))
+    print("/etc/passwd" in cramfs)  # Check if path exists
+
+    # Iterate over the whole file system.
+    for file in cramfs:
+        print(file.parent)  # Instance of Directory (None for the root directory)
+        print(file in cramfs)  # Check if file belongs to this image
+        if file.is_symlink:  # Check the file's type
+            print(file.readlink())  # Symlink target
+
+    etc = cramfs.select("/etc")  # Select a specific file or directory
+    etc = cramfs.select("etc")  # Can also be a relative path
+    rootdir = etc.select("..")  # And a special entry
+    assert rootdir == rootdir.select('.')
+    print(etc)  # print the file or directory's name
+    # The file or directory's absolute path (an instance of PurePosixPath).
+    print(etc.path)
+    print(etc.files)  # A dictionary mapping file names to File instances
+    print(len(etc))  # Number of entries in the directory (shortcut to len(etc.files))
+    print(etc.total)  # Number of entries in this whole subtree
+    # A list of this directory's children (shortcut to list(etc.files.values())).
+    print(list(etc))
+
+    # Find the first file in this subtree that has this name.
+    passwd = cramfs.find("passwd")
+    # Return the child entry if present else raise KeyError (shortcut to etc.files["passwd"]).
+    passwd = etc["passwd"]
+    print("passwd" in etc)  # Check if directory contains this file
+    print(passwd in etc)  # Also works with instances of File
+
+    # Iterate over this directory's files.
+    for file in etc:
+        print(file.inode)  # Access inode information
+        # These attributes are shortcuts to file.inode.<attr>
+        print(file.mode)
+        print(file.uid)
+        print(file.size)
+        print(file.gid)
+
+    # Iterate over this whole subtree.
+    for file in etc.riter():
+        print(file.name)  # File name, equivalent to file.path.name
+        print(file.filemode)  # File mode as a string, for example drwxrwxrwx
+    
+    # Iterate over files in the subtree that match a pattern.
+    for config_file in etc.itermatch("*.conf"):
+        print(config_file.read_bytes())  # Read the file's raw content
+        print(config_file.read_text("utf8"))  # Or as a string with optional encoding
+
+    assert etc > cramfs.select("/bin")  # Comparing instances of File compares their name
+
+    # You can use absolute paths from any directory.
+    cramfs.select("/my/dir/over/here").select("/bin")  # Selects /bin
+    cramfs.select("/my/dir/over/here").select("bin")  # Selects /my/dir/over/here/bin
+
+    # Calling find(), select() and itermatch() on cramfs
+    # is the same as calling them on cramfs.rootdir.
+
+    extract_dir(etc, "extract/etc")  # Extract a directory tree
+    extract_file(passwd, "extract/passwd")  # Extract a single file
+```
+
+### Command line
+
+pycramfs comes with a command-line interface that consists of 4 sub-commands.
+
+#### Info
+
+```
+usage: pycramfs info [-h] file
+
+Show information about all the superblocks that can be found in a file
+
+positional arguments:
+  file
+```
+
+Example output:
+```
+$ pycramfs info cramfs.bin
+Superblock #1
+Magic:     0x28CD3D45
+Size:      282,624
+Flags:     <Flag.SORTED_DIRS|FSID_VERSION_2: 3>
+Future:    0
+Signature: Compressed ROMFS
+Name:      Compressed
+CRC:       0xDEADBEEF
+Edition:   0
+Blocks:    6,926
+Files:     420
+Offset:    8157
+```
+
+#### List
+
+```
+usage: pycramfs list [-h] [-o OFFSET] [-p PATTERN] [-t TYPE [TYPE ...]] file
+
+List the contents of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET      absolute position of file system's start. Default: 0
+  -p PATTERN, --pattern PATTERN   filter by file name pattern with fnmatch
+  -t TYPE [TYPE ...], --type TYPE [TYPE ...]
+                                  filter by file type with f, d, l, p, s, b, c
+```
+
+Example that lists only directories and symlinks that match a pattern:
+```
+$ pycramfs list cramfs.bin -t d l -p "*bin*"
+drwxrwxr-x      256   123:0   /bin 
+lrwxrwxrwx        7   123:0   /bin/ash -> busybox
+lrwxrwxrwx        7   123:0   /bin/base64 -> busybox
+3 file(s) found
+```
+
+#### Extract
+
+```
+usage: pycramfs extract [-h] [-o OFFSET] [-d DEST] [-p PATH] [-f] [-q] file
+
+Extract files from the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+  -d DEST, --dest DEST         destination directory. Default: next to file
+  -p PATH, --path PATH         absolute path of directory or file to extract. Default: '/'
+  -f, --force                  overwrite files that already exist. Default: False
+  -q, --quiet                  don't print extraction status. Default: False
+```
+
+On Linux, just like `cramfsck -x` you need to run as root
+if you want to preserve file mode, owner and group.
+
+On Windows, the only reason to run as a privileged user is to be able to create
+symlinks.
+Unprivileged accounts can create symlinks if Developer Mode is enabled.
+Otherwise, a regular file containing the target will be created.
+Special files will always just be empty files.
+
+#### Check
+
+This command is similar to running `cramfsck -c file` but is not as thorough.
+
+```
+usage: pycramfs check [-h] [-o OFFSET] file
+
+Make a few superficial checks of the file system
+
+positional arguments:
+  file
+
+options:
+  -o OFFSET, --offset OFFSET   absolute position of file system's start. Default: 0
+```
+
+## References
+
+- [cramfs readme](https://github.com/torvalds/linux/blob/master/fs/cramfs/README)
+- [cramfs_fs.h](https://github.com/npitre/cramfs-tools/blob/master/linux/cramfs_fs.h)
+- [cramfsck.c](https://github.com/npitre/cramfs-tools/blob/master/cramfsck.c)
+- [mkcramfs.c](https://github.com/npitre/cramfs-tools/blob/master/mkcramfs.c)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pycramfs Version: 1.0.0 Summary: Read and extract
+Metadata-Version: 2.1 Name: pycramfs Version: 1.1.0 Summary: Read and extract
 cramfs images. Author-email: AT0myks
 dev@gmail.com> Project-URL: Issues, https://github.com/AT0myks/pycramfs/issues
 Project-URL: Source, https://github.com/AT0myks/pycramfs Keywords:
 cramfs,filesystem Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 End Users/Desktop Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: System :: Filesystems Classifier: Topic ::
-Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE # pycramfs
+Utilities Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # pycramfs
 [Python versions] [PyPI] [License]
 * [Requirements](#requirements) * [Installation](#installation) * [Usage]
 (#usage) * [References](#references) A library and tool to read and extract
 cramfs images. It is far from being as complete as the tools it's based on, but
 should be enough for simple images. For example, as of right now it only
 supports contiguous data layout. Only little endian images are supported. It
 also provides ways to extract data from an image, although you might prefer
```

