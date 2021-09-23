# Morris_etal_2021_EcolApps
Data accompanying the manuscript 'Does the legacy of historical thinning treatments foster resilience to bark beetle outbreaks in subalpine forests?' by Morris, Buonanduci, Agne, Battaglia, and Harvey published in Ecological Applications.

There are three main data files made available for reproducibility purposes:
- plot_metadata.csv
- tree_scale.csv
- stand_scale.csv


#### plot_metadata.csv

This file contains metadata associated with each plot. The following columns are included:
- *PlotID*: unique plot identifier in the format LocationPlot#_Treatment_TSI where *Location* is the sampling site (FR = Fraser), *Plot#* is the block replicate (A-D) and plot number (1-5), *Treatment* is the thinning treatment receieved in 1940 (C = control, L = light, M = moderate, H = heavy, X = clearcut), and *TSI* is the presence of additional timber stand improvement (TSI) thinning (N = absent, Y = present).
- *Plot*: 
- *Block*: replicate
- *Treatment*: thinning treatment received in 1940, classified by intensity: Control (no thinning), Light, Moderate, Heavy, and Clearcut thinning.
- *TSI*: presence (Y) or absence (N) of additional timber stand improvement (TSI) thinning.
- *Date*: date of field data collection, in YYYYMMDD. Range _.
- *Aspect_deg*: aspect of plot taken from plot center, in degrees. Range _.
- *Slope_deg*: slope of plot taken from plot center, in degrees. Range _. 
- *Elevation_m*: elevation at plot center, in meters. Range _.


#### tree_scale.csv
This file contains individual tree-level data necessary to run the tree-scale analyses. The following columns are included:
- *PlotID*: unique plot identifier.
- *Species*: four letter code indicating the species of each measured tree. ABLA = *Abies lasiocarpa*, subalpine fir; PIEN = *Picea engelmannii*, Engelmann spruce; PICO = *Pinus contorta*, lodgepole pine; POTR = *Populus tremuloides*, quaking aspen.
- *Status*: binary variable indicating live (L) or dead (D) status of each measured tree.
- *DecayClass*: 
- *DBH_cm*: tree diameter at breast height (DBH), in centimeters. Recorded for trees reaching at least 1.4 m in height. Range 0.1-49.0 cm. NA's indicate trees below 1.4 m in height.
- *BA_m2*: basal area (BA) for each tree at least 1.4 m tall, in square meters. Range 7.85e^-7-0.188575 m^2. NA's indicate trees below 1.4 m in height. 
- *Height_m*: tree height, in meters. Range 0.1-30.0 m. NA's indicate measured trees that were not standing. 
- *MPB*: binary variable indicating presence (Y) or absence (NA) of signs of mountain pine beetle (MPB; *Dendroctonus ponderosae*) attack. Signs included observed beetle galleries and/or pitch tubes.

#### stand_scale.csv
This file contains aggregated plot-level data necessary to run the stand-scale analyses. The following columns are included:
- *PlotID*:
