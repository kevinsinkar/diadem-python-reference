---
title: "IDiademAssignmentChannel.ValueIndex"
description: "Determines the row in an assignment channel with contents closest to a given value."
---

# IDiademAssignmentChannel.ValueIndex

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ValueIndex for AssignmentChannel <Data>

Determines the row in an assignment channel with contents closest to a given value.

## Signature

```python
obj.ValueIndex(ValueToSearch)
```

## Python example

```python
oMyChn = dd.Data.Root.ChannelGroups("Group1").Channels("Input")
intMyResult = oMyChn.ValueIndex(77)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ValueIndex_IDiademAssignmentChannel.htm`*
