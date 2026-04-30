---
title: "IDbFileCollection.Move"
description: "Moves a database file in the DbFiles collection to the specified position, in the Bus Log Converter ."
---

# IDbFileCollection.Move

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Move for DbFiles

Moves a database file in the DbFiles collection to the specified position, in the Bus Log Converter .

## Signature

```python
obj.Move(FromPosition, ToPosition)
```

## Python example

```python
dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles.Move(1,2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Move_IDbFileCollection.htm`*
