# Assignment 5 : Settlers of Catan

This assignment is to implement the board game Settlers of Catan in code. It includes an introduction to the stream method for Collections.

Part 1 - HexNode
  -   Complete the Implementation of HexNode
      -   A node cannot have itself as a neighbour
      -   If going WEST from node1 we reach node2, then going EAST from node2 we reach node1. That is, the graph is non-directional: if node1 is connected to node2, then node2 is connected to node1 in the opposite direction.
      -   If going EAST from node1 we reach node2, and going NORTHEAST from node1 we reach node3, then going SOUTHEAST from node3 we reach node2.
      -   the method HexNode.isValid() contains useful assertions checking that the graph is valid ac- cording to those criteria. We encourage you to use isValid() or a similar personalized method to check if your code is preserving the validity of the graph.
  -   stream() and clockwiseStream() allows to stream the nodes

Part 2 - Game Play
  -   toString() prints out the information of the graph in a board shape
  -   setResources() takes pool of resources and distributes them left to right, top to bottom over the board
  -   getResourceCounters() takes pool of resource counters and distributes them on the board in a clockwise fashion. DESERT tiles are given a count with value NONE
  -   distributeResources() given a dice roll, distributes any resources gained to players that have settlements on tiles with that number
