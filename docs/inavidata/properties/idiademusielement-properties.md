---
title: "IDiademUSIElement.Properties"
description: "Contains the Properties collection that is associated with a ChannelGroup object in the script interface for internal data."
---

# IDiademUSIElement.Properties

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Properties for Element <Data>

Contains the Properties collection that is associated with a ChannelGroup object in the script interface for internal data.

## Signature

```python
return_value = obj.Properties
```

## Python example

```python
Dim
oMyElement
oMyElement = dd.Data.Root.ActiveChannelGroup.Channels(1)
dd.MsgBoxDisp (oMyElement.Properties(5).Name + " " +
oMyElement.Properties(5).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Properties_IDiademUSIElement.htm`*
