---
title: "IRepD3AxisZInt.Numbers"
description: "Specifies the properties of the z-axis labels in a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisZInt.Numbers

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Numbers for 3DAxisZ

Specifies the properties of the z-axis labels in a 3D axis system in DIAdem REPORT.

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
oMyZAxis = oMy3DAxisSystem.AxisList.Z
oMyZAxisNumbers = oMyZAxis.Numbers
oMyZAxisNumbers.Angle = 90
oMyZAxisNumbers.Font.Size = 4
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Numbers_IRepD3AxisZInt.htm`*
