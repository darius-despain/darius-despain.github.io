---
layout: essay
type: essay
title: Linux
# All dates must be YYYY-MM-DD format!
date: 2018-09-21
labels:
  - Operating Systems
  - Open Source
---


1	Introduction

  Most operating systems are built and designed by a company, then a copy is sold to the consumer for profit to be loaded onto a computer for use. One Operating System (OS) exists that defies this standard by not being sold, but free to the public and open for users to build upon as they wish. This operating system is the Linux OS.
  
 The remainder of this paper will be organized as follows. Section 2 will discuss the history of Linux, section 3 will discuss it’s architecture, section 4 will discuss why Linux is so popular, section 5 will discuss how Linux works including how it’s developed and maintained, section 6 will discuss the differences between Android and Linux, section 7 will discuss the difference between Linux and Raspberry Pi, and section 8 is the conclusion.
 
2	History

  Linux was invented by a Finnish computer scientist named Linus Torvalds in 1991 [2] and was intended to be a non-professional, open-source, hobby level project for Torvalds. Linux initially needed the support of GNU tools and another operating system called minix in order to function, but Linux was released under the GNU General Public License and was therefore an open-source project. This means that anyone could obtain the source code, modify it, and either share their modifications or spin it off into its own version of Linux. As people added to Linux it became a standalone OS and although it was primary used with a Command Line Interface (CLI), rather than a Graphical User Interface (GUI), it started being used widely for webhosting, networking, database serving, and many other large-scale applications. 
  
  Linux was spinning off into many different versions, such as Redhat and Slackware, and inventor of Linux Linus Torvalds did not want to show favoritism to any one version of Linux, so he decided to find work elsewhere. Torvalds worked at Transmeta in the Open Source Development Labs [2], which later merged into the Linux Foundation, where Torvalds developed mobile computing solutions. Torvalds also acted as the kernel release manager for the Linux Kernel where companies would then take, modify, and implement into their own versions of Linux.
  
3	Architecture

  The Linux OS developed in C and assembly to run originally on i386 PCs but has since been ported to more hardware than any other OS in history [3] and is built on the Linux kernel. The Linux kernel is a monolithic kernel [4], compared to the hybrid kernel type used in Windows and Mac OSX, it runs everything in supervisor mode, giving the OS faster, more direct access to the hardware, with the consequence of having a larger memory footprint. The Linux kernel also allows for kernel modules called Loadable Kernel Modules to be loaded and unloaded at runtime [4]. This differs from other OSes by having the ability to add additional functionality to the base kernel without the need to reboot the system. Linux also incorporates the POSIX API, which is a set of standards established by IEEE to ensure compatibility with different OSes [5]. 
  
4 	Why is Linux Popular?

  The Linux OS is one of the most widely used OSes on the planet. This is due to a long list of reasons that differentiate Linux from other competitors. The first of these reasons is that it is free and downloadable from the internet. Whether a company wants to use Linux to power a commercial solution or a school wants to provide students with computers to use, Linux offers a free and powerful solution that cuts down on cost for the computing needs of the organization. 
  
  Another reason is that Linux is a stable and reliable way for multiple users to access a given machine over a network and even run intensive jobs without system slowdown. Linux multi-tasks very well and is known for running multiple intensive jobs simultaneously without noticeable system slowdown. Also since Linux primarily uses a CLI, it is easily accessible over a network just as if you were sitting in front of the physical machine. This coupled with the multi-tasking allows the machine to be used by multiple users with ease [6]. Since it multitasks so well without noticeable slowdown and the OS being designed to be reconfigured without needing to reboot, Linux is very stable and often has uptimes of months. These factors all combined makes Linux a very appealing option for fileservers and other commercial applications where reliability and access are a priority.
  
  Linux’s ability to add Loadable Kernel Modules allow for the system to be very configurable and make the OS adaptable to many different applications. Some of the modifications that can be made include being modified to serve as web servers, routers, and workstations as well as being able to mimic other OSes such as windows [7]. Linux is also open-source, which means any person can modify the source code if they wished to fit their custom need if any existing solutions do not exist.
  
  Linux is also highly compatible with different types of hardware. Linux is ported to more hardware configurations than any other OS in history [3], but can also read and write data on disk partitions made by Windows OSes. These two factors give Linux the ability to use almost any existing hardware and perform debugging purposes or retrieving data from a locked computer.
  
  The last reason Linux is so popular is that it is fast. Linux runs on a given set of hardware faster than other OSes. This is due to the monolithic kernel used by Linux providing faster access to hardware as well not including any bloat ware in the OS as many other manufacturers might include and due to the fact that Linux does not need to do hard drive defragmentation [8].

