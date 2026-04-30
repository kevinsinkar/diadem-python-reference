---
title: "IDiademProperty.Element"
description: "Specifies in the script interface for internal data the element to which a property belongs. The element might be a root type, a channel group type, or a channe"
---

# IDiademProperty.Element

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Element for Property <Data>

Specifies in the script interface for internal data the element to which a property belongs. The element might be a root type, a channel group type, or a channel type.

## Signature

```python
return_value = obj.Element
```

## Python example

```python
oMyChannelProperty = dd.Data.Root.ChannelGroups(1).Channels(1).Properties(2)
dd.MsgBoxDisp(oMyChannelProperty.Element.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Element_IDiademProperty.htm`*
