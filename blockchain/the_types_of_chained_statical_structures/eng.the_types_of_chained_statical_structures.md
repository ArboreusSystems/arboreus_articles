# Blockchain. The types of chained statical structures.

Need to make clear understanding of absence of unique solution for the case of developing blockchained application. Most likely only for now, in future the progress will find unique solution. For now every case where need to be implemented blockchain has to be anaylized separately.

In creating application, by the incorrect implementation of blockchain might be killed the application usability because of the very restricted access to the datum or became very slow that will make the blockchain like handbrake but not the progressive engine. Any kind of structure has been appearing only because and for reason "for something" and if it became impossible for achieving "because" by the application - no-one will use it. Not every use case for structure developing require to include blockchain. There are huge list of use cases where no any necessity of using it, there are enough of primitive and very useful solutions.

What does it mean "statical structure"? This is the structure that will have no any changing in time. It will always be like it has been created.

And now about the topic of this article - types of the structure where might be implemented blocked elements of chain. There are might be really more of examples of the structures. The type of structure totally depend on "idea" that is requiring the structure.

**1) Root-oriented or Tree-like**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_002.png)

This kind is good enough for the structures which contained constant list of elements or it's growing slowly and there are not critical time of recalculation of the formulas for blocking chain. For example: 

* any kind of desktop or mobile application where structure is the list files that is required for application
* the departments of any company, where departments is the elements of the chained structure
* servers added to the cluster, where the structure is the net with elements (servers)

It's using in classical way of blocking chains. It has been described in [Wiki blockchain page](https://en.wikipedia.org/wiki/Blockchain). When you are adding element to chain it will require you to recompute whole object.

**2) Linear or vector**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_003.png)

The structure is linear - when every element connected only to two other elements of the structure, one forward - on backward, one upstairs - one downstairs and etc. For example:

* event flow where the value of time is the blocked position relatively to others on the vector of timeline
* the path description where the sequence of points is the direction where direction is the block for elements - points 

The inherited structures:

* Circle - when last element connected to the first
* Way from root to the last element of the branch in tree-like structure

**3) Matrix**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_004.png)

One of the most complex structure because of layers of substructures and the relations between each other and the every points by the specially defined formula or algorithm. For example might me explained the use case of gathering reports of the company's departments state every 10 minutes, or gathering currency exchange values, or cron table in handling servers and etc, where the elements of matrix might be record in the DB-engine.

**4) Organic**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_005.png)

This term came from "Chemistry" - there are part of it named "Organic chemistry". It came because most obvious example of this term. This type is not standalone time, it's time kind of property to previously described where for example might be:

* the link between elements might contain value too
* element might contain limit for the connected events

There are huge list of examples of Organic structures:

* the roads, where the wide of the road and the quality road surface defining maximal value for number of the cars
* electrical networks, where the maximal possible value of the power line regulating line capacity and the connection points ability require maximal value of the connected subnetworks
* the internet 
* etc

There might be developed of defined huge variations of the structure. The structure's schema is depend only on "idea". To describe every possible variation of the structure - not the goal of this article. The goal of this article is to show that this structure based on "idea" is the start point for developing blocked chain for you own necessity.

The additional information about blockchain might be gotten from  the ["Arboreus articles: blockchain"](https://github.com/ArboreusSystems/arboreus_articles/tree/master/blockchain).

Follow author updates on [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/)

Follow AR|BO|RE|US updates on [**Twitter**](https://twitter.com/ArboreusSystems) and [**Linkedin**](www.linkedin.com/company/arboreus-systems/)