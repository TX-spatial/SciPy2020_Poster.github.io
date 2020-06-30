## Significance

### Introduction
The need for having a **road network in rural areas** exits for a number of reasons including but not limited to finding **shortest paths** for delivering goods and transporting people to a single destination or possibly multiple destinations.  Regardless of the method sought in network analysis (shortest path or **travelling salesman problem**), purpose of the trip (water delivery between water wells and oil wells, alternatively delivering COVID-19 kits to people in rural areas) amongst a **complete network** is always more desired. 

### Significance

When the Networkx is applied to a TIGER/Line dataset for the rural counties in Texas it was observed that there are lots of small non-connecting networks (**subgraphs**).  Existence of multiple subgraphs cause problem in route analysis eventhough the rural road data is provided in the same dataset.  Mitigating the causes of multiple subgraph formation is needed to improve network completeness. 

### Objective 
This study is aimed to develop an algorithm entirely in Jupyter notebooks for pre-processing TIGER/Line datasets in order to increase network completeness through **removal of parallel linestrings**, **melding of linestrings** with the same roadname, **linestring segmentation at junctions** and **end-coordinate truncation** where undershoot or overshoot is observed.  The developed approach is expected to prevent multiple subgraph formation for any given road network and allow shortest path analysis along with a more detailed and complete set of paths. 

[Back to Poster Navigation Board](./README.md#Outline)

