---
title: "IToStringItemVecInt.RemoveAll"
description: "Deletes all elements in the StringVector object in the Bus Log Converter ."
---

# IToStringItemVecInt.RemoveAll

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: RemoveAll for StringVector

Deletes all elements in the StringVector object in the Bus Log Converter .

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oDbFile = dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles(1)
oDbFile.Clusters.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_RemoveAll_IToStringItemVecInt.htm`*
