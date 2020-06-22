# Role of linestring modification in prevention of road network subgraphs
This is a repository for purposes of presenting the SciPy2020 Poster at [SciPy2020](https://www.scipy2020.scipy.org).


## Contents of the Presentation
* [Summary]


## Summary
In this study, we used coordinate truncation in TIGER/Line datasets for roads to prevent the formation of subgraphs to ensure a connected graph for network analysis. The method consists of writing code to perform truncation of end coordinates, segmentation of linestrings at the intersection points, and identification of the original linestring to the segments. Overall, the results show improved network connectivity and better performance in finding shortest paths with Networkx. Part of the road network in the state of Texas is being used to demonstrate both the effect of multiple subgraphs and the improvement comes with the proposed approach.
