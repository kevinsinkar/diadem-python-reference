---
title: "IRepSpiderInt.UpdateScaling"
description: "Refreshes the values which DIAdem REPORT uses to automatically scale a spider axis system. You can use the values specified automatically, for example, for manu"
---

# IRepSpiderInt.UpdateScaling

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: UpdateScaling for Spider

Refreshes the values which DIAdem REPORT uses to automatically scale a spider axis system. You can use the values specified automatically, for example, for manual scaling.

## Signature

```python
obj.UpdateScaling()
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider,"MySpiderSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MyNewCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyScaling = oMyAxisSystem.CategorySettings.Axis.Scaling
oMyAxisSystem.UpdateScaling()
oMyScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyScaling.End = int(oMyScaling.End) + 1

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_UpdateScaling_IRepSpiderInt.htm`*
