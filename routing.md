---
layout: default
---

# Routing

Routing using Ordnance Survey Open Roads dataset, loaded into PostGIS 2.0, with PgRouting 2.2, using QGIS in the Cloud, connected to the iShare Spatial Data Warehouse.

[qgis.astuntechnology.com](http://qgis.astuntechnology.com) (demo02/demo02)

Example Functions:

* Driving Distance/Alphashape: aka polygons of all locations a given distance away from a given point
* Shortest Path with turn restrictions (trsp(edge)): shortest path between two given points, taking notice of turn restrictions


SELECT seq, id1 AS id, cost
FROM pgr_drivingdistance(
'SELECT ogc_fid AS id, source, target, cost_len AS cost, rcost_len AS reverse_cost 
FROM routing.surrey_openroads', 
132231, -- my node from which I am calculating distances
2000, -- the distance
false, -- not a directed graph
true -- use reverse costs
);
