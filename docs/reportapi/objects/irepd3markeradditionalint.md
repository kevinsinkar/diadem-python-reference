---
title: "IRepD3MarkerAdditionalInt"
description: "The 3DAdditionalMarker object provides the properties of the markers in a 2D axis system in DIAdem REPORT."
---

# IRepD3MarkerAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalMarker

The 3DAdditionalMarker object provides the properties of the markers in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.Settings.Marker.Type = dd.eMarkerAsterisk
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3markeradditionalint-filling/">Filling</a> | <a href="../../properties/irepd3markeradditionalint-line/">Line</a> | <a href="../../properties/irepd3markeradditionalint-size/">Size</a> | <a href="../../properties/irepd3markeradditionalint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3characteristicdiagrampointsadditionalint/">3DAdditionalCharacteristicDiagramPoints</a>.<a href="../../properties/irepd3characteristicdiagrampointsadditionalint-marker/">Marker</a> | <a href="../irepd3shapeobjbarsextensionsint/">3DBarsExtensions</a>.<a href="../../properties/irepd3shapeobjbarsextensionsint-marker/">Marker</a> | <a href="../irepd3shapeobjmatrix2dextensionsint/">3DMatrix2DExtensions</a>.<a href="../../properties/irepd3shapeobjmatrix2dextensionsint-marker/">Marker</a> | <a href="../irepd3shapeobjsurfaceextensionsint/">3DSurfaceExtensions</a>.<a href="../../properties/irepd3shapeobjsurfaceextensionsint-marker/">Marker</a> | <a href="../irepd3shapeobjvectorextensionsint/">3DVectorExtensions</a>.<a href="../../properties/irepd3shapeobjvectorextensionsint-marker/">Marker</a> | <a href="../irepd3shapeobjwaterfallextensionsint/">3DWaterfallExtensions</a>.<a href="../../properties/irepd3shapeobjwaterfallextensionsint-marker/">Marker</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3MarkerAdditionalInt.htm`*
