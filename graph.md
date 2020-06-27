# Graphs

A graph is a collection of nodes and edges, usually drawn as a dot and line
diagram. Graphs can represent networks. In a transport network, nodes model
places and edges model roads or railways or flight connections. In a social
network, nodes model people and edges model acquaintances.

Normally each edge connects two different nodes and there's at most one edge between any pair of nodes
An undirected graph has at most one edge between any pair of nodes,
and each edge connects two different nodes.
In a directed graph, edges have directions, going from a source node to a target node.


## Graph properties

1. [Railroad](https://open.kattis.com/problems/railroad2) (2 LOC):
Determine if a 'closed' railway can be built, in which a train goes
continuously around. A different setting of the Königsberg bridges problem.

## Breadth-First Search

A BFS traversal visits all of a node's neighbours before visiting their
neighbours. It first visits nodes that are one hop away from the start node,
then those 2 hops away, etc.
BFS can thus find the shortest distance between a pair of nodes.

1. [Grid](https://open.kattis.com/problems/grid) (32 LOC):
Find the fewest movements to go from one corner of a grid to the opposite one,
following the possible moves.

## Depth-First Search

A DFS traversal follows one path from the start node, until the current node
leads to no new nodes. At that point, it backtracks and tries a different path.

For several connectivity problems (which nodes are connected to which),
it doesn't matter much whether to use DFS or BFS.

A recursive implementation of DFS may lead to a run time error for large graphs.

1. [Where's My Internet??](https://open.kattis.com/problems/wheresmyinternet)
(22 LOC): Find all nodes not connected to the given start node.
