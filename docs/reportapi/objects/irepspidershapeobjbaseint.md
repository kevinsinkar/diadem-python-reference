---
title: "IRepSpiderShapeObjBaseInt"
description: "The SpiderShapeObject object provides the curve properties of a spider axis system in DIAdem REPORT. The SpiderShapeObject object corresponds to one of the foll"
---

# IRepSpiderShapeObjBaseInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderShapeObject

The SpiderShapeObject object provides the curve properties of a spider axis system in DIAdem REPORT. The SpiderShapeObject object corresponds to one of the following objects:

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

oMySpiderSettings = oMyAxisSystem.Settings
oMySpiderSettings.DisplayMode = dd.eSpiderDisplayModeSpider
oMySpiderSettings.ShowBorder = True
oMySpiderSettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
oMySpiderSettings.BackgroundColor.ColorIndex = dd.eColorIndexYellow
oMySpiderSettings.AngleDirection = dd.eAngleDirectionClockwise

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="ReturnFrom">
<h2>Returned From</h2>
<p><a href="../irepspidercurveint/">SpiderCurve</a>.<a href="../../properties/irepspidercurveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderShapeObjBaseInt.htm`*
