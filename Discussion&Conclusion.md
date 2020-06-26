## Discussion

Automating TIGER/Line road data involves generating graphs for route analysis.  In the beginning, formation of a complete network from the original data was limited due to   1. Minor differences in the coordinates amongst points of interest (POIs),   2. Original TIGER/Line datasets containing parallel linestrings,   3. Multiple sections of a roadway not being truncated to the nearest decimal. 

[Solution: Truncating to the third decimal place (i.e. thousandths place) works well for easy snapping to the nearest point, but refrains from acknowledging the true infrastructures framework given that we are working with roadways.  Truncating to the fifth decimal place (i.e. hundred thousandths place) allows for connection while leaving intact most of the framework already driven spatially into the dataset.]



## Conclusion
In this study an algorithm is developed with the aim of solving the multiple subgraph existence problem in *Networkx*. The approach is developed to address the needs of the agencies such as Texas Department of Transportation (TxDOT) such as providing proper ID for the segments so relevant attribute values can be assigned.

The future work coming from this effort would reflect on putting any roadway network to the test and examining the process by which correcting linestring information would prove to help build route paths for origin-destination related shortest-path calculations.  



[Back to Poster Navigation Board](./poster_nav.md#Outline)
