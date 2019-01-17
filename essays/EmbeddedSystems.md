---
layout: essay
type: essay
title: Embedded Systems
# All dates must be YYYY-MM-DD format!
date: 2018-11-14
labels:
  - Raspberry Pi
  - Operating Systems
---



Machines are driven by some kind of controlling mechanism to process data and allow the machine to operate. Originally this was done with analog systems which were fixed and only able to fulfil one purpose, but since then the technology of computers has evolved and with-it industrial control. Embedded systems are these computers and are used in endless devices we all use every day.
  
This report is defined by the handout [1] and the remainder of this report will be organized as follows. Section 2 will discuss what an embedded system is. Section 3 will discuss its history. Section 4 will go over two popular embedded system platforms; Raspberry Pi and Arduino Uno and Yun. Section 5 will expand on different operating systems for embedded systems. Section 6 is the conclusion.

## 2	What is an Embedded System?

An embedded system is a combination of computer hardware and software that is designed for a specific function or set of specific functions [2]. Examples include industrial machines, household appliances, vending machines, and many other every day items. An embedded system can range from a system having a single function and no user interface (UI) to a multi-function graphical user interface (GUI) based mobile device. 

To perform their designated tasks, embedded systems all use either a microprocessor or a microcontroller in their hardware, compared to a normal computer that only uses a central processing unit (CPU). The difference between a microprocessor and a microcontroller is that a microprocessor is just a CPU, and a microcontroller is a microprocessor with build in components such as memory, RAM and serial ports. The microcontroller is then more easily adaptable as everything is already integrated and can be connected directly to the desired device to be controlled.

Embedded systems also use less sophisticated operating systems than that of larger computers. These operating systems are often less memory intensive but are designed to run in the Real Time environment. This coupled with the fact that the hardware of embedded systems rely on integrated circuits means that the system runs extremely quickly and performs a more limited set of tasks than normal computers.
  
## 3	History

Embedded systems have been around since the early days of computers and are now used in almost every aspect of everyone’s lives. Embedded systems are computers, so their history is tied closely with the history of personal computers and it all starts with the birth of the first digital computer. The first digital computer was built in 1944 [3] and was not programmable. This allowed us to build computers for a specific purpose, but in order to repurpose or tweak them we had to completely rebuild them. Then 2 years later in 1946 [3] the first programmable computer was made that allowed for storing programs so that the machine could serve more than 1 specific function. Moving forward computers weren’t all that commercialized until decades later when the Apollo Guidance Computer was made. The Apollo Guidance Computer was the first embedded system [4] and was one of the riskiest components of the whole mission due to the technology being so new, but it was a huge leap forward for embedded systems as it laid the ground work for other important work to rely on computing power for its tasks. 
  
## 4 	Popular Embedded Systems

Embedded systems are all over and are more common than people think. Embedded systems are also available for development projects at the consumer level that are easily purchased and programmable. These platforms are the Raspberry pi and the Arduino Uno and Yun.
	
Raspberry pi is a microcomputer on the market designed for cheap educational development in the form of projects such as home automation, wearable computer, and synced music and lights [5]. It generally has two different variants for the different possible uses, model A and B. Both models use a micro USB port for power in, a camera and display serial interface, a micro SD card slot, 3.5 mm composite video and audio out, and HDMI out [6]. Contrary to intuitive thought, model B was created first and is larger and utilizes an additional four full size USB 2.0 ports and an ethernet port [6]. Model A is a smaller and lower powered than its B variant and utilizes only 1 USB 2.0 port and no ethernet port [6]. Raspberry pi can be loaded with several operating systems, but the official OS is Raspbian which is a version of the Debian Linux distribution. Raspbian allows the raspberry pi to be used for full spectrum capability as it’s based on a full Linux distribution.
	
