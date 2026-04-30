---
title: "IRepMarkerRepetitionInt"
description: "The MarkerRepetition object provides the repeat properties of the curve markers in an axis system in DIAdem REPORT."
---

# IRepMarkerRepetitionInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: MarkerRepetition

The MarkerRepetition object provides the repeat properties of the curve markers in an axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepmarkerrepetitionint-mode/">Mode</a> | <a href="../../properties/irepmarkerrepetitionint-npercentvalue/">NPercentValue</a> | <a href="../../properties/irepmarkerrepetitionint-nvalue/">NValue</a> | <a href="../../properties/irepmarkerrepetitionint-showatbegin/">ShowAtBegin</a> | <a href="../../properties/irepmarkerrepetitionint-showatend/">ShowAtEnd</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2markeradditionalint/">2DAdditionalMarker</a>.<a href="../../properties/irepd2markeradditionalint-repetition/">Repetition</a> | <a href="../ireppolarmarkeradditionalint/">PolarAdditionalMarker</a>.<a href="../../properties/ireppolarmarkeradditionalint-repetition/">Repetition</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepMarkerRepetitionInt.htm`*
