---
title: "IRepD3AxisZInt.Line"
description: "Specifies the line of the z-axis in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisZInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 3DAxisZ

Specifies the line of the z-axis in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
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
oMyXLabel = oMy3DAxisSystem.AxisList.X.Label
oMyXLabel.Text = "This is the x-axis"
oMyXLabel.Font.Name = "Tahoma"
oMyXLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.X.Line.Width = dd.eLineWidth0140
oMyYLabel = oMy3DAxisSystem.AxisList.Y.Label
oMyYLabel.Text = "This is the y-axis"
oMyYLabel.Font.Name = "Tahoma"
oMyYLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.Y.Line.Width = dd.eLineWidth0140
oMyZLabel = oMy3DAxisSystem.AxisList.Z.Label
oMyZLabel.Text = "This is the z-axis"
oMyZLabel.Font.Name = "Tahoma"
oMyZLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.Z.Line.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD3AxisZInt.htm`*
