---
title: "IDbFileCollection.GetIndex"
description: "Returns the index of a database file from the DbFiles collection in the Bus Log Converter ."
---

# IDbFileCollection.GetIndex

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: GetIndex for DbFiles

Returns the index of a database file from the DbFiles collection in the Bus Log Converter .

## Signature

```python
iGetIndex = Object.GetIndex(Name)
```

## Python example

```python
print(dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles.GetIndex("C:\\Accelerator.dbc"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_GetIndex_IDbFileCollection.htm`*
