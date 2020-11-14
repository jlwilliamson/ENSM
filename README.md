# Files and code for Williamson &amp; Witt, 'Elevational niche-shift migration', In revision


**Files in `r_scripts` folder:** \n
`ENSM_table_species_elev_data.Rmd`: This is main analysis file for manuscript. If upper and lower elevational range limits were not available for each the breeding and non-breeding seasons for putative ENSM taxa, we used this script to download records from GBIF and estimate elevational range limits. See more detailed description of methods in the main manuscript. Script file also includes several suggestions about how to better automate and improve workflows (i.e. forloop for GBIF downloads, extracting elevations from raster layers, etc.)

Please note that the GBIF download process has changed from when I first wrote this script in 2019. I have included a new code chunk that describes how the process is currently done.

`ENSM_magnitude_of_shift_barplots.Rmd`: Not the best title - Script associated with data wrangling, plots, and figures. It includes data wrangling used for basic ENSM calculations, code to produce Figures 4, S4, S5, and S7. 

`ENSM_RadialPhylogenyFig.Rmd`: Script used to produce the radial phylogeny figure (91 tips; 12 complete ENSM species and 79 partial ENSM species) in Williamson & Witt, ENSM (Figure 2). It contains code for reading in .nex tree files and corresponding .csv files with "phenotypic" data (aka migration mode and magnitudes of elevational shift), as well as some data for labeling clades. The final tree file was read out of R in .pdf form and extensive editing took place in Illustrator afterwards. So please note: the final results produced from this script do not generate the figure. Many thanks to Chauncey R. Gadek for initial code and help with tree files and data wrangling.

Table S1 contains all final information from our elevational limit compilations. The version of this file called `TableS1_ENSM_Supplement_Nov2020.csv` contains metadata (tab 2 in the Excel sheet), while the .csv version does not contain metadata. 
Table S2 contains information about some taxa that failed to qualify as ENSM (defined as having a calculated magnitude of elevational shift of <2,000 m). The version of this file called `TableS2_Non-ENSM_Supplement_Nov2020.csv`. 

See metadata tabs available in Excel files on Dryad for metadata. 

If using data or code from this manuscript or repository, please cite: [INSERT DOI]

