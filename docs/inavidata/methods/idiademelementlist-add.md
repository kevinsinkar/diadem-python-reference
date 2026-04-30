---
title: "IDiademElementList.Add"
description: "Creates a new element in the script interface for internal data and adds this element to the ElementList collection. The Add method returns an Element object. T"
---

# IDiademElementList.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for ElementList <Data>

Creates a new element in the script interface for internal data and adds this element to the ElementList collection. The Add method returns an Element object. This method is not available if the ElementList collection is read-only.

## Signature

```python
return_value = obj.Add(DataElement)
```

## Python example

```python
oMyChns = dd.Data.GetChannels("T*")
oMyChns.Add(dd.Data.Root.ChannelGroups(1).Channels("Speed"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IDiademElementList.HTM`*
