# Comparing `tmp/fast-webflow-0.1.0.tar.gz` & `tmp/fast-webflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.1.0.tar", last modified: Sat Jul  1 14:42:49 2023, max compression
+gzip compressed data, was "fast-webflow-0.1.1.tar", last modified: Sat Jul  1 16:00:27 2023, max compression
```

## Comparing `fast-webflow-0.1.0.tar` & `fast-webflow-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 14:42:49.293462 fast-webflow-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-06-27 15:47:34.000000 fast-webflow-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3127 2023-07-01 14:42:49.293462 fast-webflow-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-07-01 11:59:59.000000 fast-webflow-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2023-07-01 14:15:03.000000 fast-webflow-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      689 2023-07-01 14:42:49.293462 fast-webflow-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 14:42:49.235846 fast-webflow-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 14:42:49.268501 fast-webflow-0.1.0/src/cms/
--rw-rw-rw-   0        0        0      152 2023-07-01 13:41:12.000000 fast-webflow-0.1.0/src/cms/__init__.py
--rw-rw-rw-   0        0        0     3662 2023-06-30 22:12:15.000000 fast-webflow-0.1.0/src/cms/collection.py
--rw-rw-rw-   0        0        0      851 2023-06-30 15:26:40.000000 fast-webflow-0.1.0/src/cms/config.py
--rw-rw-rw-   0        0        0     1715 2023-06-30 22:15:57.000000 fast-webflow-0.1.0/src/cms/item.py
--rw-rw-rw-   0        0        0     1559 2023-06-30 21:41:36.000000 fast-webflow-0.1.0/src/cms/site.py
--rw-rw-rw-   0        0        0     1572 2023-06-30 20:37:25.000000 fast-webflow-0.1.0/src/cms/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 14:42:49.284535 fast-webflow-0.1.0/src/fast_webflow.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-07-01 14:42:49.000000 fast-webflow-0.1.0/src/fast_webflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-07-01 14:42:49.000000 fast-webflow-0.1.0/src/fast_webflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 14:42:49.000000 fast-webflow-0.1.0/src/fast_webflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-01 14:42:49.000000 fast-webflow-0.1.0/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/src/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 16:00:16.000000 fast-webflow-0.1.1/src/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:00:27.380620 fast-webflow-0.1.1/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-01 16:00:27.000000 fast-webflow-0.1.1/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-01 16:00:27.000000 fast-webflow-0.1.1/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:00:27.000000 fast-webflow-0.1.1/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 16:00:27.000000 fast-webflow-0.1.1/src/fast_webflow.egg-info/top_level.txt
```

### Comparing `fast-webflow-0.1.0/LICENSE` & `fast-webflow-0.1.1/LICENSE`

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

### Comparing `fast-webflow-0.1.0/PKG-INFO` & `fast-webflow-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1
-Name: fast-webflow
-Version: 0.1.0
-Summary: A client library to communicate with the WebFlow API
-Home-page: https://github.com/tcilloni/fast-webflow
-Author: Thomas Cilloni
-Author-email: tcilloni@outlook.com
-Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Welcome to fast-webflow
-a WebFlow CMS API Client in Python
-
-[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
-
-This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
-
-Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
-
-**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
-
-
-## Roadmap
-- [ ] Add *e-commerce* functionality
-- [ ] Add *membership* functionality
-- [ ] Add tests
-- [ ] Finish documentation
-- [ ] Publish to PyPi
-
-
-## Features
-- Authenticate with the WebFlow API using your API key
-- Fetch collection data and items from WebFlow
-- Create, update, and delete items within WebFlow collections
-- Search for items within collections using filter parameters
-- Handle pagination for large datasets
-- Retrieve collection schema and field information
-- Upload files to WebFlow
-
-## Installation
-You can install the Python WebFlow CMS API Client library using pip:
-
-```bash
-pip install webflow-api
-```
-
-## Getting Started
-
-1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
-2. Import the `WebFlow` class from the `webflow` module:
-
-```python
-from webflow import WebFlow
-```
-
-3. Initialize the `WebFlow` client with your API key:
-
-```python
-api_key = 'YOUR_API_KEY'
-client = WebFlow(api_key)
-```
-
-4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
-
-```python
-collection_id = 'COLLECTION_ID'
-items = client.get_collection_items(collection_id)
-for item in items:
-    print(item)
-```
-
-## Contributing
-Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
-
-## License
-This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
+Metadata-Version: 2.1
+Name: fast-webflow
+Version: 0.1.1
+Summary: A client library to communicate with the WebFlow API
+Home-page: https://github.com/tcilloni/fast-webflow
+Author: Thomas Cilloni
+Author-email: tcilloni@outlook.com
+Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Welcome to fast-webflow
+a WebFlow CMS API Client in Python
+
+[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
+[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+
+This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
+
+Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
+
+**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
+
+
+## Roadmap
+- [ ] Add *e-commerce* functionality
+- [ ] Add *membership* functionality
+- [ ] Add tests
+- [ ] Finish documentation
+- [x] Publish to PyPi
+
+
+## Features
+- Authenticate with the WebFlow API using your API key
+- Fetch collection data and items from WebFlow
+- Create, update, and delete items within WebFlow collections
+- Search for items within collections using filter parameters
+- Handle pagination for large datasets
+- Retrieve collection schema and field information
+- Upload files to WebFlow
+
+## Installation
+You can install the Python WebFlow CMS API Client library using pip:
+
+```bash
+pip install webflow-api
+```
+
+## Getting Started
+
+1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
+2. Import the `WebFlow` class from the `webflow` module:
+
+```python
+from webflow import WebFlow
+```
+
+3. Initialize the `WebFlow` client with your API key:
+
+```python
+api_key = 'YOUR_API_KEY'
+client = WebFlow(api_key)
+```
+
+4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
+
+```python
+collection_id = 'COLLECTION_ID'
+items = client.get_collection_items(collection_id)
+for item in items:
+    print(item)
+```
+
+## Contributing
+Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
+
+## License
+This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
```

### Comparing `fast-webflow-0.1.0/README.md` & `fast-webflow-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# Welcome to fast-webflow
-a WebFlow CMS API Client in Python
-
-[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
-
-This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
-
-Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
-
-**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
-
-
-## Roadmap
-- [ ] Add *e-commerce* functionality
-- [ ] Add *membership* functionality
-- [ ] Add tests
-- [ ] Finish documentation
-- [ ] Publish to PyPi
-
-
-## Features
-- Authenticate with the WebFlow API using your API key
-- Fetch collection data and items from WebFlow
-- Create, update, and delete items within WebFlow collections
-- Search for items within collections using filter parameters
-- Handle pagination for large datasets
-- Retrieve collection schema and field information
-- Upload files to WebFlow
-
-## Installation
-You can install the Python WebFlow CMS API Client library using pip:
-
-```bash
-pip install webflow-api
-```
-
-## Getting Started
-
-1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
-2. Import the `WebFlow` class from the `webflow` module:
-
-```python
-from webflow import WebFlow
-```
-
-3. Initialize the `WebFlow` client with your API key:
-
-```python
-api_key = 'YOUR_API_KEY'
-client = WebFlow(api_key)
-```
-
-4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
-
-```python
-collection_id = 'COLLECTION_ID'
-items = client.get_collection_items(collection_id)
-for item in items:
-    print(item)
-```
-
-## Contributing
-Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
-
-## License
-This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
+# Welcome to fast-webflow
+a WebFlow CMS API Client in Python
+
+[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
+[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+
+This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
+
+Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
+
+**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
+
+
+## Roadmap
+- [ ] Add *e-commerce* functionality
+- [ ] Add *membership* functionality
+- [ ] Add tests
+- [ ] Finish documentation
+- [x] Publish to PyPi
+
+
+## Features
+- Authenticate with the WebFlow API using your API key
+- Fetch collection data and items from WebFlow
+- Create, update, and delete items within WebFlow collections
+- Search for items within collections using filter parameters
+- Handle pagination for large datasets
+- Retrieve collection schema and field information
+- Upload files to WebFlow
+
+## Installation
+You can install the Python WebFlow CMS API Client library using pip:
+
+```bash
+pip install webflow-api
+```
+
+## Getting Started
+
+1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
+2. Import the `WebFlow` class from the `webflow` module:
+
+```python
+from webflow import WebFlow
+```
+
+3. Initialize the `WebFlow` client with your API key:
+
+```python
+api_key = 'YOUR_API_KEY'
+client = WebFlow(api_key)
+```
+
+4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
+
+```python
+collection_id = 'COLLECTION_ID'
+items = client.get_collection_items(collection_id)
+for item in items:
+    print(item)
+```
+
+## Contributing
+Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
+
+## License
+This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
```

### Comparing `fast-webflow-0.1.0/setup.cfg` & `fast-webflow-0.1.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2066 6173 742d 7765 6266 6c6f 770d   = fast-webflow.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
-00000030: 0d0a 6175 7468 6f72 203d 2054 686f 6d61  ..author = Thoma
-00000040: 7320 4369 6c6c 6f6e 690d 0a61 7574 686f  s Cilloni..autho
-00000050: 725f 656d 6169 6c20 3d20 7463 696c 6c6f  r_email = tcillo
-00000060: 6e69 406f 7574 6c6f 6f6b 2e63 6f6d 0d0a  ni@outlook.com..
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
-00000080: 636c 6965 6e74 206c 6962 7261 7279 2074  client library t
-00000090: 6f20 636f 6d6d 756e 6963 6174 6520 7769  o communicate wi
-000000a0: 7468 2074 6865 2057 6562 466c 6f77 2041  th the WebFlow A
-000000b0: 5049 0d0a 6c6f 6e67 5f64 6573 6372 6970  PI..long_descrip
-000000c0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000d0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000e0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000f0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000100: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 7463 696c 6c6f 6e69 2f66 6173 742d 7765  tcilloni/fast-we
-00000130: 6266 6c6f 770d 0a70 726f 6a65 6374 5f75  bflow..project_u
-00000140: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000150: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000160: 6974 6875 622e 636f 6d2f 7463 696c 6c6f  ithub.com/tcillo
-00000170: 6e69 2f66 6173 742d 7765 6266 6c6f 772f  ni/fast-webflow/
-00000180: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
-00000190: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001e0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-000001f0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000200: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000210: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000220: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
-00000230: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000240: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000250: 6573 203d 203e 3d20 332e 380d 0a0d 0a5b  es = >= 3.8....[
-00000260: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000270: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000280: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-00000290: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000002a0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000002b0: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6661 7374 2d77 6562 666c 6f77 0a76  = fast-webflow.v
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e31 0a61  ersion = 0.1.1.a
+00000030: 7574 686f 7220 3d20 5468 6f6d 6173 2043  uthor = Thomas C
+00000040: 696c 6c6f 6e69 0a61 7574 686f 725f 656d  illoni.author_em
+00000050: 6169 6c20 3d20 7463 696c 6c6f 6e69 406f  ail = tcilloni@o
+00000060: 7574 6c6f 6f6b 2e63 6f6d 0a64 6573 6372  utlook.com.descr
+00000070: 6970 7469 6f6e 203d 2041 2063 6c69 656e  iption = A clien
+00000080: 7420 6c69 6272 6172 7920 746f 2063 6f6d  t library to com
+00000090: 6d75 6e69 6361 7465 2077 6974 6820 7468  municate with th
+000000a0: 6520 5765 6246 6c6f 7720 4150 490a 6c6f  e WebFlow API.lo
+000000b0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+000000c0: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000e0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+000000f0: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
+00000100: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000110: 6875 622e 636f 6d2f 7463 696c 6c6f 6e69  hub.com/tcilloni
+00000120: 2f66 6173 742d 7765 6266 6c6f 770a 7072  /fast-webflow.pr
+00000130: 6f6a 6563 745f 7572 6c73 203d 200a 0942  oject_urls = ..B
+00000140: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
+00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000160: 7463 696c 6c6f 6e69 2f66 6173 742d 7765  tcilloni/fast-we
+00000170: 6266 6c6f 772f 6973 7375 6573 0a63 6c61  bflow/issues.cla
+00000180: 7373 6966 6965 7273 203d 200a 0950 726f  ssifiers = ..Pro
+00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001b0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001c0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001d0: 204c 6963 656e 7365 0a09 4f70 6572 6174   License..Operat
+000001e0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001f0: 2049 6e64 6570 656e 6465 6e74 0a0a 5b6f   Independent..[o
+00000200: 7074 696f 6e73 5d0a 7061 636b 6167 655f  ptions].package_
+00000210: 6469 7220 3d20 0a09 3d20 7372 630a 7061  dir = ..= src.pa
+00000220: 636b 6167 6573 203d 2066 696e 643a 0a70  ckages = find:.p
+00000230: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000240: 203e 3d20 332e 380a 0a5b 6f70 7469 6f6e   >= 3.8..[option
+00000250: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000260: 0a77 6865 7265 203d 2073 7263 0a0a 5b65  .where = src..[e
+00000270: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
+00000280: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
+00000290: 2030 0a0a                                 0..
```

### Comparing `fast-webflow-0.1.0/src/cms/collection.py` & `fast-webflow-0.1.1/src/cms/collection.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import requests
-from collections import UserDict
-
-from .utils import string_to_dict, slugify, try_request, parallelize
-from .config import make_headers
-
-
-class Collection(UserDict):
-    id: str
-    _url: str
-    _items_url: str
-    _headers: dict[str, str]
-    _max_items_per_request: int = 100
-    delay: int
-    max_retries: int
-
-    def __init__(self, collection_id: str, max_retries: int = 50, throttle_delay: int = 10):
-        self.id = collection_id
-        self._url = f'https://api.webflow.com/collections/{collection_id}'
-        self._items_url = f'https://api.webflow.com/collections/{collection_id}/items?live="true"'
-        self._headers = make_headers()
-        self.delay = throttle_delay
-        self.max_retries = max_retries
-        self.data = self.get_data()
-    
-
-    def get_data(self) -> dict:
-        return self._request(requests.get)
-    
-
-    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
-        if url is None:
-            url = self._items_url
-        
-        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
-    
-
-    def post_item(self, fields: dict[str,any], draft: bool = False):
-        payload = {'fields': {'_archived': False, '_draft': draft}}
-        payload['fields'].update(fields)
-
-        data = self._request(requests.post, self._items_url, payload)
-        
-        return data
-
-
-    def publish_items(self, item_ids: list[str]) -> dict:
-        max_items = self._max_items_per_request  # API rule
-        url = self._url + '/items/publish'
-        data = {}
-
-        # split IDs into lists of max 100 items
-        item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
-        payloads = [{"itemIds": ids} for ids in item_ids]
-
-        # send parallel requests
-        parallel_arguments = zip(repeat(url), payloads)
-        returns  = parallelize(lambda args: requests.put(*args), parallel_arguments)
-
-        # merge responses
-        for key in ['publishedItemIds', 'errors']:
-            data[key] = [item for resp in returns for item in resp[key]]
-        
-        return data
-    
-
-    def delete_items(self, item_ids: list[str]) -> dict[str,list[any]]:
-        max_items = self._max_items_per_request  # API rule
-        data = {}
-
-        # split IDs into lists of max 100 items
-        item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
-        payloads = [{"itemIds": ids} for ids in item_ids]
-
-        # send parallel requests
-        parallel_arguments = zip(repeat(self._items_url), payloads)
-        returns  = parallelize(lambda args: requests.delete(*args), parallel_arguments)
-
-        # merge responses
-        for key in ['deletedItemIds', 'errors']:
-            data[key] = [item for resp in returns for item in resp[key]]
-
-        return data
-    
-
-    def get_all_items(self) -> list[dict]:
-        # update total number of items
-        self.data = self.get_data()
-        max_items = self._max_items_per_request  # API rule
-        total = self.data['total']
-
-        # prepare one URL request for each offset in 0..total..limit
-        item_lists = parallelize(self.get_items, range(0, total, max_items))
-        all_items = [item for item_list in item_lists for item in item_list['items']]
-        
-        return all_items
-    
-
-    def get_items(self, offset: int = 0, limit: int = 100) -> list[dict]:
-        url = self._items_url + f"&offset={offset}&limit={limit}"
-        data = self._request(requests.get, url)
-        
-        return data
-
+import requests
+from collections import UserDict
+
+from .utils import string_to_dict, slugify, try_request, parallelize
+from .config import make_headers
+
+
+class Collection(UserDict):
+    id: str
+    _url: str
+    _items_url: str
+    _headers: dict[str, str]
+    _max_items_per_request: int = 100
+    delay: int
+    max_retries: int
+
+    def __init__(self, collection_id: str, max_retries: int = 50, throttle_delay: int = 10):
+        self.id = collection_id
+        self._url = f'https://api.webflow.com/collections/{collection_id}'
+        self._items_url = f'https://api.webflow.com/collections/{collection_id}/items?live="true"'
+        self._headers = make_headers()
+        self.delay = throttle_delay
+        self.max_retries = max_retries
+        self.data = self.get_data()
+    
+
+    def get_data(self) -> dict:
+        return self._request(requests.get)
+    
+
+    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
+        if url is None:
+            url = self._items_url
+        
+        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
+    
+
+    def post_item(self, fields: dict[str,any], draft: bool = False):
+        payload = {'fields': {'_archived': False, '_draft': draft}}
+        payload['fields'].update(fields)
+
+        data = self._request(requests.post, self._items_url, payload)
+        
+        return data
+
+
+    def publish_items(self, item_ids: list[str]) -> dict:
+        max_items = self._max_items_per_request  # API rule
+        url = self._url + '/items/publish'
+        data = {}
+
+        # split IDs into lists of max 100 items
+        item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
+        payloads = [{"itemIds": ids} for ids in item_ids]
+
+        # send parallel requests
+        parallel_arguments = zip(repeat(url), payloads)
+        returns  = parallelize(lambda args: requests.put(*args), parallel_arguments)
+
+        # merge responses
+        for key in ['publishedItemIds', 'errors']:
+            data[key] = [item for resp in returns for item in resp[key]]
+        
+        return data
+    
+
+    def delete_items(self, item_ids: list[str]) -> dict[str,list[any]]:
+        max_items = self._max_items_per_request  # API rule
+        data = {}
+
+        # split IDs into lists of max 100 items
+        item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
+        payloads = [{"itemIds": ids} for ids in item_ids]
+
+        # send parallel requests
+        parallel_arguments = zip(repeat(self._items_url), payloads)
+        returns  = parallelize(lambda args: requests.delete(*args), parallel_arguments)
+
+        # merge responses
+        for key in ['deletedItemIds', 'errors']:
+            data[key] = [item for resp in returns for item in resp[key]]
+
+        return data
+    
+
+    def get_all_items(self) -> list[dict]:
+        # update total number of items
+        self.data = self.get_data()
+        max_items = self._max_items_per_request  # API rule
+        total = self.data['total']
+
+        # prepare one URL request for each offset in 0..total..limit
+        item_lists = parallelize(self.get_items, range(0, total, max_items))
+        all_items = [item for item_list in item_lists for item in item_list['items']]
+        
+        return all_items
+    
+
+    def get_items(self, offset: int = 0, limit: int = 100) -> list[dict]:
+        url = self._items_url + f"&offset={offset}&limit={limit}"
+        data = self._request(requests.get, url)
+        
+        return data
+
```

### Comparing `fast-webflow-0.1.0/src/cms/config.py` & `fast-webflow-0.1.1/src/cms/config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import requests
-from .utils import string_to_dict
-
-_auth_token = None
-
-
-def make_headers() -> dict[str, str]:
-    assert _auth_token, 'You must first set the `auth_token` variable.'
-
-    headers = {
-        "accept": "application/json",
-        "content-type": "application/json",
-        "authorization": f"Bearer {_auth_token}"
-    }
-
-    return headers
-
-
-def authenticate(auth_token: str) -> None:
-    global _auth_token
-
-    # set the new token
-    _auth_token = auth_token
-    response = requests.get("https://api.webflow.com/user", headers = make_headers())
-
-    # check if it is valid
-    if response.status_code == 200:
-        user = string_to_dict(response.text)['user']
-        print(f'User "{user["firstName"]} {user["lastName"]}" authenticated successfully.')
-    else:
+import requests
+from .utils import string_to_dict
+
+_auth_token = None
+
+
+def make_headers() -> dict[str, str]:
+    assert _auth_token, 'You must first set the `auth_token` variable.'
+
+    headers = {
+        "accept": "application/json",
+        "content-type": "application/json",
+        "authorization": f"Bearer {_auth_token}"
+    }
+
+    return headers
+
+
+def authenticate(auth_token: str) -> None:
+    global _auth_token
+
+    # set the new token
+    _auth_token = auth_token
+    response = requests.get("https://api.webflow.com/user", headers = make_headers())
+
+    # check if it is valid
+    if response.status_code == 200:
+        user = string_to_dict(response.text)['user']
+        print(f'User "{user["firstName"]} {user["lastName"]}" authenticated successfully.')
+    else:
         raise Exception(response.text)
```

### Comparing `fast-webflow-0.1.0/src/cms/item.py` & `fast-webflow-0.1.1/src/cms/item.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import requests
-from collections import UserDict
-
-from .utils import string_to_dict, slugify, try_request, parallelize
-from .config import make_headers
-
-
-class Item(UserDict):
-    id: str
-    _url: str
-    _headers: dict[str, str]
-    delay: int
-    max_retries: int
-
-    def __init__(self, collection_id: str, item_id: str, max_retries: int = 50, throttle_delay: int = 10):
-        self.id = item_id
-        self._url = f'https://api.webflow.com/collections/{collection_id}/items/{item_id}?live=true'
-        self._headers = make_headers()
-        self.delay = throttle_delay
-        self.max_retries = max_retries
-        self.data = self.get_data()
-    
-
-    def get_data(self) -> dict:
-        return self._request(requests.get)
-    
-
-    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
-        if url is None:
-            url = self._url
-        
-        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
-    
-
-    def update(self, fields: dict[str,any], draft: bool = False) -> dict:
-        payload = {'fields': {'_archived': False, '_draft': draft}}
-        payload['fields'].update(fields)
-
-        data = self._request(requests.put, self._url, payload)
-        
-        return data
-    
-
-    def path(self, fields: dict[str,any], draft: bool = False) -> dict:
-        payload = {'fields': {'_archived': False, '_draft': draft}}
-        payload['fields'].update(fields)
-
-        data = self._request(requests.patch, self._url, payload)
-        
-        return data
-
-
-    def delete(self) -> dict:
-        data = self._request(requests.delete, self._url)
-        return data
-
+import requests
+from collections import UserDict
+
+from .utils import string_to_dict, slugify, try_request, parallelize
+from .config import make_headers
+
+
+class Item(UserDict):
+    id: str
+    _url: str
+    _headers: dict[str, str]
+    delay: int
+    max_retries: int
+
+    def __init__(self, collection_id: str, item_id: str, max_retries: int = 50, throttle_delay: int = 10):
+        self.id = item_id
+        self._url = f'https://api.webflow.com/collections/{collection_id}/items/{item_id}?live=true'
+        self._headers = make_headers()
+        self.delay = throttle_delay
+        self.max_retries = max_retries
+        self.data = self.get_data()
+    
+
+    def get_data(self) -> dict:
+        return self._request(requests.get)
+    
+
+    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
+        if url is None:
+            url = self._url
+        
+        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
+    
+
+    def update(self, fields: dict[str,any], draft: bool = False) -> dict:
+        payload = {'fields': {'_archived': False, '_draft': draft}}
+        payload['fields'].update(fields)
+
+        data = self._request(requests.put, self._url, payload)
+        
+        return data
+    
+
+    def path(self, fields: dict[str,any], draft: bool = False) -> dict:
+        payload = {'fields': {'_archived': False, '_draft': draft}}
+        payload['fields'].update(fields)
+
+        data = self._request(requests.patch, self._url, payload)
+        
+        return data
+
+
+    def delete(self) -> dict:
+        data = self._request(requests.delete, self._url)
+        return data
+
```

### Comparing `fast-webflow-0.1.0/src/cms/site.py` & `fast-webflow-0.1.1/src/cms/site.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import requests
-from collections import UserDict
-
-from .utils import string_to_dict, slugify, try_request
-from .config import make_headers
-
-
-def list_sites():
-    data = try_request(requests.get, 'https://api.webflow.com/sites', make_headers())
-    return data
-
-
-class Site(UserDict):
-    id: str
-    _url: str
-    _headers: dict[str, str]
-    delay: int
-    max_retries: int
-
-    def __init__(self, site_id: str, max_retries: int = 50, throttle_delay: int = 10):
-        self.id = site_id
-        self._url = f'https://api.webflow.com/sites/{site_id}'
-        self._headers = make_headers()
-        self.delay = throttle_delay
-        self.max_retries = max_retries
-        self.data = self.get_data()
-    
-
-    def get_data(self) -> dict:
-        return self._request(requests.get)
-
-
-    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
-        if url is None:
-            url = self._url
-        
-        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
-    
-
-    def publish(self, domains: list[str] = None) -> dict:
-        if not domains:
-            domains = [domain['name'] for domain in self.get_domains()]
-
-        return self._request(requests.post, self._url + '/publish', {"domains": domains})
-    
-
-    def get_domains(self) -> dict:
-        return self._request(requests.get, self._url + '/domains')
-
-
-    def get_collections(self) -> list[dict]:
+import requests
+from collections import UserDict
+
+from .utils import string_to_dict, slugify, try_request
+from .config import make_headers
+
+
+def list_sites():
+    data = try_request(requests.get, 'https://api.webflow.com/sites', make_headers())
+    return data
+
+
+class Site(UserDict):
+    id: str
+    _url: str
+    _headers: dict[str, str]
+    delay: int
+    max_retries: int
+
+    def __init__(self, site_id: str, max_retries: int = 50, throttle_delay: int = 10):
+        self.id = site_id
+        self._url = f'https://api.webflow.com/sites/{site_id}'
+        self._headers = make_headers()
+        self.delay = throttle_delay
+        self.max_retries = max_retries
+        self.data = self.get_data()
+    
+
+    def get_data(self) -> dict:
+        return self._request(requests.get)
+
+
+    def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict:
+        if url is None:
+            url = self._url
+        
+        return try_request(request_fn, url, self._headers, data, self.max_retries, self.delay)
+    
+
+    def publish(self, domains: list[str] = None) -> dict:
+        if not domains:
+            domains = [domain['name'] for domain in self.get_domains()]
+
+        return self._request(requests.post, self._url + '/publish', {"domains": domains})
+    
+
+    def get_domains(self) -> dict:
+        return self._request(requests.get, self._url + '/domains')
+
+
+    def get_collections(self) -> list[dict]:
         return self._request(requests.get, self._url + '/collections')
```

### Comparing `fast-webflow-0.1.0/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.1.1/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1
-Name: fast-webflow
-Version: 0.1.0
-Summary: A client library to communicate with the WebFlow API
-Home-page: https://github.com/tcilloni/fast-webflow
-Author: Thomas Cilloni
-Author-email: tcilloni@outlook.com
-Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Welcome to fast-webflow
-a WebFlow CMS API Client in Python
-
-[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
-[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
-
-This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
-
-Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
-
-**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
-
-
-## Roadmap
-- [ ] Add *e-commerce* functionality
-- [ ] Add *membership* functionality
-- [ ] Add tests
-- [ ] Finish documentation
-- [ ] Publish to PyPi
-
-
-## Features
-- Authenticate with the WebFlow API using your API key
-- Fetch collection data and items from WebFlow
-- Create, update, and delete items within WebFlow collections
-- Search for items within collections using filter parameters
-- Handle pagination for large datasets
-- Retrieve collection schema and field information
-- Upload files to WebFlow
-
-## Installation
-You can install the Python WebFlow CMS API Client library using pip:
-
-```bash
-pip install webflow-api
-```
-
-## Getting Started
-
-1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
-2. Import the `WebFlow` class from the `webflow` module:
-
-```python
-from webflow import WebFlow
-```
-
-3. Initialize the `WebFlow` client with your API key:
-
-```python
-api_key = 'YOUR_API_KEY'
-client = WebFlow(api_key)
-```
-
-4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
-
-```python
-collection_id = 'COLLECTION_ID'
-items = client.get_collection_items(collection_id)
-for item in items:
-    print(item)
-```
-
-## Contributing
-Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
-
-## License
-This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
+Metadata-Version: 2.1
+Name: fast-webflow
+Version: 0.1.1
+Summary: A client library to communicate with the WebFlow API
+Home-page: https://github.com/tcilloni/fast-webflow
+Author: Thomas Cilloni
+Author-email: tcilloni@outlook.com
+Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Welcome to fast-webflow
+a WebFlow CMS API Client in Python
+
+[![License](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+<!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
+[![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
+
+This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
+
+Check out an example website built with the help of *fast-webflow*: [liguriasegreta.com](https://www.liguriasegreta.com)
+
+**DISCLAIMER**: This is an unofficial abstraction over WebFlow's API and I am not associated with the WebFlow team.
+
+
+## Roadmap
+- [ ] Add *e-commerce* functionality
+- [ ] Add *membership* functionality
+- [ ] Add tests
+- [ ] Finish documentation
+- [x] Publish to PyPi
+
+
+## Features
+- Authenticate with the WebFlow API using your API key
+- Fetch collection data and items from WebFlow
+- Create, update, and delete items within WebFlow collections
+- Search for items within collections using filter parameters
+- Handle pagination for large datasets
+- Retrieve collection schema and field information
+- Upload files to WebFlow
+
+## Installation
+You can install the Python WebFlow CMS API Client library using pip:
+
+```bash
+pip install webflow-api
+```
+
+## Getting Started
+
+1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
+2. Import the `WebFlow` class from the `webflow` module:
+
+```python
+from webflow import WebFlow
+```
+
+3. Initialize the `WebFlow` client with your API key:
+
+```python
+api_key = 'YOUR_API_KEY'
+client = WebFlow(api_key)
+```
+
+4. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
+
+```python
+collection_id = 'COLLECTION_ID'
+items = client.get_collection_items(collection_id)
+for item in items:
+    print(item)
+```
+
+## Contributing
+Contributions to the Python WebFlow CMS API Client library are welcome! If you encounter any bugs, have suggestions, or would like to contribute new features, please feel free to open an issue or submit a pull request on GitHub.
+
+## License
+This project is licensed under the GNU GPLv3 License. See the [LICENSE](./LICENSE) file for more information.
```

