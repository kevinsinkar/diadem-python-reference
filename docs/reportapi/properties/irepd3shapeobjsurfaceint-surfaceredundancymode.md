---
title: "IRepD3ShapeObjSurfaceInt.SurfaceRedundancyMode"
description: "Specifies in a curve display in the Surface display mode in a 3D axis system in DIAdem REPORT the point that DIAdem displays in color on the screen or in the pr"
---

# IRepD3ShapeObjSurfaceInt.SurfaceRedundancyMode

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SurfaceRedundancyMode for 3DSurface

Specifies in a curve display in the Surface display mode in a 3D axis system in DIAdem REPORT the point that DIAdem displays in color on the screen or in the printout if several measured values lie on the same display point due to too low resolution.

## Signature

```python
obj.SurfaceRedundancyMode
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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SurfaceRedundancyMode_IRepD3ShapeObjSurfaceInt.htm`*
