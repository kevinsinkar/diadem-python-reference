---
title: "IRepD3AxisYInt.UseNumbersAutoPosition"
description: "Specifies whether DIAdem REPORT determines the y-scaling label position automatically in a 3D axis system."
---

# IRepD3AxisYInt.UseNumbersAutoPosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseNumbersAutoPosition for 3DAxisY

Specifies whether DIAdem REPORT determines the y-scaling label position automatically in a 3D axis system.

## Signature

```python
obj.UseNumbersAutoPosition
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureMatrix
oMyX = oMy3DAxisSystem.AxisList.X
oMyX.UseLabelAutoAngle = True
oMyX.UseNumbersAutoPosition = True
oMyXLabel = oMyX.Label
oMyXLabel.Text = "This is the x-axis"
oMyXLabel.Font.Name = "Tahoma"
oMyXLabel.Font.Size = 5
oMyY = oMy3DAxisSystem.AxisList.Y
oMyY.UseLabelAutoAngle = True
oMyY.UseNumbersAutoPosition = True
oMyYLabel = oMyY.Label
oMyYLabel.Text = "This is the y-axis"
oMyYLabel.Font.Name = "Tahoma"
oMyYLabel.Font.Size = 5
oMyZ = oMy3DAxisSystem.AxisList.Z
oMyZ.UseLabelAutoAngle = True
oMyZ.UseNumbersAutoPosition = True
oMyZLabel = oMyZ.Label
oMyZLabel.Text = "This is the z-axis"
oMyZLabel.Font.Name = "Tahoma"
oMyZLabel.Font.Size = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseNumbersAutoPosition_IRepD3AxisYInt.htm`*
