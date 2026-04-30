---
title: "ICANConverter.ResultSettings"
description: "Returns the settings for the conversion results in the Bus Log Converter . You cannot overwrite the ResultSettings property."
---

# ICANConverter.ResultSettings

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: ResultSettings for BusLogToTDM

Returns the settings for the conversion results in the Bus Log Converter . You cannot overwrite the ResultSettings property.

## Signature

```python
return_value = obj.ResultSettings
```

## Python example

```python
oMyBusFilter = dd.BusLogToTDM.ResultSettings
dd.MsgBoxDisp(oMyBusFilter.ResultFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_ResultSettings_ICANConverter.htm`*
