---
title: "IRepD2ShapeObjSpikesSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses for a spikes display in a 2D axis system."
---

# IRepD2ShapeObjSpikesSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DSpikesSettings

Specifies the properties of the palette which DIAdem REPORT uses for a spikes display in a 2D axis system.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Report_EXPL","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpikes, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyPalette = oMyShape.Settings.Palette
oMyPalette.ValueType = dd.e2DPaletteValueTypeAxisScalingRange
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjSpikesSettingsInt.htm`*
