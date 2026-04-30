---
title: "IRepD2AxisYScalingInt.AutoScalingType"
description: "Specifies whether and how DIAdem REPORT scales the y-axis of the 2D axis system."
---

# IRepD2AxisYScalingInt.AutoScalingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AutoScalingType for 2DAxisYScaling

Specifies whether and how DIAdem REPORT scales the y-axis of the 2D axis system.

## Signature

```python
obj.AutoScalingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisAutoScalingManual` | 0 | Manual |
| `eAxisAutoScalingCompleteAutomatic` | 1 | Fully automatic |
| `eAxisAutoScalingBeginEndManual` | 2 | Begin/end manual |
| `eAxisAutoScalingSpanWidthTickManual` | 3 | Range and ticks manual |
| `eAxisAutoScalingTickManual` | 4 | Ticks manual |
| `eAxisAutoScalingBeginTickManual` | 5 | Begin and ticks manual |
| `eAxisAutoScalingCustom` | 6 | User-defined axis scaling |
| `eAxisAutoScalingBeginManualEndAutomatic` | 7 | Manual begin and automatic end |
| `eAxisAutoScalingBeginAutomaticEndManual` | 8 | Automatic begin and manual end |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyXScaling.Type = dd.e2DXScalingLogarithmic
oMyXScaling.Begin = 0.01
oMyXScaling.End = 100
oMyXScaling.Origin = 1
oMyXScaling.Tick.Distance = 1
oMyXScaling.MiniTickCount = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.Begin = 0
oMyYScaling.End = 100
oMyYScaling.Origin = 50
oMyYScaling.Tick.Distance = 12.5
oMyYScaling.MiniTickCount = 10
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AutoScalingType_IRepD2AxisYScalingInt.htm`*
