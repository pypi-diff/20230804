# Comparing `tmp/construct-dataclasses-1.1.2.tar.gz` & `tmp/construct-dataclasses-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-dataclasses-1.1.2.tar", last modified: Thu Jul 13 15:45:55 2023, max compression
+gzip compressed data, was "construct-dataclasses-1.1.3.tar", last modified: Fri Jul 14 18:24:41 2023, max compression
```

## Comparing `construct-dataclasses-1.1.2.tar` & `construct-dataclasses-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:45:55.276564 construct-dataclasses-1.1.2/
--rw-rw-rw-   0        0        0    35802 2023-07-12 04:34:56.000000 construct-dataclasses-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6835 2023-07-13 15:45:55.277567 construct-dataclasses-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5578 2023-07-13 06:41:17.000000 construct-dataclasses-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 15:45:55.260370 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/
--rw-rw-rw-   0        0        0     6835 2023-07-13 15:45:54.000000 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-13 15:45:55.000000 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:45:54.000000 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 15:45:54.000000 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-13 15:45:54.000000 construct-dataclasses-1.1.2/construct_dataclasses.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15001 2023-07-13 15:33:51.000000 construct-dataclasses-1.1.2/construct_dataclasses.py
--rw-rw-rw-   0        0        0       42 2023-07-13 15:45:55.283564 construct-dataclasses-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-07-13 15:43:29.000000 construct-dataclasses-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:24:41.654134 construct-dataclasses-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-07-14 18:24:30.000000 construct-dataclasses-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-14 18:24:41.654134 construct-dataclasses-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-14 18:24:30.000000 construct-dataclasses-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:24:41.654134 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-14 18:24:41.000000 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-14 18:24:41.000000 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:24:41.000000 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 18:24:41.000000 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 18:24:41.000000 construct-dataclasses-1.1.3/construct_dataclasses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14578 2023-07-14 18:24:30.000000 construct-dataclasses-1.1.3/construct_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:24:41.654134 construct-dataclasses-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-14 18:24:30.000000 construct-dataclasses-1.1.3/setup.py
```

### Comparing `construct-dataclasses-1.1.2/LICENSE` & `construct-dataclasses-1.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
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
+GNU GENERAL PUBLIC LICENSE
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

