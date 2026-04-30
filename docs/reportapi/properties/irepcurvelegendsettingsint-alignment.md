---
title: "IRepCurveLegendSettingsInt.Alignment"
description: "Specifies the relative position of the legend label in relation to the symbols in an axis system in DIAdem REPORT. If the legend contains more than one text col"
---

# IRepCurveLegendSettingsInt.Alignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Alignment for CurveLegendSettings

Specifies the relative position of the legend label in relation to the symbols in an axis system in DIAdem REPORT. If the legend contains more than one text column, the text columns are always displayed to the right of the symbols. If the extended legend setting is turned off, automatic alignment always takes place.

## Signature

```python
obj.Alignment
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLegendTextAlignmentAutomatic` | 0 | Automatic |
| `eLegendTextAlignmentTop` | 1 | Top |
| `eLegendTextAlignmentBottom` | 2 | Bottom |
| `eLegendTextAlignmentLeft` | 3 | Left |
| `eLegendTextAlignmentRight` | 4 | Right |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegendSettings = oMyCurveLegend.Settings
oMyCurveLegendSettings.Font.Name = "Times Roman"()
oMyCurveLegendSettings.Font.Bold = True
oMyCurveLegendSettings.ExpansionDirection = dd.eLegendGrowthExpansionBottomUp
oMyCurveLegendSettings.Angle = dd.eAngle0
oMyCurveLegendSettings.Alignment = dd.eLegendTextAlignmentLeft
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Alignment_IRepCurveLegendSettingsInt.htm`*
