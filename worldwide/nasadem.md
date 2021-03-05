# NASADEM

## Official download links

Direct link to all files: https://e4ftl01.cr.usgs.gov/MEASURES/NASADEM_HGT.001/2000.02.11/

Link via: https://lpdaac.usgs.gov/products/nasadem_hgtv001/#tools


## Download links

This linux bash command create the file [nasadem-files.txt](./nasadem-files.txt). It's a list with 14520 ZIP files, about 100 GB. 

`
curl -s "https://e4ftl01.cr.usgs.gov/MEASURES/NASADEM_HGT.001/2000.02.11/" | cut -d'>' -f3 | grep .zip\< | cut -d'<' -f1 | xargs -I {} echo "https://e4ftl01.cr.usgs.gov/MEASURES/NASADEM_HGT.001/2000.02.11/{}" >>nasadem-files.txt
`

## Automatic/scripted download

Downloads are limited for anonymous users. You need to create a NASA earth data user account on:

https://urs.earthdata.nasa.gov/users/new/



Then you can do a parallel download e.g. with the tool `parallel`:

`
parallel -j 10 wget -nv --user=USERNAME --password=PASSWORD < nasadem-files.txt
`