### Comparing `construct-dataclasses-1.1.2/PKG-INFO` & `construct-dataclasses-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-Metadata-Version: 2.1
-Name: construct-dataclasses
-Version: 1.1.2
-Summary: enhancement for the python package 'construct' that adds support for dataclasses.
-Home-page: https://github.com/MatrixEditor/construct-dataclasses
-Author: MatrixEditor
-License: GNU GPLv3
-Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
-Platform: POSIX
-Platform: Windows
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# construct-dataclasses
-
-[![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
-![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
-![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
-[![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
-
-This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
-
-## Installation
-
-You can install the package via pip or just copy the python file as it is only one.
-
-```bash
-pip install construct-dataclasses
-```
-
-## Usage
-
-More usage examples are placed in the [*examples/*](/examples/) directory.
-
-### Define dataclasses
-
-Before we can start declaring fields on a dataclass, the class itself has to be created. Currently, there are two ways on how to create
-a dataclass usable by this package.
-
-1. Use the standard `@dataclass` decorator and create the parser instance afterwards:
-
-    ```python
-    from construct_dataclasses import DataclassStruct
-
-    @dataclasses.dataclass
-    class Foo: ...
-
-    # Create the parser manually
-    parser = DataclassStruct(Foo)
-    instance = parser.parse(...)
-    ```
-
-2. Use the `@dataclass_struct` decorator to define a new dataclass and automatically create a parser instance that will be assigned as a class attribute:
-
-    ```python
-    from construct_dataclasses import dataclass_struct
-
-    @dataclass_struct
-    class Foo: ...
-
-    # Use the class-parser to parse
-    instance = Foo.parser.parse(...)
-    # or to build
-    data = Foo.parser.build(instance)
-    ```
-
-### Define fields
-
-This module defines a new way how to declare fields of a dataclass. In order to combine the python package construct with python's dataclasses module, this project introduces the following two methods:
-
-- `csfield`: Default definition of a field using a subcon or other dataclass
-
-    ```python
-    @dataclass_struct
-    class ImageHeader:
-        signature: bytes         = csfield(cs.Const(b"BMP"))
-        orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
-    ```
-
-- `subcsfield`: Definition of nested constructs that are contained in list-like structures.
-
-    ```python
-    @dataclass_struct
-    class Image:
-        header: ImageHeader = csfield(ImageHeader) # dataclass reference
-        width: int          = csfield(cs.Int8ub)
-        height: int         = csfield(cs.Int8ub)
-        # Note that we have to convert our dataclass into a struct using
-        # the method "to_struct(...)"
-        pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
-    ```
-
-- `tfield`: a simple typed field that tries to return an instance of the given model class. **Use `subcsfield` for dataclass models and enum types with this function**.
-
-    ```python
-    @dataclass_struct
-    class ImageHeader:
-        orientation: Orientation = tfield(Orientation, cs.Enum(cs.Int8ul, Orientation))
-    ```
-
-
-### Convert dataclasses
-
-By default, all conversion is done automatically if you don't use instances of `SubContruct` classes in your field definitions. If you have to define a subcon that needs a nested subcon, like `Array` or `RepeatUntil` and you would like to parse a dataclass struct, it is required to convert the defined dataclass into a struct.
-
-- `to_struct`: This method converts all fields defined in a dataclass into a single `Struct` or `AlignedStruct` instance.
-
-    ```python
-    @dataclass_struct
-    class Pixel:
-        data: int = csfield(cs.Int8ub)
-
-    pixel_struct: construct.Struct = to_struct(Pixel)
-    ```
-- `to_object`: In order to use data returned by `Struct.parse`, this method can be used to apply this data and create a dataclass object from it.
-
-    ```python
-    data = pixel_struct.parse(b"...")
-    pixel = to_object(data, Pixel)
-    ```
-
-The complete example is shown below:
-
-```python
-# Example modifed from here: https://github.com/timrid/construct-typing/
-import dataclasses
-import enum
-import construct as cs
-
-from construct_dataclasses import dataclass_struct, csfield, to_struct, subcsfield
-
-class Orientation(enum.IntEnum):
-    NONE = 0
-    HORIZONTAL = 1
-    VERTICAL = 2
-
-@dataclass_struct
-class ImageHeader:
-    signature: bytes         = csfield(cs.Const(b"BMP"))
-    orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
-
-@dataclass_struct
-class Pixel:
-    data: int = csfield(cs.Int8ub)
-
-@dataclass_struct
-class Image:
-    header: ImageHeader = csfield(ImageHeader)
-    width: int          = csfield(cs.Int8ub)
-    height: int         = csfield(cs.Int8ub)
-    pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
-
-obj = Image(
-    header=ImageHeader(
-        orientation=Orientation.VERTICAL
-    ),
-    width=3,
-    height=2,
-    pixels=[Pixel(1), Pixel(2), Pixel(3), Pixel(4), Pixel(5), Pixel(6)]
-)
-
-print(Image.parser.build(obj))
-print(Image.parser.parse(b"BMP\x02\x03\x02\x01\x02\x03\x04\x05\06"))
-```
-
-The expected output would be:
-
-    b'BMP\x02\x03\x02\x01\x02\x03\x04\x05\x06'
-    Image(
-        header=ImageHeader(signature=b'BMP', orientation=<Orientation.VERTICAL: 2>),
-        width=3, height=2,
-        pixels=[Pixel(data=1), Pixel(data=2), Pixel(data=3), Pixel(data=4), Pixel(data=5), Pixel(data=6)]
-    )
+Metadata-Version: 2.1
+Name: construct-dataclasses
+Version: 1.1.3
+Summary: enhancement for the python package 'construct' that adds support for dataclasses.
+Home-page: https://github.com/MatrixEditor/construct-dataclasses
+Author: MatrixEditor
+License: GNU GPLv3
+Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
+Platform: POSIX
+Platform: Windows
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# construct-dataclasses
+
+[![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
+![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
+![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
+[![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
+
+This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
+
+## Installation
+
+You can install the package via pip or just copy the python file as it is only one.
+
+```bash
+pip install construct-dataclasses
+```
+
+## Usage
+
+More usage examples are placed in the [*examples/*](/examples/) directory.
+
+### Define dataclasses
+
+Before we can start declaring fields on a dataclass, the class itself has to be created. Currently, there are two ways on how to create
+a dataclass usable by this package.
+
+1. Use the standard `@dataclass` decorator and create the parser instance afterwards:
+
+    ```python
+    from construct_dataclasses import DataclassStruct
+
+    @dataclasses.dataclass
+    class Foo: ...
+
+    # Create the parser manually
+    parser = DataclassStruct(Foo)
+    instance = parser.parse(...)
+    ```
+
+2. Use the `@dataclass_struct` decorator to define a new dataclass and automatically create a parser instance that will be assigned as a class attribute:
+
+    ```python
+    from construct_dataclasses import dataclass_struct
+
+    @dataclass_struct
+    class Foo: ...
+
+    # Use the class-parser to parse
+    instance = Foo.parser.parse(...)
+    # or to build
+    data = Foo.parser.build(instance)
+    ```
+
+### Define fields
+
+This module defines a new way how to declare fields of a dataclass. In order to combine the python package construct with python's dataclasses module, this project introduces the following two methods:
+
+- `csfield`: Default definition of a field using a subcon or other dataclass
+
+    ```python
+    @dataclass_struct
+    class ImageHeader:
+        signature: bytes         = csfield(cs.Const(b"BMP"))
+        orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
+    ```
+
+- `subcsfield`: Definition of nested constructs that are contained in list-like structures.
+
+    ```python
+    @dataclass_struct
+    class Image:
+        header: ImageHeader = csfield(ImageHeader) # dataclass reference
+        width: int          = csfield(cs.Int8ub)
+        height: int         = csfield(cs.Int8ub)
+        # Note that we have to convert our dataclass into a struct using
+        # the method "to_struct(...)"
+        pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
+    ```
+
+- `tfield`: a simple typed field that tries to return an instance of the given model class. **Use `subcsfield` for dataclass models and enum types with this function**.
+
+    ```python
+    @dataclass_struct
+    class ImageHeader:
+        orientation: Orientation = tfield(Orientation, cs.Enum(cs.Int8ul, Orientation))
+    ```
+
+
+### Convert dataclasses
+
+By default, all conversion is done automatically if you don't use instances of `SubContruct` classes in your field definitions. If you have to define a subcon that needs a nested subcon, like `Array` or `RepeatUntil` and you would like to parse a dataclass struct, it is required to convert the defined dataclass into a struct.
+
+- `to_struct`: This method converts all fields defined in a dataclass into a single `Struct` or `AlignedStruct` instance.
+
+    ```python
+    @dataclass_struct
+    class Pixel:
+        data: int = csfield(cs.Int8ub)
+
+    pixel_struct: construct.Struct = to_struct(Pixel)
+    ```
+- `to_object`: In order to use data returned by `Struct.parse`, this method can be used to apply this data and create a dataclass object from it.
+
+    ```python
+    data = pixel_struct.parse(b"...")
+    pixel = to_object(data, Pixel)
+    ```
+
+The complete example is shown below:
+
+```python
+# Example modifed from here: https://github.com/timrid/construct-typing/
+import dataclasses
+import enum
+import construct as cs
+
+from construct_dataclasses import dataclass_struct, csfield, to_struct, subcsfield
+
+class Orientation(enum.IntEnum):
+    NONE = 0
+    HORIZONTAL = 1
+    VERTICAL = 2
+
+@dataclass_struct
+class ImageHeader:
+    signature: bytes         = csfield(cs.Const(b"BMP"))
+    orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
+
+@dataclass_struct
+class Pixel:
+    data: int = csfield(cs.Int8ub)
+
+@dataclass_struct
+class Image:
+    header: ImageHeader = csfield(ImageHeader)
+    width: int          = csfield(cs.Int8ub)
+    height: int         = csfield(cs.Int8ub)
+    pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
+
+obj = Image(
+    header=ImageHeader(
+        orientation=Orientation.VERTICAL
+    ),
+    width=3,
+    height=2,
+    pixels=[Pixel(1), Pixel(2), Pixel(3), Pixel(4), Pixel(5), Pixel(6)]
+)
+
+print(Image.parser.build(obj))
+print(Image.parser.parse(b"BMP\x02\x03\x02\x01\x02\x03\x04\x05\06"))
+```
+
+The expected output would be:
+
+    b'BMP\x02\x03\x02\x01\x02\x03\x04\x05\x06'
+    Image(
+        header=ImageHeader(signature=b'BMP', orientation=<Orientation.VERTICAL: 2>),
+        width=3, height=2,
+        pixels=[Pixel(data=1), Pixel(data=2), Pixel(data=3), Pixel(data=4), Pixel(data=5), Pixel(data=6)]
+    )
```

### Comparing `construct-dataclasses-1.1.2/README.md` & `construct-dataclasses-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `construct-dataclasses-1.1.2/construct_dataclasses.egg-info/PKG-INFO` & `construct-dataclasses-1.1.3/construct_dataclasses.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-Metadata-Version: 2.1
-Name: construct-dataclasses
-Version: 1.1.2
-Summary: enhancement for the python package 'construct' that adds support for dataclasses.
-Home-page: https://github.com/MatrixEditor/construct-dataclasses
-Author: MatrixEditor
-License: GNU GPLv3
-Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
-Platform: POSIX
-Platform: Windows
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# construct-dataclasses
-
-[![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
-![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
-![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
-[![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
-
-This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
-
-## Installation
-
-You can install the package via pip or just copy the python file as it is only one.
-
-```bash
-pip install construct-dataclasses
-```
-
-## Usage
-
-More usage examples are placed in the [*examples/*](/examples/) directory.
-
-### Define dataclasses
-
-Before we can start declaring fields on a dataclass, the class itself has to be created. Currently, there are two ways on how to create
-a dataclass usable by this package.
-
-1. Use the standard `@dataclass` decorator and create the parser instance afterwards:
-
-    ```python
-    from construct_dataclasses import DataclassStruct
-
-    @dataclasses.dataclass
-    class Foo: ...
-
-    # Create the parser manually
-    parser = DataclassStruct(Foo)
-    instance = parser.parse(...)
-    ```
-
-2. Use the `@dataclass_struct` decorator to define a new dataclass and automatically create a parser instance that will be assigned as a class attribute:
-
-    ```python
-    from construct_dataclasses import dataclass_struct
-
-    @dataclass_struct
-    class Foo: ...
-
-    # Use the class-parser to parse
-    instance = Foo.parser.parse(...)
-    # or to build
-    data = Foo.parser.build(instance)
-    ```
-
-### Define fields
-
-This module defines a new way how to declare fields of a dataclass. In order to combine the python package construct with python's dataclasses module, this project introduces the following two methods:
-
-- `csfield`: Default definition of a field using a subcon or other dataclass
-
-    ```python
-    @dataclass_struct
-    class ImageHeader:
-        signature: bytes         = csfield(cs.Const(b"BMP"))
-        orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
-    ```
-
-- `subcsfield`: Definition of nested constructs that are contained in list-like structures.
-
-    ```python
-    @dataclass_struct
-    class Image:
-        header: ImageHeader = csfield(ImageHeader) # dataclass reference
-        width: int          = csfield(cs.Int8ub)
-        height: int         = csfield(cs.Int8ub)
-        # Note that we have to convert our dataclass into a struct using
-        # the method "to_struct(...)"
-        pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
-    ```
-
-- `tfield`: a simple typed field that tries to return an instance of the given model class. **Use `subcsfield` for dataclass models and enum types with this function**.
-
-    ```python
-    @dataclass_struct
-    class ImageHeader:
-        orientation: Orientation = tfield(Orientation, cs.Enum(cs.Int8ul, Orientation))
-    ```
-
-
-### Convert dataclasses
-
-By default, all conversion is done automatically if you don't use instances of `SubContruct` classes in your field definitions. If you have to define a subcon that needs a nested subcon, like `Array` or `RepeatUntil` and you would like to parse a dataclass struct, it is required to convert the defined dataclass into a struct.
-
-- `to_struct`: This method converts all fields defined in a dataclass into a single `Struct` or `AlignedStruct` instance.
-
-    ```python
-    @dataclass_struct
-    class Pixel:
-        data: int = csfield(cs.Int8ub)
-
-    pixel_struct: construct.Struct = to_struct(Pixel)
-    ```
-- `to_object`: In order to use data returned by `Struct.parse`, this method can be used to apply this data and create a dataclass object from it.
-
-    ```python
-    data = pixel_struct.parse(b"...")
-    pixel = to_object(data, Pixel)
-    ```
-
-The complete example is shown below:
-
-```python
-# Example modifed from here: https://github.com/timrid/construct-typing/
-import dataclasses
-import enum
-import construct as cs
-
-from construct_dataclasses import dataclass_struct, csfield, to_struct, subcsfield
-
-class Orientation(enum.IntEnum):
-    NONE = 0
-    HORIZONTAL = 1
-    VERTICAL = 2
-
-@dataclass_struct
-class ImageHeader:
-    signature: bytes         = csfield(cs.Const(b"BMP"))
-    orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
-
-@dataclass_struct
-class Pixel:
-    data: int = csfield(cs.Int8ub)
-
-@dataclass_struct
-class Image:
-    header: ImageHeader = csfield(ImageHeader)
-    width: int          = csfield(cs.Int8ub)
-    height: int         = csfield(cs.Int8ub)
-    pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
-
-obj = Image(
-    header=ImageHeader(
-        orientation=Orientation.VERTICAL
-    ),
-    width=3,
-    height=2,
-    pixels=[Pixel(1), Pixel(2), Pixel(3), Pixel(4), Pixel(5), Pixel(6)]
-)
-
-print(Image.parser.build(obj))
-print(Image.parser.parse(b"BMP\x02\x03\x02\x01\x02\x03\x04\x05\06"))
-```
-
-The expected output would be:
-
-    b'BMP\x02\x03\x02\x01\x02\x03\x04\x05\x06'
-    Image(
-        header=ImageHeader(signature=b'BMP', orientation=<Orientation.VERTICAL: 2>),
-        width=3, height=2,
-        pixels=[Pixel(data=1), Pixel(data=2), Pixel(data=3), Pixel(data=4), Pixel(data=5), Pixel(data=6)]
-    )
+Metadata-Version: 2.1
+Name: construct-dataclasses
+Version: 1.1.3
+Summary: enhancement for the python package 'construct' that adds support for dataclasses.
+Home-page: https://github.com/MatrixEditor/construct-dataclasses
+Author: MatrixEditor
+License: GNU GPLv3
+Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,dataclasses
+Platform: POSIX
+Platform: Windows
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# construct-dataclasses
+
+[![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
+![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
+![License](https://img.shields.io:/static/v1?label=License&message=GNU+GPLv3&color=blue)
+[![PyPI](https://img.shields.io/pypi/v/construct-dataclasses)](https://pypi.org/project/construct-dataclasses/)
+
+This small repository is an enhancement of the python package [*construct*](https://pypi.org/project/construct/), which is a powerful tool to declare symmetrical parsers and builders for binary data. This project combines construct with python's dataclasses with support for nested structs.
+
+## Installation
+
+You can install the package via pip or just copy the python file as it is only one.
+
+```bash
+pip install construct-dataclasses
+```
+
+## Usage
+
+More usage examples are placed in the [*examples/*](/examples/) directory.
+
+### Define dataclasses
+
+Before we can start declaring fields on a dataclass, the class itself has to be created. Currently, there are two ways on how to create
+a dataclass usable by this package.
+
+1. Use the standard `@dataclass` decorator and create the parser instance afterwards:
+
+    ```python
+    from construct_dataclasses import DataclassStruct
+
+    @dataclasses.dataclass
+    class Foo: ...
+
+    # Create the parser manually
+    parser = DataclassStruct(Foo)
+    instance = parser.parse(...)
+    ```
+
+2. Use the `@dataclass_struct` decorator to define a new dataclass and automatically create a parser instance that will be assigned as a class attribute:
+
+    ```python
+    from construct_dataclasses import dataclass_struct
+
+    @dataclass_struct
+    class Foo: ...
+
+    # Use the class-parser to parse
+    instance = Foo.parser.parse(...)
+    # or to build
+    data = Foo.parser.build(instance)
+    ```
+
+### Define fields
+
+This module defines a new way how to declare fields of a dataclass. In order to combine the python package construct with python's dataclasses module, this project introduces the following two methods:
+
+- `csfield`: Default definition of a field using a subcon or other dataclass
+
+    ```python
+    @dataclass_struct
+    class ImageHeader:
+        signature: bytes         = csfield(cs.Const(b"BMP"))
+        orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
+    ```
+
+- `subcsfield`: Definition of nested constructs that are contained in list-like structures.
+
+    ```python
+    @dataclass_struct
+    class Image:
+        header: ImageHeader = csfield(ImageHeader) # dataclass reference
+        width: int          = csfield(cs.Int8ub)
+        height: int         = csfield(cs.Int8ub)
+        # Note that we have to convert our dataclass into a struct using
+        # the method "to_struct(...)"
+        pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
+    ```
+
+- `tfield`: a simple typed field that tries to return an instance of the given model class. **Use `subcsfield` for dataclass models and enum types with this function**.
+
+    ```python
+    @dataclass_struct
+    class ImageHeader:
+        orientation: Orientation = tfield(Orientation, cs.Enum(cs.Int8ul, Orientation))
+    ```
+
+
+### Convert dataclasses
+
+By default, all conversion is done automatically if you don't use instances of `SubContruct` classes in your field definitions. If you have to define a subcon that needs a nested subcon, like `Array` or `RepeatUntil` and you would like to parse a dataclass struct, it is required to convert the defined dataclass into a struct.
+
+- `to_struct`: This method converts all fields defined in a dataclass into a single `Struct` or `AlignedStruct` instance.
+
+    ```python
+    @dataclass_struct
+    class Pixel:
+        data: int = csfield(cs.Int8ub)
+
+    pixel_struct: construct.Struct = to_struct(Pixel)
+    ```
+- `to_object`: In order to use data returned by `Struct.parse`, this method can be used to apply this data and create a dataclass object from it.
+
+    ```python
+    data = pixel_struct.parse(b"...")
+    pixel = to_object(data, Pixel)
+    ```
+
+The complete example is shown below:
+
+```python
+# Example modifed from here: https://github.com/timrid/construct-typing/
+import dataclasses
+import enum
+import construct as cs
+
+from construct_dataclasses import dataclass_struct, csfield, to_struct, subcsfield
+
+class Orientation(enum.IntEnum):
+    NONE = 0
+    HORIZONTAL = 1
+    VERTICAL = 2
+
+@dataclass_struct
+class ImageHeader:
+    signature: bytes         = csfield(cs.Const(b"BMP"))
+    orientation: Orientation = csfield(cs.Enum(cs.Int8ub, Orientation))
+
+@dataclass_struct
+class Pixel:
+    data: int = csfield(cs.Int8ub)
+
+@dataclass_struct
+class Image:
+    header: ImageHeader = csfield(ImageHeader)
+    width: int          = csfield(cs.Int8ub)
+    height: int         = csfield(cs.Int8ub)
+    pixels: list[Pixel] = subcsfield(Pixel, cs.Array(this.width * this.height, to_struct(Pixel)))
+
+obj = Image(
+    header=ImageHeader(
+        orientation=Orientation.VERTICAL
+    ),
+    width=3,
+    height=2,
+    pixels=[Pixel(1), Pixel(2), Pixel(3), Pixel(4), Pixel(5), Pixel(6)]
+)
+
+print(Image.parser.build(obj))
+print(Image.parser.parse(b"BMP\x02\x03\x02\x01\x02\x03\x04\x05\06"))
+```
+
+The expected output would be:
+
+    b'BMP\x02\x03\x02\x01\x02\x03\x04\x05\x06'
+    Image(
+        header=ImageHeader(signature=b'BMP', orientation=<Orientation.VERTICAL: 2>),
+        width=3, height=2,
+        pixels=[Pixel(data=1), Pixel(data=2), Pixel(data=3), Pixel(data=4), Pixel(data=5), Pixel(data=6)]
+    )
```

### Comparing `construct-dataclasses-1.1.2/construct_dataclasses.py` & `construct-dataclasses-1.1.3/construct_dataclasses.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,436 +1,439 @@
-# Copyright (C) 2023 MatrixEditor
-
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from __future__ import annotations
-
-import dataclasses
-import inspect
-import textwrap
-import enum
-
-import construct as cs
-
-__all__ = [
-    "csfield",
-    "subcsfield",
-    "dataclass_struct",
-    "tfield",
-    "to_struct",
-    "to_object",
-    "DataclassStruct",
-    "DataclassBitStruct",
-]
-
-
-def subcsfield(
-    model: type,
-    subcon,
-    doc: str | None = None,
-    parsed=None,
-) -> dataclasses.Field:
-    """
-    Helper method to define `cs.Subconstruct` fields in a dataclass that reference another
-    dataclass, e.g.::
-
-        >>> @dataclasses.dataclass
-        >>> class InnerBlob:
-        ...     length: int = csfield(Int8ub)
-        ...
-        >>> @dataclasses.dataclass
-        >>> class Blob:
-        ...     blobs = subcsfield(InnerBlob, Array(3, to_struct(InnerBlob)))
-        ...
-
-    The defined `blobs` field will store a list of `InnerBlob` objects. Note that you have to
-    convert your dataclass into a `Struct` object first, before you can use it with another
-    "Construct" or "SubConstruct". The easiest approach is to use `to_struct(...)` (also exported
-    by this package).
-
-    :param model: the dataclass type
-    :type model: type
-    :param subcon: the sub-construct
-    :type subcon: Construct | SubConstruct
-    :return: the created dataclasses Field
-    :rtype: dataclasses.Field
-    """
-    if not dataclasses.is_dataclass(model):
-        raise TypeError(f"Provided class {model} is not a dataclass!")
-
-    return _process_csfield(
-        model=model,
-        subcon=subcon,
-        doc=doc,
-        parsed=parsed,
-    )
-
-
-def csfield(
-    subcon: cs.Construct | type,
-    doc: str | None = None,
-    parsed=None,
-    depth=None,
-    reverse=False,
-    aligned=None,
-) -> dataclasses.Field:
-    """
-    Helper method for :class:`DataclassStruct` and `DataclassBitStruct` to create dataclass
-    fields based on sub-construct definitions. This method takes a simple construct object
-    or a class type that references another dataclass.
-
-    To apply nested constructs like `Array` or `ReadUntil`, you have to use `subcsfield`
-    with some workarounds.
-
-    Note that the returned dataclasses field will contain the following metadata attributes:
-
-    - `subcon`: The created sub-construct that will be used to create the final `Struct`
-    - `subcon_orig_type`: The original subcon type or dataclass type (if a model is provided)
-
-    :param subcon: the sub-construct or dataclass class reference
-    :type subcon: cs.Construct | type
-    :param doc: additional documentation for the field, defaults to None
-    :type doc: str | None, optional
-    :param depth: the maximum recursion depth (None for infinity), defaults to None
-    :type depth: int | None, optional
-    :param reverse: whether all fields should be processed in reverse order, defaults to False
-    :type reverse: bool, optional
-    :param aligned: argument for `AlignedStruct` objects, defaults to None
-    :type aligned: int, optional
-    :return: the created dataclasses field instance
-    :rtype: dataclasses.Field
-
-    Example::
-
-        >>> @dataclasses.dataclass
-        >>> class BlobHeader:
-        ...     version = csfield(Int32ub)
-        ...     timestamp = csfield(Int32ub)
-        ...
-        >>> @dataclasses.dataclass
-        >>> class Blob:
-        ...     length: int = csfield(Int32ub)
-        ...     header: BlobHeader = csfield(BlobHeader)
-        ...
-    """
-    target_subcon = subcon
-    model = type(subcon)
-    if dataclasses.is_dataclass(subcon):
-        target_subcon = to_struct(subcon, depth, reverse, aligned)
-        model = subcon
-
-    return _process_csfield(
-        model=model,
-        subcon=target_subcon,
-        doc=doc,
-        parsed=parsed,
-    )
-
-def tfield(
-    model: type,
-    subcon: cs.Construct,
-    doc: str | None = None,
-    parsed=None,
-) -> dataclasses.Field:
-    """Creates a typed field. (instance of model will be returned).
-
-    To apply a typed field to dataclasses, use `subcsfield`.
-    """
-    return _process_csfield(model, subcon, doc, parsed)
-
-def _process_csfield(
-    # The model can be the actual model class (dataclass) or the type
-    # of construct used.
-    model,
-    # The subcon stores the actual sub-construct object that will be passed
-    # to the Struct class constructor later on.
-    subcon,
-    doc: str | None = None,
-    parsed=None,
-) -> dataclasses.Field:
-    target_subcon = subcon
-    if (doc is not None) or (parsed is not None):
-        doc = doc or textwrap.dedent(str(doc)).strip("\n")
-        target_subcon = cs.Renamed(target_subcon, newdocs=doc, newparsed=parsed)
-
-    if target_subcon.flagbuildnone is True:
-        init = False
-        default = False
-    else:
-        init = True
-        default = dataclasses.MISSING
-
-    # create default values
-    if isinstance(target_subcon, cs.Const):
-        default = target_subcon.value
-    elif isinstance(target_subcon, cs.Default):
-        if callable(target_subcon.value):
-            default = None
-        else:
-            default = target_subcon.value
-
-    return dataclasses.field(
-        default=default,
-        init=init,
-        metadata={
-            "subcon": target_subcon,
-            "subcon_orig_type": model or type(subcon),
-        },
-    )
-
-
-def to_struct(
-    model: type, depth=None, reverse=False, aligned=None, union=False
-) -> cs.Struct | cs.Union:
-    """Transforms the given dataclass into a construct `Struct` or `Union`.
-
-    :param model: the dataclass class reference
-    :type model: type
-    :param depth: maximum recursion depth, defaults to None
-    :type depth: int, optional
-    :param reverse: whether fields should be processed in reverse order, defaults to False
-    :type reverse: bool, optional
-    :param aligned: whether aligned struct should be created from the "aligned" value, defaults to None
-    :type aligned: int, optional
-    :raises TypeError: if the given model is not a dataclass class
-    :return: the created struct instance
-    :rtype: construct.Struct
-    """
-    if isinstance(model, cs.Construct):
-        # not sure if we want to do that
-        return model
-
-    if not inspect.isclass(model) or not dataclasses.is_dataclass(model):
-        raise TypeError("Model must be a dataclass!")
-
-    return _to_struct_inner(
-        model, max_depth=depth, reverse=reverse, aligned=aligned, union=union
-    )
-
-
-def _to_struct_inner(
-    obj, max_depth=None, depth=0, reverse=False, aligned=None, union=False
-):
-    if dataclasses.is_dataclass(obj):
-        fields = dataclasses.fields(obj)
-        if reverse:
-            fields = reversed(fields)
-
-        subcon_fields = {}
-        for dc_field in fields:
-            if (max_depth is not None and depth < max_depth) or max_depth is None:
-                cs_field = _to_struct_inner(
-                    dc_field.metadata["subcon"], max_depth, depth + 1, reverse
-                )
-            else:
-                cs_field = dc_field.metadata["subcon"]
-
-            subcon_fields[dc_field.name] = cs_field
-        if aligned is not None:
-            return cs.AlignedStruct(aligned, **subcon_fields)
-
-        if union:
-            return cs.Union(**subcon_fields)
-
-        return cs.Struct(**subcon_fields)
-
-    elif isinstance(obj, cs.Construct):
-        return obj
-
-
-def to_object(obj: cs.Container | cs.ListContainer, model: type):
-    """Converts a parsed container back into a dataclass object.
-
-    :param obj: the parsed data
-    :type obj: cs.Container | cs.ListContainer
-    :param model: the type of which an instance should be created
-    :type model: type
-    :raises TypeError: if the given model is not a dataclass
-    :return: the created instance
-    """
-    if not dataclasses.is_dataclass(model):
-        raise TypeError(f"The class <{model}> is not a dataclass!")
-
-    fields = dataclasses.fields(model)
-    # We first have to extract all fields that are needed to instantiate
-    # the model class.
-    init_fields = {}
-    for dc_field in fields:
-        if dc_field.init:
-            if isinstance(obj, cs.ListContainer):
-                value = [_to_object_inner(x, dc_field) for x in obj]
-            else:
-                value = obj.get(dc_field.name) if obj is not None else None
-            init_fields[dc_field.name] = _to_object_inner(value, dc_field)
-
-    instance = model(**init_fields)
-    # Now we can apply all other fields
-    for dc_field in fields:
-        if not dc_field.init:
-            if isinstance(obj, cs.ListContainer):
-                value = [_to_object_inner(x, dc_field) for x in obj]
-            else:
-                value = obj.get(dc_field.name) if obj is not None else None
-            setattr(instance, dc_field.name, _to_object_inner(value, dc_field))
-
-    return instance
-
-
-def _to_object_inner(value, field: dataclasses.Field):
-    # Check if we have an inner struct first
-    subcon_type = field.metadata["subcon_orig_type"]
-    field_type = field.type
-    if isinstance(field_type, str):
-        # normal type annotations are stored as string
-        field_type = subcon_type
-
-    if isinstance(value, cs.ListContainer):
-        return list(map(lambda x: _to_object_inner(x, field), value))
-    elif dataclasses.is_dataclass(subcon_type):
-        return to_object(value, subcon_type)
-    elif isinstance(value, cs.EnumIntegerString):
-        # Allow list declarations of enum values. If there is a type hint
-        # with a list-like type, we can take the first type argument and use
-        # it as our enum type
-        if hasattr(field_type, "__origin__") and issubclass(
-            field_type.__origin__, list
-        ):
-            (field_type,) = field_type.__args__
-
-        if issubclass(field_type, enum.IntEnum):
-            # Search for enum value within defined ones
-            for enum_val in field_type:
-                if enum_val.value == value.intvalue:
-                    return enum_val
-
-        else:
-            return value.intvalue
-
-    return value
-
-
-def _process_struct_dataclass(
-    cls, bitwise=False, depth=None, reverse=False, union=False
-):
-    new_cls = dataclasses.dataclass(cls)
-    if hasattr(new_cls, "parser"):
-        raise ValueError(
-            f"Invalid field definition: field 'parser' alredy exists in class {new_cls}"
-        )
-
-    if hasattr(new_cls, "struct"):
-        raise ValueError(
-            f"Invalid field definition: field 'struct' alredy exists in class {new_cls}"
-        )
-
-
-    if bitwise:
-        ds_struct = DataclassBitStruct(cls, depth, reverse, union=union)
-    else:
-        ds_struct = DataclassStruct(cls, depth, reverse, union=union)
-
-    setattr(new_cls, "parser", ds_struct)
-    setattr(new_cls, "struct", ds_struct.subcon)
-    return new_cls
-
-
-def dataclass_struct(cls, /, *, bitwise=False, depth=None, reverse=False, union=False):
-    """Creates a dataclass that stores a class-parser instance.
-
-    Example::
-
-        >>> @dataclass_struct
-        ... class Blob:
-        ...     length: int = csfield(cs.Int8ul)
-        ...     data: bytes = csfield(cs.Bytes(cs.this.length))
-        ...
-        >>> b = Blob.parser.parse(b"\\x05\\x00\\x00\\x00\\x00\\x00")
-        >>> Blob.parser.build(b)
-        b'\\x05\\x00\\x00\\x00\\x00\\x00'
-
-    :param bitwise: whether the struct should run bitwise, defaults to False
-    :type bitwise: bool, optional
-    :param depth: the maximum recursion depth, defaults to None
-    :type depth: int, optional
-    :param reverse: tells the builder to parse fields in reverse order, defaults to False
-    :type reverse: bool, optional
-    :param union: whether the struct should be treated as a union, defaults to False
-    :type union: bool, optional
-    """
-
-    def wrap(cls):
-        # Make dataclass and create parser instance
-        return _process_struct_dataclass(
-            cls, bitwise=bitwise, depth=depth, reverse=reverse, union=union
-        )
-
-    # See if we're being called as @struct or @struct().
-    if cls is None:
-        return wrap
-
-    return wrap(cls)
-
-
-class DataclassStruct(cs.Adapter):
-    """Adapter for dataclasses structs.
-
-    :param model: the defined dataclasses class
-    :type model: type
-    :param depth: maximum recursion depth when creating structs, defaults to None
-    :type depth: int, optional
-    :param reverse: whether fields should be processed in reverse order, defaults to False
-    :type reverse: bool, optional
-
-    Example taken from "construct_typed"::
-
-    >>> import dataclasses
-    >>> from construct import Bytes, Int8ub, this
-    >>> from construct_dataclasses import DataclassStruct, csfield
-    >>> @dataclasses.dataclass
-    ... class Image:
-    ...     width: int = csfield(Int8ub)
-    ...     height: int = csfield(Int8ub)
-    ...     pixels: bytes = csfield(Bytes(this.height * this.width))
-    ...
-    >>> ds = DataclassStruct(Image)
-    >>> ds.parse(b"\x01\x0212")
-    Image(width=1, height=2, pixels=b'12')
-    """
-
-    def __init__(
-        self, model: type, depth=None, reverse=False, aligned=None, union=False
-    ) -> None:
-        self.model = model
-        if not dataclasses.is_dataclass(self.model):
-            raise TypeError(f"The class {self.model} is not a dataclass!")
-
-        self.reverse = reverse
-        self.depth = depth
-        self.aligned = aligned
-        self.union = union
-        super().__init__(
-            to_struct(self.model, self.depth, self.reverse, self.aligned, self.union)
-        )
-
-    def _decode(self, obj: cs.Container, context: cs.Context, path: cs.PathType):
-        return to_object(obj, self.model)
-
-    def _encode(self, obj, context: cs.Context, path: cs.PathType) -> dict:
-        if not dataclasses.is_dataclass(obj):
-            raise TypeError(f"Model class <{type(obj)}> is not a dataclass!")
-
-        return dataclasses.asdict(obj)
-
-
-def DataclassBitStruct(model: type, depth=None, reverse=False, union=False):
-    """Makes a DataclassStruct inside a Bitwise."""
-    return cs.Bitwise(DataclassStruct(model, depth, reverse, union))
+# Copyright (C) 2023 MatrixEditor
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
+
+import dataclasses
+import inspect
+import textwrap
+import enum
+
+import construct as cs
+
+__all__ = [
+    "csfield",
+    "subcsfield",
+    "dataclass_struct",
+    "tfield",
+    "to_struct",
+    "to_object",
+    "DataclassStruct",
+    "DataclassBitStruct",
+]
+
+
+def subcsfield(
+    model: type,
+    subcon,
+    doc: str | None = None,
+    parsed=None,
+) -> dataclasses.Field:
+    """
+    Helper method to define `cs.Subconstruct` fields in a dataclass that reference another
+    dataclass, e.g.::
+
+        >>> @dataclasses.dataclass
+        >>> class InnerBlob:
+        ...     length: int = csfield(Int8ub)
+        ...
+        >>> @dataclasses.dataclass
+        >>> class Blob:
+        ...     blobs = subcsfield(InnerBlob, Array(3, to_struct(InnerBlob)))
+        ...
+
+    The defined `blobs` field will store a list of `InnerBlob` objects. Note that you have to
+    convert your dataclass into a `Struct` object first, before you can use it with another
+    "Construct" or "SubConstruct". The easiest approach is to use `to_struct(...)` (also exported
+    by this package).
+
+    :param model: the dataclass type
+    :type model: type
+    :param subcon: the sub-construct
+    :type subcon: Construct | SubConstruct
+    :return: the created dataclasses Field
+    :rtype: dataclasses.Field
+    """
+    if not dataclasses.is_dataclass(model):
+        raise TypeError(f"Provided class {model} is not a dataclass!")
+
+    return _process_csfield(
+        model=model,
+        subcon=subcon,
+        doc=doc,
+        parsed=parsed,
+    )
+
+
+def csfield(
+    subcon: cs.Construct | type,
+    doc: str | None = None,
+    parsed=None,
+    depth=None,
+    reverse=False,
+    aligned=None,
+) -> dataclasses.Field:
+    """
+    Helper method for :class:`DataclassStruct` and `DataclassBitStruct` to create dataclass
+    fields based on sub-construct definitions. This method takes a simple construct object
+    or a class type that references another dataclass.
+
+    To apply nested constructs like `Array` or `ReadUntil`, you have to use `subcsfield`
+    with some workarounds.
+
+    Note that the returned dataclasses field will contain the following metadata attributes:
+
+    - `subcon`: The created sub-construct that will be used to create the final `Struct`
+    - `subcon_orig_type`: The original subcon type or dataclass type (if a model is provided)
+
+    :param subcon: the sub-construct or dataclass class reference
+    :type subcon: cs.Construct | type
+    :param doc: additional documentation for the field, defaults to None
+    :type doc: str | None, optional
+    :param depth: the maximum recursion depth (None for infinity), defaults to None
+    :type depth: int | None, optional
+    :param reverse: whether all fields should be processed in reverse order, defaults to False
+    :type reverse: bool, optional
+    :param aligned: argument for `AlignedStruct` objects, defaults to None
+    :type aligned: int, optional
+    :return: the created dataclasses field instance
+    :rtype: dataclasses.Field
+
+    Example::
+
+        >>> @dataclasses.dataclass
+        >>> class BlobHeader:
+        ...     version = csfield(Int32ub)
+        ...     timestamp = csfield(Int32ub)
+        ...
+        >>> @dataclasses.dataclass
+        >>> class Blob:
+        ...     length: int = csfield(Int32ub)
+        ...     header: BlobHeader = csfield(BlobHeader)
+        ...
+    """
+    target_subcon = subcon
+    model = type(subcon)
+    if dataclasses.is_dataclass(subcon):
+        target_subcon = to_struct(subcon, depth, reverse, aligned)
+        model = subcon
+
+    return _process_csfield(
+        model=model,
+        subcon=target_subcon,
+        doc=doc,
+        parsed=parsed,
+    )
+
+def tfield(
+    model: type,
+    subcon: cs.Construct,
+    doc: str | None = None,
+    parsed=None,
+) -> dataclasses.Field:
+    """Creates a typed field. (instance of model will be returned).
+
+    To apply a typed field to dataclasses, use `subcsfield`.
+    """
+    return _process_csfield(model, subcon, doc, parsed)
+
+def _process_csfield(
+    # The model can be the actual model class (dataclass) or the type
+    # of construct used.
+    model,
+    # The subcon stores the actual sub-construct object that will be passed
+    # to the Struct class constructor later on.
+    subcon,
+    doc: str | None = None,
+    parsed=None,
+) -> dataclasses.Field:
+    target_subcon = subcon
+    if (doc is not None) or (parsed is not None):
+        doc = doc or textwrap.dedent(str(doc)).strip("\n")
+        target_subcon = cs.Renamed(target_subcon, newdocs=doc, newparsed=parsed)
+
+    if target_subcon.flagbuildnone is True:
+        init = False
+        default = False
+    else:
+        init = True
+        default = dataclasses.MISSING
+
+    # create default values
+    if isinstance(target_subcon, cs.Const):
+        default = target_subcon.value
+    elif isinstance(target_subcon, cs.Default):
+        if callable(target_subcon.value):
+            default = None
+        else:
+            default = target_subcon.value
+
+    return dataclasses.field(
+        default=default,
+        init=init,
+        metadata={
+            "subcon": target_subcon,
+            "subcon_orig_type": model or type(subcon),
+        },
+    )
+
+
+def to_struct(
+    model: type, depth=None, reverse=False, aligned=None, union=False
+) -> cs.Struct | cs.Union:
+    """Transforms the given dataclass into a construct `Struct` or `Union`.
+
+    :param model: the dataclass class reference
+    :type model: type
+    :param depth: maximum recursion depth, defaults to None
+    :type depth: int, optional
+    :param reverse: whether fields should be processed in reverse order, defaults to False
+    :type reverse: bool, optional
+    :param aligned: whether aligned struct should be created from the "aligned" value, defaults to None
+    :type aligned: int, optional
+    :raises TypeError: if the given model is not a dataclass class
+    :return: the created struct instance
+    :rtype: construct.Struct
+    """
+    if isinstance(model, cs.Construct):
+        # not sure if we want to do that
+        return model
+
+    if not inspect.isclass(model) or not dataclasses.is_dataclass(model):
+        raise TypeError("Model must be a dataclass!")
+
+    return _to_struct_inner(
+        model, max_depth=depth, reverse=reverse, aligned=aligned, union=union
+    )
+
+
+def _to_struct_inner(
+    obj, max_depth=None, depth=0, reverse=False, aligned=None, union=False
+):
+    if dataclasses.is_dataclass(obj):
+        fields = dataclasses.fields(obj)
+        if reverse:
+            fields = reversed(fields)
+
+        subcon_fields = {}
+        for dc_field in fields:
+            if (max_depth is not None and depth < max_depth) or max_depth is None:
+                cs_field = _to_struct_inner(
+                    dc_field.metadata["subcon"], max_depth, depth + 1, reverse
+                )
+            else:
+                cs_field = dc_field.metadata["subcon"]
+
+            subcon_fields[dc_field.name] = cs_field
+        if aligned is not None:
+            return cs.AlignedStruct(aligned, **subcon_fields)
+
+        if union:
+            return cs.Union(**subcon_fields)
+
+        return cs.Struct(**subcon_fields)
+
+    elif isinstance(obj, cs.Construct):
+        return obj
+
+
+def to_object(obj: cs.Container | cs.ListContainer, model: type):
+    """Converts a parsed container back into a dataclass object.
+
+    :param obj: the parsed data
+    :type obj: cs.Container | cs.ListContainer
+    :param model: the type of which an instance should be created
+    :type model: type
+    :raises TypeError: if the given model is not a dataclass
+    :return: the created instance
+    """
+    if not dataclasses.is_dataclass(model):
+        raise TypeError(f"The class <{model}> is not a dataclass!")
+
+    if obj is None: # support optional types
+        return None
+
+    fields = dataclasses.fields(model)
+    # We first have to extract all fields that are needed to instantiate
+    # the model class.
+    init_fields = {}
+    for dc_field in fields:
+        if dc_field.init:
+            if isinstance(obj, cs.ListContainer):
+                value = [_to_object_inner(x, dc_field) for x in obj]
+            else:
+                value = obj.get(dc_field.name)
+            init_fields[dc_field.name] = _to_object_inner(value, dc_field)
+
+    instance = model(**init_fields)
+    # Now we can apply all other fields
+    for dc_field in fields:
+        if not dc_field.init:
+            if isinstance(obj, cs.ListContainer):
+                value = [_to_object_inner(x, dc_field) for x in obj]
+            else:
+                value = obj.get(dc_field.name)
+            setattr(instance, dc_field.name, _to_object_inner(value, dc_field))
+
+    return instance
+
+
+def _to_object_inner(value, field: dataclasses.Field):
+    # Check if we have an inner struct first
+    subcon_type = field.metadata["subcon_orig_type"]
+    field_type = field.type
+    if isinstance(field_type, str):
+        # normal type annotations are stored as string
+        field_type = subcon_type
+
+    if isinstance(value, cs.ListContainer):
+        return list(map(lambda x: _to_object_inner(x, field), value))
+    elif dataclasses.is_dataclass(subcon_type):
+        return to_object(value, subcon_type)
+    elif isinstance(value, cs.EnumIntegerString):
+        # Allow list declarations of enum values. If there is a type hint
+        # with a list-like type, we can take the first type argument and use
+        # it as our enum type
+        if hasattr(field_type, "__origin__") and issubclass(
+            field_type.__origin__, list
+        ):
+            (field_type,) = field_type.__args__
+
+        if issubclass(field_type, enum.IntEnum):
+            # Search for enum value within defined ones
+            for enum_val in field_type:
+                if enum_val.value == value.intvalue:
+                    return enum_val
+
+        else:
+            return value.intvalue
+
+    return value
+
+
+def _process_struct_dataclass(
+    cls, bitwise=False, depth=None, reverse=False, union=False
+):
+    new_cls = dataclasses.dataclass(cls)
+    if hasattr(new_cls, "parser"):
+        raise ValueError(
+            f"Invalid field definition: field 'parser' alredy exists in class {new_cls}"
+        )
+
+    if hasattr(new_cls, "struct"):
+        raise ValueError(
+            f"Invalid field definition: field 'struct' alredy exists in class {new_cls}"
+        )
+
+
+    if bitwise:
+        ds_struct = DataclassBitStruct(cls, depth, reverse, union=union)
+    else:
+        ds_struct = DataclassStruct(cls, depth, reverse, union=union)
+
+    setattr(new_cls, "parser", ds_struct)
+    setattr(new_cls, "struct", ds_struct.subcon)
+    return new_cls
+
+
+def dataclass_struct(cls=None, /, *, bitwise=False, depth=None, reverse=False, union=False):
+    """Creates a dataclass that stores a class-parser instance.
+
+    Example::
+
+        >>> @dataclass_struct
+        ... class Blob:
+        ...     length: int = csfield(cs.Int8ul)
+        ...     data: bytes = csfield(cs.Bytes(cs.this.length))
+        ...
+        >>> b = Blob.parser.parse(b"\\x05\\x00\\x00\\x00\\x00\\x00")
+        >>> Blob.parser.build(b)
+        b'\\x05\\x00\\x00\\x00\\x00\\x00'
+
+    :param bitwise: whether the struct should run bitwise, defaults to False
+    :type bitwise: bool, optional
+    :param depth: the maximum recursion depth, defaults to None
+    :type depth: int, optional
+    :param reverse: tells the builder to parse fields in reverse order, defaults to False
+    :type reverse: bool, optional
+    :param union: whether the struct should be treated as a union, defaults to False
+    :type union: bool, optional
+    """
+
+    def wrap(cls):
+        # Make dataclass and create parser instance
+        return _process_struct_dataclass(
+            cls, bitwise=bitwise, depth=depth, reverse=reverse, union=union
+        )
+
+    # See if we're being called as @struct or @struct().
+    if cls is None:
+        return wrap
+
+    return wrap(cls)
+
+
+class DataclassStruct(cs.Adapter):
+    """Adapter for dataclasses structs.
+
+    :param model: the defined dataclasses class
+    :type model: type
+    :param depth: maximum recursion depth when creating structs, defaults to None
+    :type depth: int, optional
+    :param reverse: whether fields should be processed in reverse order, defaults to False
+    :type reverse: bool, optional
+
+    Example taken from "construct_typed"::
+
+    >>> import dataclasses
+    >>> from construct import Bytes, Int8ub, this
+    >>> from construct_dataclasses import DataclassStruct, csfield
+    >>> @dataclasses.dataclass
+    ... class Image:
+    ...     width: int = csfield(Int8ub)
+    ...     height: int = csfield(Int8ub)
+    ...     pixels: bytes = csfield(Bytes(this.height * this.width))
+    ...
+    >>> ds = DataclassStruct(Image)
+    >>> ds.parse(b"\x01\x0212")
+    Image(width=1, height=2, pixels=b'12')
+    """
+
+    def __init__(
+        self, model: type, depth=None, reverse=False, aligned=None, union=False
+    ) -> None:
+        self.model = model
+        if not dataclasses.is_dataclass(self.model):
+            raise TypeError(f"The class {self.model} is not a dataclass!")
+
+        self.reverse = reverse
+        self.depth = depth
+        self.aligned = aligned
+        self.union = union
+        super().__init__(
+            to_struct(self.model, self.depth, self.reverse, self.aligned, self.union)
+        )
+
+    def _decode(self, obj: cs.Container, context: cs.Context, path: cs.PathType):
+        return to_object(obj, self.model)
+
+    def _encode(self, obj, context: cs.Context, path: cs.PathType) -> dict:
+        if not dataclasses.is_dataclass(obj):
+            raise TypeError(f"Model class <{type(obj)}> is not a dataclass!")
+
+        return dataclasses.asdict(obj)
+
+
+def DataclassBitStruct(model: type, depth=None, reverse=False, union=False):
+    """Makes a DataclassStruct inside a Bitwise."""
+    return cs.Bitwise(DataclassStruct(model, depth, reverse, union))
```

