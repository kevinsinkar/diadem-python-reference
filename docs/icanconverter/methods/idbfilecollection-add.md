---
title: "IDbFileCollection.Add"
description: "Adds a database file to the DbFiles collection in the Bus Logfile Converter ."
---

# IDbFileCollection.Add

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Add for DbFiles

Adds a database file to the DbFiles collection in the Bus Logfile Converter .

## Signature

```python
return_value = obj.Add(Name)
```

## Python example

```python
dd.BusLogToTDM.BusDBConfig.Buses("CAN1").DbFiles.Add("C:\\Accelerator.dbc")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Add_IDbFileCollection.htm`*
