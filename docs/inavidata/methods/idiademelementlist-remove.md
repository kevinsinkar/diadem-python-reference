---
title: "IDiademElementList.Remove"
description: "Deletes one element from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is rea"
---

# IDiademElementList.Remove

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Remove for ElementList <Data>

Deletes one element from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is read-only.

## Signature

```python
obj.Remove(Index)
```

## Python example

```python
oMyChns = dd.Data.GetChannels("T*")
for i in range( oMyChns.Count, 1+1, -1):
    if InStr(oMyChns(i).Name,"Temperature") :
        oMyChns.Remove(i)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Remove_IDiademElementList.HTM`*
