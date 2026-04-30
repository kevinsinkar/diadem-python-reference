---
title: "IRepD2ShapeObjCoordinateSettingsInt.Palette"
description: "Specifies the properties of the palette which DIAdem REPORT uses in the Coordinate display mode in a 2D axis system."
---

# IRepD2ShapeObjCoordinateSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DCoordinateSettings

Specifies the properties of the palette which DIAdem REPORT uses in the Coordinate display mode in a 2D axis system.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyShape = oMyCurveLine.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.BoundingPosition = dd.e2DCoordinateBoundingInterpolation
oMyCoordShape.BoundingXChannel.Reference = "[1]/[1]"
oMyCoordShape.BoundingyChannel.Reference = "[1]/[2]"
oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordShape.Settings.Size = 4
oMyCoordShape.Settings.MarkerFilling.ColorIndex = dd.eColorIndexPalette
MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY
oMyPalette = oMyCoordShape.Settings.Palette
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

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjCoordinateSettingsInt.htm`*
