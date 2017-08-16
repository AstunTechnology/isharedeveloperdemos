---
layout: default
---

# QGIS in the cloud

[qgis.astuntechnology.com](http://qgis.astuntechnology.com){:target="_demo"} (demo02/demo02)

## Metadata

Use metasearch plugin to discover data from [http://geonetwork.astuntechnology.com/geonetwork/astun](http://geonetwork.astuntechnology.com/geonetwork/astun){:target="_demo"}, also available at [http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx](http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx){:target="_demo"}


## Routing

Routing using Ordnance Survey Open Roads dataset, loaded into PostGIS 2.0, with PgRouting 2.2, using QGIS in the Cloud, connected to the iShare Spatial Data Warehouse.

__Example Functions:__

* Driving Distance (Alphashape): returns polygons of all locations a given distance away from a given point
* Shortest Path with turn restrictions (trsp(edge)): shortest path between two given points, taking notice of turn restrictions
