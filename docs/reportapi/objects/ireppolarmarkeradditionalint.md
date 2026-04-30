---
title: "IRepPolarMarkerAdditionalInt"
description: "The PolarAdditionalMarker object provides the properties of the curve markers for a polar curve in DIAdem REPORT."
---

# IRepPolarMarkerAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarAdditionalMarker

The PolarAdditionalMarker object provides the properties of the curve markers for a polar curve in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyAddMarker = oMyShape.Extensions.Marker
oMyAddMarker.Type = dd.eMarkerCircle
oMyAddMarker.Size = 3
oMyExtension = oMyShape.Extensions
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionEveryNthPoint
oMyExtension.Marker.Repetition.NValue = 50
oMyAddMarker.Line.UseCurveColor = False
oMyAddMarker.Line.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMyAddMarker.Line.Width = dd.eLineWidth0280
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarmarkeradditionalint-channel/">Channel</a> | <a href="../../properties/ireppolarmarkeradditionalint-filling/">Filling</a> | <a href="../../properties/ireppolarmarkeradditionalint-line/">Line</a> | <a href="../../properties/ireppolarmarkeradditionalint-minimumdisplaysize/">MinimumDisplaySize</a> | <a href="../../properties/ireppolarmarkeradditionalint-repetition/">Repetition</a> | <a href="../../properties/ireppolarmarkeradditionalint-size/">Size</a> | <a href="../../properties/ireppolarmarkeradditionalint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarshapeobjlineandpointsextensionsint/">PolarLineAndPointsExtensions</a>.<a href="../../properties/ireppolarshapeobjlineandpointsextensionsint-marker/">Marker</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarMarkerAdditionalInt.htm`*