5	How does Linux Work?

  Linux is not a single OS, but a collection of different operating systems all based on the Linux Kernel, which is released and maintained by Linus Torvalds [9]. Linux versions are called Distribution projects or distros for short and build off of the Linux Kernel to make an OS. Distros are both made by companies and publicly developed and offer a wide range of features for different types of users.
	
  An example of a company that manages a distro is Redhat, who manages Fedora Linux and Redhat Linux versions. Redhat makes these distros available for free to the public as it is an open-source based software, but they do make money as a company. Redhat primarily makes its money through support services for its distros and supplemental software to the OS. While this might not sound like a big money maker, a great many users require support. According to [10], paid support is one of the common sources of revenue for Redhat. This revenue allows Redhat to operate and maintain its distros as well as remain profitable.
  
6	Linux vs Android

  The Android OS is one of the most widely used OSes on the planet as it’s now in most smartphones, but this OS is in fact based on Linux. Android is not a version of Linux as Redhat and Ubuntu are, but it is based on the Linux Kernel [11]. One might wonder why it is not a version of Linux if it is based on the Linux Kernel, but the answer is simple. Linux uses GNU libraries and a graphical X server to run applications, but Android uses the Dalvik virtual machine to run java applications [11]. This means that Android cannot run the same applications that Linux can, and Linux natively cannot run Android applications either.
  
7	Linux vs Raspberry Pi

  Raspberry Pi is a platform widely used to develop smart devices and perform other small tasks at an affordable price, but Raspberry Pi also runs on Linux. Raspberry Pi runs on a version of Linux called Rasbian, which is based on the Debian Linux distro [12]. This means that Raspberry Pi natively runs on a version of Linux since the OS it uses is based on a Linux distro. 
	
  With Raspberry Pi running on a version of Linux, it enjoys all of the benefits of Linux OSes including being free and fast. This enables Raspberry Pi units to be used for many applications such as web servers, game servers, desktop computers, robot controllers, media centers, and much more. With a Raspberry Pi running Linux it is highly customizable and leaves an open-ended platform for developers who want to create a technology.
  
8	Conclusion

  In summary Linux is an open-source OS that has numerous different versions made by different companies and communities, but are all based on the Linux Kernel by Linus Torvalds. This OS is a fast, capable, adaptable piece of software that is the backbone of countless servers and workstations across the world. It is the backbone of even our smartphone Android OS and it runs on machines like the Raspberry Pi which enables development of countless different new applications for the end user.
  
  References
[1] G Sasaki (n.d.). EE468-Writing-Linux [Online]. Available: https://laulima.hawaii.edu
[2] “Linux History,” Email Viruses - Attachments, Scripts, Protection, Help. [Online]. Available: https://www.livinginternet.com/i/iw_unix_gnulinux.htm. [Accessed: 21-Sep-2018].
[3] “Understanding the architecture of the modern Linux operating system,” Cumulus Networks engineering blog, 04-Jan-2018. [Online]. Available: https://cumulusnetworks.com/blog/linux-architecture/. [Accessed: 21-Sep-2018].
[4] J. Garrison, “What is the Linux Kernel and What Does It Do?,” How-To Geek, 12-Jul-2017. [Online]. Available: https://www.howtogeek.com/howto/31632/what-is-the-linux-kernel-and-what-does-it-do/. [Accessed: 21-Sep-2018].
[5] “What Is POSIX Shell?,” nixCraft, 03-Dec-2013. [Online]. Available: https://www.cyberciti.biz/faq/what-is-posix-shell/. [Accessed: 21-Sep-2018].
[6] J. G. Mackinnon, “The Linux Operating System: Debian GNU/Linux,” rep.
[7] "25 Reasons to Convert to Linux, compiled by The Linux Information Project", Linfo.org, 2018. [Online]. Available: http://www.linfo.org/reasons_to_convert.html. [Accessed: 21- Sep- 2018].
[8] "Why Linux Doesn’t Need Defragmenting", How-To Geek, 2018. [Online]. Available: https://www.howtogeek.com/115229/htg-explains-why-linux-doesnt-need-defragmenting/. [Accessed: 21- Sep- 2018].
[9] "Chapter 1: What is Linux?", Swift.siphos.be, 2018. [Online]. Available: http://swift.siphos.be/linux_sea/whatislinux.html#idm3571768989216. [Accessed: 21- Sep- 2018].
[10] "Yes, You Can Make Money with Open Source", Harvard Business Review, 2018. [Online]. Available: https://hbr.org/2013/01/yes-you-can-make-money-with-op. [Accessed: 21- Sep- 2018].
[11] "Android is Based on Linux, But What Does That Mean?", How-To Geek, 2018. [Online]. Available: https://www.howtogeek.com/189036/android-is-based-on-linux-but-what-does-that-mean/. [Accessed: 21- Sep- 2018].
[12] G. Thomas and G. Thomas, "Raspbian explained", SciFiNow, 2018. [Online]. Available: https://www.gadgetdaily.xyz/raspbian-explained/. [Accessed: 21- Sep- 2018].
