# More Modest

## Overview

More Modest is the next generation version of an old blog engine I
wrote called modest. Instead of some complicated Python script with
lots of dependencies, More Modest utilizes tools you probably already
have.

## Install

1. Install [discount][]
2. Clone/fork this repo and type `make run`

### Requirements

This has only been tested on GNU/Linux with the following:

* GNU Make 4.0
* Discount 2.1.6
* GNU bash 4.3.18
* GNU awk 4.1.1
* GNU sed 4.2.2

## Customization

The Makefile has some variables in there, which specify where to find
files, and what to stick in the generated [ATOM]() feed. If you have
a non-standard, i.e., it's not in your shell's `PATH`, location for 
discount's `theme` executable, edit the `THEME` variable.

Template files are in the `$THEMEDIR`, which defaults to `theme/`. Posts
and pages, go in `$SRCDIR`, and things get built to `$BUILDDIR`.

Static files default to `$SRCDIR/static`. The directory gets copied
verbatim into `$BUILDDIR/static`

## Authors

Andrew Gwozdziewycz <web@apgwoz.com>

## Contributors

Wub TheCaptain

## Copyright

Copyright 2014, Andrew Gwozdziewycz, <web@apgwoz.com>

Licensed under the GNU GPLv3. See LICENSE for more details



[discount]: http://www.pell.portland.or.us/~orc/Code/discount/
[ATOM]: http://atompub.org/
