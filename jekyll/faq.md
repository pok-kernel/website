---
layout: page
title: faq 
permalink: /faq/
---


# What is POK ?
POK is a partitioned operating system.
It provides separation functionnalities to isolate different software components.
With this separation, different software components can be collocated on the same machine ensuring safety and security enforcement:

1. A failure of one component does not affect the others (safety)
2. A partition cannot access to the data/code of another partition (security)

The concept of partitioned architectures is introduced in ARINC653 and MILS standards. POK tries to provide a generic partitioned concept that can fit with these standards.

# What is AADL ?

[AADL](http://www.aadl.info) is a modeling language that describes system architectures. 
With AADL, you can represent your runtime architecture (processor, partition, communications, etc.)
and their constraints (security level of a partition, scheduling policy of a processor, etc.).
Such a representation can be processed to validate system architecture.

In POK, we use the AADL to generate the code of the kernel. 
You model your system with its partitioning constraints using AADL. 
Then, a code generator automatically generate the code that configures kernel and partitions. Using this development method, you avoid manual code production, which is, most of the time, error-prone.

# Where can I find the Ocarina AADL toolsuite ?

Go on the [Ocarina github page](https://github.com/OpenAADL/ocarina).

# Can I use POK without AADL ?
Yes, but in that case, you'll lose code generation benetifs and you'll have to write the configuration code of the kernel by yourself. The documentation of POK provides necessary items to configure POK by yourself.

# What standards POK supports ?
At this time, POK supports ARINC653 and MILS standards. For ARINC653, the C layer is available. For MILS, we check MILS compliance at the model-level, with an AADL model validator.

# How much does it cost ?
POK is a free-software (free as in “free speech”, not as in “free beer”): the code is released under the [BSD license](https://en.wikipedia.org/wiki/BSD_licenses).
You can modify, adapt code and join our developer team.

# Who provides support for POK?

There might be available support through different companies.
[Reblochon](http://www.reblochon.io) provides commercial support for POK.
