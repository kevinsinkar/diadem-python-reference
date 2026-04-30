---
title: "IRepSpiderCategoryListInt.Item"
description: "Returns the category of a specific index of a spider axis system in DIAdem REPORT."
---

# IRepSpiderCategoryListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for Categories

Returns the category of a specific index of a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Item(Index)
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
oMyCategorySettings.Mode = dd.eCategoryModeFreeText
oMyCategorySettings.Categories.Count = 1
oMyCategorySettings.Categories(1).Enable = True
oMyCategorySettings.Categories(1).Name = "MyCategory"
oMyCategorySettings.UseCategories = True
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepSpiderCategoryListInt.htm`*
