---
title: "IBusFilterBusCollection.Count"
description: "Specifies the number of buses that the Bus Log Converter still converts when the filter is active, in the Bus Log Converter . You cannot overwrite the Count pro"
---

# IBusFilterBusCollection.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for UsedBuses

Specifies the number of buses that the Bus Log Converter still converts when the filter is active, in the Bus Log Converter . You cannot overwrite the Count property.

## Signature

```python
obj.Count
```

## Python example

```python
oMyBuses = dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses
for i in range(1, oMyBuses.Count+1):
    dd.MsgBoxDisp(oMyBuses(i).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Count_IBusFilterBusCollection.htm`*
