---
title: "IRepD3ShapeObjSurfaceInt.ReferencePlaneZValue"
description: "Specifies the value of the z-level DIAdem uses to determine the measurement value that has the greatest distance to the z-reference level, in a curve display in"
---

# IRepD3ShapeObjSurfaceInt.ReferencePlaneZValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ReferencePlaneZValue for 3DSurface

Specifies the value of the z-level DIAdem uses to determine the measurement value that has the greatest distance to the z-reference level, in a curve display in the Surface display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.ReferencePlaneZValue
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
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.SurfaceRedundancyMode = eDSurfaceRedundancyReferencePlane
oMy3DCurve.Shape.ReferencePlaneZValue = 0
oMy3DCurve.Shape.Settings.Line.Color.ColorIndex = dd.eColorIndexGlobalColorPalette1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2></h2>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ReferencePlaneZValue_IRepD3ShapeObjSurfaceInt.htm`*
