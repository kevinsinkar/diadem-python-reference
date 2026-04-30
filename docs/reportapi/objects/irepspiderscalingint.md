---
title: "IRepSpiderScalingInt"
description: "The SpiderScaling object provides the scaling properties of the default axes of a spider axis system in DIAdem REPORT."
---

# IRepSpiderScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderScaling

The SpiderScaling object provides the scaling properties of the default axes of a spider axis system in DIAdem REPORT.

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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyScaling = oMyAxisSystem.CategorySettings.Axis.Scaling
oMyScaling.Type = dd.eSpiderScalingLinear
oMyScaling.AutoScalingType = dd.eAxisScalingManual
oMyScaling.Begin = 10
oMyScaling.End = 300
oMyScaling.MiniTickCount = 5

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspiderscalingint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/irepspiderscalingint-begin/">Begin</a> | <a href="../../properties/irepspiderscalingint-end/">End</a> | <a href="../../properties/irepspiderscalingint-minitickcount/">MiniTickCount</a> | <a href="../../properties/irepspiderscalingint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspideraxisint/">SpiderAxis</a>.<a href="../../properties/irepspideraxisint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderScalingInt.htm`*
