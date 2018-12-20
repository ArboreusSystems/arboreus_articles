# Vessel IT Infrastructure.

For understanding the principles that you need to be followed in case of developing (modelling) vessel's IT infrastructure you have to imagine all of vessel devices like informational source or carrier. For example:

* [Radar](https://en.wikipedia.org/wiki/Marine_radar) - the source of information about position of physical objects related to the vessel position, where surface of it might to reflect electromagnetic waves of defined frequency - used in process of navigation and steering of the vessel
* [AIS (Automatic identification system)](https://en.wikipedia.org/wiki/Automatic_identification_system) - the source of information about vessels located in range of the vessel AIS system, used in process of navigation and steering of the vessel
* Fuel Level Sensor - source of information of amount of the fuel in the defined tank where sensor located, used in process of maintaining vessel and might to affect the process of navigation and steering of the vessel
* The sensor of ballast water level in tank - the source of information about amount of water in tank, used in process of maintaining vessel and might to affect the process of navigation and steering of the vessel
* The sensor of the main engine temperature - the source of the information ...
* etc

Like all devices, every member of the crew - the source or user of the information and like devices the huge part of the vessel's informational process.

In the article ["Vessel Informational Security"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/it_notice_for_mariners/vessel_informational_security/eng.vessel_informational_security.md) described how the imaging all of devices, all of crew members like source of information making more simpler the process of understanding the problems related to the informational security.

And now about the process that is using data from sources. All of process might be divided on few groups:

* process of navigation and vessel steering 
* cargo process: loading - unloading and physical integrity (safety), for the case of passengers - might be added by few point more
* vessel maintaining, technical condition controlling and usage for sailing
* the security process
* the communication and document management process between vessel and onshore facilities (PSC, Custom, Coast Guard and etc)
* the communication and document management process between vessel and vessel owner or cargo owner
* the informational exchange process between crew members itself and between crew members and theirs onshore relatives (THE MOST IMPORTANT POINT in case of informational (cyber) security)

If there are big amount of information in one group of process, better to divide it on sub-groups for simpler understanding and modelling.

The IT infrastructure projecting is based on building of information exchange model of the vessel by the analysing the links sources-users in every process. For every source describing the protocol and format, for every link - the amount of data to be transferred, how the data critical and the source trustable and reliable in context of the process (specially noticed for the case of informational security) and as result of data exchange model you are choosing the technical solution.

Separately every group of process well enough equipped by the IT solution. Especially for the case of digital charts and navigation supplying. There are big list of solutions for the Internet connection. There are huge list of solutions for fire fighting. And other, other ...

But! There are always but ..., 2 GIANT PROBLEM:

* at time of formalising technical requirements for the vessels systems developing no-one has been reasoning that the vessel system might be hacked (the vessel is at see - who and how will hack it, but the technology do not staying at one place)
* at time of projecting no-one has been imaging vessel like one solid and well organised source of information (kind of library where you might to find any book in one second) or the vessel itself like user of the information (there are huge list of protocols and formats for huge list of systems: firefighting, doors locking, navigation and etc), no one has been looking on it like universal event system (why it mentioned here you might to get in this article ["Event driven"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/event/event_driven/eng.event_driven.md)) equipped by the universal protocol

The most interesting thing - that every pice of this problems solved on shore. And the solution in developing not so expensive like it might looks for the first glance. You need only adopt it for the case of using at sea and organise infrastructure in following vessel process requirements.

For the first point developer tremendous list of solution that is very useful onshore and used everywhere, in every office even small one. There are solutions for: VPN, Firewalls, WAN/NAT, IPSec and etc. Who is stoping to use it onboard for securing vessel's network itself and vessels devices? Who is stoping imagine the vessel like remote office connected to the main network?

Onshore you might find the term IoT - Internet of Things. Essentially the vessel is like IoT, being more precise LNoT - Local Network of Things, where instead of teapots and vacuum cleaners you using radars and steering. Who is stoping to use the technology stack from it for the vessel's purpose? Who is stoping to use architectural and data exchange protocols for the vessel's purpose? And other who is stoping ...

No-one is saying that you need to use it blindly. Every peace of technology has to be adopted and tested. If you will read the technical review of network security, remote or unmanned technology from different vendors - all of them using similar architectural solutions. Again - who is stoping to use it for vessels? From experience most of the problems will not be connected to the software, for this kind of systems it will depend on quality of materials that used in devices: the wires quality, the plastic vibration endurance and etc.

For solving this kind of informational problems need to be done:

* developing prototype of vessel network for the case of building well maintained and secured enough vessels networks, especially for the case of using old devices developing without meaning of "cyber security precautions"
* developing informational code for using like protocol for building vessel information exchange models for the case of vessel - shore and inside vessel data exchange
* developing platform that will contain all of standards and codes mentioned above, will be developed within meaning that "vessel" - the source of information and provide shipyards and vessel devices vendors the universal data exchange interface (for example, kind of MarinerBSD, based on FreeBSD, the reasons of choosing this OS described in articles ["Why FreeBSD?"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/freebsd/why_freebsd/eng.why_freebsd.md) and in ["Vessel Informational Security"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/it_notice_for_mariners/vessel_informational_security/eng.vessel_informational_security.md))
* based on this platform create the technical requirements for vessel device vendors that will be looking like Plu&Play for computers but for vessel devices (the universal technical requirements will reduce price for maintenance and will reduce security risks too)