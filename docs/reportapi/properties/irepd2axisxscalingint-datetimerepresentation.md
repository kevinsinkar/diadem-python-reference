---
title: "IRepD2AxisXScalingInt.DateTimeRepresentation"
description: "Specifies whether the x-axis of a 2D axis system in DIAdem REPORT displays the time values as absolute or as relative time values."
---

# IRepD2AxisXScalingInt.DateTimeRepresentation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DateTimeRepresentation for 2DAxisXScaling

Specifies whether the x-axis of a 2D axis system in DIAdem REPORT displays the time values as absolute or as relative time values.

## Signature

```python
obj.DateTimeRepresentation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDateTimeRepresentationLegacy` | 0 | Compatible: DIAdem displays the time part of the waveform channels with a relative time axis. DIAdem displays all other time channels on an absolute time axis. |
| `eDateTimeRepresentationAbsolute` | 1 | Absolute: DIAdem displays the time part on an absolute time axis. |
| `eDateTimeRepresentationRelative` | 2 | Relative: DIAdem displays the time part on a relative time axis. DIAdem ignores the start times of all channels and plots the channels from the time zero. |
| `eDateTimeRepresentationRelativeWithOffset` | 3 | Relative with offset: DIAdem displays the time part with a relative time axis. DIAdem takes into account the relative start times of the channels. DIAdem plots the channel with the earliest start time from the time zero. If the time part of another channel begins later, DIAdem draws this channel with the corresponding offset on the time axis. |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByBorder
oMyPos.Left = 20
oMyPos.Bottom = 20
oMyPos.Right = 20
oMyPos.Top = 20
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyScaling = oMy2DAxisSystem.XAxis.Scaling
oMyScaling.Type = dd.e2DXScalingDateTime
oMyScaling.DateTimeRepresentation = eDateTimeRepresentationAutomatic
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DateTimeRepresentation_IRepD2AxisXScalingInt.htm`*
