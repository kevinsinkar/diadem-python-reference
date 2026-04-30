---
title: "IRepSpiderAxisInt.TickType"
description: "Specifies how DIAdem REPORT plots the scale ticks of the axis in a spider axis system."
---

# IRepSpiderAxisInt.TickType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TickType for SpiderAxis

Specifies how DIAdem REPORT plots the scale ticks of the axis in a spider axis system.

## Signature

```python
obj.TickType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderAxisTickNone` | 0 | None |
| `eSpiderAxisTickBothSides` | 1 | Both sides |
| `eSpiderAxisTickLeft` | 2 | Left |
| `eSpiderAxisTickRight` | 3 | Right |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPosition = oMyAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MyCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyCategorySettings = oMyAxisSystem.CategorySettings
oMyCategorySettings.Channel.Reference = "[5]/[1]"
oMyCategorySettings.Axis.Scaling.Type = dd.eSpiderScalingLinear
oMyCategorySettings.UseCategories = True

oMyCategories = oMyCategorySettings.Categories
oMyCategories.Count = 5
oMyCategories(1).Enable = True
oMyCategories(1).Name = "My First Category"
oMyCategories(1).UnitString = "s"

oMyCategorieAxis = oMyCategories(1).Axis
oMyCategorieAxis.Numbers.Font.Color.ColorIndex = dd.eColorIndexDarkRed
oMyCategorieAxis.Label.Text = "MyAxis"
oMyCategorieAxis.UseLabelAutoAngle = True
oMyCategorieAxis.Line.Width = dd.eLineWidth0035
oMyCategorieAxis.Line.Color.ColorIndex = dd.eColorIndexDarkGreen
oMyCategorieAxis.ShowMiniTicks = True
oMyCategorieAxis.ShowTicks = True
oMyCategorieAxis.TickType = dd.eSpiderAxisTickBothSides

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TickType_IRepSpiderAxisInt.htm`*
