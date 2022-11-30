# TravellingSalesman

This is an interactive demo for the famous Travelling Salesman problem. I created this as a learning tool for my computer science students.
Use the create node button at the top of the page to randomly add nodes to the page, these nodes represent the cities that the salesman will have to visit.
Use the solve button to run the three included algorithms. Each algorithm has been chosen to spark discussion regarding the topic.

## The Travelling Salesman

The Travelling Salesman problem is a great way to explore the advantages and disadvantges of heuristic techniques.
The problem asks the developer to create an algorithm that will find the salesman the shortest path which visits each city (node) once and then returns back to the starting node.

The demo shows how three seperate algorithms could tackle the same problem (and the same input).

##### Best Path

This algorithm will find the absolute best path. It is very inefficient and will check every possible combination before providing a final output. For large datasets, this algorithms could take many hours to compute the best path.
This algorithms is included to help students reason whether knowing the definite best path is worth the time it takes to calculate it.

##### Shuffle Path

This algorithm creates 1000 random paths. The best path is stored and displayed as the final result.
For a medium sized dataset (between 5 and 10 nodes) this algorithm usually produces an sub-optimal but okay path.
It is included to raise questions regarding the choice between an optimal and approximate value, what if a company using the algorithm continually gets dealt a poor path and wastes time and resources?

##### Greedy Path

This heuristic algorithm is efficient and usually produces an acceptable path.
The greedy path algorithm starts at a chosen node and then moves to the closest node to the current node. It does this until all nodes are visited and then moves back to the starting node. It does this for each node in the set and outputs the shortest path found.
This technique uses logic rather than random selection and raises the point that there are optimal and sub-optimal heuristic techniques.

## Inheritance

The source code also demonstrates class inheritance in JavaScript. There is a standard Path class from which the three algorithms above inherit.
The standard Path class encapsulates the functions which are similar between the algorithms.
