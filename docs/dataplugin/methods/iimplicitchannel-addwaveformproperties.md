---
title: "IImplicitChannel.AddWaveformProperties"
description: "Adds waveform properties to the implicit channel to generate a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. Th"
---

# IImplicitChannel.AddWaveformProperties

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddWaveformProperties for ImplicitChannel

Adds waveform properties to the implicit channel to generate a waveform channel. Waveform channels contain the x-part and the y-part of a curve in a channel. The y-part contains the (measurement) values. The x-part might be the measured time. The Waveform properties specify the x-part that is a linear specification with a start value and a step width.

## Signature

```python
obj.AddWaveformProperties(Increment, StartOffset, [XChannelName], [XChannelUnit], [StartTime], [TimePreference], [NumberOfSamples])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTimeAbsolute` | 1 | Absolute time |
| `eTimeRelative` | 2 | Relative Time |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyChn.AddWaveformProperties(1, 0, "Time", "s")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddWaveformProperties_IImplicitChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
