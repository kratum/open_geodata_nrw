VRS DATA

`wget http://download.vrsinfo.de/gtfs/google_transit.zip`

`unzip google_transit.zip -d gtfs_vrs`

[NRW Data](https://www.opendata-oepnv.de/ht/de/organisation/bundeslaender/nrw/startseite?tx_vrrkit_view%5Bdataset_name%5D=soll-fahrplandaten-nrw&tx_vrrkit_view%5Baction%5D=details&tx_vrrkit_view%5Bcontroller%5D=View)

`wget https://www.opendata-oepnv.de/dataset/3c97be05-1f89-4fc8-89f0-a9228ae0395e/resource/8fdf1313-aa12-4318-9e55-121e50f56a2a/download/20220308_gtfs_nrw.zip`

`unzip 20220308_gtfs_nrw.zip -d solldaten_nrw`

Check the notebook [read_gtfs.ipynb](https://github.com/kratum/open_geodata_nrw/blob/master/06_get_gtfs_nrw.ipynb)

Calculated stop_times per stop 
[Stops_stop_times_count](https://github.com/kratum/open_geodata_nrw/blob/master/stops_stop_times_count.geojson)

Example - renderd with aerialod
![nrw_stop_count](https://user-images.githubusercontent.com/11678642/162461246-df2a7122-2bf2-41ef-9be1-5b9dba41014d.PNG)
