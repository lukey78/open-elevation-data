# ALOS Global Digital Surface Model - by JAXA

According to https://www.aw3d.jp/en/products/standard/

"AW3D Standard is the world’s best global DEM. More than 3 million satellite images are used to create the most comprehensive high-resolution digital 3D imagery available today.
AW3D Standard is based on PRISM data acquired by the Advanced Land Observing Satellite (ALOS) from the Japan Aerospace Exploration Agency (JAXA)."

The model is available with 2m-5m resolution, but the "free-of-charge" version is only 30m - which is still good for a globally available model.


## Official download site

You need a user account to download the tiles.

### Registration

https://www.eorc.jaxa.jp/ALOS/en/aw3d30/registration.htm

Register there. Once completed, you receive a mail with username and password.

With these credentials, you can login here to download individual tiles:

https://www.eorc.jaxa.jp/ALOS/en/aw3d30/data/index.htm


## Scripted download

An individual tile has the following link:

https://www.eorc.jaxa.jp/ALOS/aw3d30/data/release_v2012/N045E090/N049E090.zip

A 5x5 degrees tiles ZIP has the following link:

https://www.eorc.jaxa.jp/ALOS/aw3d30/data/release_v2012/N080W030_N085W025.zip


They use a quite crude way for publishing the download links (an XML is loaded by a JS file that has js download links inside...).

[jaxa-aw3d30-5x5-tiles.txt](./jaxa-aw3d30-5x5-tiles.txt) is a download list with all 5x5 tile ZIPs available.

You can do an automatic download of them with:

`
parallel -j 10 wget -nv --user=USERNAME --password=PASSWORD < jaxa-aw3d30-5x5-tiles.txt
`


## File format info

Current version 3.1 (2020):

https://www.eorc.jaxa.jp/ALOS/en/aw3d30/aw3d30v31_product_e_a.pdf

File naming:

[Product ID]_[Tile ID]_[Kind of file].[Extention]

The DSM file seems to be the GeoTiff file.

Example：

- ALPSMLC30_N035E138_DSM.tif (DSM file)
- ALPSMLC30_N035E138_MSK.tif (Mask file)
- ALPSMLC30_N035E138_STK.tif (Stacking number file)
- ALPSMLC30_N035E138_HDR.txt (Header information file)
- ALPSMLC30_N035E138_QAI.txt (Quality assurance information file)
- ALPSMLC30_N035E138_LST.txt (List file)
