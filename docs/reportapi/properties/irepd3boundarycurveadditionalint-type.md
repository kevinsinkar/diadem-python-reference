---
title: "IRepD3BoundaryCurveAdditionalInt.Type"
description: "Specifies the origin of the boundary curve in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT."
---

# IRepD3BoundaryCurveAdditionalInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 3DAdditionalBoundaryCurve

Specifies the origin of the boundary curve in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>DIAdem creates the full load curve from the points with the greatest y-value of each partial load. DIAdem creates the lower limit curve from the points with the smallest y-value of each partial load. A partial load is made up of points with x-values that lie in a narrow tolerance range.</td></tr></table>
</div>

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\engine_characteristic_map.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
oMyShape.Extensions.BoundaryCurve.Visible = True
oMyShape.Extensions.BoundaryCurve.Type = dd.e3DBoundaryCurveConvexHull
oMyShape.Extensions.BoundaryPoints.Visible = True
oMyLabel = oMyShape.Extensions.BoundaryPoints.Label
oMyLabel.Visible = True
oMyLabel.Font.Size = 4
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD3BoundaryCurveAdditionalInt.htm`*
