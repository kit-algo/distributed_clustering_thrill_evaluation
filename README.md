# Distributed Graph Clustering using Thrill - Evaluation

This repository contains Jupyter notebooks to analyse the results of the experimental evaluation of [kit-algo/distributed_clustering_thrill](https://github.com/kit-algo/distributed_clustering_thrill).

If you want to explore our data on your own you can download it [here](https://github.com/kit-algo/distributed_clustering_thrill_evaluation/releases/download/europar_final/results.tar.xz).
This archive contains a bunch of `json` files in which the output from the experiments (runtimes, quality scores, comparison scores) is stored in a database-like way.
Our notebooks assume that the content of this archive live in a folder next to this repository, but you can change the paths if you put it somewhere else.
To run the notebooks `cd` into the `notebooks` folder and run `jupyter notebook` (or `jupyter lab`).
See our existing notebooks on how to work with the data.

We also plan to make the actual raw data of our experiments available (input graphs, obtained clusterings, raw output of the programs), but so far we haven't found a good place to host this 1TB blob of data :see_no_evil:.
You can of course contact us to obtain it directly.

## Dependencies

The notebooks use [`pandas`](https://pandas.pydata.org/) for data analysis.
We used v0.20.3 but anything above and some below should do as well.
For plotting, `matplotlib 2.0` and `seaborn 0.8` were used.
Finally, you need `jupyter` in version `1.0.0` or above.

### Optional

The graph generation script makes use of [Networkit](https://github.com/kit-parco/networkit).
To be able to write our binary graphs you will need at least version 4.6.
