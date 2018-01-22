[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1133782.svg)](https://doi.org/10.5281/zenodo.1133782)


Build instructions for Linux are in INSTALL, which is generated by automake.
Also see ./configure --help for some useful options. Additional information 
can be found in the HACKING file, including hints for Mac users and 
instructions for recent HDF5 library updates.

Dependencies are:

perl
====
LanlGeoMag links against libperl, so you need perl development headers.
Ubuntu package: libperl-dev

GNU Scientific Library
======================
Again, the development package is required.
Ubuntu packge: libgsl0-dev

HDF5 1.8
========
Must be version 1.8 or later. Development package required.
Ubuntu package: any package that provides libhdf5-dev. libhdf5-serial-dev is suggested.

GNU Autoconf, Automake and Libtool
==================================
LanlGeoMag uses GNU autotools to build the configure scripts and makefiles.
On GNU systems these are provided with the operating system. On Mac these were 
provided with XCode prior to version 4.3 (Shipped with OS X).
Mac install: (MacPorts) sudo port --verbose install autoconf automake libtool

GNU argp
========
On non-GNU systems argp must be installed prior to building LanlGeoMag.
Mac package: argp-standalone (known to be provided by MacPorts and HomeBrew)
