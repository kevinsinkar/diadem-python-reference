---
title: "IToStringItemVecInt.Count"
description: "Counts the clusters or XNET channels contained in a string vector in the Bus Log Converter ."
---

# IToStringItemVecInt.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for StringVector

Counts the clusters or XNET channels contained in a string vector in the Bus Log Converter .

## Signature

```python
obj.Count
```

## Python example

```python
oDbFile = dd.BusLogToTDM.BusDbConfig.Buses("CANBus").DbFiles.Add("D:\\Logfiles\\XNET_TDMS\\TDMS_Test.xml")
oDbFile.IdMode = dd.eDbFileIdModeDefault
oDbFile.Clusters.Add("HighBusLoad")
dd.MsgBoxDisp(oDbFile.Clusters.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Count_IToStringItemVecInt.htm`*
