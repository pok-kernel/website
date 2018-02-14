---
layout: page
title: about
description: Description of what is POK
permalink: /about/
---

# What is POK?

POK is a real-time embedded operating system for safety-critical systems (avionics, aerospace and so on).
It provides several functionalities and complies with many industrial standards, such as ARINC653 or POSIX.
POK was designed to be used in safety-critical systems as well as in public systems.

The kernel was designed to be very small and targets full
verification/certification.
Actually, more than 90% of the kernel code is covered without any effort.
Moreover, its design, closed to microkernel architectures, isolates device drivers to avoid crashes and increase system safety. In addition, it isolates each communication channels to improve safety and security.

Available toolset is available to build applications with the POK operating system: we provide a code generator that automatically configures and deploy applications from architecture models (AADL).

POK is available as a free software under the BSD licence. It is developed by an academic and industrial community. 

# Existing GPLv3 fork
It has been forked and re-licensed under the GPLv3 by ISPRAS under the name [JetOS](http://www.ispras.ru/en/proceedings/isp_29_2017_3/isp_29_2017_3_171/). You can
find the source code of the fork [here](https://github.com/yoogx/forge.ispras.ru-git-chpok).
This fork is [actually used](http://www.startlr.com/in-russia-it-is-planned-to-create-an-operating-system-for-aircraft/) for commercial airplanes in Russia:
*"There is already a working prototype of the RTOS, operating on the platforms of domestic developers. A certification package that meets the requirements of the Russian aviation authorities is planned to be received in accordance with the concluded contracts at the end of 2019"*

# Open Source Support
Open Source support is done through github. You can open a new issue (or browse existing
and resolved issues) on the [github issue tracker](https://github.com/pok-kernel/pok/issues).


# Commercial Support
[Reblochon Development Company](http://www.reblochon.ai) provides commercial support for POK.
You can contact them directly for further information.


