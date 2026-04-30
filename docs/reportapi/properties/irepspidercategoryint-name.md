---
title: "IRepSpiderCategoryInt.Name"
description: "Specifies the name of a category in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCategoryInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Category

Specifies the name of a category in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Name
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

oMyCategorie = oMyCategorySettings.Categories
oMyCategorie.Count = 5
oMyCategorie.Item(2).Enable = True
oMyCategorie.Item(2).Name = "My Second Category"
oMyCategorie.Item(2).UnitString = "s"
print(oMyCategorie.Item(2).Index)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Name_IRepSpiderCategoryInt.htm`*
