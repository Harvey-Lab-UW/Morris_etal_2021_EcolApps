# Morris_etal_2021_EcolApps
Data accompanying the manuscript 'Does the legacy of historical thinning treatments foster resilience to bark beetle outbreaks in subalpine forests?' by Morris, Buonanduci, Agne, Battaglia, and Harvey published in Ecological Applications. See the main text of the manuscript for complete descriptions of how data were collected, and greater specifics on values and classifications.  

[![DOI](https://zenodo.org/badge/390809096.svg)](https://zenodo.org/badge/latestdoi/390809096)

There are three main data files made available for reproducibility purposes:
- plot_metadata.csv
- tree_scale.csv
- stand_scale.csv


### plot_metadata.csv
This file contains metadata associated with each plot. The following columns are included:
- **PlotID**: unique plot identifier in the format Plot_Treatment_TSI. 
  - *Plot* is the site (Fraser, FR), block replicate (A-D), and plot number (1-5)
  - *Treatment* is the thinning treatment receieved in 1940 (C = control, L = light, M = moderate, H = heavy, X = clearcut)
  - *TSI* is the presence of additional timber stand improvement (TSI) thinning (N = absent, Y = present).
- **Plot**: code identifying each plot with site (Fraser, FR), block replicate (A-D), and plot number (1-5).
- **Block**: code identifying the treatment replicate containing each plot, A-D.
- **Treatment**: thinning treatment received in 1940, classified by intensity: Control (no thinning), Light, Moderate, Heavy, and Clearcut thinning.
- **TSI**: presence (Y) or absence (N) of additional timber stand improvement (TSI) thinning.
- **Date**: calendar date of field data collection, in YYYYMMDD. Range 20180705 to 20180822.
- **Aspect_deg**: aspect of plot taken from plot center using a compass, in degrees. Range 14-357 deg.
- **Slope_deg**: slope of plot taken from plot center using a TruPulse 200 laser rangefinder, in degrees. Range 5.6 to 25.9 deg. 
- **Elevation_m**: elevation at plot center using a Garmin GPS unit, in meters. Range 2,799 to 2,999 m.


### tree_scale.csv
This file contains individual tree-level data necessary to run the tree-scale analyses. The following columns are included:
- **PlotID**: unique plot identifier.
- **Species**: four letter code indicating the species of each measured tree. 
  - ABLA = *Abies lasiocarpa*, subalpine fir
  - PIEN = *Picea engelmannii*, Engelmann spruce
  - PICO = *Pinus contorta*, lodgepole pine
  - POTR = *Populus tremuloides*, quaking aspen.
- **Status**: binary variable indicating live (L) or dead (D) status of each measured tree.
- **DecayClass**: decay measure for dead trees ranging from 1 (least decayed) to 5 (most decayed). NA's indicate live trees and/or trees with DBH < 5 cm.
- **DBH_cm**: tree diameter at breast height (DBH), in centimeters. Recorded for trees ≥1.4 m in height. Range 0.1 to 49.0 cm. NA's indicate tree height < 1.4 m.
- **MPB**: binary variable indicating presence (Y) or absence (NA) of signs of mountain pine beetle (MPB; *Dendroctonus ponderosae*) attack. Signs included observed beetle galleries and/or pitch tubes.


### stand_scale.csv
This file contains aggregated plot-level data necessary to run the stand-scale analyses. The following columns are included:
- **PlotID**: unique plot identifier.
- **Susc_TotalBA_m2_ha**: total basal area (BA) of susceptible lodgepole pine trees (live and DBH ≥ 12 cm prior to outbreak), in square meters per hectare. 
- **Susc_LiveBA_m2_ha**: total basal area (BA) of susceptible lodgepole pine trees that survived the MPB outbreak, in m<sup>2</sup>/ha.
- **Susc_TotalStems_ha**: total density of susceptible lodgepole pine trees (live and DBH ≥ 12 cm prior to outbreak), in stems per hectare.
- **Susc_LiveStems_ha**: total density of susceptible lodgepole pine trees that survived the MPB outbreak, in stems/hectare.
- **Total_QMD_cm**: quadratic mean diameter (QMD) for all live trees ≥1.4 m in height, in centimeters.
  - **PICO_QMD_cm**: QMD for live lodgepole pine, in cm.
  - **ABLA_QMD_cm**: QMD for live subalpine fir, in cm.
  - **PIEN_QMD_cm**: QMD for live Engelmann spruce, in cm.
  - **POTR_QMD_cm**: QMD for live quaking aspen, in cm.
- **Total_BA_m2_ha**: total basal area (BA) for all live trees ≥1.4 m in height, in square meters per hectare.
  - **PICO_BA_m2_ha**: BA for live lodgepole pine trees, in m<sup>2</sup>/ha.
  - **ABLA_BA_m2_ha**: BA for live subalpine fir trees, in m<sup>2</sup>/ha.
  - **PIEN_BA_m2_ha**: BA for live Engelmann spruce trees, in m<sup>2</sup>/ha.
  - **POTR_BA_m2_ha**: BA for live quaking aspen trees, in m<sup>2</sup>/ha.
- **Total_OvrBA_m2_ha**: total basal area (BA) for all live overstory trees (DBH ≥ 12 cm), in square meters per hectare.
  - **PICO_OvrBA_m2_ha**: BA for live overstory lodgepole pine (PICO) trees, in m<sup>2</sup>/ha.
  - **ABLA_OvrBA_m2_ha**: BA for live overstory subalpine fir (ABLA) trees, in m<sup>2</sup>/ha.
  - **PIEN_OvrBA_m2_ha**: BA for live overstory Engelmann spruce trees, in m<sup>2</sup>/ha.
  - **POTR_OvrBA_m2_ha**: BA for live overstory quaking aspen trees, in m<sup>2</sup>/ha.
- **Total_MidBA_m2_ha**: total basal area (BA) for all live midstory trees (5 cm ≤ DBH < 12 cm), in square meters per hectare.
  - **PICO_MidBA_m2_ha**: BA for live midstory lodgepole pine trees, in m<sup>2</sup>/ha.
  - **ABLA_MidBA_m2_ha**: BA for live midstory subalpine fir trees, in m<sup>2</sup>/ha.
  - **PIEN_MidBA_m2_ha**: BA for live midstory Engelmann spruce trees, in m<sup>2</sup>/ha.
  - **POTR_MidBA_m2_ha**: BA for live midstory quaking aspen trees, in m<sup>2</sup>/ha.
- **Total_SapBA_m2_ha**: total basal area (BA) for all sapling trees (DBH < 5 cm), in square meters per hectare.
  - **PICO_SapBA_m2_ha**: BA for live sapling lodgepole pine trees, in m<sup>2</sup>/ha.
  - **ABLA_SapBA_m2_ha**: BA for live sapling subalpine fir trees, in m<sup>2</sup>/ha.
  - **PIEN_SapBA_m2_ha**: BA for live sapling Engelmann spruce trees, in m<sup>2</sup>/ha.
  - **POTR_SapBA_m2_ha**: BA for live sapling quaking aspen trees, in m<sup>2</sup>/ha.
- **Total_Stems_ha**: total density of all live trees ≥0.1 m in height, in stems per hectare.
  - **PICO_Stems_ha**: density of all live lodgepole pine trees, in stems/ha.
  - **ABLA_Stems_ha**: density of all live subalpine fir trees, in stems/ha.
  - **PIEN_Stems_ha**: density of all live Engelmann spruce trees, in stems/ha.
  - **POTR_Stems_ha**: density of all live quaking aspen trees, in stems/ha.
- **Total_OvrStems_ha**: total density of all live overstory (DBH ≥ 12 cm) trees, in stems per hectare.
  - **PICO_OvrStems_ha**: density of live overstory lodgepole pine (PICO) trees, in stems/ha.
  - **ABLA_OvrStems_ha**: density of live overstory subalpine fir (ABLA) trees, in stems/ha.
  - **PIEN_OvrStems_ha**: density of live overstory Engelmann spruce trees, in stems/ha.
  - **POTR_OvrStems_ha**: density of live overstory quaking aspen trees, in stems/ha.
- **Total_MidStems_ha**: total density of all live midstory trees (5 cm ≤ DBH < 12 cm), in stems per hectare.
  - **PICO_MidStems_ha**: density of live midstory lodgepole pine (PICO) trees, in stems/ha
  - **ABLA_MidStems_ha**: density of live midstory subalpine fir (ABLA) trees, in stems/ha.
  - **PIEN_MidStems_ha**: density of live midstory Engelmann spruce trees, in stems/ha.
  - **POTR_MidStems_ha**: density of live midstory quaking aspen trees, in stems/ha.
- **Total_SapStems_ha**: total density of all live sapling trees (DBH < 5 cm), in stems per hectare.
  - **PICO_SapStems_ha**: density of live sapling lodgepole pine (PICO) trees, in stems/ha
  - **ABLA_SapStems_ha**: density of live sapling subalpine fir (ABLA) trees, in stems/ha.
  - **PIEN_SapStems_ha**: density of live sapling Engelmann spruce trees, in stems/ha.
  - **POTR_SapStems_ha**: density of live sapling quaking aspen trees, in stems/ha.
- **Total_SdlStems_ha**: total density of all live seedling trees (0.1 m ≤ height < 1.4 m), in stems per hectare.
  - **PICO_SdlStems_ha**: density of live seedling lodgepole pine (PICO) trees, in stems/ha
  - **ABLA_SdlStems_ha**: density of live seedling subalpine fir (ABLA) trees, in stems/ha.
  - **PIEN_SdlStems_ha**: density of live seedling Engelmann spruce trees, in stems/ha.
  - **POTR_SdlStems_ha**: density of live seedling quaking aspen trees, in stems/ha.

