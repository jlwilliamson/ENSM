# Files and code for Williamson &amp; Witt, 'Elevational niche-shift migration', In revision


Files in `r_scripts` folder: 
`ENSM_table_species_elev_data.Rmd`: This is main analysis file for manuscript. If upper and lower elevational range limits were not available for each the breeding and non-breeding seasons for putative ENSM taxa, we used this script to download records from GBIF and estimate elevational range limits. See more detailed description of methods in the main manuscript. Script file also includes several suggestions about how to better automate and improve workflows (i.e. forloop for GBIF downloads, extracting elevations from raster layers, etc.)

Please note that the GBIF download process has changed from when I first wrote this script in 2019. I have included a new code chunk that describes how the process is currently done.

`ENSM_magnitude_of_shift_barplots.Rmd`: Quick summary  calculations to generate magnitude of elevation shift barplots for the supplement (Figs S4-S5) of Williamson & Witt, 'Elevational niche-shift migration'.

`ENSM_RadialPhylogenyFig.Rmd`: Script used to produce the radial phylogeny figure (91 tips; 12 complete ENSM species and 79 partial ENSM species) in Williamson & Witt, ENSM (Figure 2). It contains code for reading in .nex tree files and corresponding .csv files with "phenotypic" data (aka migration mode and magnitudes of elevational shift), as well as some data for labeling clades. The final tree file was read out of R in .pdf form and extensive editing took place in Illustrator afterwards. So please note: the final results produced from this script do not generate the figure. Many thanks to Chauncey R. Gadek for initial code and help with tree files and data wrangling.