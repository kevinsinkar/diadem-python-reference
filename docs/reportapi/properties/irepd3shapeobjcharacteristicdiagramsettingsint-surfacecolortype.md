---
title: "IRepD3ShapeObjCharacteristicDiagramSettingsInt.SurfaceColorType"
description: "Specifies whether DIAdem REPORT displays the surface with the colors defined in the contour table or with the colors from a global color palette."
---

# IRepD3ShapeObjCharacteristicDiagramSettingsInt.SurfaceColorType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SurfaceColorType for 3DCharacteristicDiagramSettings

Specifies whether DIAdem REPORT displays the surface with the colors defined in the contour table or with the colors from a global color palette.

## Signature

```python
obj.SurfaceColorType
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMySettings = oMyShape.Settings
oMySettings.SurfaceColorType = dd.e3DCharacteristicSurfaceColorGlobalColorPalette1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SurfaceColorType_IRepD3ShapeObjCharacteristicDiagramSettingsInt.htm`*
