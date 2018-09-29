---
layout: page
title: Frequently Asked Questions
permalink: /faq/
---


### What is POK?
POK is a partitioned operating system, which means it isolates drivers and
applications in time and space. No driver/application can use more than its
allocated resources.

The concept of partitioned architectures is introduced in [ARINC653](https://en.wikipedia.org/wiki/ARINC_653) 
and
[MILS](https://en.wikipedia.org/wiki/Multiple_Independent_Levels_of_Security) standards. 
POK is fully compatible with these standards.

### Why POK isolates applications?

Drivers and applications isolation is done for safety and security reasons.
By isolating in space, we make sure that each partition cannot access
other address space.

Time isolation means that each partition has enough time to be
executed. We guarantee that a function has the timeslice it requires to be 
executed and no other application can preempt it.

By using a minimal micro-kernel and separating each component in each own
partition, we also facilitate the system analysis and certification.


### What is AADL?

[AADL](http://www.aadl.info) is a modeling language that describes system architectures. 
We use this language has a frontend to model and validate the architecture and generate the
configuration and runtime code.

### What is Ocarina?

Ocarina is an AADL toolsuite that is used to process AADL models and generate
configuration code for POK.
You can get the source code of Ocarina on the [Ocarina github page](https://github.com/OpenAADL/ocarina).

No worries, you can use POK without Ocarina.

### Can I use POK without AADL ?
Yes, but you lose code generation benetifs and need to write the configuration
and runtime code yourself.


### How much does it cost ?
POK is a free-software (free as in “free speech”, not as in “free beer”): the code is released under the [BSD license](https://en.wikipedia.org/wiki/BSD_licenses).
You can modify, adapt code and join our developer team.

### What is JetOS?
POK has been forked and re-licensed under the GPLv3 by ISPRAS under the name [JetOS](http://www.ispras.ru/en/proceedings/isp_29_2017_3/isp_29_2017_3_171/). You can
find the source code of the fork [here](https://github.com/yoogx/forge.ispras.ru-git-chpok).
This fork is [actually used](http://www.startlr.com/in-russia-it-is-planned-to-create-an-operating-system-for-aircraft/) for commercial airplanes in Russia:
*"There is already a working prototype of the RTOS, operating on the platforms of domestic developers. A certification package that meets the requirements of the Russian aviation authorities is planned to be received in accordance with the concluded contracts at the end of 2019"*


### Who provides support for POK?

There might be available support through different companies.
[Reblochon](http://www.reblochon.io) provides commercial support for POK.
