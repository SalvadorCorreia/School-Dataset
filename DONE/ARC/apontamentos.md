# Complex Networks Notes
## Definitions
### Closeness Centrality (CC)
Closeness Centrality is a metric used to describe the distance of a node to all other nodes. It is measured as the inverse of the sum of the lengths of the shortest paths from a node to all other nodes. For unweighted graphs, the best method to calculate it would be a **BFS**, with complexity of O(V+E), where V representes the Verticies of the Network and E the Edges.
### Betweenness Centrality (BC)
Betweenness Centrality is a metric used to describe how often a node is part of the shortest path between all other nodes. For unweighted graphs, the best method to calculate it would be a **BFS** for each node, with complexity of O(V*(V+E)), where V representes the Verticies of the Network and E the Edges.
### Page Rank (PR)
Page Rank tries to measure the importance of nodes in **Directed Graphs** through the importance of its peers. It does this by giving each node a starting value, then each node evenly distributes its value through all their outgoing connections. After some iterations each node's value will reach an equilibrium representing how important they are. The most common method to measure it would be the **Power Iteration**, with complexity of O(k(V+E)), where k representes the number of iterations needed for the values to reach an equilibrium, V represents the Verticies of the Network and E the Edges.
$$
PR(v) = d \sum_{u \in In(v)} \frac{PR(u)}{Out(u)}
$$
### Average Path Length (APL)
Average Path Length is the average length of the shortest path between all pairs of nodes in a network.
### Small World Networks
Small World networks are networks with **High Clustering** and **Low Average Path Length**.

High clustering means that a nodes neighbors are very likely to be neighbors with each other.
Low Average Path Length means that it would take a small amount of steps to go from one node to any other node.
### Watts-Strogatz model
