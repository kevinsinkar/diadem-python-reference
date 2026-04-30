---
title: "IResultSettings.BusFilter"
description: "Specifies the settings for the bus filter in the Bus Log Converter . You cannot overwrite the BusFilter property."
---

# IResultSettings.BusFilter

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: BusFilter for ResultSettings

Specifies the settings for the bus filter in the Bus Log Converter . You cannot overwrite the BusFilter property.

## Signature

```python
return_value = obj.BusFilter
```

## Python example

```python
oMyBusFilter = dd.BusLogToTDM.ResultSettings.BusFilter
dd.MsgBoxDisp(oMyBusFilter.Active)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_BusFilter_IResultSettings.htm`*
