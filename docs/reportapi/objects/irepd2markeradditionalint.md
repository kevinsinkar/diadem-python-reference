---
title: "IRepD2MarkerAdditionalInt"
description: "The 2DAdditionalMarker object provides the properties of the curve markers in a 2D axis system in DIAdem REPORT."
---

# IRepD2MarkerAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAdditionalMarker

The 2DAdditionalMarker object provides the properties of the curve markers in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyExtension = oMyShape.Extensions
oMyExtension.Marker.Type = dd.eMarkerCircle
oMyExtension.Marker.Size = 3
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyExtension.Marker.Repetition.NValue = 20
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2markeradditionalint-channel/">Channel</a> | <a href="../../properties/irepd2markeradditionalint-filling/">Filling</a> | <a href="../../properties/irepd2markeradditionalint-line/">Line</a> | <a href="../../properties/irepd2markeradditionalint-minimumdisplaysize/">MinimumDisplaySize</a> | <a href="../../properties/irepd2markeradditionalint-repetition/">Repetition</a> | <a href="../../properties/irepd2markeradditionalint-size/">Size</a> | <a href="../../properties/irepd2markeradditionalint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjlineandpointsextensionsint/">2DLineAndPointsExtensions</a>.<a href="../../properties/irepd2shapeobjlineandpointsextensionsint-marker/">Marker</a> | <a href="../irepd2shapeobjlineextensionsint/">2DLineExtensions</a>.<a href="../../properties/irepd2shapeobjlineextensionsint-marker/">Marker</a> | <a href="../irepd2shapeobjspecialcombinationextensionsint/">2DSpecialCombinationExtensions</a>.<a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-marker/">Marker</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2MarkerAdditionalInt.htm`*
