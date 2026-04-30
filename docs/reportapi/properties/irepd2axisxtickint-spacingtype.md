---
title: "IRepD2AxisXTickInt.SpacingType"
description: "Specifies whether DIAdem REPORT takes the positions of the scaling ticks of the x-axis from a data channel or calculates the positions automatically."
---

# IRepD2AxisXTickInt.SpacingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SpacingType for 2DAxisXTick

Specifies whether DIAdem REPORT takes the positions of the scaling ticks of the x-axis from a data channel or calculates the positions automatically.

## Signature

```python
obj.SpacingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisTickSpacingDefinedByDistance` | 0 | Calculated from tick distance |
| `eAxisTickSpacingReadFromChannel` | 1 | Read from tick channel |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyXScaling.Type = dd.e2DXScalingLinear
oMyXScaling.Begin = 0
oMyXScaling.End = 4
oMyXScaling.Tick.SpacingType = dd.eAxisTickSpacingReadFromChannel
oMyXScaling.Tick.Channel.Reference = "[6]/[3]"
oMyXScaling.MiniTickCount = 10
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingManual
oMyYScaling.Type = dd.e2DYScalingLinear
oMyYScaling.Begin = 0
oMyYScaling.End = 4
oMyYScaling.Tick.SpacingType = dd.eAxisTickSpacingReadFromChannel
oMyYScaling.Tick.Channel.Reference = "[6]/[3]"
oMyYScaling.MiniTickCount = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SpacingType_IRepD2AxisXTickInt.htm`*
