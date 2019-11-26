## QGIS mit PostGIS verbinden

Benötigte Informationen über die Datenbank:
- DB-Name
- Host
- Port
- Username
- Passwort


In QGIS im [Bedienfeld Browser](https://docs.qgis.org/3.4/de/docs/user_manual/managing_data_source/opening_data.html#the-browser-panel) `Rechtsklick` auf PostGIS und Neue Verbindung erstellen

<img src="https://github.com/kratum/open_geodata_nrw/raw/master/images/04_01.PNG" alt="drawing" width="200"/>


Die entsprechenden Datenbankinformationen eingeben und OK. Anschliessend wird nach den User Informationen gefragt

Feld | Bemerkung
--- | ---
Name | Frei gewählter Name für die Verbindung
Dienst | localhost für lokale Datenbankem, sonst IP des DB-Servers
Port | Port der DB
Datenbank | Name der Datenbank


<img src="https://github.com/kratum/open_geodata_nrw/raw/master/images/04_02.PNG" alt="drawing" width="200"/>

## Zugriffmöglichkeiten auf PostGIS aus QGIS



(Sollten Bedienfelder oder Werkzeuge in der Oberfläche nicht sichtbar sein, lassen diese sich über einen `Rechtsklick` ins Menü aktivieren.)

Zwischen dem [Bedienfeld Layer](https://docs.qgis.org/3.4/de/docs/user_manual/introduction/general_tools.html#label-legend) und dem [Bedienfeld Browser](https://docs.qgis.org/3.4/de/docs/user_manual/managing_data_source/opening_data.html#the-browser-panel) können Layer per Drag-and-Drop hin und her geschoben werden. Werden Layer aus der Datenbank in QGIS geladen, also aus dem Bedienfeld Browser ins Bedienfeld Layer gezogen, so wird direkt auf die Datenbank zugegriffen. Das heißt Änderungen am Layer betreffen die Daten in der Datenbank. Wird ein Layer aus QGIS in die Datenbank geladen, wird der Layer in der Datenbank gespeichert.

Über das Datenbankmenü im Hauptmenü lässt sich die [DB-Verwaltung](https://docs.qgis.org/3.4/de/docs/user_manual/plugins/core_plugins/plugins_db_manager.html#dbmanager) öffnen. Hier können Informationen über die Datenbank und einzelne Layer eingesehen werden. Darüberhinaus lassen sich die Daten eines Layers per SQL abfragen.

Über das [Bedienfeld Verarbeitungswerkzeuge](https://docs.qgis.org/3.4/de/docs/user_manual/processing/intro.html) lassen sich ebenfalls Tools finden um mit der Datenbank zu kommunizieren.


<img src="https://github.com/kratum/open_geodata_nrw/raw/master/images/04_03.PNG" alt="drawing" width="200"/>

