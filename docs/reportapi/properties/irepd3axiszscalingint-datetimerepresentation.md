---
title: "IRepD3AxisZScalingInt.DateTimeRepresentation"
description: "Specifies whether the z-axis of a 3D axis system in DIAdem REPORT displays the time values as obsolute or as relative time values."
---

# IRepD3AxisZScalingInt.DateTimeRepresentation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DateTimeRepresentation for 3DAxisZScaling

Specifies whether the z-axis of a 3D axis system in DIAdem REPORT displays the time values as obsolute or as relative time values.

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
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMyXScaling = oMy3DAxisSystem.AxisList.X.Scaling
oMyXScaling.Type = dd.e3DScalingDateTime
oMyXScaling.DateTimeRepresentation = eDateTimeRepresentationAutomatic
oMyYScaling = oMy3DAxisSystem.AxisList.X.Scaling
oMyYScaling.Type = dd.e3DScalingDateTime
oMyYScaling.DateTimeRepresentation = eDateTimeRepresentationAutomatic
oMyZScaling = oMy3DAxisSystem.AxisList.X.Scaling
oMyZScaling.Type = dd.e3DScalingDateTime
oMyZScaling.DateTimeRepresentation = eDateTimeRepresentationAutomatic
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DateTimeRepresentation_IRepD3AxisZScalingInt.htm`*
