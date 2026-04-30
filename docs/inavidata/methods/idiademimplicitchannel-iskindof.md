---
title: "IDiademImplicitChannel.IsKindOf"
description: "Checks the type of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.IsKindOf

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: IsKindOf for ImplicitChannel <Data>

Checks the type of an implicit channel in the script interface for internal data.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Python example

```python
oMyChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
if oMyChannel.IsKindOf(dd.eDataImplicitChannel) :
    dd.MsgBoxDisp("Implicit Channel")
else:
    dd.MsgBoxDisp("No Implicit Channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_IsKindOf_IDiademImplicitChannel.htm`*
