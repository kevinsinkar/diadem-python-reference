---
title: "IRepSpiderGridInt"
description: "The SpiderGrid object provides the grid properties of a spider axis system in DIAdem REPORT."
---

# IRepSpiderGridInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderGrid

The SpiderGrid object provides the grid properties of a spider axis system in DIAdem REPORT.

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

oMyGrid = oMyAxisSystem.Settings.Grid
oMyGrid.ShowLine = True
oMyGrid.ShowMiniTickLine = True
oMyGrid.Line.Color.ColorIndex = dd.eColorIndexDarkYellow
oMyGrid.MiniTickLine.Color.ColorIndex = dd.eColorIndexGreen

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspidergridint-line/">Line</a> | <a href="../../properties/irepspidergridint-minitickline/">MiniTickLine</a> | <a href="../../properties/irepspidergridint-showline/">ShowLine</a> | <a href="../../properties/irepspidergridint-showminitickline/">ShowMiniTickLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidersettingsint/">SpiderSettings</a>.<a href="../../properties/irepspidersettingsint-grid/">Grid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderGridInt.htm`*
