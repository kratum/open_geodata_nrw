# Load data from http://linfos.api.naturschutzinformationen.nrw.de/atlinfos/de/start 

### get data from linfos - alleenkataster
`wget https://www.opengeodata.nrw.de/produkte/umwelt_klima/naturschutz/linfos/Alleenkataster_EPSG25832_Shape.zip`

### unzip and upload to database
`unzip Alleenkataster_EPSG25832_Shape.zip`
`shp2pgsql vw_alpolylineproved.shp alleen | psql -U ccnrw -d ccnrw`

