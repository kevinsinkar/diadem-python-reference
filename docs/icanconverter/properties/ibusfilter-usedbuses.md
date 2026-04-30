---
title: "IBusFilter.UsedBuses"
description: "Returns in the Bus Log Converter all buses the Bus Log Converter converts when the filter is active. You cannot overwrite the UsedBuses property."
---

# IBusFilter.UsedBuses

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: UsedBuses for BusFilter

Returns in the Bus Log Converter all buses the Bus Log Converter converts when the filter is active. You cannot overwrite the UsedBuses property.

## Signature

```python
return_value = obj.UsedBuses
```

## Python example

```python
oMyUsedBuses = dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses
dd.MsgBoxDisp(oMyUsedBuses.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_UsedBuses_IBusFilter.htm`*
