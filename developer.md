---
layout: default
---

# iShareMaps and GIS Integration Scenarios

## Linking to iShareMaps or GIS from a URL

Use case: call centres, sending emails to people

* Example: opening iShareMaps at a specific address

[http://maps.astuntechnology.com/iShareLIVE.Web/atmyresponsivecouncil.aspx?tab=maps&action=SetAddress&UniqueId=101729](http://maps.astuntechnology.com/iShareLIVE.Web/atmyresponsivecouncil.aspx?tab=maps&action=SetAddress&UniqueId=101729){:target="_demo"}

* Opening iShareGIS in a particular profile, with particular layers activated, zoomed to a particular location

[http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx?ms=mapsources/Education&layers=Wards_OGC,Primary_Schools_OGC&starteasting=499472.5&startnorthing=170925&startzoom=1670](http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx?ms=mapsources/Education&layers=Wards_OGC,Primary_Schools_OGC&starteasting=499472.5&startnorthing=170925&startzoom=1670){:target="_demo"}

## Getting iShare information in text format

Uses- for displaying data on a different web page, or for consuming as a web service by an external system

* Example: getting a list of hospitals in json format

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices&#124;Hospitals](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices&#124;Hospitals){:target="_demo"}

* or a list near a specific UPRN:

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices&#124;Hospitals&uid=101726](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices&#124;Hospitals&uid=101726){:target="_demo"}

## Address searches

Uses: any sort of remote address search, such as linking from elsewhere in the website or from a remote application

* Example: Getting a list of addresses from a partial postcode (or address)

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?service=Location&RequestType=LocationSearch&location=GU18&pagesize=10&startnum=1](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?service=Location&RequestType=LocationSearch&location=GU18&pagesize=10&startnum=1){:target="_demo"}

## Querying tables in the database

Uses: querying any table in the database by sending one or more filter parameters

* Example: Searching for a council tax band for a property

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=json&Type=data&ds=council_tax&select=uniqueid,tax_band&filter=^uniqueid^='101739'](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=json&Type=data&ds=council_tax&select=uniqueid,tax_band&filter=^uniqueid^='101739'){:target="_demo"}

* Example: Searching for crimes committed in a particular month

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=json&Type=data&ds=crime.street_accumulated&select=location,month,total_crime&filter=^month^=2012-09'](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=json&Type=data&ds=crime.street_accumulated&select=location,month,total_crime&filter=^month^='2012-09'){:target="_demo"}

## Running queries on data in the database

Uses: integration with external applications such as planning portals

* Example: Finding the nearest addresses to a given coordinate

[https://gis.astuntechnology.com/isharegislive.web/GetData.aspx?callback=results&RequestType=xsl&Type=jsonp&service=DataFunc&xsl=xml/atJSONDatatable.xsl&ds=NearestAddress&params=499472~170925~5000~10](https://gis.astuntechnology.com/isharegislive.web/GetData.aspx?callback=results&RequestType=xsl&Type=jsonp&service=DataFunc&xsl=xml/atJSONDatatable.xsl&ds=NearestAddress&params=499472~170925~5000~10){:target="_demo"}

## Producing a pdf for a location from MyHouse

Uses: 

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=pdf&tab=0&enablejs=True&uid=101726&cookieVersion=1](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?requesttype=pdf&tab=0&enablejs=True&uid=101726&cookieVersion=5.6.4.4222){:target="_demo"}






