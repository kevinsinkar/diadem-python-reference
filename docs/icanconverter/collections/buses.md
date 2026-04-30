---
title: "Buses"
description: "Collection of all the buses that are entered in the logfiles and that the Bus Log Converter therefore includes in the conversion. You use the buses collection t"
---

# Buses

!!! abstract "Collection &middot; `ICANConverter.chm`"
    Collection: Buses

Collection of all the buses that are entered in the logfiles and that the Bus Log Converter therefore includes in the conversion. You use the buses collection to add new buses, or to delete or move buses. Every element in the buses collection is a Bus object .

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ibuscollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ibuscollection-add/">Add</a> | <a href="../../methods/ibuscollection-addbytype/">AddByType</a> | <a href="../../methods/ibuscollection-exists/">Exists</a> | <a href="../../methods/ibuscollection-existsbusno/">ExistsBusNo</a> | <a href="../../methods/ibuscollection-existsbusnobytype/">ExistsBusNoByType</a> | <a href="../../methods/ibuscollection-getindex/">GetIndex</a> | <a href="../../methods/ibuscollection-item/">Item</a> | <a href="../../methods/ibuscollection-move/">Move</a> | <a href="../../methods/ibuscollection-remove/">Remove</a> | <a href="../../methods/ibuscollection-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ibusdbconfig/">BusDbConfig</a>.<a href="../../properties/ibusdbconfig-buses/">Buses</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IBusCollection.htm`*
