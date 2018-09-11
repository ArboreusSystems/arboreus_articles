# Blockchain. The types of chained structures.

Need to make clear understanding of absence of unique solution for the case of developing blockchained application. Most likely only for now, in future the progress will find unique solution. For now every case where need to be implemented blockchain has to be anaylized separately.

In creating application, by the incorrect implementation of blockchain might be killed the application usability because of the very restricted access to the datum or became very slow that will make the blockchain like handbrake but not the progressive engine. Any kind of structure has been appearing only because and for reason "for something" and if it became impossible for achieving "because" by the application - no-one will use it. Not every use case for structure developing require to include blockchain. There are huge list of use cases where no any necessity of using it, there are enough of primitive and very useful solutions.

And now about the topic of this article - types of the structure where might be implemented blocked elements of chain.

**1) Root-oriented or Tree-like**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_structures/illustrations/blockchain_002.png)

This kind is good enough for the structures which contained constant list of elements or it's growing slowly and there are not critical time of recalculation of the formulas for blocking chain. For example: 

* any kind of desktop or mobile application where structure is the list files that is required for application
* the departments of any company, where departments is the elements of the chained structure
* servers added to the cluster, where the structure is the net with elements (servers)

**2) Linear or vector**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_structures/illustrations/blockchain_003.png)

The structure is linear - when every element connected only to two other elements of the structure, one forward - on backward, one upstairs - one downstairs and etc. For example:

* event flow where the value of time is the blocked position relatively to others on the vector of timeline
* the path description where the sequence of points is the direction where direction is the block for elements - points 

**3) Matrix**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_structures/illustrations/blockchain_004.png)

One of the most complex structure because of layers of substructures and the relations between each other and the every points by the specially defined formula or algorithm. For example might me explained the use case of gathering reports of the company's departments state every 10 minutes, or gathering currency exchange values, or cron table in handling servers and etc, where the elements of matrix might be record in the DB-engine.

**4) Organic**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_structures/illustrations/blockchain_005.png)

This term came from "Chemistry" - there are part of it named "Organic chemistry". It came because most obvious example of this term. This type is not standalone time, it's time kind of property to previously described where for example might be:

* the link between elements might contain value too
* element might contain limit for the connected events

There are huge list of examples of Organic structures:

* the roads, where the wide of the road and the quality road surface defining maximal value for number of the cars
* electrical networks, where the maximal possible value of the power line regulating line capacity and the connection points ability require maximal value of the connected subnetworks
* the internet 
* etc

There might be developed of defined huge variations of the structure, to describe every possible - not the goal of this article. The goal was to show where the block of the chains of the elements and how to defend the statically-oriented structure agains dynamic changing (data manipulation, fraud and etc). For the case of dynamically-oriented structure, mostly for security cases - to avoid statical fixation of the structure, when the statical fixation of the structure is the potential breach in structure defence line.