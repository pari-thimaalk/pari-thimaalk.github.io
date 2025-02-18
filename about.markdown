---
layout: page
title: about
permalink: /about/
---

I'm a Junior in Computer Engineering at UIUC and currently a GPU Design Verification Intern at Apple. When I was on campus, I helped run [ECE391](https://courses.grainger.illinois.edu/ECE391/sp2024/overview.html), participated in research and occasionally attended [SIGPwny](https://sigpwny.com/) meetings to understand [what is going on with my computer](https://xkcd.com/627/).

I occasionally play ultimate frisbee, ride my longboard and watch [football](https://www.youtube.com/watch?v=WkXZRHG5RxQ). Not at the same time though.

## projects
Ones where I learned a lot.

[**32-bit RV32IM CPU**](https://github.com/pari-thimaalk/rv32im_ooo_cpu)\
Designed an Out of Order CPU from scratch, with Explicit Register Renaming. Implemented features such as G-share Branch Prediction, Split Load-Store Queues, Return Address Stack and Next-Line Prefetching.

[**32-bit x86 Unix Kernel**](https://github.com/pari-thimaalk/wnaj_OS)\
Built an operating system from scratch, that runs on a single core processor. Implemented paging, system calls, device drivers and scheduling, using various data structures. Mostly in C, a sprinkle of x86 for culture. Built and tested using a version of Qemu that was before terminal scrollbacks were a thing.

[**FPGA Network Stack**](https://github.com/pari-thimaalk/HTTP_lwip_FPGA)\
Developed a HTTP client to interface with the Urbana FPGA Board. Fixed a number of bugs in AMD Xilinx's implementation of lightweight-IP (lwIP), to get TCP/IP working. Made a hardware block design that interfaces with an external PHY, as the Urbana Board does not come with one. My group was the first to ever connect this FPGA board to the Internet.
[Report](/files/Networking_FPGA_Final_Report.pdf)

[**Fair Division Algorithms**](https://github.com/pari-thimaalk/Fair_Division)\
Implemented some [fair division](https://en.wikipedia.org/wiki/Fair_division) algorithms in an android app, as part of research under PHD student Aniket Murhekar.

**Linear Voltage Regulator**\
Built a full wave rectifier, low pass filter and amplifier onto a breadboard to verify circuit characteristics, before soldering the components onto a PCB. Had fun using ADALM Scopy.


## classes
The ones I remember the most (fondly), split by subdisciplines

**Computer Systems**
- Operating Systems and Kernel Development
- Communication Networks
- Distributed Systems

**Digital/Hardware Design**
- Computer Organization and Design (Architecture)
- Digital Systems Lab with FPGAs

**Software Engineering**
- Algorithms and Models of Computation
- Data Structures

**Electronics and Signal Processing**
- Electronic Circuits: BJT and MOSFET configurations, Amplifiers
- Digital Signal Processing
- Analog Signal Processing
