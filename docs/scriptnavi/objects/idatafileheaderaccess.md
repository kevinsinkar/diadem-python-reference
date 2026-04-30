---
title: "IDataFileHeaderAccess"
description: "The DataFileHeaderAccess object provides access to an ASAM data store, which you can use to read, write, modify, or delete channel properties, group properties,"
---

# IDataFileHeaderAccess

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: DataFileHeaderAccess

The DataFileHeaderAccess object provides access to an ASAM data store, which you can use to read, write, modify, or delete channel properties, group properties, or file properties from TDM files or TDMS files.

## Python example

```python
oMyDataFileHeaderAccess = CreateDataFileHeaderAccess
oMyDataStore            = oMyDataFileHeaderAccess.Open(dd.DataReadPath + "Example.tdm" ,"TDM", False)
print(oMyDataStore.RootElements(1).Children(1).Children(2).Name)
```

## Members

<div markdown="1">
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatafileheaderaccess-open/">Open</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataFileHeaderAccess.htm`*
