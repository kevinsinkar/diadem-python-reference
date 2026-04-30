---
title: "DbFiles"
description: "Collection of all the database files that are assigned to one bus in the Bus Log Converter . Every element in the DbFiles collection is a DbFile object ."
---

# DbFiles

!!! abstract "Collection &middot; `ICANConverter.chm`"
    Collection: DbFiles

Collection of all the database files that are assigned to one bus in the Bus Log Converter . Every element in the DbFiles collection is a DbFile object .

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idbfilecollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idbfilecollection-add/">Add</a> | <a href="../../methods/idbfilecollection-exists/">Exists</a> | <a href="../../methods/idbfilecollection-getindex/">GetIndex</a> | <a href="../../methods/idbfilecollection-item/">Item</a> | <a href="../../methods/idbfilecollection-move/">Move</a> | <a href="../../methods/idbfilecollection-remove/">Remove</a> | <a href="../../methods/idbfilecollection-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ibus/">Bus</a>.<a href="../../properties/ibus-dbfiles/">DbFiles</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IDbFileCollection.htm`*
