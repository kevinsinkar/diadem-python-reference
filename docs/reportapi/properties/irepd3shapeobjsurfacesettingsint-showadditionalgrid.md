---
title: "IRepD3ShapeObjSurfaceSettingsInt.ShowAdditionalGrid"
description: "Specifies whether DIAdem REPORT plots grid lines in the 3D axis system when displaying a surface with a color palette."
---

# IRepD3ShapeObjSurfaceSettingsInt.ShowAdditionalGrid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowAdditionalGrid for 3DSurfaceSettings

Specifies whether DIAdem REPORT plots grid lines in the 3D axis system when displaying a surface with a color palette.

## Signature

```python
obj.ShowAdditionalGrid
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
oMySettings.Line.Color.ColorIndex = dd.eColorIndexGlobalColorPalette1
oMySettings.ShowSurfaceFilled = True
oMySettings.ShowAdditionalGrid = True
oMySettings.AdditionalGridColor.SetPredefinedColor(dd.eColorIndexDarkYellow)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowAdditionalGrid_IRepD3ShapeObjSurfaceSettingsInt.htm`*
