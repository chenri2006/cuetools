# cuetools [![Build Status](https://travis-ci.org/svend/cuetools.svg?branch=master)](https://travis-ci.org/svend/cuetools)

cue and toc file parsers and utilities

https://github.com/svend/cuetools

Copyright (C) 2004, 2005, 2006, 2007, 2013 Svend Sorensen

cuetools is a set of utilities for working with Cue Sheet (cue) and Table of
Contents (toc) files.

It includes:

- `cueconvert` convert between the cue and toc formats
- `cuebreakpoints` print the breakpoints from a cue or toc file
- `cueprint` print disc and track information for a cue or toc file

Directory layout:

- `doc/` documentation (including man pages)
- `src/` all source files
- `src/lib/` scanning, parsing, and printing library
- `src/tools/` cue and toc tools

Install instruction (tested on a centos 7 host):

```
aclocal
autoconf 
automake --add-missing
autoreconf
automake --add-missing

./configure
make
sudo make install
```

If you want to create a standard gnu tar ball, then do

    make dist
