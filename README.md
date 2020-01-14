# mfe20
----
 [MEDNAFEN](http://mednafen.sourceforge.net/) is a multi-console rewinding game emulator that is being developed actively. its launching is not trivial, so it needs a frontend wrapper
 
![mfe logo](resources/mfe.png)
 https://github.com/hristoast/mfe is one of them, but it is late for several steps from contemporary phase of MEDNAFEN.
this is a derivative work for mednafen wrapper. 

![mfe logo](resources/mfe.png)

A GUI frontend for [mednafen](http://mednafen.sourceforge.net/).

Originally by Jordan Callicoat,
forked for modern systems by me.

## Installation

First, install the dependencies. On Debian-like systems this should suffice:

    apt-get install python mednafen python-gtk2 python-glade2 python-configobj

Then, as a privileged user:

    make install

This will install the executable `mfe`, just launch that and game away!

If you are on a Debian system you can create a .deb installer:

    make deb

This will create a .deb package in `..`, you can install that to add `mfe` to your package management system

## Uninstall

To uninstall `mfe`, as a privileged user:

    make uninstall

If you've created a deb, you'll need to run this (also as a privileged user):

    apt-get purge mednafenfe

And that's it.

## FAQ

Q) I don't have any sound!

A) Use the 'sdl' audio backend.
