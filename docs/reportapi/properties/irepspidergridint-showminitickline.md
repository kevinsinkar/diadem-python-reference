---
title: "IRepSpiderGridInt.ShowMiniTickLine"
description: "Specifies whether DIAdem displays minitick lines in the grid of a spider axis system in DIAdem REPORT. Use the MiniTickLine property to define the lines. DIAdem"
---

# IRepSpiderGridInt.ShowMiniTickLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowMiniTickLine for SpiderGrid

Specifies whether DIAdem displays minitick lines in the grid of a spider axis system in DIAdem REPORT. Use the MiniTickLine property to define the lines. DIAdem REPORT only displays the lines if the property UseCategories has the value False .

## Signature

```python
obj.ShowMiniTickLine
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

*Source: `ReportApi/properties/Report_property_ShowMiniTickLine_IRepSpiderGridInt.htm`*
