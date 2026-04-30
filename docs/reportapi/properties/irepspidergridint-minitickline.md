---
title: "IRepSpiderGridInt.MiniTickLine"
description: "Specifies the properties of the minitick lines of a spider network in DIAdem REPORT. DIAdem REPORT only displays the minitick lines when the property ShowMiniTi"
---

# IRepSpiderGridInt.MiniTickLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniTickLine for SpiderGrid

Specifies the properties of the minitick lines of a spider network in DIAdem REPORT. DIAdem REPORT only displays the minitick lines when the property ShowMiniTickLine has the value True and the property UseCategories has the value False .

## Signature

```python
return_value = obj.MiniTickLine
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyCategorySettings = oMyAxisSystem.CategorySettings
oMyCategorySettings.UseCategories = False

oMyGrid = oMyAxisSystem.Settings.Grid
oMyGrid.ShowLine = True
oMyGrid.ShowMiniTickLine = True
oMyGrid.Line.Color.ColorIndex = dd.eColorIndexDarkYellow
oMyGrid.MiniTickLine.Color.ColorIndex = dd.eColorIndexGreen

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniTickLine_IRepSpiderGridInt.htm`*
