---
title: "IRepSpiderScalingInt.End"
description: "Specifies the value up to which DIAdem REPORT displays the axis of a spider axis system. DIAdem REPORT only includes the End property if you assign the value eA"
---

# IRepSpiderScalingInt.End

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: End for SpiderScaling

Specifies the value up to which DIAdem REPORT displays the axis of a spider axis system. DIAdem REPORT only includes the End property if you assign the value eAxisScalingManual to the AutoScalingType property.

## Signature

```python
obj.End
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

*Source: `ReportApi/properties/Report_property_End_IRepSpiderScalingInt.htm`*
