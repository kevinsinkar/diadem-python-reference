---
title: "IToStringItemVecInt.Add"
description: "Adds a text to the StringVector collection in the Bus Log Converter ."
---

# IToStringItemVecInt.Add

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Add for StringVector

Adds a text to the StringVector collection in the Bus Log Converter .

## Signature

```python
obj.Add(Value)
```

## Python example

```python
oDbFile = dd.BusLogToTDM.BusDbConfig.Buses("CANBus").DbFiles.Add("D:\\Logfiles\\XNET_TDMS\\TDMS_Test.xml")
oDbFile.IdMode = dd.eDbFileIdModeDefault
oDbFile.Clusters.Add("HighBusLoad")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Add_IToStringItemVecInt.htm`*
