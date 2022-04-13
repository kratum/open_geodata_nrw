# get data from linfos - alleenkataster
`wget https://www.opengeodata.nrw.de/produkte/umwelt_klima/naturschutz/linfos/Alleenkataster_EPSG25832_Shape.zip`

# unzip
`unzip Alleenkataster_EPSG25832_Shape.zip`

# upload to datapase
`shp2pgsql vw_alpolylineproved.shp alleen | psql -U ccnrw -d ccnrw`
