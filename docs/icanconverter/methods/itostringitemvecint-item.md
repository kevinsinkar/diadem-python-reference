---
title: "IToStringItemVecInt.Item"
description: "Specifies in the Bus Log Converter text associated to a specific index."
---

# IToStringItemVecInt.Item

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Item for StringVector

Specifies in the Bus Log Converter text associated to a specific index.

## Signature

```python
sItem = Object.Item(Index)
```

## Python example

```python
MyClusterName = dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles(1).Clusters.Item(1)
dd.MsgBoxDisp(MyClusterName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Item_IToStringItemVecInt.htm`*
