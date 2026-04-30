---
title: "IRepD3ShapeObjSurfaceSettingsInt.UseMassiveDisplay"
description: "Specifies whether DIAdem REPORT plots the surface of a 3D axis system in the Surface display mode as the slice plane of a solid cube."
---

# IRepD3ShapeObjSurfaceSettingsInt.UseMassiveDisplay

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseMassiveDisplay for 3DSurfaceSettings

Specifies whether DIAdem REPORT plots the surface of a 3D axis system in the Surface display mode as the slice plane of a solid cube.

## Signature

```python
obj.UseMassiveDisplay
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
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.UseMassiveDisplay = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseMassiveDisplay_IRepD3ShapeObjSurfaceSettingsInt.htm`*
