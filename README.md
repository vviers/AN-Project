# AN-Project

## Network analysis of voting patterns French Members of Parliament between 2012 and 2017 (14ème législature)
DataSource : [Assemblée Nationale - Open Data](http://data.assemblee-nationale.fr/)

----

This repository contains all data and code used for my [Applied Econometrics & Public Policy](https://github.com/bryangraham/Ec142) final project: _a network analysis of the voting behavior of French Members of Parliament (MP) between 2012 and 2017._

The project can be thought of as three distinct parts:
+ **Data generation** – extracting adjacency matrices between all MP for each major vote from the `XML` file available online. This is _far_ from being straightforward given the structure of the original data. The code used to generate the data can be found in `Generate_Data.ipynb` and `Vote_Assemblee_Nationale_Adjacency_Matrix.ipynb`. The resulting data can be found in the [`adjacency_matrices/`](https://github.com/vviers/AN-Project/tree/master/adjacency_matrices) folder. Some other data is sort of all over the place in the repo right now. Cleaning this is on my todo list.
+ Some interesting **Data description** can be found in `Basic EDA.ipynb` and at the begining of `Data_Analysis_Econ142.ipynb`(which is the file I submitted for my final project)
+ Finally, I design and estimate a **context-relevant model of centrality** for the MP graph in `Data_Analysis_Econ142.ipynb`. I fit the "lobbyist model" by Monte-Carlo simulation and compute bootstrapped standard errors for my measures. I export the resulting rankings as CSV files in the repo in `full_2_waves_ranking.csv`.

----
Any comment / critique is most welcome!
