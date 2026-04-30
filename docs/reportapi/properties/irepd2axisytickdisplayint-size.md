---
title: "IRepD2AxisYTickDisplayInt.Size"
description: "Specifies the length of the scaling ticks on the y-axis of a 2D axis system as a percentage of the width of the axis system in DIAdem REPORT. DIAdem only includ"
---

# IRepD2AxisYTickDisplayInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for 2DAxisYTickDisplay

Specifies the length of the scaling ticks on the y-axis of a 2D axis system as a percentage of the width of the axis system in DIAdem REPORT. DIAdem only includes the property Size if you assign the value FALSE to the property UseAutoSize .

## Signature

```python
obj.Size
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

*Source: `ReportApi/properties/Report_property_Size_IRepD2AxisYTickDisplayInt.htm`*
