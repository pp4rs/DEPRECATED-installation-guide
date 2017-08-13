# Geographical data with R

R has many tools to deal with Geo-spatial data.
We will introduce the essentials to get you up and started.

## Mac Users

Follow the following steps:

1.  Download GDAL complete
2.  Doubleclick and install the .dmg file as you are used to on a Mac
3.  Proceed to `Installing Additonal R Packages`

!!! tip "Hat-tip"
    We borrowed heavily from Nick Eubank's installation guide for 'Spatial Data in R' to assist in the Mac installation.
    Nick's install guide is available [here](http://www.nickeubank.com/wp-content/uploads/2015/10/RGIS1_SpatialDataTypes_part0_setup.html)

## Linux Users

Follow these steps:

1.  In your terminal type the following, then hit `Return`

        sudo add-apt-repository ppa:ubuntugis/ppa && sudo apt-get update

2.  Hit enter when prompted, then enter the following before again hitting the `Return` key:

        sudo apt-get install gdal-bin

3.  To verify after installation, try:
        ogrinfo
If the installation was successful, you will see something like this:

        Usage: ogrinfo [--help-general] [-ro] [-q] [-where restricted_where]
                       [-spat xmin ymin xmax ymax] [-fid fid]
                       [-sql statement] [-al] [-so] [-fields={YES/NO}]
                       [-geom={YES/NO/SUMMARY}][--formats]
                       datasource_name [layer [layer ...]]

4.  Proceed to `Installing Additonal R Packages`

!!! tip "Hat-tip"
    We borrowed heavily from Sara Safavi to learn how to install `GDAL` on Ubuntu.
    She provides an install guide [here](http://www.sarasafavi.com/installing-gdalogr-on-ubuntu.html)

## Windows Users

!!! success
    For once, Windows is ahead of the game. We only need to install R packages!


## Installing Additional R Packages

We will need some additional libraries to conduct our GIS analysis. Proceed as follows:

*   Open RStudio
*   In the **console**, copy and paste the following:

```r
uzh_gistools <- c("rgeos", "ggmap", "sf",
                    "sp","raster"  "tmaptools",
                    "rgdal", "gdalUtils", "mapview", "tmap")

install.packages(uzh_gistools)
```
