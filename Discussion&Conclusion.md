## Discussion

#### Challenges
Automating TIGER/Line road data involves **generating graphs** for **_route analysis_**. In the beginning, formation of a **complete network** from the original data was limited due to 
1. **Undershoot/overshoot** were observed on the end points of linestrings
2. Original TIGER/Line datasets containing **parallel linestrings**
3. **Multiple sections** of a roadway not being **truncated** to the nearest decimal.
4. Not all the road sections (linestrings) have an **assigned name**

#### Solution Approach

Using road names in the **_FULLNAME field_** of **TIGER/_Line_** data allowed the grouping of linestrings which permitted the following:
**1.** Parallel linestrings were identified and dropped
**2.** Remaining linestrings were ordered and meld
**3.** Truncation (three decimal digits) was applied only to the end points where undershoot/overshoot were observed


## Conclusion
In this study an algorithm is developed with the aim of solving the **_multiple subgraph existence_** problem in **TIGER/_Line_** road dataset for selected Texas counties with *Networkx*. The approach is developed to address the needs of the agencies such as Texas Department of Transportation (TxDOT) such as providing proper ID for the segments so relevant attribute values can be assigned.

The future work coming from this effort would reflect on putting any roadway network to the test and examining the process by which correcting linestring information would prove to help build route paths for origin-destination related shortest-path calculations.



[Back to Poster Navigation Board](./README.md#Outline)

