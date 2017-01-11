# Linux Distributions

This module provides brief and editorial introductions to selected Linux
distributions.


## Debian

Debian exhibits a strong focus on proliferation and promotion of free
(as in speech) software and is widely regarded as a reliable Linux
distribution well suited to production server environments.
The Debian Free Software Guidelines
[(DFSG)](https://www.debian.org/social_contract#guidelines Debian Free
Software Guidelines)
outline the social contract necessary for software to be included in the
Debian distribution (main) while other packages may be maintained in
a compatible form (non-free or contrib) but are not considered part of
the Debian distribution proper.
The Debian reputation for stability is legendary and is typified by its
organization into stable, testing, and unstable releases where
the lifetime of a new feature progresses from introduction and bug
fixing in unstable, through maturation and code freeze within testing,
and finally transitions to stable where the security team is focused
on ensuring that security updates and threats to stability are
identified and addressed in a timely fashion.

### Debian Releases

The current stable release is version 8 codenamed `jessie` (10jan2017)
and exists within a maintenance stage of its lifecycle where the main
focus is on backporting security updates. Packages available in stable
tend to remain available for a long period of time, on the order of the
lifetime of a server. Users are encouraged to install stable where
possible for the most consistent and reliable experience with Debian.

The current testing release is named `stretch` (10jan2017) and contains
packages which have not yet been incorporated into stable but are 
progressing along the release lifecycle to a point where the entire
testing release will transition to stable.
Packages available in testing are less likely to be reverted to
an earlier version than those in unstable and typically see multiple
rounds of bug fixing and updates out of unstable before being a code
freeze and verification phase leading into progression of this release
to stable which will mark the previous stable release as obsolete.
The testing distribution tends to have fairly recent packages and
typically goes multiple years before transitioning into stable.

The current unstable release is always named `sid` and represents the
current development snapshot of Debian and as such may change daily
or many times in a day as packages are updated, reverted, removed, or
tested. Unlike other releases, the name `sid` sticks with unstable and
many desktop users may find unstable is tricky to use for daily work
due to its rapidly changing nature.

[Jessie Wheezy Sarge](https://mat.exon.name/releasepics/)
[Testing to Release](https://www.lucas-nussbaum.net/blog/?p=775)

### Distributions Derived from Debian

Many distributions are derived in some way from Debian including the
well known Ubuntu and Knoppix distributions and the Debian family tree
is quite impressive if you are inclined to learn more about this topic.

As a more progressive and up-to-date distribution which cut it's teeth
with desktop Linux users Ubuntu tends to derive from Debian testing and
unstable releases whereas packages included in stable would tend to be
lack the new features that Ubuntu target userbase looks for.

[List of Linux
Distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)

### Debian Package Management

The Debian package format (.deb) and package manager (dpkg) have a long
history of solid dependency management and have been made more
accessible through the advent of apt.

### New in Debian 7

Listed among the wheezy release notes are the following updates:
* Multiarch support - install packages for multiple architectures, side
by side, on the same system
* AppArmor - mandatory access controls for application isolation and
sandboxing
* LSB header stanza based dependency sequencing of sysvinit scripts
enabled by default
* Many packages are now build with GCC hardening flags enabled 
* GNOME 3 - update from GNOME 2 in Debian 6 `squeeze`
* GNOME support for Network Manager
* OpenStack and XenCloudPlatform support
* Consolidation of tempfs under /run
* /tmp is not tmpfs by default
* Tech preview of systemd replacement for sysvinit
