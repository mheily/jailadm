# jailadm

## Synopsis

A jail manager for FreeBSD

## Overview

jailadm is a port of the OpenSolaris zone management utilities to FreeBSD.
It can be used to manage FreeBSD jails using the same commands that one
would use to manage Solaris zones.

There are two commands for managing jails:
 * [jailadm(8)](man/jailadm.8.txt) - control a jail; start, stop, create, destroy, etc.
 * [jailcfg(8)](man/jailcfg.8.txt) - configure a jail

See the manpages linked above for more details about each command.

## Current status

- The manpages and source code have been imported from Illumos
- The manpages have been adjusted to document FreeBSD jails instead of Solaris zones

** WARNING ** This is pre-alpha code; it does not compile or do anything useful.

## Licensing

This project is licensed under the Common Development and Distribution License (CDDL).

See the COPYING file for the complete terms of the license.


## Credits

The jailadm project was created by Mark Heily <mark@heily.com>.

The source code for the original Illumos zoneadm/zonecfg commands
were copied from https://github.com/illumos/illumos-gate.git
