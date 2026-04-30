---
title: "IRepD3AxisYInt.TickType"
description: "Specifies how DIAdem REPORT plots the scale ticks of the y-axis in a 3D axis system."
---

# IRepD3AxisYInt.TickType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TickType for 3DAxisY

Specifies how DIAdem REPORT plots the scale ticks of the y-axis in a 3D axis system.

## Signature

```python
obj.TickType
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
oMyAxisList = oMy3DAxisSystem.AxisList
oMyAxisList.X.TickType = dd.e3DAxisXYTickBothSides
oMyAxisList.X.Scaling.Type = dd.e3DScalingDateTime
oMyAxisList.Y.TickType = dd.e3DAxisXYTickInNegZDirection
oMyAxisList.Y.Scaling.Type = dd.e3DScalingLinear
oMyAxisList.Z.TickType =dd.e3DAxisZTickRight
oMyAxisList.Z.Scaling.Type = dd.e3DScalingLinear
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TickType_IRepD3AxisYInt.htm`*
