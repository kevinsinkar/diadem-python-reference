---
title: "IBusCollection.Add"
description: "Use the AddByType instead of the Add method in order to add a bus to the Buses collection and to specify the bus type. Adds a bus to the Buses collection in the"
---

# IBusCollection.Add

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Add for Buses

Use the AddByType instead of the Add method in order to add a bus to the Buses collection and to specify the bus type. Adds a bus to the Buses collection in the Bus Log Converter .

## Signature

```python
return_value = obj.Add(Name, BusNumber)
```

## Python example

```python
dd.BusLogToTDM.Clear()
oMyBus = dd.BusLogToTDM.BusDbConfig.Buses.Add("NewCANBus",1)
dd.MsgBoxDisp (oMyBus.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Add_IBusCollection.htm`*
