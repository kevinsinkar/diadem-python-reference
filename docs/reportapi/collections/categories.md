---
title: "Categories"
description: "Collection of all Category objects in DIAdem REPORT. Use the Categories collection to access a single category in a spider axis system. To access a single Categ"
---

# Categories

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: Categories

Collection of all Category objects in DIAdem REPORT. Use the Categories collection to access a single category in a spider axis system. To access a single Category object , the value of the Count property must be greater than 0.

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
<p><a href="../../properties/irepspidercategorylistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepspidercategorylistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepspidercategorysettingsint/">CategorySettings</a>.<a href="../../properties/irepspidercategorysettingsint-categories/">Categories</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderCategoryListInt.htm`*
