---
title: "IDiademElementList.Item"
description: "Returns the ElementList object of a specific index in the script interface for internal data."
---

# IDiademElementList.Item

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Item for ElementList <Data>

Returns the ElementList object of a specific index in the script interface for internal data.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyChns = dd.Data.GetChannels("T*")
dd.MsgBoxDisp("Name of first channel: " + oMyChns.Item(1).Name)
dd.MsgBoxDisp("Name of first channel: " + oMyChns(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Item_IDiademElementList.HTM`*
