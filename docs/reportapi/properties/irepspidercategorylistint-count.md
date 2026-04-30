---
title: "IRepSpiderCategoryListInt.Count"
description: "Specifies the number of categories in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCategoryListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for Categories

Specifies the number of categories in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Count
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
oMyCategorySettings.Categories.Count = 5
oMyCategorySettings.Categories(1).Enable = True
oMyCategorySettings.Categories(1).Name = "MyCategory"
oMyCategorySettings.UseCategories = True

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepSpiderCategoryListInt.htm`*
