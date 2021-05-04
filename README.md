# Code for Williamson &amp; Witt 2021, 'Elevational niche-shift migration', Ornithology 138: 1-26.
 
If using data and code, please cite https://doi.org/10.1093/ornithology/ukaa087 & https://doi.org/10.5061/dryad.t1g1jwt1b.

See Dryad data publication (DOI above) for all raw data files, descriptions, and associated metadata. 

**Files in `r_scripts` folder:**

`ENSM_table_species_elev_data.Rmd`: This is main analysis file for manuscript. If upper and lower elevational range limits were not available for each the breeding and non-breeding seasons for putative ENSM taxa, we used this script to download records from GBIF and estimate elevational range limits. See more detailed description of methods in the main manuscript. Script file also includes several suggestions about how to better automate and improve workflows (i.e. forloop for GBIF downloads, extracting elevations from raster layers, etc.)

Please note that the GBIF download process has changed from when I first wrote this script in 2019. I have included a new code chunk that describes how the process is currently done (In fall 2020).

`ENSM_magnitude_of_shift_barplots.Rmd`: Script associated with data wrangling, plots, and figures. It includes data wrangling used for basic ENSM calculations, code to produce Figures 4, S4, S5, and S7. 

`ENSM_RadialPhylogenyFig.Rmd`: Script used to produce the radial phylogeny in Figure 2 (91 tips; 12 complete ENSM species and 79 partial ENSM species). It contains code for reading in .nex tree files and corresponding .csv files with "phenotypic" data (aka migration mode and magnitudes of elevational shift), as well as some data for labeling clades. The final tree file was read out of R in .pdf form and extensive editing took place in Illustrator afterwards. So please note: the final results produced from this script do not generate the figure. Many thanks to Chauncey R. Gadek for initial code and help with tree files and data wrangling.

`TableS1_ENSM_Supplement_Nov2020.csv`: Table S1 containing all final information from our elevational limit compilations. The Excel version of this file called contains metadata in tab 2 of the Excel workbook; the .csv version of this file contains metadata in 'TableS1_ENSM_Supplement_Nov2020_METADATA.csv'.  

`TableS2_Non-ENSM_Supplement_Nov2020.csv`: Table S2 containing information about candidate taxa that failed to qualify as ENSM (defined as having a calculated magnitude of elevational shift of <2,000 m). The Excel version of this file called contains metadata in tab 2 of the Excel workbook; the .csv version of this file contains metadata in 'TableS2_ENSM_Supplement_Nov2020_METADATA.csv'.  

If using data or code from this manuscript or repository, please cite: 

Williamson, Jessie; Witt, Christopher (2020), Elevational niche-shift migration: Why the degree of elevational change matters for the ecology, evolution, and physiology of migratory birds to Ornithology, Dryad, Dataset, https://doi.org/10.5061/dryad.t1g1jwt1b

---

Note (3 May 2021): Thanks very much to David Vander Pluym for bringing Tamarugo Conebill (*Conirostrum tamarugense*) to our attention as a probable ENSM species. Tamarugo Conebill breeds in northern Chile from sea level to 2,950 m (per BOW) or 3,500 m (per Jaramillo et al. 2004) and shifts upwards to ~3,400-4,100 in southern Peru for the non-breeding season. Some birds appear to move between lower elevations and 3,500 m in Chile only (Jaramillo et al. 2004). Schulenberg et al. 2007 note that *C. tamarugense* is an austral migrant; Fjeldsa and Krabbe 1990 note that some birds may breed at high elevations (suggesting residency? Partial austral migration only?). We have not accessed GBIF records or analyzed seasonal elevational range data for this species, though it is worth noting that it may be a partial ENSM species. 
