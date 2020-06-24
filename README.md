# Role of linestring modification in prevention of road network subgraphs
This is a repository for purposes of presenting the SciPy2020 Poster at [SciPy2020](https://www.scipy2020.scipy.org). All the scheduled presentations can be viewed at [SciPy2020 Schedule](https://na.eventscloud.com/ehome/487022?&t=d2917a15274e1daf79d80a4253f01e7a).


## Contents of the Presentation
* [Summary]


## Summary
In this study, we used coordinate truncation in TIGER/Line datasets for roads to prevent the formation of subgraphs to ensure a connected graph for network analysis. The method consists of writing code to perform truncation of end coordinates, segmentation of linestrings at the intersection points, and identification of the original linestring to the segments. Overall, the results show improved network connectivity and better performance in finding shortest paths with Networkx. Part of the road network in the state of Texas is being used to demonstrate both the effect of multiple subgraphs and the improvement comes with the proposed approach.

## Objective
This study is aimed to develop an algorithm entirely in Jupyter notebooks for pre-processing TIGER/Line dataset to increase network completeness through coordinate truncation and proper segmentation of linestrings.  The developed approach is expected to prevent multiple subgraph formation for a given road network and allow shortest path analysis.  

## Data

The road network data is obtained from [TIGER/Line Shapefiles](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2019&layergroup=Roads) for the selected counties of the state of Texas. The data sets can be also fetched directly from the [Census FTP](https://www2.census.gov/geo/tiger/TIGER2019/ROADS/) by using the [county FIPS number](https://tx.postcodebase.com/state_county). If you prefer to fetch multiple county road datasets you may use [census_fetcher.py](https://gist.github.com/flibbertigibbet/8092460) by Kathryn Killebrew. In this study we decided to use TIGER/Line datasets instead of other open source data such as [OpenStreetMap](https://download.geofabrik.de/index.html) due to better rural area coverage provided by the former source. While volunteers work on 

## Analysis

Inital Networkx analysis of the road network data of all four counties is summarized in Table 1

|    | County     |   FIPS |   No of linestrings |   Total length |   No_nodes |   No_edges |   Avg_degree |
|---:|:-----------|-------:|--------------------:|---------------:|-----------:|-----------:|-------------:|
|  0 | Kimble     |  48267 |                3389 |           2413 |       4285 |       3290 |       1.5356 |
|  1 | Menard     |  48327 |                1424 |           1289 |       1853 |       1388 |       1.4981 |
|  2 | Schleicher |  48413 |                4079 |           2639 |       4397 |       3989 |       1.8144 |
|  3 | Sutton     |  48435 |                6047 |           3265 |       6452 |       5891 |       1.8261 |




## Codes


An example code is given below, which will be replaced with actual codes from the study.
```python
import pandas as pd
import geopandas as gpd
import shapely
```

## Tables
The tables are obtained from pandas dataframes with `df.to_markdown()`command.

Sample table

| Row  |    A |    B |
| :--- | ---: | ---: |
| a    |    1 |    1 |
| a    |    2 |    2 |
| b    |    3 |    3 |

## Conclusion

 In this study an algorithm is developed with the aim of solving the multiple subgraph existence problem in *Networkx*. The approach is developed to address the needs of the agencies such as Texas Department of Transportation (TxDOT) such as providing proper ID for the segments so relevant attribute values can be assigned.    



#### Maps of the Kimble County

![A-Kimble](img/A-Kimble.png)

![B-Kimble](img/B-Kimblemulti.png)