Arduinos are a microcontroller platform with many variants to fit the needs of endless projects, today we will discuss the Arduino Uno and Arduino Yun. The Arduino Uno is the most used board of them all and has a USB type B port, 14 digital input/output pins, 6 analog input pins along with the power connector [7]. The Uno is useful for relatively simple controller projects where a simple input or output is needed and generally repetitive programs as Arduinos run on loops. The Arduino Yun is a currently discontinued board that features a built in WiFi card, an ethernet port, a USB type A port, a micro USB port, a micro SD card slot, and 20 digital input/output pins [8]. This board is different because it has native network capability along with the ability to load a Linux distribution named Linino OS, allowing it to perform as a low-cost networked computer with the ease of Arduino.
  
## 5	Embedded System Operating Systems

There are several different operation systems used in embedded systems called Real Time Operating Systems (RTOS). These RTOS are designed to process data as it comes in, usually set with fixed time constraints that the system must process the data within or else the system will fail. This section will discuss the following RTOS; Apache Mynewt, ChibiOS/RT, Contiki, RIOT, RTLinux (Linux support of RT services), VxWorks, and Zephyr.

Apache Mynewt is an open source RTOS under the Apache Software Foundation. It aims to provide an easy platform to develop applications for microcontroller environments with power and cost constraints. Its features include low memory footprint (8 KB - 16 MB), reduced code size (64 KB - 32 MB), low processing speed (10-200 MHz), low power operation (operates in a sleep mode to conserve power), and scheduled processing on a calendared or periodic basis [9]. All of these features allow for an OS that conserves power and uses less resources to keep cost down while maintaining real time operation.

ChibiOS is an open source RTOS and aims to provide a complete solution for all embedded devices. It is built on its fundamental requirements of focus for code elegance and consistency, fully, unambiguously static, short code paths for all operations, compact, feature complete installation, and strong abstraction [10]. ChibiOS utilizes a RT scheduler to enable fast computation for its embedded devices, this scheduler is broken into two internal layers, the RT portable kernel, and the RT port layer. [11]

Contiki is an open source RTOS that aims to connect tiny low-cost, low-power microcontrollers to the internet to add to the Internet of Things. Contiki works by making good on its mission to connect tiny low-cost, low-power microcontrollers by operating on a very small amount of memory, providing mechanisms for estimating power consumption and being designed to run in extremely low-power systems, full IP networking, and many more features [12]. Contiki also uses cooperative scheduling, which means that processes are only started upon boot up, a module is loaded, or something else happens such as a timer or sensor going off and the processes are all run only one after the other. This scheduling allows the OS to devote resources to the current process to finish on time, then move onto the next. All of these features allow Contiki to connect to other devices and the internet to provide a network of devices on the internet.

RIOT is another open source RTOS that also aims to connect the Internet of Things by focusing on low-power wireless IoT devices. It is based on a microkernel architecture and allows for flexible memory management, high resolution long-term timers, support for over 100 boards, and IPv6 support allowing devices to connect to the internet [13]. RIOT utilizes a tickless, preemptive, priority-based scheduler to allow processes to be executed using interrupts and according to a priority system [14]. These features combined make RIOT a very capable OS for use in many IoT devices.

RTLinux is a RTOS that is a version of Linux that operates in real time. It takes the Linux kernel and modifies it by emulating interrupts, where the normal Linux kernel isn’t time bound due to its size and open source nature [15]. RTLinux fixes this by adding a layer between the kernel and the hardware to handle scheduling correctly where the kernel wouldn’t do this correctly. This enables RTLinux to act in hard real time and still be based on the Linux kernel, making it a version of Linux with all of the features of regular Linux, but with real time support.

VxWorks is a commercial RTOS created and sold by Wind River Systems. It provides a RTOS that uses less processing power than unix and runs at faster speeds also including IPv6 capability and a slew of file systems including Network File System (NFS), High Reliability File System (HRFS), and Disk Operating System Filing System (DOSFS) [16]. VxWorks also utilizes round-robin scheduling and fast interrupt response to schedule processes, utilizing hardware interrupts on a timer. VxWorks is also used in the space industry on projects such as the Mars Reconnaissance Orbiter and the Pheonix Mars Lander.

Zephyr is an open source RTOS that is designed for resource constrained systems. It works with everything from embedded sensors to smart wearable tech such as smartwatches. It offers power management services through a tickles idle and advanced idling infrastructure [17] and dynamically allocated memory to allow for resource conservation. It uses interrupts in cooperative and pre-emptive scheduling and earliest deadline first methods to ensure processes are executed on time. 

