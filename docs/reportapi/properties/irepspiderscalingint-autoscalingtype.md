---
title: "IRepSpiderScalingInt.AutoScalingType"
description: "Specifies whether DIAdem REPORT scales the axis of a spider axis system automatically."
---

# IRepSpiderScalingInt.AutoScalingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AutoScalingType for SpiderScaling

Specifies whether DIAdem REPORT scales the axis of a spider axis system automatically.

## Signature

```python
obj.AutoScalingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisScalingManual` | 0 | Manual |
| `eAxisScalingCompleteAutomatic` | 1 | Automatic |

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
oMyScaling.End = 20
oMyScaling.MiniTickCount = 5

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AutoScalingType_IRepSpiderScalingInt.htm`*
