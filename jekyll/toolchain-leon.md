---
layout: page
title: toolchain PPC
permalink: /toolchain-leon/
---

# Compile and install SPARC/LEON3 toolchain

This has been done on Linux. At this time, the SPARC toolchain does not work on Windows.

The target is ```sparc-elf```. So, you have to build binutils and gcc for this target. First, build and install binutils. Then, compile gcc.

It has been tested with the following versions :
* binutils : 2.20
* gcc : 4.4.2

## Build and install binutils

1. Download the lastest version of binutils
2. Untar the archive
3. Invoke configure for the sparc-elf target : ```./configure --target=sparc-elf```
4. Compile and install : make all install


## Build and install gcc
Be sure that the pre-compiled binutils are in your PATH variable
1. Download gcc
2. Untar gcc (tar zxvf gcc...tgz)
3. Create a separate directory to build gcc (mkdir build)
4. Enter this directory (cd build)
5. Configure gcc distribution : ```../gcc-x.x.x/configure --enable-languages=c --target=sparc-elf --disable-nls --disable-libssp -C --without-headers --with-gnu-as –with-gnu-ld --with-newlib```
6. Invoke make for building gcc
7. Install, invoke make install

## Configure the POK toolchain

Issue ```make configure``` in the top directory of POK. If the toolchain is installed, it should print an appropriate message, showing that GCC and binutils for SPARC have been detected.


