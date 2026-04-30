---
title: "ICANConverter.LogSettings"
description: "Specifies in the Bus Log Converter the logfiles to be converted and the type of these logfiles. You cannot overwrite the LogSettings property."
---

# ICANConverter.LogSettings

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: LogSettings for BusLogToTDM

Specifies in the Bus Log Converter the logfiles to be converted and the type of these logfiles. You cannot overwrite the LogSettings property.

## Signature

```python
return_value = obj.LogSettings
```

## Python example

```python
oMyLogSettings = dd.BusLogToTDM.LogSettings
dd.MsgBoxDisp(oMyLogSettings.FileType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_LogSettings_ICANConverter.htm`*
