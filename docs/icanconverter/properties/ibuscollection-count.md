---
title: "IBusCollection.Count"
description: "Specifies the number of buses to be converted in the Bus Log Converter . You cannot overwrite the Count property."
---

# IBusCollection.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for Buses

Specifies the number of buses to be converted in the Bus Log Converter . You cannot overwrite the Count property.

## Signature

```python
obj.Count
```

## Python example

```python
oMyBuses = dd.BusLogToTDM.BusDbConfig.Buses
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

*Source: `ICANConverter/properties/CANConverter_property_Count_IBusCollection.htm`*
