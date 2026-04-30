---
title: "IToPolarChartInt.DateTimeRepresentation"
description: "DIAdem does not support this property at the moment. Specifies whether DIAdem VIEW displays time values as absolute or relative time values."
---

# IToPolarChartInt.DateTimeRepresentation

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: DateTimeRepresentation for Polar

DIAdem does not support this property at the moment. Specifies whether DIAdem VIEW displays time values as absolute or relative time values.

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_DateTimeRepresentation_IToPolarChartInt.htm`*
