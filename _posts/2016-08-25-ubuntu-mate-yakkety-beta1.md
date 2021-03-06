---
layout: blog-post
class: blog
title: Ubuntu MATE 16.10 Beta 1
permalink: /blog/ubuntu-mate-yakkety-beta1/
description: Ubuntu MATE 16.10 (Yakkety Yak) Beta 1
category: dev
author: Martin Wimpress
lang: en
discourse_topic_id: 21317
---

We are underwhelmed to announce, quite possibly, our most uninteresting
beta release *E-V-E-R!* `;-)` This beta release is all about the
plumbing that transitions Ubuntu MATE to GTK 3.20. It really isn't very
interesting from an end-users perspective.

From this point forward we'll be focusing on fixing as many issues as
we can on the lead up to Beta 2 and the final release of Ubuntu MATE
16.10. The 16.10 development cycle was all about the migration to GTK3+
and creating the new foundations upon which to build our
*"retrospective future"*.

We are preparing Ubuntu MATE 16.10 (Yakkety Yak) for distribution on
[October 13th, 2016](https://wiki.ubuntu.com/YakketyYak/ReleaseSchedule)
With this *Beta* pre-release, you can see what we are trying out in
preparation for our next (stable) version.

{:.center}
![Ubuntu MATE 16.10 Beta 1](/images/blog/ubuntu-mate-1610-beta1.png)
**As is now customary, our release artwork was made by <a href="https://www.youtube.com/channel/UCglkWuyZDppWD2BVsyI4r3A" target="_blank"><i>Ghost Sixtyseven</i></a>.**

## What works?

People tell us that Ubuntu MATE is stable. You may, or may not, agree.

Ubuntu MATE *Beta Releases* are *NOT* recommended for:

  * Regular users who are not aware of pre-release issues
  * Anyone who needs a stable system
  * Anyone uncomfortable running a possibly frequently broken system
  * Anyone in a production environment with data or workflows that need to be reliable

Ubuntu MATE *Beta Releases* are recommended for:

  * Regular users who want to help us test by finding, reporting, and/or fixing bugs
  * Ubuntu MATE, MATE, and GTK+ developers

## What changed since the Ubuntu MATE 16.10 Alpha 2 release?

This is what has been added, updated or removed.

  * **Migrated to GTK 3.20**
    * This has been a huge undertaking and was only made possible
    thanks to the Ubuntu MATE [crowd funding](/sponsors/) which has
    funded the updating of the Ubuntu MATE themes and some upstream
    GTK3+ porting.
  * Updated to **MATE Dock Applet 0.74**
    * Which didn't make the iso image, but will be immediately available as an update.
  * Updated many MATE packages for **improved GTK 3.20 support**
    * `caja` 1.14.2
    * `mate-settings-daemon` 1.14.1
    * `mate-session-manager` 1.14.1
    * `mate-panel` 1.14.2
    * `mate-control-center` 1.14.1
    * `mate-media` 1.14.1
    * `mate-system-monitor` 1.14.1
    * `atril` 1.14.2
    * `caja-extensions` 1.14.1
    * `eom` 1.14.2
    * `mate-applets` 1.14.1
    * `mate-terminal` 1.14.1
    * `mate-utils` 1.14.1
    * `pluma` 1.14.1
  * Rebuilt a few MATE package for **improved GTK 3.20 support**
    * `mate-notification-daemon`
    * `mate-screen-saver`
    * `mate-power-manager`
  * Removed **MATE Heads-Up Display (HUD)**
    * Testing during Alpha 2 revealed some show stopping issues. **We will revisit this feature in 17.04**.
    * If you installed Ubuntu MATE 16.10 prior to Beta 1 then please `sudo apt purge mate-hud`.

{% include blog/jumbotron.html
    title = "Download Ubuntu MATE 16.10"
    text = "Join the fun and experience a retrospective future."
    button_text = "Download"
    button_url = "/download/"
%}

## Known Issues

Here are the known issues.

### Ubuntu MATE issues

  * MATE Tweak will segfault when switching to Compiz due to a `gsettings` schema change in Metacity.
    * A fix has already been commited and an updated package will land soon after Beta 1.
  * Weather reports in the Clock and Weather applets are currently unavailable.
    * A fix has already been commited and an updated package will land soon after Beta 1.

  * The Mutiny theme can be unstable, updates to fix this will land soon after Beta 1.
    * Updates for **topmenu-gtk 0.3 package which now has GTK3+ support for MATE Desktop**.
  * Some GTK3+ theming is incorrect.
    * The remaining theming issues will be addressed over on the lead up to Beta 2.

### Ubuntu family issues

This is our known list of bugs that affect all flavours.

  * Choosing an Entire Disk install on PowerPC may result in an unbootable system.
    * The work around is to manually partition your hard disk.
    * [#1606089](https://bugs.launchpad.net/bugs/1606089),
    [#1607128](https://bugs.launchpad.net/bugs/1607128)

  * R300 GPU accelerated graphics do not work on PowerPC
    * [#1432949](https://bugs.launchpad.net/bugs/1432949),
    [#1575391](https://bugs.launchpad.net/bugs/1575391)

  * Ubiquity installer Slideshows and Ubuntu MATE Welcome display a blank window on PowerPC. This is due to a bug in WebKit 2.
    * [#1561573](https://bugs.launchpad.net/bugs/1561573),
    [#1597764](https://bugs.launchpad.net/bugs/1597764)

  * Running Linux on PowerPC can require some tinkering and the following are useful references.
    * [PowerPC Known Issues](https://wiki.ubuntu.com/PowerPCKnownIssues)
    * [PowerPC FAQ](https://wiki.ubuntu.com/PowerPCFAQ)

You'll also want to check the Ubuntu MATE bug tracker to see what has already
been reported. These issues will be addressed in due course.

  * [Ubuntu MATE Bug Tracker](https://bugs.launchpad.net/ubuntu-mate)

## Feedback

Is there anything you can help with or want to be involved in? Maybe you just
want to discuss your experiences or ask the maintainers some questions. Please
[come and talk to us](https://ubuntu-mate.community/).
