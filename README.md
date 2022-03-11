# repo_cc_rsd
Global trends in grassland carrying capacity and relative stocking density of livestock.
Contains self-explanatory scripts needed to reproduce the analysis. 

Input data for MODIS land cover type and MODIS NPP, as well as for tree canopy cover downloaded via Google Earth Engine (GEE). See GEE_codes.txt.
This input data, as well as other input data, is processed in the file rast_processing_res000449.Rmd.

After that, we simulate the data in the file simulation.Rmd. Then, we plot figures for the main text in the file figures.Rmd and extract_countries.Rmd.
See also files areas_for_fig_classes.Rmd and cc_trend_with_linear_regression.Rmd for the figures.

Other files are needed to produce supplementary maps and data.

The files should be used in following order:
1) creating_TreeCoverMultiplier.Rmd
2) GEE_codes.txt
3) rast_processing_res000449.Rmd
4) simulation.Rmd
5) cc_trend_with_linear_regression.Rmd
6) figures.Rmd
7) extract_countries.Rmd
8) gather_isimip_data.Rmd
9) simulate_isimip_agb.Rmd
10) gather_glw_aw_for_figure_S4.Rmd
11) areas_for_fig_classes.Rmd

