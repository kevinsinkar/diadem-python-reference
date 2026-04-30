---
title: "IRepPolarAxisScalingInt.DateTimeRepresentation"
description: "Specifies whether the radial axis of a Polar axis system in DIAdem REPORT displays the time values as obsolute or as relative time values."
---

# IRepPolarAxisScalingInt.DateTimeRepresentation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DateTimeRepresentation for PolarAxisScaling

Specifies whether the radial axis of a Polar axis system in DIAdem REPORT displays the time values as obsolute or as relative time values.

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
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[2]"
oMyCurve.Shape.YChannel.Reference = "[1]/[1]"
oMyPolarAxisSystem.RadialAxis.Scaling.Type =dd.ePolarScalingDateTime
oMyPolarAxisSystem.RadialAxis.Scaling.DateTimeRepresentation = eDateTimeRepresentationAutomatic
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DateTimeRepresentation_IRepPolarAxisScalingInt.htm`*
