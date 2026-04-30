---
title: "IRepMarkerRepetitionInt.ShowAtEnd"
description: "Specifies whether DIAdem REPORT displays the marker symbol at the end of the curve in a 2D axis system."
---

# IRepMarkerRepetitionInt.ShowAtEnd

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowAtEnd for MarkerRepetition

Specifies whether DIAdem REPORT displays the marker symbol at the end of the curve in a 2D axis system.

## Signature

```python
obj.ShowAtEnd
```

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
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionEveryNPercent
oMyExtension.Marker.Repetition.NValue = 20
oMyExtension.Marker.Repetition.ShowAtBegin = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowAtEnd_IRepMarkerRepetitionInt.htm`*
