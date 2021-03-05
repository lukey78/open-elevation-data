# Open elevation data project

The goal of this project is to maintain the most up-to-date resource for freely available elevation data worldwide (DEM = Digital Elevation Model).

We don't want to collect ALL resources, but select the BEST resources for worldwide or region/country coverage.

Most countries in the world do not provide good elevation data (resolutions < 30m) free of charge, but for often horrendous cost. There're exceptions, e.g. Switzerland providing great quality DEMs with 0.5m resolution since 2021.

The first step in this project is to collect the best resources available, preferably with direct download links.

Processing DEM data is a topic for itself, because data size is usually huge, processing takes long and requires a lot of resources. Let's gather some tips to efficiently process the data, e.g. for filling gaps, creating contour lines, creating hillshade or slope maps.

The next step would be to generate freely available elevation maps and hillshade models for single countries or the whole world.


## CONTRIBUTE!

If you know good sources of elevation data, please provide the information ideally by creating a pull request or through an issue.

Feel free to add your country to the list!


## THE DATA

| Property    | Meaning   |
|-------------|-----------|
| Name (w/link)  | official name, linked to the resource with information   |
| Provider  | Who gathered or processed the data? And when?  |
| Resolution  | how many meters between each point in the elevation grid? Sometimes this is given in arcseconds. 1 arcsecond = ~30m.  |
| Coverage   | What region is covered by the whole dataset? Either in degrees (WGS84) or in (sub-)regions.  |
| Quality  | A quality indicator - or quality notices (no standard defined yet)   |
| Size    | The rough size of the whole dataset in Gigabytes (GB)   |
| Download tips/links  | Preferably a link to a markdown document in this repository describing in detail how to fetch the resources. Download scripts welcome!   |
| Notes   | place for a little info    |


### Global (worldwide) resources

| Name (w/link)     | Provider, date   | Resolution (meters)  | Coverage  | Quality   | Size   | Download tips/links   | Notes        |
| ------------------|------------------|----------------------|-----------|-----------|--------|-----------------------|--------------|
| [NASADEM](https://earthdata.nasa.gov/esds/competitive-programs/measures/nasadem) | NASA, ~2020   | 30-50  | 60° N - 56° S (~80% of landmass) | medium  | ~100 GB  | [Download NASADEM](worldwide/nasadem.dem)  | NASADEM is reprocessed SRTM data, with some gaps filled and optimizations applied. Still not great, but one of the best resources with worldwide coverage.   |


### Country specific resources

