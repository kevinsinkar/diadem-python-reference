---
title: "IRepCurveLegendSettingsInt.UseWordWrap"
description: "Specifies whether DIAdem wraps the legend label of an axis system at the edge of the legend column. You must assign the value TRUE to the UseTextClipping proper"
---

# IRepCurveLegendSettingsInt.UseWordWrap

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseWordWrap for CurveLegendSettings

Specifies whether DIAdem wraps the legend label of an axis system at the edge of the legend column. You must assign the value TRUE to the UseTextClipping property and the value FALSE to the UseAutoFontSize property in order to use the UseWordWrap property.

## Signature

```python
obj.UseWordWrap
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 30
oMyPosition.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyShape = oMy2DCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegendPos = oMyLegend.Position
oMyLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyLegendPos.Anchor.PageRelatedX = 15
oMyLegendPos.Anchor.PageRelatedY = 20
oMyLegendPos.ElementHeight = 15
oMyLegendPos.ElementWidth = 20
oMyLegendSettings = oMyLegend.Settings
oMyLegendSettings.UseAutoFontSize = False
oMyLegendSettings.Font.Size = 6
oMyLegendSettings.UseTextClipping = True
oMyLegendSettings.UseWordWrap = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseWordWrap_IRepCurveLegendSettingsInt.htm`*
