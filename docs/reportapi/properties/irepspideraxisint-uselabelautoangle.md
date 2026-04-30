---
title: "IRepSpiderAxisInt.UseLabelAutoAngle"
description: "Specifies whether DIAdem determines the font angle of axis texts in a spider axis system automatically."
---

# IRepSpiderAxisInt.UseLabelAutoAngle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseLabelAutoAngle for SpiderAxis

Specifies whether DIAdem determines the font angle of axis texts in a spider axis system automatically.

## Signature

```python
obj.UseLabelAutoAngle
```

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

oMyCategorie = oMyCategorySettings.Categories
oMyCategorie.Count = 5
oMyCategorie(1).Enable = True
oMyCategorie(1).Name = "My First Category"
oMyCategorie(1).UnitString = "s"

oMyCategorieAxis = oMyCategorie(1).Axis
oMyCategorieAxis.Numbers.Font.Color.ColorIndex = dd.eColorIndexDarkRed
oMyCategorieAxis.Label.Text = "MyAxis"
oMyCategorieAxis.UseLabelAutoAngle = True
oMyCategorieAxis.Line.Width = dd.eLineWidth0035
oMyCategorieAxis.Line.Color.ColorIndex = dd.eColorIndexDarkGreen

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseLabelAutoAngle_IRepSpiderAxisInt.htm`*
