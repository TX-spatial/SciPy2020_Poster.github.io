# Role of linestring modification in prevention of road network subgraphs
Mehmet Kunt<sup>1</sup>,PhD, Jennifer Zuehlke<sup>2</sup>, Randy Machemehl<sup>2</sup>, PhD, PE

<sup>1</sup>[Eastern Mediterranean University](https://www.emu.edu.tr/en), <sup>2</sup>[The University of Texas at Austin](https://www.utexas.edu/)

This is a repository for purposes of presenting the SciPy2020 Poster at [SciPy2020](https://www.scipy2020.scipy.org). All the scheduled presentations can be viewed at [SciPy2020 Schedule](https://na.eventscloud.com/ehome/487022?&t=d2917a15274e1daf79d80a4253f01e7a).


## Summary
In this study, we used **coordinate truncation** in **TIGER/_Line_** datasets for roads to prevent the formation of subgraphs and to ensure a connected graph for network analysis. The method consists of writing a structured code to perform **_truncation of end coordinates_**, **_segmentation of linestrings at the intersection points_**, and **_identification of the original linestring to the segments_**. Overall, the results show improved network connectivity and better performance in finding shortest paths with Networkx. Part of the road network in the state of Texas is being used to demonstrate both the effect of multiple subgraphs and the improvement comes with the proposed approach.

## Outline

| <center>Poster</center>           | <center>Navigation</center>   | <center>Board</center>                              |
|:----------------------------------|:------------------------------|:----------------------------------------------------|
| [Significance](./significance.md#Significance) |    | [Discussion](./Discussion&Conclusion.md#Discussion) |
| [Data](./Data.md#Data)                 | [Analysis](./Analysis.md#Analysis)     | [Conclusion](./Discussion&Conclusion.md#Conclusion) |
| [Methodology](./Methodology.md#Methodology)   |      | [Tools](./tools.md#Tools)   