## 6	Conclusion

In summary, embedded systems are an invaluable tool that the industry relies on and is available for consumers to develop as well. Consumers can buy Raspberry Pi or Arduino units themselves and explore functionality as well as utilizing current real time operating systems to perform the functions they need on varying hardware requirements. This technology will allow the world to evolve so we can have smarter and more convenient everyday lives. 
  
## References

[1] G Sasaki (n.d.). EE468-Writing-Embedded [Online]. Available: https://laulima.hawaii.edu
[2] "What is embedded system? - Definition from WhatIs.com", IoT Agenda, 2018. [Online]. Available: https://internetofthingsagenda.techtarget.com/definition/embedded-system. [Accessed: 14- Nov- 2018].
[3] "Milestones in embedded systems design", Embedded, 2018. [Online]. Available: https://www.embedded.com/design/prototyping-and-development/4007514/Milestones-in-embedded-systems-design. [Accessed: 14- Nov- 2018].
[4] F. Knoegell, "history of embedded system", Academia.edu, 2018. [Online]. Available: https://www.academia.edu/8286031/history_of_embedded_system?auto=download. [Accessed: 14- Nov- 2018].
[5] T. Agarwal, "Raspberry pi Technology, Working and Its Applications", Edgefxkits International, 2018. [Online]. Available: https://www.efxkits.com/blog/raspberry-pi-technology-with-applications/. [Accessed: 14- Nov- 2018].
[6] "The Raspberry Pi Board Guide: Zero vs. Model A and B", MakeUseOf, 2018. [Online]. Available: https://www.makeuseof.com/tag/raspberry-pi-board-guide/. [Accessed: 14- Nov- 2018].
[7] "Arduino Uno Rev3", Store.arduino.cc, 2018. [Online]. Available: https://store.arduino.cc/usa/arduino-uno-rev3. [Accessed: 14- Nov- 2018].
[8] "Arduino Yún", Store.arduino.cc, 2018. [Online]. Available: https://store.arduino.cc/usa/arduino-yun. [Accessed: 14- Nov- 2018].
[9] "Mynewt Documentation — Apache Mynewt latest documentation", Mynewt.apache.org, 2018. [Online]. Available: http://mynewt.apache.org/latest/index.html. [Accessed: 14- Nov- 2018].
[10] "ChibiOS free embedded RTOS - Introduction", Chibios.org, 2018. [Online]. Available: http://www.chibios.org/dokuwiki/doku.php?id=chibios:book:intro. [Accessed: 14- Nov- 2018].
[11] "ChibiOS free embedded RTOS - ChibiOS General Architecture", Chibios.org, 2018. [Online]. Available: http://www.chibios.org/dokuwiki/doku.php?id=chibios:book:architecture. [Accessed: 14- Nov- 2018].
[12] "Open Source RTOS", Osrtos.com, 2018. [Online]. Available: https://www.osrtos.com/rtos/contiki-os. [Accessed: 14- Nov- 2018].
[13] "RIOT-OS/RIOT", GitHub, 2018. [Online]. Available: https://github.com/RIOT-OS/RIOT. [Accessed: 14- Nov- 2018].
[14] "Scheduler", Riot-os.org, 2018. [Online]. Available: https://riot-os.org/api/group__core__sched.html. [Accessed: 14- Nov- 2018].
[15] Yodaiken.com, 2018. [Online]. Available: http://www.yodaiken.com/papers/BarabanovThesis.pdf. [Accessed: 14- Nov- 2018].
[16] "What is VxWorks? - Definition from Techopedia", Techopedia.com, 2018. [Online]. Available: https://www.techopedia.com/definition/15969/vxworks. [Accessed: 14- Nov- 2018].
[17] "Introducing Zephyr — Zephyr Project Documentation", Docs.zephyrproject.org, 2018. [Online]. Available: https://docs.zephyrproject.org/latest/introduction/introducing_zephyr.html. [Accessed: 14- Nov- 2018].
