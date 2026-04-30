---
title: "IRepD3AxisYInt.Numbers"
description: "Specifies the properties of the y-axis labels in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisYInt.Numbers

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Numbers for 3DAxisY

Specifies the properties of the y-axis labels in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Numbers
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
oMyYAxis = oMy3DAxisSystem.AxisList.Y
oMyYAxisNumbers = oMyYAxis.Numbers
oMyYAxisNumbers.Angle = 90
oMyYAxisNumbers.Font.Size = 4
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Numbers_IRepD3AxisYInt.htm`*
