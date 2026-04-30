---
title: "IRepColorLegendSettingsInt.Orientation"
description: "Specifies how DIAdem REPORT aligns the components of the legend of an axis system."
---

# IRepColorLegendSettingsInt.Orientation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Orientation for ColorLegendSettings

Specifies how DIAdem REPORT aligns the components of the legend of an axis system.

## Signature

```python
obj.Orientation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendOrientationAutomatic` | 0 | Automatic—DIAdem aligns the legend horizontally if the height/width ratio is higher than 0.7, otherwise the alignment is vertical. |
| `eLegendOrientationHorizontal` | 1 | Horizontal—DIAdem positions the components of the legend next to each other and positions the labels below the respective component. |
| `eLegendOrientationVertical` | 2 | Vertical—DIAdem positions the components of the legend underneath each other and positions the labels next to the respective components. |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 10
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyColorLegend.Settings.Orientation = dd.eLegendOrientationVertical
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.ddde"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Orientation_IRepColorLegendSettingsInt.htm`*
