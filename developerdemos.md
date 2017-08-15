#iShareMaps and GIS Integration Scenarios

## Linking to iShareMaps or GIS from a URL

Use case: call centres, sending emails to people

* Example- opening iShareMaps at a specific address

[http://maps.astuntechnology.com/iShareLIVE.Web/atmyresponsivecouncil.aspx?tab=maps&action=SetAddress&UniqueId=101729](http://maps.astuntechnology.com/iShareLIVE.Web/atmyresponsivecouncil.aspx?tab=maps&action=SetAddress&UniqueId=101729)

* Opening iShareGIS in a particular profile, with particular layers activated, zoomed to a particular location

[http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx?ms=mapsources/Education&layers=Wards_OGC,Primary_Schools_OGC&starteasting=499472.5&startnorthing=170925&startzoom=1670](http://gis.astuntechnology.com/isharegislive.web/isharegis.aspx?ms=mapsources/Education&layers=Wards_OGC,Primary_Schools_OGC&starteasting=499472.5&startnorthing=170925&startzoom=1670)

## Getting ishare information in text format

Uses- for displaying data on a different web page, or for consuming as a web service by an external system

* Example- getting a list of hospitals in json format

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices|Hospitals](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices|Hospitals)

* or a list near a specific UPRN:

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices|Hospitals&uid=101726](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices|Hospitals&uid=101726)

## Address Searches

Uses, any sort of remote address search, such as linking from elsewhere in the website or from a remote application

* Example- Getting a list of addresses from a partial postcode (or address)

[http://maps.astuntechnology.com/isharelive.web/getdata.aspx?service=Location&RequestType=LocationSearch&location=GU18&pagesize=10&startnum=1](http://maps.astuntechnology.com/isharelive.web/getdata.aspx?RequestType=LocalInfo&ms=mapsources/default&format=JSON&group=NHS%20Choices|Hospitals&uid=101726)