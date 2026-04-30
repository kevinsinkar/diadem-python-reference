---
title: "IRepCurvelegendContentColumnInt.Title"
description: "Specifies the text for the general label of a legend column in an axis system in DIAdem REPORT."
---

# IRepCurvelegendContentColumnInt.Title

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Title for CurveLegendColumn

Specifies the text for the general label of a legend column in an axis system in DIAdem REPORT.

## Signature

```python
obj.Title
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 30
oMyPosition.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMyShape = oMy2DCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyCurveLegendPos = oMy2DaxisSystem.CurveLegend.Position
oMyCurveLegendPos.RelativePosition = dd.eLegendRelativePositionBottomRight
oMyCurveLegendPos.SizeMode = dd.eLegendSizeElementwise
oMyCurveLegendPos.ElementHeight = 6
oMyCurveLegendPos.ElementWidth = 35
oMy2DaxisSystem.CurveLegend.Settings.Font.Size = 4
oMyLegendColumns = oMy2DaxisSystem.CurveLegend.Columns
oMyLegendColumns.Add()
oMyLegendColumns(1).Title = "First title"
oMyLegendColumns(1).Type = dd.eLegendTextCustomText
oMyLegendColumns(1).RelativeWidth = 2
oMyLegendColumns(1).Text = "First col - longer text"
oMyLegendColumns(2).Title = "Second title"
oMyLegendColumns(2).Type = dd.eLegendTextCustomText
oMyLegendColumns(2).RelativeWidth = 1
oMyLegendColumns(2).Text = "SecondCol"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Title_IRepCurvelegendContentColumnInt.htm`*
