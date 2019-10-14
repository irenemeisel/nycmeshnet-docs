---
title: Overview of the Mesh
weight: 200
---

NYC Mesh is several things at once.

* The **technical implementation** of NYC Mesh is known as a *mesh network*.
* The **organization itself** is a non-commercial *Wireless ISP*.
* The **connected participants** operate numerous *community networks* "on the mesh" for the purpose of supporting various neighborhood initiatives that are of interest to local residents.

{{< youtube id="glW_S9bKAHk" >}}

## NYC Mesh as a mesh network

The term *mesh network* refers to the pathways connecting various participating members of the community. Rather than having a single gatekeeper through which all network traffic must be routed, each participant (called a *node* in our lingo) connects directly to as many other participants as they can. This means that as more members join the network, creating more and more nodes, there are more and more interconnections between members, which means there are more and more possible routes to get "there" from "here."

Put another way, as a mesh, various nodes connect to each other in a non-hierarchical way. Traffic flows between nodes in either direction, i.e., each node both receives or relays messages that originated at other nodes and sends out its own messages. In order for a message (called a *packet*, *frame*, or *segment* in formal networking terminology) to get to its destination, it must travel through one or more intermediary nodes, so each node in the mesh also dynamically routes these messages and responds to changing network conditions in real time, such as congestion or link failures. If one route to "there" becomes unavailable, the message will simply be re-routed along a different path between nodes, i.e., it will take a detour. Refer to our [Network Design Reference § Mesh Design]({{< relref "network-design/mesh" >}}) for more information regarding details of our meshing setup.

This general setup may already sound very familiar to you, because it's also how the Internet works! In fact, if you think of NYC Mesh's mesh network as a "small Internet" that just happens to be available in New York City, you would have a good general idea of how our network operates. Of course, NYC Mesh is *not* "the Internet," but it does *connect to* the Internet, because NYC Mesh is also a Wireless ISP.

## NYC Mesh as a Wireless ISP

Among the many benefits of [joining NYC Mesh](https://nycmesh.net/join) is lower-cost, high-speed Internet access. This means that by participating in our mesh network, you can visit websites like Wikipedia, check your email, read local and international news, and do all the things you would expect to be able to do online with any other Internet service. In this sense, NYC Mesh functions very much like a commercial Internet Service Provider (ISP), except that NYC Mesh is a non-profit community group (not a commercial enterprise), and we use slightly different methods to connect you to the Internet.

Unlike many traditional ISPs that use physical copper or fiber cabling buried under streets and sidewalks to connect their subscribers to the Internet, we use radio antennae mounted on building rooftops to increase our coverage area. This is where the *wireless* in Wireless ISP (WISP) comes in. Whenever we install a new antenna on a rooftop, the physical coverage area of our network expands exactly as far as the radio signal will reach. The [specifics of each installation]({{< relref "nodes" >}}) varies but, in general, every new node adds more coverage and creates more resilient network for NYC Mesh members.

In order to provide our members with Internet connectivity so that they can visit sites like Wikipedia that do not have servers within NYC Mesh's physical mesh network, we also operate a computer at a major NYC Internet exchange point (IXP) such as [DE-CIX](https://www.de-cix.net/en/locations/united-states/new-york). Because this computer is physically connected both to the rest of the Internet *and* to the NYC Mesh wireless mesh network, all connected NYC Mesh nodes can also access the rest of the Internet.

## NYC Mesh as a community network

Finally, some NYC Mesh participants who are involved in hyperlocal neighborhood projects run their own servers within the NYC Mesh network to offer services to friends and neighbors, or to solve problems that are specific to their area. These services, called [intra-mesh services]({{< relref "intra-mesh-services" >}}), range from simple blogs to software source code hosting. They offer intra-mesh alternatives to popular, commercial sites on the larger Internet. Most of these services are available *only* to other NYC Mesh participants; they are not accessible unless you are also connected to the NYC Mesh network itself.

In this way, NYC Mesh is also a community network, providing Internet-like services (website hosting, email, and so forth) to New York City locals without requiring them to travel across any part of the commercial Internet or across any non-neutral company's infrastructures. This ability for New Yorkers to connect to digital services run by their fellow New Yorkers over a physical network infrastructure of hardware devices fully owned by other New Yorkers is, for many, one of the most exciting parts of participating in NYC Mesh.
