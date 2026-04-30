---
title: "IDiademImplicitChannel.DataType"
description: "Specifies the data type of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.DataType

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DataType for ImplicitChannel <Data>

Specifies the data type of an implicit channel in the script interface for internal data.

## Signature

```python
obj.DataType
```

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    if (oMyChn.IsKindOf(dd.eImplicit)) :
        dd.MsgBoxDisp("Channel name: " + oMyChn.Name + "\r\n" + "Data type: " + oMyChn.DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DataType_IDiademImplicitChannel.htm`*
