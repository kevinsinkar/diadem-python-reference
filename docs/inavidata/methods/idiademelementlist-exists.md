---
title: "IDiademElementList.Exists"
description: "Checks in the script interface for internal data whether a data element already exists. The Exists method checks when the data element first occurs in the eleme"
---

# IDiademElementList.Exists

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Exists for ElementList <Data>

Checks in the script interface for internal data whether a data element already exists. The Exists method checks when the data element first occurs in the elements list.

## Signature

```python
bExists = Object.Exists(Element)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You cannot use the <span class="Monospace">Exists</span> method with wildcards.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Crash.tdm")
oMyElementList = dd.Data.GetChannels("*")
if oMyElementList.Exists(dd.Data.Root.ChannelGroups(1).Channels("time")) :
    for I in range( 1, oMyElementList.Count+1):
        dd.MsgBoxDisp(oMyElementList.Item(I).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Exists_IDiademElementList.htm`*
