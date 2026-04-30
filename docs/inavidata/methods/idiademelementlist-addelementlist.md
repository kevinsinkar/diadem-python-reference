---
title: "IDiademElementList.AddElementList"
description: "Connects two element lists in the Script interface for internal data."
---

# IDiademElementList.AddElementList

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddElementList for ElementList <Data>

Connects two element lists in the Script interface for internal data.

## Signature

```python
obj.AddElementList(DataElementList, [ListMergeMode])
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyElementList1 = dd.Data.GetChannels("Example/1")
oMyElementList2 = dd.Data.GetChannels("Example/2")
oMyElementList1.AddElementList(oMyElementList2, dd.ListMergeModeAdd)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddElementList_IDiademElementList.htm`*
