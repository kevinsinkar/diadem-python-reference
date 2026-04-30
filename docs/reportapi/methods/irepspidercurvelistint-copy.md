---
title: "IRepSpiderCurveListInt.Copy"
description: "Copies a curve in a spider axis system in DIAdem REPORT and adds it to the spider axis system."
---

# IRepSpiderCurveListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for SpiderCurves

Copies a curve in a spider axis system in DIAdem REPORT and adds it to the spider axis system.

## Signature

```python
return_value = obj.Copy(NameOrIndex, NewName, InsertBeforeNameOrIndex)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider,"MySpiderAxisSystem")
oMyPosition = oMyAxisSys.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30

oMyCurve1 = oMyAxisSys.CurvesSpider.Add(dd.eSpiderShapeLine, "MyNewCurve1")
oMyCurve1.Shape.Channel.Reference= "[5]/[3]"
oMySpiderCurves = oMyAxisSys.CurvesSpider
oMyCurve2 = oMySpiderCurves.Copy("MyNewCurve1","NewCurve2",1)
print("Number of curves: " + oMySpiderCurves.Count)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepSpiderCurveListInt.htm`*
