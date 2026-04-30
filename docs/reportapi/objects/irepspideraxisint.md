---
title: "IRepSpiderAxisInt"
description: "The SpiderAxis object provides a curve in a spider axis system in DIAdem REPORT. If the CategorySettings . Axis property returns the SpiderAxis object, the obje"
---

# IRepSpiderAxisInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderAxis

The SpiderAxis object provides a curve in a spider axis system in DIAdem REPORT. If the CategorySettings . Axis property returns the SpiderAxis object, the object is the standard axis. DIAdem uses the standard axis for all categories if you assigned the value False to the UseCategories for CategorySettings property. If you assigned the value True to the property UseCategories for CategorySettings , DIAdem also uses the standard axis for the categories whose property Enable for Category has the value False . DIAdem also uses the standard axis for the categories whose property Name for Category is empty when the property Mode for CategorySettings has the value eCategoryModeFreeText .

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

oMyCategorieAxis = oMyCategories(1).Axis
oMyCategorieAxis.Numbers.Font.Color.ColorIndex = dd.eColorIndexDarkRed
oMyCategorieAxis.Line.Width = dd.eLineWidth0035
oMyCategorieAxis.Line.Color.ColorIndex = dd.eColorIndexDarkGreen
oMyCategorieAxis.TickType = dd.eSpiderAxisTickBothSides

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="#" data-unresolved="1">Label</a> | <a href="../../properties/irepspideraxisint-line/">Line</a> | <a href="../../properties/irepspideraxisint-numbers/">Numbers</a> | <a href="../../properties/irepspideraxisint-scaling/">Scaling</a> | <a href="../../properties/irepspideraxisint-ticktype/">TickType</a> | <a href="../../properties/irepspideraxisint-uselabelautoangle/">UseLabelAutoAngle</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidercategoryint/">Category</a>.<a href="../../properties/irepspidercategoryint-axis/">Axis</a> | <a href="../irepspidercategorysettingsint/">CategorySettings</a>.<a href="../../properties/irepspidercategorysettingsint-axis/">Axis</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderAxisInt.htm`*
