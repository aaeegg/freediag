# FREEDIAG - Free diagnostic software for OBD-II compliant motor vehicles.

This package contains 'core' software (called 'scantool') which can be used to access your car's diagnostic system using a laptop and a suitable interface cable.

scantool's user interface is a simiple interactive command-line. There is also an application interface ("freediag AIF") that lets more sophisticated programs use the freediag core whilst presenting the user with a more appealing interface.

The backend library `libdiag` can also be used without the CLI.

Under this directory are the following sub-directories:

* doc      -- Documentation that applies to the package as a whole.
* doc_interfaces -- some interface-specific notes and specifications
* scantool -- Source code for the 'freediag' core package (libdiag and freediag CLI)
* schedSetter -- a linux utility to allow freediag to run as a high-priority but unpriviledged process.


## Licensing
freediag and its backend library `libdiag` are licensed under GPL.

## Authors
Each package contains a list of its contributors.

## OS Requirements
Linux and Windows are the main platforms, Mac OS could work (in theory).
As of 2021/02 , freediag should run at least on these setups:

- Windows 7 and up
- Windows XP if compiled with mingw or borland compilers
- Anything linux-based that supports serial ports (physical or USB-based)


## Compilation/Installation

Refer to doc/build_system.txt for more information;

For the moment, you should not run 'make install' as it will probably copy files to inappropriate destinations.

freediag uses CMake and your choice of compiler toolchain.
The win32 release is usually compiled with the mingw toolchain.


## Running

To use freediag, you'll need an appropriate interface to connect a laptop computer to the OBD-II port on your car.  With most available interfaces, it would be inadvisable to use a computer powered from wall socket because your car may not be adequately grounded.
 
See doc/Scantool-Manual.html for instructions to use the freediag CLI.

## Support/Contribution
https://github.com/fenugrec/freediag
https://freediag.sourceforge.io

Issues should be reported on the github project page.
There is also an IRC channel on freenode (irc.freenode.net), #freediag
The current maintainer (fenugrec) can be reached directly @ fenugrec
at users.sourceforge .net.
