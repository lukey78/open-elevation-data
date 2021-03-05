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


### Global resources

| Name (w/link)     | Provider, date   | Resolution (meters)  | Coverage  | Quality   | Fromat & Size   | Download tips/links   | Notes        |
| ------------------|------------------|----------------------|-----------|-----------|--------|-----------------------|--------------|
| [NASADEM](https://earthdata.nasa.gov/esds/competitive-programs/measures/nasadem) | NASA, (data: 2000, reprocessing: 2020)   | 30-50  | 60° N - 56° S (~80% of landmass) | medium  | GeoTiff, ~100 GB  | [Download NASADEM](worldwide/nasadem.md)  | NASADEM is reprocessed SRTM data, with some gaps filled and optimizations applied. Still not great, but one of the best resources with worldwide coverage.   |

### Large regions (e.g. continents)

| Name (w/link)     | Provider, date   | Resolution (meters)  | Coverage  | Quality   | Fromat & Size   | Download tips/links   | Notes        |
| ------------------|------------------|----------------------|-----------|-----------|--------|-----------------------|--------------|
| [Europe by Sonny](https://data.opendataportal.at/dataset/dtm-europe) | different sources, compiled by Sonny   | 20-30  | not fully covered  | medium  | HGT, ? GB  | [Download on Google Drive / 1" tiles](https://drive.google.com/drive/folders/0BxphPoRgwhnoWkRoTFhMbTM3RDA)  | A great resource with processed 1" tiles that can be used to overwrite SRTM or NASADEM data with a better quality version   |


### Country specific resources

| Name (w/link)     | Provider, date   | Resolution (meters)  | Coverage  | Quality   | Size   | Download tips/links   | Notes        |
| ------------------|------------------|----------------------|-----------|-----------|--------|-----------------------|--------------|
| [Austria](https://data.opendataportal.at/dataset/dtm-austria) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.5 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/196F_YOWQiUGv_mvJV2vtiFsCDExvdR8u)  | already combined, 1 huge tiff file    |
| [Belgium](https://data.opendataportal.at/dataset/dtm-belgium) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.1 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1_raU4UamyM11DOJswFY6L08EgS82CKsA)  | already combined, 1 huge tiff file    |
| [Denmark](https://data.opendataportal.at/dataset/dtm-denmark) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.1 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1hP5ZeGqHYuek8FtAlL681aOxGnJ_SL_c)  | already combined, 1 huge tiff file    |
| [Estonia](https://data.opendataportal.at/dataset/dtm-estonia) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.3 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1u0e4gQi2NjP0zConEE30mA0C9RCsqL2q)  | already combined, 1 huge tiff file    |
| [Finland](https://data.opendataportal.at/dataset/dtm-finland) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | HGT, ? GB   | [Download on Google Drive / 1" HGT-ZIP](https://drive.google.com/drive/folders/1u0e4gQi2NjP0zConEE30mA0C9RCsqL2q)  |     |
| [France](https://data.opendataportal.at/dataset/dtm-france) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 2 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1IybnvVH3-iaxB-0vIMDD0_twbM97Unsx)  | already combined, 1 huge tiff file    |
| [Germany](https://data.opendataportal.at/dataset/dtm-germany) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | Bayern, Berlin, Brandenburg, Hamburg, NRW, Rheinland Pfalz, Sachen, Thüringen    | good  | GeoTiff, ? GB   | [separate regions, download here](https://data.opendataportal.at/dataset/dtm-germany)  | data separate for each region, many regions missing   |
| [Iceland](https://data.opendataportal.at/dataset/dtm-iceland) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.5 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/11i81eelPS9S3yrylMO1ToXEMxAIOjlSu)  | already combined, 1 huge tiff file    |
| [Italy](https://data.opendataportal.at/dataset/dtm-italy) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 2 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1wVeRFeL-r5Z-Y32xunL6VzSFm7lHfdC8)  | already combined, 1 huge tiff file    |
| [Latvia](https://data.opendataportal.at/dataset/dtm-latvia) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.2 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1F_vtaSuCZqG2qvUE3X8O_hEsomC4yLoX)  | already combined, 1 huge tiff file    |
| [Luxembourg](https://data.opendataportal.at/dataset/dtm-luxembourg) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.01 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1-8HH5Kkj8vj-yQW9lMwPjXevwTtlor5x)  | already combined, 1 huge tiff file    |
| [Netherlands](https://data.opendataportal.at/dataset/dtm-netherlands) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.3 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1SpdptwzuuyS2Lfkc3TwXK2Ez3nWIHXfm)  | already combined, 1 huge tiff file    |
| [Norway](https://data.opendataportal.at/dataset/dtm-norway) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 2 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1CrW3b80Ll3Ig3I96oZiLRmE4KRPa-mYa)  | already combined, 1 huge tiff file    |
| [Slovenia](https://data.opendataportal.at/dataset/dtm-slovenia) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 0.1 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1C-jW7NLUNXRb3G-eJV1sM0Le0HFXdIcJ)  | already combined, 1 huge tiff file    |
| [Spain](https://data.opendataportal.at/dataset/dtm-spain) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%, mainland   | good  | GeoTiff, 2 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/17P85Orz6tTET01pN_GPtsBuheUYljHab)  | already combined, 1 huge tiff file    |
| [Spain](https://data.opendataportal.at/dataset/dtm-spain) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%, canary islands   | good  | GeoTiff, 0.05 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1Q06QSN2I6xpbnHx7TJyDG243Xfc4fKDu)  | already combined, 1 huge tiff file    |
| [Sweden](https://data.opendataportal.at/dataset/dtm-sweden) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | HGT, ? GB   | [Download on Google Drive / 1" tiles](https://drive.google.com/drive/folders/1CkcFqcXUic1e7tbVaDL7iMDMpsy9G2bM)  | data separate for each region, many regions missing   |
| [Switzerland](https://www.swisstopo.admin.ch/de/geodata/height/alti3d.html)  | [Swisstopo](https://www.swisstopo.ch), 2021  | 0.3-0.5    | 100%   | great    | GeoTiff, ~700 GB  | [Download Switzerland](countries/switzerland/switzerland.md) |  one of the most precise DEMs available    |  
| [United Kingdom](https://data.opendataportal.at/dataset/dtm-united_kingdom) | [OpenDataPortal, by Sonny](https://data.opendataportal.at/dataset/dtm-europe), 2018   | 20-30   | 100%   | good  | GeoTiff, 1 GB   | [Download on Google Drive / 20m TIFF](https://drive.google.com/drive/folders/1LJgFMEajBACo2QVVg7DsWLspr2ar4Y-Q)  | already combined, 1 huge tiff file    |


## Other great collections

Some of the links above originate from one of these collections.

- [Digital LiDAR terrain models of Europe](https://data.opendataportal.at/dataset/dtm-europe) - a great resource, please donate to the mainetainer Sonny!

