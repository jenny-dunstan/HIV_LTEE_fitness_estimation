# HIV LTEE fitness estimation

The data and code to accompany the paper "Estimating fitness effects of mutations that evolve in a long-term evolution experiment of HIV-1".

## Directories

### Analysis
This directory contains all the code for the analysis performed in the paper. It requires only data supplied in the Data directory, and will produce the files in the Out directory as well as the figures in the Figures directory.

This directory consists of 10 Jupyter notebook files which can be run independently. For each notebook, the required packages are listed at the top. 

An overview of each notebook file:
1. Ancestor: analysis of the ancestor population sequence data
2. Process data: first exploration of the sequencing data and preparation of the data for the MPL method
3. Data analysis: analysis of the sequencing data including looking at the coverage, mutation accumulation and positions
4. MPL: fitness estimation using the MPL method and exploration of the resulting distribution of fitness effects
5. Assays: comparison of population fitness estimates to estimates from competition assay experiments
6. Simulations: simulations of an evolution experiment to allow fitness estimation methods to be tested in different regimes
7. Characteristics analysis: analysis of how the estimated fitness effects are associated with different characteristics via multiple statistical tests
8. Fitness analysis: analysis of the estimated fitness effects including parallel mutations, the beneficial tail, the fitness effects against fixation time and the true covariance matrix
9. DMS comparison: compares the estimated fitness effects to previous estimates from deep mutational scanning on two datasets
10. Sensitivity testing: explores how the fitness effects are sensitive to sequencing depth and parameters of the MPL method


### Data
This directory contains the data required for the analysis in the paper. 

Deep Mutational Scanning data reproduced from Haddox et al. 2018 and Hong et al. 2024 is supplied in the directory DMS.

Other files contain the processed mutation data from the HIV LTEE (Bons et al. 2020) (all_dels.pkl, all_ins.pkl and all_muts.pkl contain the deletion, insertion and substitution mutations repsectively), the ancestor population consensus sequence (ancestor_consensus.fasta), population fitness estimates from competition assays (assay_fitness_estimates.npz), the HIV-1 gene positions (genes.csv), and details of the substitution mutations from Bons et al. 2020 (mutation_types.pkl).

Some data (sequence files from each evolutionary line and the ancestor population) are too large to submit here and instead can be found on Zenodo at: https://doi.org/10.5281/zenodo.24590954

### Figures
All figures produced by the analysis files are found here. This includes combined figures for the paper. Almost all are stored as .pdf except three which are stored as .png as they are very large .pdf files.

### Out
Data files produced by the analysis files are found here. This includes the table of all mutations and their estimated fitness effects as well as the estimated and true covariance matrices.
