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

> Tara Safavi, Maryam Davoodi, Danai Koutra. _Career Transitions and Trajectories: A Case Study in Computing_. ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, August 2018.

BibTeX:

```
@inproceedings{Safavi:2018:CTT:3219819.3219863,
 author = {Safavi, Tara and Davoodi, Maryam and Koutra, Danai},
 title = {Career Transitions and Trajectories: A Case Study in Computing},
 booktitle = {Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery \&\#38; Data Mining},
 series = {KDD '18},
 year = {2018},
 isbn = {978-1-4503-5552-0},
 location = {London, United Kingdom},
 pages = {675--684},
 numpages = {10},
 url = {http://doi.acm.org/10.1145/3219819.3219863},
 doi = {10.1145/3219819.3219863},
 acmid = {3219863},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {career mining, computing research, graph mining, hits, professional trajectories},
} 
```


