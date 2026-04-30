---
title: "IRepSpiderCurveListInt.Move"
description: "Moves a curve to a different position in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for SpiderCurves

Moves a curve to a different position in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Move(NameOrIndexFrom, NameOrIndexTo)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider,"MySpiderAxisSystem")
oMyPosition = oMyAxisSys.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 10
oMyPosition.Y2 = 40

oMyCurve1 = oMyAxisSys.CurvesSpider.Add(dd.eSpiderShapeLine, "MyNewCurve1")
oMyCurve1.Shape.Channel.Reference = "[5]/[3]"
oMyCurve2 = oMyAxisSys.CurvesSpider.Add(dd.eSpiderShapeLine, "MyNewCurve2")
oMyCurve2.Shape.Channel.Reference = "[5]/[4]"
oMySpiderCurves = oMyAxisSys.CurvesSpider
oMySpiderCurves.Move(1,2)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepSpiderCurveListInt.htm`*
