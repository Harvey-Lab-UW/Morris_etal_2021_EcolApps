# Morris_etal_2021_EcolApps
Data accompanying the manuscript 'Does the legacy of historical thinning treatments foster resilience to bark beetle outbreaks in subalpine forests?' by Morris, Buonanduci, Agne, Battaglia, and Harvey published in Ecological Applications.

There are three main data files made available for reproducibility purposes:
- plot_metadata.csv
- tree_scale.csv
- stand_scale.csv


### plot_metadata.csv
This file contains metadata associated with each plot. The following columns are included:
- *PlotID*: unique plot identifier in the format LocationPlot#_Treatment_TSI. 
-- *Location* is the sampling site (FR = Fraser)
-- *Plot#* is the block replicate (A-D) and plot number (1-5)
-- *Treatment* is the thinning treatment receieved in 1940 (C = control, L = light, M = moderate, H = heavy, X = clearcut)
-- *TSI* is the presence of additional timber stand improvement (TSI) thinning (N = absent, Y = present).
- *Plot*: 
- *Block*: replicate
- *Treatment*: thinning treatment received in 1940, classified by intensity: Control (no thinning), Light, Moderate, Heavy, and Clearcut thinning.
- *TSI*: presence (Y) or absence (N) of additional timber stand improvement (TSI) thinning.
- *Date*: date of field data collection, in YYYYMMDD. Range 20180705-20180822.
- *Aspect_deg*: aspect of plot taken from plot center, in degrees. Range 14-357 deg.
- *Slope_deg*: slope of plot taken from plot center, in degrees. Range 5.6-25.9 deg. 
- *Elevation_m*: elevation at plot center, in meters. Range 2,799-2,999 m.


### tree_scale.csv
This file contains individual tree-level data necessary to run the tree-scale analyses. The following columns are included:
- *PlotID*: unique plot identifier.
- *Species*: four letter code indicating the species of each measured tree. ABLA = *Abies lasiocarpa*, subalpine fir; PIEN = *Picea engelmannii*, Engelmann spruce; PICO = *Pinus contorta*, lodgepole pine; POTR = *Populus tremuloides*, quaking aspen.
- *Status*: binary variable indicating live (L) or dead (D) status of each measured tree.
- *DecayClass*: decay measure for dead trees ranging from 1 (least decayed) to 5 (most decayed). NA's indicate live trees.
- *DBH_cm*: tree diameter at breast height (DBH), in centimeters. Recorded for trees reaching at least 1.4 m in height. Range 0.1-49.0 cm. NA's indicate trees below 1.4 m in height.
- *BA_m2*: basal area (BA) for each tree at least 1.4 m tall, in square meters. Range 7.85e^-7-0.188575 m^2. NA's indicate trees below 1.4 m in height. 
- *Height_m*: tree height, in meters. Range 0.1-30.0 m. NA's indicate measured trees that were not standing. 
- *MPB*: binary variable indicating presence (Y) or absence (NA) of signs of mountain pine beetle (MPB; *Dendroctonus ponderosae*) attack. Signs included observed beetle galleries and/or pitch tubes.

### stand_scale.csv
This file contains aggregated plot-level data necessary to run the stand-scale analyses. The following columns are included:
- *PlotID*: unique plot identifier.
- *Susc_TotalBA_m2_ha*
- *Susc_LiveBA_m2_ha*
- *Susc_TotalStems_ha*
- *Susc_LiveStems_ha* 
- *Total_QMD_cm* 
- *PICO_QMD_cm* 
- *ABLA_QMD_cm* 
- *PIEN_QMD_cm* 
- *POTR_QMD_cm* 
- *Total_BA_m2_ha* 
- *PICO_BA_m2_ha*
- *ABLA_BA_m2_ha* 
- *PIEN_BA_m2_ha*
- *POTR_BA_m2_ha*  
- *Total_OvrBA_m2_ha*
- *PICO_OvrBA_m2_ha* 
- *ABLA_OvrBA_m2_ha* 
- *PIEN_OvrBA_m2_ha* 
- *POTR_OvrBA_m2_ha* 
- *Total_MidBA_m2_ha*
- *PICO_MidBA_m2_ha* 
- *ABLA_MidBA_m2_ha* 
- *PIEN_MidBA_m2_ha* 
- *POTR_MidBA_m2_ha* 
- *Total_SapBA_m2_ha*
- *PICO_SapBA_m2_ha*  
- *ABLA_SapBA_m2_ha*  
- *PIEN_SapBA_m2_ha*  
- *POTR_SapBA_m2_ha*  
- *Total_Stems_ha*  
- *PICO_Stems_ha*
- *ABLA_Stems_ha*
- *PIEN_Stems_ha*
- *POTR_Stems_ha*
- *Total_OvrStems_ha*
- *PICO_OvrStems_ha* 
- *ABLA_OvrStems_ha* 
- *PIEN_OvrStems_ha* 
- *POTR_OvrStems_ha* 
- *Total_MidStems_ha*
- *PICO_MidStems_ha* 
- *ABLA_MidStems_ha* 
- *PIEN_MidStems_ha* 
- *POTR_MidStems_ha* 
- *Total_SapStems_ha*
- *PICO_SapStems_ha* 
- *ABLA_SapStems_ha* 
- *PIEN_SapStems_ha* 
- *POTR_SapStems_ha* 
- *Total_SdlStems_ha*
- *PICO_SdlStems_ha* 
- *ABLA_SdlStems_ha* 
- *PIEN_SdlStems_ha* 
- *POTR_SdlStems_ha* 

