---
title: "IRepMarkerRepetitionInt.NPercentValue"
description: "Specifies that DIAdem REPORT displays the curve markers in a 2D axis system at every nth percent of the curve length if you assign the value eMarkerRepetitionEv"
---

# IRepMarkerRepetitionInt.NPercentValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: NPercentValue for MarkerRepetition

Specifies that DIAdem REPORT displays the curve markers in a 2D axis system at every nth percent of the curve length if you assign the value eMarkerRepetitionEveryNPercent to the Mode property.

## Signature

```python
obj.NPercentValue
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
oMyExtension.Marker.Repetition.NPercentValue = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_NPercentValue_IRepMarkerRepetitionInt.htm`*
