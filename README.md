# Design ocean sampling strategies

Codes to design ocean sampling strategies with different instruments.

## 1) Sampling strategy using a Moving Vessel Profiler (MVP) along transects in a rotated radiator grid.

[`Sampling_strategy_MVP_rotated_radiator_grid_FaST-SWOT_across_swaths.ipynb`](https://github.com/bbarcelollull/design_ocean_sampling_strategies/blob/main/Sampling_strategy_MVP_rotated_radiator_grid_FaST-SWOT_across_swaths.ipynb)

This code provides the (lon, lat, time) coordinates of the extremes of each transect (information needed for navigation), as well as the (lon, lat, depth, time) coordinates of each MVP profile (information needed to do OSSEs) on a rotated sampling grid. It needs as inputs: 
* Northwestern position (position where the sampling starts)
* Sampling strategy parameters: length of transects, separation between transects, number of transects and angle of the rotated grid
* MVP parameters: time resolution (cycle time) and maximum depth
* Ship velocity in knots
* Minimum profile depth and vertical resolution
* Initial date and time of the sampling

Note that this strategy consists of a vessel moving from west to east sampling one transect, then moving down to the next transect, which will be sampled from east to west, and so on (see figure). 

The instrument used in this experiment is the [MVP30-350 from AML Oceanographic](https://drive.google.com/file/d/1VsDxaqGG8NF7p5lkK-a7Cr0INjDSjywx/view).

Example of the information provided by this code:

![MVP_sampling_strategy_extreme_coordinates_small_region_cropped](https://user-images.githubusercontent.com/46760038/232018124-698ba46b-26cb-4841-ba5a-e8e689da8fb7.png)

### Additional files

Files needed to replicate the same figures are located in the folders [`bathymetry`](https://github.com/bbarcelollull/design_ocean_sampling_strategies/tree/main/bathymetry) and [`swath_swot`](https://github.com/bbarcelollull/design_ocean_sampling_strategies/tree/main/swath_swot).

### Acknowledgments

*Codes written by Bàrbara Barceló-Llull (IMEDEA, Spain) and Elisabet Verger Miralles (UIB-IMEDEA, Spain) in the framework of the FaSt-SWOT project to plan the FaSt-SWOT experiments. These codes are based on the codes developed during the H2020 EuroSea project ([Barceló-Llull, 2023](https://doi.org/10.5281/zenodo.7543697)).*

*The FaSt-SWOT project is funded by the Spanish Research Agency and the European Regional Development Fund (AEI/FEDER, UE) under Grant Agreement (PID2021-122417NB-I00)).*

*The EuroSea project is funded by the European Union’s Horizon 2020 research and innovation programme under grant agreement No 862626.*
