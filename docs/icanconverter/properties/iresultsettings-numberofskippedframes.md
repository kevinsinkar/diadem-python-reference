---
title: "IResultSettings.NumberOfSkippedFrames"
description: "Specifies the number of frames at the beginning, which the Bus Log Converter ignores when converting."
---

# IResultSettings.NumberOfSkippedFrames

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: NumberOfSkippedFrames for ResultSettings

Specifies the number of frames at the beginning, which the Bus Log Converter ignores when converting.

## Signature

```python
obj.NumberOfSkippedFrames
```

## Python example

```python
if dd.BusLogToTDM.ResultSettings.SkipFirstFrames :
    dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.NumberOfSkippedFrames)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_NumberOfSkippedFrames_IResultSettings.htm`*
