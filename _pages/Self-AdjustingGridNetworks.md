---
layout: single
author_profile: true
title: "Self-Adjusting Grid Networks "
permalink: /Self-AdjustingGridNetworks
---

Source: C. Avin, M. Borokhovich, B. Haeupler, and Z. Lotker, “[Self-adjusting grid networks to minimize expected path length](https://doi.org/10.1007/978-3-319-03578-9_29),” Theor. Comput. Sci.. 584: 91–102 2015.

Network size 30 * 30. Number of clusters 8, 50% of nodes are inactive

![animation](/assets/images/animation3.gif){: .align-center}

---

In this animation, we can see how a local greedy switching algorithm adjusts the network so that the nodes belonging to the same cluster (same color) will be located closer together, thus, minimizing the expected path (route) length.
Nodes surrounded by a **black** rectangle are the centers of their clusters.

The algorithm goes as follows. Every node can switch (exchange locations) with its direct neighbor (any node at the distance of 1 hop in torus) or with a node that is located at a distance of 3 but not at the same line (i.e., a node that can be reached by a move of a chess knight). The switch is performed only if the expected path length of the network decreases as a result of the switch.

---

In the animation below, we have 900 nodes randomly separated into 16 clusters, i.e., there are on average 900/16 nodes in every cluster.

<iframe width="640" height="360" src="http://www.youtube.com/embed/RFG-zMk6uwo" frameborder="1" allowfullscreen></iframe>


----
In the second animation bellow, we have 450 inactive randomly located nodes, and the rest 450 nodes are separated into 8 clusters, i.e., there are in average 450/8 = 900/16 nodes in every cluster.
(:includeurl "http://www.youtube.com/embed/ZaaLXEPpY6o"  border=1:)
