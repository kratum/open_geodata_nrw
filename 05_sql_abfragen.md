# SQL Abfragen

Da PostGIS PostgreSQL erweitert und PostgreSQL mit SQL abgefragt wird müssen PostGIS Funktionen in SQL Statements eingebaut werden.

### Hilfe


https://www.w3schools.com/sql/sql_intro.asp

https://docs.qgis.org/3.4/de/docs/training_manual/spatial_databases/spatial_queries.html?highlight=postgis

https://docs.qgis.org/3.4/de/docs/training_manual/spatial_databases/index.html

http://www.postgresqltutorial.com/



### Anzahl der Adressen nach Stadtteilen

```
SELECT count(*) as count, text
FROM stadtteile as a, gebref_lev_25832 as b
WHERE ST_WITHIN(b.the_geom, a.geom)
Group By a.text
Order BY count DESC
```

### 
