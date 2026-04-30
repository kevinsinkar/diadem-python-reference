---
title: "IBusFilterBusCollection.Exists"
description: "Checks in the Bus Log Converter whether a bus with a specific name already exists in the filtered bus collection."
---

# IBusFilterBusCollection.Exists

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Exists for UsedBuses

Checks in the Bus Log Converter whether a bus with a specific name already exists in the filtered bus collection.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses.Exists("CAN3"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Exists_IBusFilterBusCollection.htm`*
