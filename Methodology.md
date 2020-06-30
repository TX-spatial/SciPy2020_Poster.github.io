## Methodology

The issues mentioned in the [Significance](./significance.md#Significance) section required a solution that will address them.  Accordingly, the following steps form the methodology:
* Inspecting the TIGER/Line dataset
  1. Obtaining the network structure (# of subgraphs)
  1. Existence of tiny linestrings
  2. Existence of parallel linestrings
* Pre-processing to mitigate above problems
  1. Removal of parallel linestrings
  2. Melding several linestrings of roads by employing itertools and Networkx
* Finding the crossing points or Point of interest (POIs) of each road 
* Segmenting the linestring
* Finding the end points where there exist
  1. Undershoot
  2. Overshoot
* Applying trucation (3 decimal digits) to end points obtained in the previous step
* Using Networkx to generate the graph and apply shortest path







[Back to Poster Navigation Board](./README.md#Outline)
