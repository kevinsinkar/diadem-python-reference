---
title: "IDbFileCollection.Exists"
description: "Checks in the Bus Log Converter whether a database file with a specific name already exists for a bus."
---

# IDbFileCollection.Exists

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Exists for DbFiles

Checks in the Bus Log Converter whether a database file with a specific name already exists for a bus.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses("CAN1").DbFiles.Exists("C:\\CAN1.ncd"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Exists_IDbFileCollection.htm`*
