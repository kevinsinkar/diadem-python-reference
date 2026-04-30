---
title: "IDiademImplicitChannel.OperationalFlags"
description: "Specifies whether DIAdem assigns a flag to the value of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.OperationalFlags

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: OperationalFlags for ImplicitChannel <Data>

Specifies whether DIAdem assigns a flag to the value of an implicit channel in the script interface for internal data.

## Signature

```python
obj.OperationalFlags(Index)
```

## Python example

```python
oMyImplChn = dd.Data.Root.ActiveChannelGroup.Channels(1)
oMyImplChn.OperationalFlags[1] = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_OperationalFlags_IDiademImplicitChannel.htm`*
