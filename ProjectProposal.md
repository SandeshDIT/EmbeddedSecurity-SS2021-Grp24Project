# CS24 Project Proposal: Dijkstra Algorithm Implementation using FPGA

> Sandesh Gharge, Yogesh Nagor

## Overview

Our aim is to implement Dijkstra Algorithm using FPGA.

## Background

Dijkstra Algorithm is used to find the shortest path between two points in a given graph. Also distance calculations from any two points is independent of other calculations, this where FPGA can prove useful.

## Implementation Strategy

We will implement Dijkstra Algorithm using C++ Language.

Here’s how the algorithm is implemented:

- Mark all nodes as unvisited.

- Mark the initially selected node with the current distance of 00 and the rest with infinity.

- Set the initial node as the current node.

- For the current node, consider all of its unvisited neighbors and calculate their distances by adding the current distance of the current node to the weight of the edge that connects the current node to the neighboring node.

- Compare the newly calculated distance to the current distance assigned to the neighboring node. If it is smaller, set it as the new current distance of the neighboring node otherwise, keep the previous weight.

- When you’re done considering all of the unvisited neighbors of the current node, mark the current node as visited.

- Select the unvisited node that is marked with the smallest distance, set it as the new current node, and go back to step 4.

- Now repeat this process, until all the nodes are marked as visited.

Later this C++ file will be used to create Overlay.

And finally using PYNQ Framework Overlay will be tested.

## Tasks

1. Defining Dijkstra Algorithm
2. Creating Overlay
3. PYNQ Framework designing with following points :-
	3.1 Displaying shortest distance between all points
	3.2 Displaying path of each calculated distance
4. Testing

### Estimated Timeline

**(Core)**

* Task 1 (2 hours)
* Task 2 (4-5 hours)
* Task 3 (3-4 hours)
* Task 4 (2 hours)

## Resources

We took reference from following website - "https://www.geeksforgeeks.org/dijkstras-shortest-path-algorithm-greedy-algo-7/" for Algorithm.
