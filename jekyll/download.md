---
layout: page
title: download & quickstart
permalink: /usage/
---

# Source code

The source code can be found on the following [github
account](https://github.com/pok-kernel/pok).

## Download the source code
Just issue the following command
```
git clone https://github.com/pok-kernel/pok.git
```

# Dependencies
Make sure you have the following packages:
* qemu
* mtools

If you are on ubuntu, you can install these packages using the following
command:
```
apt-get install mtools qemu
```

You can check what packages are missing by issuing the following command
```
make configure
```

# Test your first example

1. Set the POK_PATH variable
```
export POK_PATH=/where/you/have/the/pok/sources
```

2. Configure your runtime by typing the following command.
```
cd $POK_PATH
make configure
```
The x86 architecture should be configured. If not, install
the missing packages.
3. Go to the example and compile
```
cd examples/semaphores
make all
make run
```

You should see QEMU starting with the compiled program.

![POK in QEMU]({{ "/assets/qemu.png" | absolute_url }})
