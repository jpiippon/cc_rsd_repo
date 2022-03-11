# repo_cc_rsd
Global trends in grassland carrying capacity and relative stocking density of livestock.
Contains self-explanatory scripts needed to reproduce the analysis. 

Input data for MODIS land cover type (Sulla-Menashe & Friedl, 2018) and MODIS NPP (Running & Zhao, 2019), as well as for tree canopy cover (Sexton et al., 2013) downloaded via Google Earth Engine (GEE). See GEE_codes.txt for this input data. For downloading the data for temperature (Abatzoglou et al., 2018), terrain slopes (Amatulli et al., 2020), gridded livestock of the world (Gilbert et al., 2018) and global livestock production systems (Robinson et al., 2011), see references at the end of this document. This input data is processed in the file rast_processing_res000449.Rmd.

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

For country polygons we used 10m data from Natural Earth. See https://www.naturalearthdata.com/
and regional macroregion polygons adapted from Kummu et al. (2010). 

References:

Abatzoglou, J. T., Dobrowski, S. Z., Parks, S. A., & Hegewisch, K. C. (2018). TerraClimate, a high-resolution global dataset of monthly climate and climatic water balance from 1958–2015. Scientific Data, 5(1), 170191. https://doi.org/10.1038/sdata.2017.191

Amatulli, G., McInerney, D., Sethi, T., Strobl, P., & Domisch, S. (2020). Geomorpho90m, empirical evaluation and accuracy assessment of global high-resolution geomorphometric layers. Scientific Data, 7(1), 162. https://doi.org/10.1038/s41597-020-0479-6

Gilbert, M., Nicolas, G., Cinardi, G., Van Boeckel, T. P., Vanwambeke, S. O., Wint, G. R. W., & Robinson, T. P. (2018). Global distribution data for cattle, buffaloes, horses, sheep, goats, pigs, chickens and ducks in 2010. Scientific Data, 5, 180227. https://doi.org/10.1038/sdata.2018.227

Kummu, M., Ward, P. J., Moel, H. de, & Varis, O. (2010). Is physical water scarcity a new phenomenon? Global assessment of water shortage over the last two millennia. Environmental Research Letters, 5(3), 034006. https://doi.org/10.1088/1748-9326/5/3/034006

Robinson, T. P., & Food and Agriculture Organization of the United Nations (Eds.). (2011). Global livestock production systems. Food and Agriculture Organization of the United Nations.

Running, S. W., & Zhao, M. (2019). MOD17A3HGF MODIS/Terra Net Primary Production Gap-Filled Yearly L4 Global 500 m SIN Grid V006. 2019, distributed by NASA EOSDIS Land Processes DAAC. 35. https://doi.org/10.5067/MODIS/MOD17A3HGF.006

Sexton, J. O., Song, X.-P., Feng, M., Noojipady, P., Anand, A., Huang, C., Kim, D.-H., Collins, K. M., Channan, S., DiMiceli, C., & Townshend, J. R. (2013). Global, 30-m resolution continuous fields of tree cover: Landsat-based rescaling of MODIS vegetation continuous fields with lidar-based estimates of error. International Journal of Digital Earth, 6(5), 427–448. https://doi.org/10.1080/17538947.2013.786146
Sulla-Menashe, D., & Friedl, M. A. (2018). User guide to collection 6 MODIS land cover (MCD12Q1 and MCD12C1) product. USGS: Reston, VA, USA, 1–18. https://doi.org/10.5067/MODIS/MCD12Q1.006

