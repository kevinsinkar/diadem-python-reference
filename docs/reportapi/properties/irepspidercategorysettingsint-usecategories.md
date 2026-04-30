---
title: "IRepSpiderCategorySettingsInt.UseCategories"
description: "Specifies whether you can configure category axes individually in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCategorySettingsInt.UseCategories

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCategories for CategorySettings

Specifies whether you can configure category axes individually in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.UseCategories
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
oMyCategorySettings.Mode = dd.eCategoryModeChannel
oMyCategorySettings.Channel.Reference = "[5]/[1]"
oMyCategorySettings.UseCategories = True

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCategories_IRepSpiderCategorySettingsInt.htm`*
