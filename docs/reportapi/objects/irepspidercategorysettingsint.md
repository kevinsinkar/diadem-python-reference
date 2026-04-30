---
title: "IRepSpiderCategorySettingsInt"
description: "The CategorySettings object provides the settings for a category in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCategorySettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CategorySettings

The CategorySettings object provides the settings for a category in a spider axis system in DIAdem REPORT.

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
<p><a href="../../properties/irepspidercategorysettingsint-axis/">Axis</a> | <a href="../../properties/irepspidercategorysettingsint-categories/">Categories</a> | <a href="../../properties/irepspidercategorysettingsint-channel/">Channel</a> | <a href="../../properties/irepspidercategorysettingsint-mode/">Mode</a> | <a href="../../properties/irepspidercategorysettingsint-unitchannel/">UnitChannel</a> | <a href="../../properties/irepspidercategorysettingsint-usecategories/">UseCategories</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspiderint/">Spider</a>.<a href="../../properties/irepspiderint-categorysettings/">CategorySettings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderCategorySettingsInt.htm`*
