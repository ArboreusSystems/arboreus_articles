# Private cloud.

This article based on real world experience of organising private cloud computing cluster for the purpose of different kind of organisation:

* the developers test environment equipped by ability to automate HUGE list of tests for different kind of applications: servers load tests, UI application test and etc 
* the web-design agency kind of private hosting provider for small companies holding 
* the university computation cluster and studying environment for students within ability to provide at least one server instance for every student 
* medical company purposed to care about huge amount of installed application required to be used by regulations 
* etc 

First of all - What doest it mean "cloud". In accordance of definition in public resources it looks like sharing resources of one server through the couple of users. In [Wiki](https://en.wikipedia.org/wiki/Cloud_computing) you might to find explanation and historical approach to this term.

The global issue - to share resources. For now the are a lot of expensive solution fitted for huge companies. All of technology descried in this article - software covered by any kind of free use license (BSD, GNU, etc). It's mean you don't need additional money for this software.

Again about sharing resources. In terms of transport (this kind of analogy is more illustrative for the case of showing what is cloud computation). 

Cloud computation - something like bus that is following strictly defined path where defined stops and you able to go out or go in only at this stops. This bus equipped by on engine, one driver, one air-condition and one whatever you want, but it doesn't mean you are alone in this bus. And it doesn't mean that the stop where you need to go out closely to the point of your destination. How about of heavy baggage (in IT terms big-data)? Might be taxi much more better?

Beside all of it you need to make very clear:

* the company that is owning the bus-fleet interested in profit only, the comfort of passenger interesting them only in case of minimal price for getting passengers in bus;
* you are not controlling real technical condition of the bus, you might even know that the any part of the bus in critical condition and you risking yourself by being in this bus (for example USA HIPAA contain special part for public hosting and HIPAA compliant hosting cost HUGE money, in most cases to build own data center might be much cheaper (not simpler) then pay for it to any company because they will do totally the same like any System Administrator, but will add to price their own profit, you are always paying for your own disability in case of necessity)
* you are not controlling the situation when in bus might be presented couple of hooligans that is disturbing anyone around them and the bus driver have to call police and stopped the bus, but you in hurry to somewhere and carrying about something very valuable in your pocket
* etc

There might be huge amount of examples illustrating of it, but this is not the topic for this article. If you need about choosing the type of hosting you might to read this article ["Cloud. Collocation. Private."](https://github.com/ArboreusSystems/arboreus_articles/blob/master/data_storage/cloud_collocation_private/eng.cloud_collocation_private.md)

The main goal for this article is to provide you with information of how technically to organise the small private cloud that might be scaled in future in case of growing your company by free resources. The level of solutions might be even comparable to the leaders like Amazon, Heroku, GoDady and etc. Be aware of that every leader doing the same thing like any System Administrator in general. You will never be like Google while you are using Google.

For releasing your own cloud solution you will need:

* [FreeBSD](https://www.freebsd.org) (you might to use any other operational system, but the authors using it because more performance in case of high load)
* The Virtualisation or Pseudo-Virtualisation Tools: [VirtualBox](https://www.virtualbox.org/wiki/Downloads) or [FreeBSD Jails](https://www.freebsd.org/doc/handbook/jails.html)(for being more precise Jails and Ezjail Tool not the virtualisation itself, its solution for sharing resources)
* Automation server [Jenkins](https://jenkins.io), this is the leader in this segment equipped by huge community and very well documented
* 2 servers at least: one like host-server with resources going to be shared and automation server where going to be installed Jenkins (in case of restricted resources you might to install it even on your home-based laptop)
* System Administrator within very beginner knowledge of how it works, there are HUGE amount of manuals and references that might be used by your own, there are nothing really difficult

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/freebsd/private_cloud/illustrations/private_cloud_001.png)

How it works?

Any kind of virtualisation tool has an ability to be managed through the shell commands and Jenkins allow you to run any shell command on any connected server. THIS IS ALL THAT YOU NEED FOR SOLVING THIS PROBLEM! - Run shell command on server.

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/freebsd/private_cloud/illustrations/private_cloud_002.png)

The Jenkins UI provide you constructor for assigning "button-make-me-good" for shell command on any server you want. It might be physical server, virtual server and other. It's might be even device that is equipped by unix-shell, for example based on [Raspberry](https://www.raspberrypi.org).

You might to use IT-Developers tool for non-IT-at-all companies.  For example transport company, medical facility, firefighting, ecology monitoring and other and other. For your own purpose might be realised kind internet-of-things via Jenkins UI and applications that is running under it.

The documentation for installing every part of this schema might  be gotten from this links:

* [Install FreeBSD](https://www.freebsd.org/doc/handbook/bsdinstall.html)
* [Install VirtualBox](https://www.freebsd.org/doc/handbook/virtualization-host-virtualbox.html)
* [Install Ezjail](https://www.freebsd.org/doc/handbook/jails-ezjail.html)
* [Install Jenkins](https://wiki.jenkins.io/display/JENKINS/FreeBSD)
* [SSH plugin for Jenkins](https://wiki.jenkins.io/display/JENKINS/SSH+plugin)

Beside all of it you might to get non official documentation about how-to-manage this kind of issues. If after all of this articles you need assistance you might be contacted to authors of this article via daemon.arboreus(a)gmail.com for consulting.
