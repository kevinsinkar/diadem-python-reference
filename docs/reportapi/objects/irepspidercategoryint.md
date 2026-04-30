---
title: "IRepSpiderCategoryInt"
description: "The Category object provides a category in a spider axis system curve in DIAdem REPORT. To access an individual Category object, the value of the property Count"
---

# IRepSpiderCategoryInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Category

The Category object provides a category in a spider axis system curve in DIAdem REPORT. To access an individual Category object, the value of the property Count must be greater than 0.

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
oMyCategorySettings.UseCategories = True

oMyCategories = oMyCategorySettings.Categories
oMyCategories.Count = 1
oMyCategories(1).Enable = True
oMyCategories(1).Name = "My First Category"
oMyCategories(1).UnitString = "s"

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepspidercategoryint-axis/">Axis</a> | <a href="../../properties/irepspidercategoryint-enable/">Enable</a> | <a href="../../properties/irepspidercategoryint-index/">Index</a> | <a href="../../properties/irepspidercategoryint-name/">Name</a> | <a href="../../properties/irepspidercategoryint-unitstring/">UnitString</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/categories/">Categories</a>.<a href="../../methods/irepspidercategorylistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderCategoryInt.htm`*
