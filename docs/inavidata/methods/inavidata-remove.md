---
title: "INaviData.Remove"
description: "Deletes a list of elements from the Data Portal, in the script interface for internal data."
---

# INaviData.Remove

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Remove for Data

Deletes a list of elements from the Data Portal, in the script interface for internal data.

## Signature

```python
obj.Remove(ElementListToDelete)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>After deleting the list, DIAdem renumbers the channels in ascending order starting at one according to the Data Portal structure view.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm")
oMyAssgnList = dd.Data.GetChannels("S*")
dd.Data.Remove(oMyAssgnList)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Remove_INaviData.htm`*
