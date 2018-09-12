# Why Freebsd?

**Prerequisites**

Every issue has to have the balanced solution that is allowing to achieve the maximal result by minimal resources. All of information in this article based on real world projects developed previously or at least finished test.

The task: develop the data storage within capability to serve the high-load data access and storing big amounts of data, sort of solution for high-load access to big data when required storing data from "now" to 2-3 years more for operational usage and for being capable to store in long term, from 3 to 15 years, or might be more. The solution has to be fitted for small companies from begin and be scalable for case of using it in large companies.

More details about the task:

* any kind of solution for High-Load will always require you to handle huge traffic income/outcome or inner. In come cases, when required complex logic for handling or storing data the ratio between outcome/income and inner might be 1:10. It's mean the OS has to be capable to handle this amount of traffic
* high level of fault tolerance and reliability
* high level of security
* and etc

The list of this properties might be prolonged more. This list enough for this article, other less important in this context.

**FreeBSD vs Linux**

FreeBSD vs Linux - is most incorrect way to solve this problem. Why? Because the FreeBSD is the full features OS but Linux is only core (this core written by [Linus Torvalds](https://en.wikipedia.org/wiki/Linus_Torvalds)) that is starting family of OS named like [Linux-family](https://en.wikipedia.org/wiki/Linux) because of core. The whole Linux-family history might be gotten from this image [Linux Distribution Timeline](https://en.wikipedia.org/wiki/Linux#/media/File:Linux_Distribution_Timeline.svg)

The correct way for computation has to be like:

* Ubuntu vs FreeBSD
* Fedora or RedHat vs FreeBSD
* FreeBSD vs SlackWare
* etc

When were the tests for the case of choosing base OS, were tested Ubuntu, SlackWare, FreeBSD and Fedora. Tests has been taken 2 month for each of platform for totally constant issue, totally the same for every platform.

To be honest, when your project is serving less then 2K connections per second there are nothing about to use the FreeBSD because result is equal to each other and the Linux distributive is more simple for maintaining to intermediate or beginner level and in most cases fitted for small companies. The difference appearing when you reaching the level of 5K connections per second (there were appearing long-time response via TCP) and became obvious after reaching point of 10K. Some time difference get value of 5-7 percents. The reason of this difference - the TCP Stack used in FreeBSD, it's really faster then any from Linux-family. Only SlackWare within tuned core came closer to FreeBSD within "in-box" core, but SlackWare is very specific OS and it's hard to be maintained in case of long term storage.

For the case of developing "heavy load" projects 5-7 percents might be valuable reason for FreeBSD.

**The history of maintainer and OS**

The history of UNIX-like system might be gotten from the image behind.

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/freebsd/why_freebsd/illustrations/unix_history.png)

In case of Long Term Storage (5-15 years) the huge speed of changing in modern and progressive OS might to play bad tricks to your system because of inheritance that your system has to be fitted to care from begin.

During operations less amount of problems for the case of inheritance came from FreeBSD because the Linux is more progressive. The FreeBSD is more balanced solution for this case.

**Security**

When you are trying to be clear about security need to divide it  on two points:

* The System security itself - the FreeBSD one of the most rare operational system that appearing the security troubles. You might to check it by your own [Top 50 Vendors By Total Number Of "Distinct" Vulnerabilities](https://www.cvedetails.com/top-50-vendors.php?year=0) - the 27th place for FreeBSD and 8th place for Linux-family
* The ability to create various security policies for different cases of OS usage - from begin FreeBSD designed for companies and state organisations, there are huge list of "in-box" solutions that might make you able to ensure high level of security if you have enough knowledge of "how-to"

**Fault tolerant and reliability**

There are joke that is spread through the System Administrators - if you remember how looking your server case and where it located - it's under Microsoft Windows, if you remember IP address and configuration of your server - it's under Linux, if you've got forgotten IP, configuration and where it located and it works - it's under FreeBSD

This joke is most illustrious fact about maintaining FreeBSD.

**THE HUGE-MEGA-SUPER-MAIN POINT - L-I-C-E-N-S-E**

This might be most important point in case of developing solution that been mentioning above.

Between BSD and Linux is the huge divide named Free Software (BSD) vs Open Source (GNU). For the first glance there are nothing to worry about. But! The BSD license allow anyone to do anything with the sources of OS but the any kind of Linux obliging you to publish whatever you change publicly. Would you like to talk about freedom?

You might to find in the Internet huge definitions about all of this licenses

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/freebsd/why_freebsd/illustrations/license_001.png)

In real world example it might looks like for the case of security you changed something for being able to follow the main security rule "nothing usual" on the level of OS Sources for achieving maximum of productivity and security and you system going to be cracked not by hackers but by lawyers that will come to you and ask you to publish whatever you done for your own safety publicly. Would you like to talk about security?

In case of developing highly secured solutions for storing data for long term storing - it might be key-point for using FreeBSD. If you asking "Why do I need to adjust OS sources?" - mean you haven't got this kind of issues and this article not for you.

**Resume**

The choosing FreeBSD has to be the reasoned choice. The FreeBSD will rise you more difficulties at time of start project but will rise you upon less expenses that you have to care at time of maintain. If you have no specialists equipped by enough level of knowledge or you not enough of resources to be studied it you are risking to get fail in using FreeBSD but in opposite direction it allow you develop very securable and reliable solution for your unique task.