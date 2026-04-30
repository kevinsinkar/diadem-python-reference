---
title: "IRepD3ShapeObjSurfaceSettingsInt.AdditionalGridColor"
description: "When DIAdem displays surfaces with a color palette, this variable specifies the color for the grid lines in DIAdem REPORT. You must first assign the value True "
---

# IRepD3ShapeObjSurfaceSettingsInt.AdditionalGridColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AdditionalGridColor for 3DSurfaceSettings

When DIAdem displays surfaces with a color palette, this variable specifies the color for the grid lines in DIAdem REPORT. You must first assign the value True to the ShowSurfaceFilled property and assign a palette to the surface color .

## Signature

```python
return_value = obj.AdditionalGridColor
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
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AdditionalGridColor_IRepD3ShapeObjSurfaceSettingsInt.htm`*
