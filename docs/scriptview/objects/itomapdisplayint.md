---
title: "IToMapDisplayInt"
description: "The Map object provides access to a map display in DIAdem VIEW. Use the Map object to specify the properties of the map view and the channels to be synchronized"
---

# IToMapDisplayInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Map

The Map object provides access to a map display in DIAdem VIEW. Use the Map object to specify the properties of the map view and the channels to be synchronized with the view.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\VIEW_MapDisplay.tdm")
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Map"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.MapType = "OSM Mapnik"
oMyObj.ZoomLevel = 14
oMyObj.SynchronisationChannelName = "[1]/TimeStamp"
oMyObj.LongitudeChannelName = "[1]/Longitude"
oMyObj.LatitudeChannelName = "[1]/Latitude"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itomapdisplayint-area/">Area</a> | <a href="../../properties/itomapdisplayint-cachepath/">CachePath</a> | <a href="../../properties/itomapdisplayint-colorchannelname/">ColorChannelName</a> | <a href="../../properties/itomapdisplayint-latitudechannelname/">LatitudeChannelName</a> | <a href="../../properties/itomapdisplayint-latitudedimension/">LatitudeDimension</a> | <a href="../../properties/itomapdisplayint-longitudechannelname/">LongitudeChannelName</a> | <a href="../../properties/itomapdisplayint-longitudedimension/">LongitudeDimension</a> | <a href="../../properties/itomapdisplayint-mapmovingmode/">MapMovingMode</a> | <a href="../../properties/itomapdisplayint-maptype/">MapType</a> | <a href="../../properties/itomapdisplayint-showtrack/">ShowTrack</a> | <a href="../../properties/itomapdisplayint-synchronisationchannelname/">SynchronisationChannelName</a> | <a href="../../properties/itomapdisplayint-synchronisationdimension/">SynchronisationDimension</a> | <a href="../../properties/itomapdisplayint-toolbarvisible/">ToolbarVisible</a> | <a href="../../properties/itomapdisplayint-usecache/">UseCache</a> | <a href="../../properties/itomapdisplayint-zoomlevel/">ZoomLevel</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itomapdisplayint-isbusy/">isBusy</a> | <a href="../../methods/itomapdisplayint-showmapdlg/">ShowMapDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToMapDisplayInt.htm`*
