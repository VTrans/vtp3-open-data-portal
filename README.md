vtp3-open-data-portal
=====================

"All data we share should be available on the AGOL Open Data Portal"

#[Open Data Portal](http://vtransparency.vtrans.opendata.arcgis.com/)

Examples: 
- [Esri default example](http://beta.esri.opendata.arcgis.com/)
- [Maryland iMap](http://data.imap.maryland.gov/)


#Setup

[Documentation](http://doc.arcgis.com/en/open-data)

###All feature services have to be published with `Feature Access` capability and the `Query` operation allowed. [(ref)](http://doc.arcgis.com/en/open-data/provider/specify-groups-for-open-data.htm)

####[ArcGIS Online Group](http://vtrans.maps.arcgis.com/home/group.html?id=6e800ae91782448c8263a1456a783fc6)

###Publishing Services

**In ArcMap**

1. Add data from registered data source
2. File -> Share As -> Service
3. Fill out a name 
4. Put it in the `vtp3` folder
5. Enable `Feature Acces` capability
6. Disable `KML` capability
7. Under `Mapping`, check "Allow per request modification..."
8. Under `Feature Access`, disable **Create, Delete, Update** operations
9. Fill out summary and tags under `Item Description` settings
10. Check `My Content` in the `Sharing` settings

**In ArcGIS Online**

1. Find your `FeatureService` URL [here](http://vtransmap01.aot.state.vt.us/arcgis/rest/services)
2. In `My Content`, click Add Item
3. Choose `On the web` from the dropdown
4. Paste in the `FeatureService` URL
5. Click Add Item
6. Go to the item
7. Click Share
8. Select `Everyone` and `VTransparency (open data)`  
9. Hit OK

**OpenData admin panel**
[admin panel link](https://opendata.arcgis.com/admin/#/sites)


```
There seems to be a problem with the Open Data Portal for ArcGIS Online
Here is an issue discussing the problem on GeoNet 
https://geonet.esri.com/thread/107927
Waiting on reply from French @ Esri
```
Reply 10/22/14 4:26:
```
They acknowledged the issue as a bug, however they don’t know exactly what dataset elements cause it during harvesting.  The recommendation was to try publishing as a hosted feature service in ArcGIS Online to test, and serve temporarily while the fix is developed (expected 2-3 weeks).   

Can you test the data (or subset) with a hosted service and report back?  That will help our teams nail down the issue.

```

#Metadata Standards
Needed
