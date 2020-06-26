## Methodology

Several steps form the methodology
* Inspecting the TIGER/Line dataset
  1. Obtaining the network structure (# of subgraphs)
  1. Existence of tiny linestrings
  2. Existence of parallel linestrings
* Pre-processing of to mitigate above problems
  1. Removal of parallel linestrings
  2. Melding several linestrings of roads by employing itertools and Networkx
* Finding the crossing points of each road
* Segmenting the linestring
* Finding the end points where there exist
  1. Undershoot
  2. Overshoot
* Applying trucation (3 decimal digits) to end points obtained in the previous step
* Saving the road network in shp format
* Using Networkx to generate the graph and apply shortest path







[Back to Poster Navigation Board](./poster_nav.md#Outline)
