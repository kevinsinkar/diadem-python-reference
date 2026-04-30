---
title: "IRepCurveLegendSettingsInt.ShowSymbolFrame"
description: "Specifies whether DIAdem REPORT frames the legend symbols of an axis system."
---

# IRepCurveLegendSettingsInt.ShowSymbolFrame

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowSymbolFrame for CurveLegendSettings

Specifies whether DIAdem REPORT frames the legend symbols of an axis system.

## Signature

```python
obj.ShowSymbolFrame
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegend.Settings.ShowSymbolFrame = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowSymbolFrame_IRepCurveLegendSettingsInt.htm`*
