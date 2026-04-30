---
title: "IDbFile.Clusters"
description: "Specifies one or several clusters in a Fibex database file in the Bus Log Converter ."
---

# IDbFile.Clusters

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Clusters for DbFile

Specifies one or several clusters in a Fibex database file in the Bus Log Converter .

## Signature

```python
return_value = obj.Clusters
```

## Python example

```python
oDbFile = dd.BusLogToTDM.BusDbConfig.Buses("CANBus").DbFiles.Add("D:\\ConfigFiles\\TDMS_01.xml")
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

*Source: `ICANConverter/properties/CANConverter_property_Clusters_IDbFile.htm`*
