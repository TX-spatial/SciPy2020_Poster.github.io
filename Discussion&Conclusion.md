## Discussion

In this study a methodology is being proposed for automating TIGER/Line road data to generate graphs for route analysis.  There were multiple issues which prevented the formation of a complete network from the original data.  Minor differences in the coordinates caused the formation of many subgraphs as we observed in Table 2 for all of the counties considered in this study. The original TIGER/Line datasets contained parallel linestrings and multiple sections of a roadway which were causing problems in graph formation and in the use of truncation.  The rounding of the coordinates to five decimal digits worked well as the three decimal digit truncation at selected coordinates helped to improve the graph.



## Conclusion
In this study an algorithm is developed with the aim of solving the multiple subgraph existence problem in *Networkx*. The approach is developed to address the needs of the agencies such as Texas Department of Transportation (TxDOT) such as providing proper ID for the segments so relevant attribute values can be assigned. 



[Back to Poster Navigation Board](./poster_nav.md#Outline)
