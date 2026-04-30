---
title: "IResultSettings.TimeFilter"
description: "Returns the settings for the time channels in the Bus Log Converter . You cannot overwrite the TimeFilter property."
---

# IResultSettings.TimeFilter

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: TimeFilter for ResultSettings

Returns the settings for the time channels in the Bus Log Converter . You cannot overwrite the TimeFilter property.

## Signature

```python
return_value = obj.TimeFilter
```

## Python example

```python
oMyResultSettings = dd.BusLogToTDM.ResultSettings
dd.MsgBoxDisp(oMyResultSettings.TimeFilter.Active)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_TimeFilter_IResultSettings.htm`*
