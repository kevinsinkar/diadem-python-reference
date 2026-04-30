---
title: "StringVector"
description: "The StringVector object provides clusters or XNET channels in the Bus Log Converter ."
---

# StringVector

!!! abstract "Collection &middot; `ICANConverter.chm`"
    Collection: StringVector

The StringVector object provides clusters or XNET channels in the Bus Log Converter .

## Python example

```python
oDbFile = dd.BusLogToTDM.BusDbConfig.Buses("CANBus").DbFiles.Add("D:\\Logfiles\\XNET_TDMS\\TDMS_01.xml")
oDbFile.IdMode = dd.eDbFileIdModeDefault
oDbFile.Clusters.Add("HighBusLoad")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itostringitemvecint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itostringitemvecint-add/">Add</a> | <a href="../../methods/itostringitemvecint-item/">Item</a> | <a href="../../methods/itostringitemvecint-remove/">Remove</a> | <a href="../../methods/itostringitemvecint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idbfile/">DbFile</a>.<a href="../../properties/idbfile-clusters/">Clusters</a> | <a href="../../objects/ilogfile/">LogFile</a>.<a href="../../properties/ilogfile-xnettdmschannels/">XnetTdmsChannels</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IToStringItemVecInt.htm`*
