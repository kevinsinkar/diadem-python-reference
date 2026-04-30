---
title: "IDiademImplicitChannel.IsReadOnly"
description: "Specifies whether an implicit channel is read-only."
---

# IDiademImplicitChannel.IsReadOnly

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: IsReadOnly for ImplicitChannel <Data>

Specifies whether an implicit channel is read-only.

## Signature

```python
obj.IsReadOnly
```

## Python example

```python
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
dd.MsgBoxDisp(oMyImplChannel.IsReadOnly)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_IsReadOnly_IDiademImplicitChannel.htm`*
