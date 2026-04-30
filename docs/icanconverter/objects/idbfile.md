---
title: "IDbFile"
description: "The DbFile object provides the database file for a specific bus in the Bus Log Converter."
---

# IDbFile

!!! abstract "Object &middot; `ICANConverter.chm`"
    Object: DbFile

The DbFile object provides the database file for a specific bus in the Bus Log Converter.

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles.Item(1).File)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idbfile-clusters/">Clusters</a> | <a href="../../properties/idbfile-displayfile/">DisplayFile</a> | <a href="../../properties/idbfile-file/">File</a> | <a href="../../properties/idbfile-idmode/">IdMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/dbfiles/">DbFiles</a>.<a href="../../methods/idbfilecollection-add/">Add</a> | <a href="../../collections/dbfiles/">DbFiles</a>.<a href="../../methods/idbfilecollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IDbFile.htm`*
