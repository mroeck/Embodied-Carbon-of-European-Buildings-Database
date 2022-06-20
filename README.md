Embodied-Carbon-of-European-Buildings-Database (EU-ECB-DB)
==============

***A public repository focused on Embodied Carbon Data of Buildings across Europe. The repository provides the building LCA data compiled, processed and analyzed as well as the scripts used for processing, analysis and visualisation.***

**Authors:** Developed by [Martin Röck (KU Leuven)](https://www.linkedin.com/in/martinroeck/)
and [Andreas Sorensen (Ramboll)](https://www.linkedin.com/in/a-soerensen/) within the ['Towards embodied carbon benchmarks for buildings in Europe' project](https://c.ramboll.com/lets-reduce-embodied-carbon).



# Documentation
## Usage Notes
The scripts provided in this repository have been established as [Jupyter Notebooks](https://jupyter.org/) which contain annotations and comments for improved understanding. Documentation on the dataset, how it was built as well as some analyses and visualiation can be found in the related reports
* Towards embodied carbon benchmarks for buildings in Europe - #1 Facing the data challenge (https://doi.org/10.5281/zenodo.6120522)
* Towards embodied carbon benchmarks for buildings in Europe - #2 Setting the baseline. A bottom-up approach" (https://doi.org/10.5281/zenodo.5895051)

## Data
Folder <code>/00_data/</code> contains the embodied carbon data (.xls/.csv) in multiple versions. The folder includes raw data from the original sources in the respective formats; the preprocessed and cleaned data; a harmonized version of the dataset including data from all sources, following a consistent data structure acc. to the pre-established EU-ECB data collection form (developed based on [Röck et al. 2020](https://doi.org/10.1016/j.apenergy.2019.114107)); as well as a version including additional features engineered in the respective scripts.
* <code>.../0_data_input_raw/</code> - Original data in the respective formats. Including  data collected via the EU-ECB data collection form.
* <code>.../1_data_pre_processed/</code> - Data preprocessed based on the original formats
* <code>.../2_data_concatenated/</code> - Data from all sources, concatenated in a harmonized format based on the data collection template form. 
* <code>.../3_data_feature_engineered/</code> - Concatenated data in harmonized format with additional engineered features.

## Running
To rerun the whole preprocessing and visualization pipeline run [00_Main.ipynb] script. Open and run individual notebooks from the root directory to only run selected parts of the procedure.
* <code>00_Main.ipynb</code> - Script for running the full preprocessing, feature engineering and visualization pipeline, i.e. calling all other scripts in consectutive order.
* <code>01_Prepoc*.ipynb</code> - Scripts for preprocessing of the respective data based on their original formats.
* <code>02_Data_Concat.ipynb</code> - Script for concatenating the original data in a common format.
* <code>03_Data_FeatEng.ipynb</code> - Script for engineering additional features based on the harmonized, concatenated data.
* <code>04_DataAnalysis*.ipynb</code> - Script for analysis and visualization of the data.

## Figures
Folder <code>/01_figures/</code> contains various visual outputs of the analysis including boxplots and heatmaps. The contents of this folder can be updated and are overwritten(!) when running <code>04_DataAnalysis*.ipynb</code> script.


# Background
## Embodied Carbon in the Building Sector
Funded by the [Laudes Foundation](https://www.laudesfoundation.org/), the project '['Towards embodied carbon benchmarks for buildings in Europe' project](https://c.ramboll.com/lets-reduce-embodied-carbon), by [Ramboll](https://ramboll.com/) in collaboration with leading researchers from [Aalborg University Build](https://www.build.aau.dk/) and [KU Leuven](https://www.kuleuven.be/english/research/), set out a framework for benchmarking and limiting the embodied carbon of new buildings.

The study identified solutions to measure embodied carbon emissions, define carbon budgets and targets. Importantly it includes recommendations for a baseline of current embodied carbon levels in new buildings, as well as considerations of the available carbon budget for these emissions. This will form the basis of a performance system in the shape of benchmarks for the reduction of embodied carbon.

## Download all reports
* #1 Facing the data challenge (https://doi.org/10.5281/zenodo.6120522)
* #2 Setting the baseline. A bottom-up approach (https://doi.org/10.5281/zenodo.5895051)
* #3 Defining budget-based targets. A top-down approach (https://doi.org/10.5281/zenodo.6120882)
* #4 Bridging the embodied carbon performance gap (https://doi.org/10.5281/zenodo.6120874)
* Summary report  - The important takeaways in short (https://doi.org/10.5281/zenodo.6397514)


# License and attribution
This data is published under a [CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/). When using this data and/or scripts, plese cite the respective DOIs of this repository as well as the related project reports (https://doi.org/10.5281/zenodo.6120522 & https://doi.org/10.5281/zenodo.5895051) and share your outputs under similar conditions. Thank you.
