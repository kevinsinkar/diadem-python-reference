---
title: "IRepD2ShapeObjOutlBarsHorizontalSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses for the Horizontal outlined bars display mode in a 2D axis system."
---

# IRepD2ShapeObjOutlBarsHorizontalSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DOutlineBarsHorizontalSettings

Specifies the properties of the palette which DIAdem REPORT uses for the Horizontal outlined bars display mode in a 2D axis system.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.ColorIndex = dd.eColorIndexPalette
oMySetting.Palette.ValueType = dd.e2DPaletteValueTypeAxisScalingRange
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjOutlBarsHorizontalSettingsInt.htm`*
