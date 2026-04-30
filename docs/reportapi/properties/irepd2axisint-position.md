---
title: "IRepD2AxisInt.Position"
description: "Specifies the position of a 2D axis system in a DIAdem REPORT worksheet."
---

# IRepD2AxisInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for 2DAxisSystem

Specifies the position of a 2D axis system in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"

oMy2DAxisSystem.Position.ByCoordinate.X1 = 10
oMy2DAxisSystem.Position.ByCoordinate.X2 = 40
oMy2DAxisSystem.Position.ByCoordinate.Y1 = 50
oMy2DAxisSystem.Position.ByCoordinate.Y2 = 80
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepD2AxisInt.htm`*
