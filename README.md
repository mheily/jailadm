# jailadm

## Synopsis

A jail manager for FreeBSD.

## Overview

jailadm is a port of the OpenSolaris zone management utilities to FreeBSD.
It can be used to manage FreeBSD jails using the same commands that one
would use to manage Solaris zones.

There are two commands for managing jails:
 * [jailadm(8)](https://raw.githubusercontent.com/mheily/jailadm/master/man/jailadm.8.txt) - control a jail; start, stop, create, destroy, etc.
 * [jailcfg(8)](https://raw.githubusercontent.com/mheily/jailadm/master/man/jailcfg.8.txt) - configure a jail

See the manpages linked above for more details about each command.

## Goals

* Develop a jail manager that uses [launchd(8)](https://github.com/mheily/relaunchd) as the backend.
* Deprecate the jail(8) command in the FreeBSD base system, and import jailadm(8) and jailcfg(8)
into the base system as the officially supported jail manager.  The jail(8) command should be 
removed from FreeBSD in a future release.

## Current status

- The manpages and source code have been imported from Illumos
- The manpages have been adjusted to document FreeBSD jails instead of Solaris zones

** WARNING ** This is pre-alpha code; it does not compile or do anything useful.

## Licensing

The manual pages and Illumos source code is licensed under the Common Development and Distribution License (CDDL).

See the COPYING file for the complete terms of the license.

## Credits

The jailadm project was created by Mark Heily <mark@heily.com>.

The source code for the original Illumos zoneadm/zonecfg commands
were copied from https://github.com/illumos/illumos-gate.git
