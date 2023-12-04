# SRN_MIDAS

This is a repository containing the processed data used in the project titled, "Data-Driven Traffic Assignment Through Density-Based Road-Specific Congestion Function Estimation".

The data set is for the England Strategic Road Network. It was created using MIDAS traffic data from the period September 2018 to May 2019. 

The methodology for producing the processed data from the raw data is described in the paper "Data-Driven Traffic Assignment Through Density-Based Road-Specific Congestion Function Estimation", IEEE Access (tbc).

## Contents
The repository contains two folders. E2 is the full network used for analysising the England Strategic Road Network. This graph representation has 73 nodes and 156 edges. E1 is a simplified version of E2, with a number of junctions and roads omitted. It contains 30 nodes and 70 edges. It has been used for more computationally demanding analysis.

For both E1 and E2, a node table and edge table are supplied. This can be used to create a network representation of the road system (for instance using Matlab or NetworkX).

Time bin flow and speed data are provided for E2. The JSON files contain the the average flow (veh/hr) and speed (km/hr) for each edge on the network on each selected weekday of analysis for the time bins: AM (6 am - 10 am), MD (10 am - 4 pm), and PM (4 pm - 8 pm). Only time bin flow data is provided for E1.

Additionaly, per-minute flow (veh/hr), occupancy (%) and speed (km/hr) data are provided for E2. This has been used for the fitting of congestion (a.k.a. Volume-Delay) functions. The JSON files contain the processed per-minute observations for each edge on the network for each minute of the time bin on each selected weekday of analysis.

## Related publications
Alexander Roocroft, Giuliano Punzo, Muhamad Azfar Ramli. Link Count Data-driven Static Traffic Assignment Models Through Network Modularity Partitioning. Transportation, Springer. September, 2023. (Available: [here](https://doi.org/10.1007/s11116-023-10416-x))

Alexander Roocroft, Muhamad Azfar Ramli, Giuliano Punzo. Improved Data-Driven Optimal Traffic Assignment Through Density-Based Road-Specific Congestion Function Estimation. IEEE Access. 2023 (under review).

Alexander Roocroft, Giuliano Punzo, Muhamad Azfar Ramli. System Optimal Routing and Distribution of Benefits on National Road Networks. In: Transportation Procedia, 2023. (In Press).

Alexander Roocroft, Muhamad Azfar Ramli, Giuliano Punzo. Efficient Computation of Optimal Traffic Assignment in Nationwide Highway Networks from Raw Loop Detector Data. In: Transportation Research Board 100th Annual Meeting, Washington D.C., 2021


## Licensing
This code is available under the MIT License. Copyright (c) 2023 Alex Roocroft

## Authors
Alexander Roocroft ([ORCID](https://orcid.org/0000-0002-6551-1800), a.roocroft@tudelft.nl)

Giuliano Punzo (g.punzo@sheffield.ac.uk)

Muhamad Azfar Ramli (ramlimab@ihpc.a-star.edu.sg)




