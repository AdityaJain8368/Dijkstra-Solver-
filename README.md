# Dijkstra-Solver

## About the Dijkstra Algorithm : 
  It is an algorithm for finding the shortest paths between nodes in a graph,
  which may represent, for example, road networks. It was conceived by
  computer scientist Edsger W. Dijkstra in 1956 and published three years later.
  Dijkstra thought about the shortest path problem when working at the Mathematical Center in
  Amsterdam in 1956 as a programmer to demonstrate the capabilities of a new computer called
  ARMAC. His objective was to choose both a problem and a solution (that would be produced 
  by computer) that non-computing people could understand. He designed the shortest path 
  algorithm and later implemented it for ARMAC for a slightly simplified transportation map of 
  64 cities in the Netherlands (64, so that 6 bits would be sufficient to encode the city number).
  A year later, he came across another problem from hardware engineers working on the institute's
  next computer: minimize the amount of wire needed to connect the pins on the back panel of the
  machine. As a solution, he re-discovered the algorithm known as Prim's minimal spanning 
  tree algorithm (known earlier to Jarník, and also rediscovered by Prim).[11][12] Dijkstra
  published the algorithm in 1959, two years after Prim and 29 years after Jarník.[13][14]
 
 ![image](https://user-images.githubusercontent.com/110038824/182672374-71051cdb-6a91-4915-865b-99fe62e6c44b.png)


Algorithm 
1) Create a set sptSet (shortest path tree set) that keeps track of vertices included in the shortest-path tree, i.e., whose minimum distance from the source is calculated and finalized. Initially, this set is empty. 
2) Assign a distance value to all vertices in the input graph. Initialize all distance values as INFINITE. Assign distance value as 0 for the source vertex so that it is picked first. 
3) While sptSet doesn’t include all vertices 
….a) Pick a vertex u which is not there in sptSet and has a minimum distance value. 
….b) Include u to sptSet. 
….c) Update distance value of all adjacent vertices of u. To update the distance values, iterate through all adjacent vertices. For every adjacent vertex v, if the sum of distance value of u (from source) and weight of edge u-v, is less than the distance value of v, then update the distance value of v. 

## 
