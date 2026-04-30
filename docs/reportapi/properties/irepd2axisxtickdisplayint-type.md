---
title: "IRepD2AxisXTickDisplayInt.Type"
description: "Specifies on which side of the x-axis DIAdem REPORT plots the axis ticks in a 2D axis system."
---

# IRepD2AxisXTickDisplayInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DAxisXTickDisplay

Specifies on which side of the x-axis DIAdem REPORT plots the axis ticks in a 2D axis system.

## Signature

```python
obj.Type
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
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXTickDisplay = oMy2DAxisSystem.XAxis.TickDisplay
oMyXTickDisplay.UseAutoSize = False
oMyXTickDisplay.Size = 5
oMyXTickDisplay.Type = dd.e2DAxisXTickBothSides
oMyYTickDisplay = oMy2DAxisSystem.YAxis.TickDisplay
oMyYTickDisplay.UseAutoSize = False
oMyYTickDisplay.Size = 5
oMyYTickDisplay.Type = dd.e2DAxisXTickBothSides
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD2AxisXTickDisplayInt.htm`*
