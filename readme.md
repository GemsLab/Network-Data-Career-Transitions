# About

This repository hosts two anonymized network datasets of post-PhD career transitions and trajectories in computing research. We analyzed this data in a [paper](https://arxiv.org/abs/1805.06534) studying the evolution of computing research as a profession on the levels of individuals (people with PhDs in computer science), organizations (companies, schools, agencies, etc), and sectors (one of academia, industry, or government). 

# Data directory contents

The ```organizations.csv``` file maps organization IDs to their respective sectors.

The ```temporal.csv``` network is weighted, directed, and temporal.
Each node in this network is an organization ID. 
Each edge encodes a source organization, a destination organization, and the number of people moving from the source to the destination at the specified year. 

The ```bipartite.csv``` network is a heterogeneous bipartite graph connecting people to organizations. 
Per edge, the first node is an individual ID and the second node an organization ID. 
An individual is connected to an organization if (1) they did their PhD there or (2) they worked there at some point in their career. 
The ```EdgeType``` attribute encodes whether the individual in question did their PhD or worked at the connected organization.

# Citation

If you use this dataset, please cite:

> Tara Safavi, Maryam Davoodi, Danai Koutra. _Career Transitions and Trajectories: A Case Study in Computing_. ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (_to appear_), August 2018.


