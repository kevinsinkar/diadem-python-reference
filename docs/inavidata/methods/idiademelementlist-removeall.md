---
title: "IDiademElementList.RemoveAll"
description: "Deletes all elements from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is re"
---

# IDiademElementList.RemoveAll

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RemoveAll for ElementList <Data>

Deletes all elements from the ElementList collection in the script interface for internal data. This method is not available if the ElementList collection is read-only.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyChns = dd.Data.GetChannels("T*")
# futher instructions
oMyChns.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RemoveAll_IDiademElementList.HTM`*
