# Switzerland (CH)

In March 2021 Switzerland published all geographic data previously only available for paid customers to the general public, free of charge.

The digital elevation model "SwissAlti3d" covers the whole country with a resolution of ~0.5m.


## Download links

You can generate the download links on your own on:

https://www.swisstopo.admin.ch/de/geodata/height/alti3d.html

select "whole dataset" and the desired resolution - 0.5m or 2m. It created a CSV file with the download links.

[Download links, GeoTiff with 0.5m](./switzerland-files-0.5m.txt)


## Automatic/scripted download

Try a parallel download e.g. with the tool `parallel`:

`
parallel -j 10 wget -nv  < switzerland-files-0.5m.txt
`

