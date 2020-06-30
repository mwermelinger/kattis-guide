# Graphs

A graph is a collection of nodes and edges, usually drawn as a dot and line
diagram. Graphs can represent networks. In a transport network, nodes model
places and edges model roads or railways or flight connections. In a social
network, nodes model people and edges model acquaintances.

Nodes are also called vertices; edges are also called arcs or links.

There are various kinds of graphs. In a simple undirected graph, there's
at most one edge between any pair of nodes,
and each edge connects two different nodes.
In a digraph, short for directed graph, each edge has a direction,
going from a source node to a target node.
In a weighted (directed or undirected) graph,
each edge has a number that represents some attribute of interest, e.g.
the distance, time or cost to move along the edge from one node to the other.

## Graph properties

1. [Railroad](https://open.kattis.com/problems/railroad2) (2 LOC):
   Determine if a 'closed' railway, in which a train goes continuously around,
   can be built. A different setting of the Königsberg bridges problem.

1. [Weak Vertices](https://open.kattis.com/problems/weakvertices) (16 LOC):
   Three nodes A, B and C form a triangle if there are edges A-B, B-C and C-A.
   Find all nodes that aren't part of any triangle.

## Breadth-First Search

A BFS traversal visits all of a node's neighbours before visiting their
neighbours. It first visits nodes that are one hop away from the start node,
then those 2 hops away, etc.
BFS can thus find the shortest distance between a pair of nodes.

1. [Grid](https://open.kattis.com/problems/grid) (32 LOC):
   Find the fewest movements to go from a corner of a grid to the opposite one,
   following the possible moves.

## Depth-First Search

A DFS traversal follows one path from the start node, until the current node
leads to no new nodes. At that point, it backtracks and tries a different path.
A recursive implementation of DFS may lead to a run time error for large graphs.

For several connectivity problems (which nodes are connected to which),
it doesn't matter much whether to use DFS or BFS.

1. [Where's My Internet??](https://open.kattis.com/problems/wheresmyinternet)
   (22 LOC): Find all nodes not connected to the given start node.
