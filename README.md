# Revisiting Reynolds 2021

In the repository we perform a reanalysis of the single-cell RNA seq skin dataset from [Reynolds et al. (2021)](https://doi.org/10.1126/science.aba6500).
The initial analysis was focused on the analysis of the healthy fibroblasts, in order to check the replicability of our results with other fibroblast datasets in [Ascensión et al. (2020)](https://doi.org/10.1016/j.jid.2020.11.028).

Our main discoveries from the analysis are:
* Main population profiles from our publication (A1, A2, B1, B2 fibroblasts) can be replicated in Reynolds et al. dataset.
* However, we find that the FB2 population from the original analysis are fibroblasts affected by sample manipulation. 
* Also, half of the Fb1 + Fb3 populations show a clear hypoxic profile. The other half shows neither a hypoxic not stress profile.
* The three fibroblast populations partly conserve the fibroblast (A1/A2/B1/B2) profiles, but are separated in the manifold by stress/hypoxia.
* The rest of cell types (pericytes, keratinocytes, endovascular cells, immune cells) also replicate these stress/hypoxia profiles.


## Understanding the repository
In the repo you will find 3 notebooks:
* `0_data_extraction.ipynb`: it contains the code to download the preprocessed AnnData with all cells, as well as the code to download and process the raw data to loom files.
* `1_fibroblast_analysis.ipynb`: it contains the analysis on fibroblasts (from loom files). There we describe the first 4 discoveries.
* `2_stress_hypoxia_all_populations.ipynb`: it contains the analysis on the rest of cell types, in healthy, diseased and all donors.

The notebooks are empty. To see the notebooks with output, we have stored them alongside relevant intermediate AnnData files in our [Zenodo repository](https://doi.org/10.5281/zenodo.4709059)