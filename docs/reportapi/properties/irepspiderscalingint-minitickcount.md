---
title: "IRepSpiderScalingInt.MiniTickCount"
description: "Specifies the number of miniticks between the scale ticks on the axis in a spider axis system in DIAdem REPORT."
---

# IRepSpiderScalingInt.MiniTickCount

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniTickCount for SpiderScaling

Specifies the number of miniticks between the scale ticks on the axis in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.MiniTickCount
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MyAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyScaling = oMyAxisSystem.CategorySettings.Axis.Scaling
oMyScaling.Type = dd.eSpiderScalingLinear
oMyScaling.AutoScalingType = dd.eAxisScalingManual
oMyScaling.Begin = 10
oMyScaling.End = 20
oMyScaling.MiniTickCount = 5

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniTickCount_IRepSpiderScalingInt.htm`*
