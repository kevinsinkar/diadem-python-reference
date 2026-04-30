---
title: "IDiademUSIElement.Name"
description: "Specifies the name of an element in the script interface for internal data. The element might be a root type, a channel group type, or a channel type."
---

# IDiademUSIElement.Name

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Name for Element <Data>

Specifies the name of an element in the script interface for internal data. The element might be a root type, a channel group type, or a channel type.

## Signature

```python
obj.Name
```

## Python example

```python
oMyElement = dd.Data.Root.ChannelGroups(1).Channels(1)
dd.MsgBoxDisp (oMyElement.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Name_IDiademUSIElement.htm`*
