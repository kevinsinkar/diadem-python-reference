---
title: "IBusFilterBusCollection.GetIndex"
description: "Returns the index of a bus within the UsedBuses collection in the Bus Log Converter ."
---

# IBusFilterBusCollection.GetIndex

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: GetIndex for UsedBuses

Returns the index of a bus within the UsedBuses collection in the Bus Log Converter .

## Signature

```python
iGetIndex = Object.GetIndex(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses.GetIndex("CAN5"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_GetIndex_IBusFilterBusCollection.htm`*
