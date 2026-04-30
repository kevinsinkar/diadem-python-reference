---
title: "IRepAxisLabelInt.Angle"
description: "Specifies the angle of the axis label in an axis system in DIAdem REPORT. DIAdem only includes the Angle property in the objects 3DAxisX , 3DAxisY , and 3DAxisZ"
---

# IRepAxisLabelInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for AxisLabel

Specifies the angle of the axis label in an axis system in DIAdem REPORT. DIAdem only includes the Angle property in the objects 3DAxisX , 3DAxisY , and 3DAxisZ if you assign the value FALSE to the UseLabelAutoAngle property.

## Signature

```python
obj.Angle
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.Label.Text = "x-axis"
oMy2DAxisSystem.YAxis.Label.Text = "y-axis"
oMy2DAxisSystem.XAxis.Label.Angle = 45
oMy2DAxisSystem.YAxis.Label.Angle = 45
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepAxisLabelInt.htm`*
