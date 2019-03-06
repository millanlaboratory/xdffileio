
# XDFFILEIO

Presentation
============

This library provides a unified interface to read/write EEG file format
in realtime. It has been designed to provide a consistent and common
interface to all supported file formats while minimizing the CPU cost on the
main loop. It thus performs all the expensive operation (scaling, data
convertion and file operation) in a separated thread. 

The library does not support non-continous recording neither channels
sampled at different sampling rate.

It currently supports the following file formats: EDF, BDF, GDF 1.X, GDF 2.X


Supported platforms
===================

Any POSIX platform (and windows) using a byte size of 8 bits (i.e. all
modern CPU) should be able to compile and run this library. However, it has
been only tested on the following platform: GNU/Linux x86, GNU/Linux x86-64,
Windows x86.


Compilation
===========

This library is organized as a GNU package and can be compiled and
installed in the same way (see INSTALL file for further information).

