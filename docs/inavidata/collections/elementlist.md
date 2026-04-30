---
title: "ElementList"
description: "Collection of elements in the script interface for internal data. Use the ElementList collection to access channels, channel groups, or the root. You can add el"
---

# ElementList

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: ElementList <Data>

Collection of elements in the script interface for internal data. Use the ElementList collection to access channels, channel groups, or the root. You can add elements to the collection or remove elements from the collection. The data in the Data Portal remains unchanged. Every element of the collection ElementList is an Element .

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The commands <a href="../../../comoff/commands/datafileload/">DataFileLoad</a>, <a href="../../../comoff/commands/datafileloadred/">DataFileLoadRed</a>, <a href="../../../comoff/commands/datafileloadsel/">DataFileLoadSel</a>, and <a href="../../../comoff/commands/storageimport/">StorageImport</a> and the methods <a href="../../../scriptnavi/objects/inavigator/">Navigator</a>.<a href="../../../scriptnavi/methods/inavigator-loaddata/">LoadData</a> and <a href="../../../scriptnavi/objects/inavigator/">Navigator</a>.<a href="../../../scriptnavi/methods/inavigator-loadproperty/">LoadProperty</a> return an ElementList object.</td></tr></table>
</div>

## Python example

```python
oChn1 = dd.Data.GetChannel("[1]/Speed")
oChn2 = dd.Data.GetChannel("[1]/RPM")
oChnList = dd.Data.CreateElementList()

oChnList.Add(oChn1)
oChnList.Add(oChn2)

print(oChnList.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademelementlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../methods/idiademelementlist-addelementlist/">AddElementList</a> | <a href="../../methods/idiademelementlist-exists/">Exists</a> | <a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../../methods/idiademelementlist-remove/">Remove</a> | <a href="../../methods/idiademelementlist-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavidata/">Data</a>.<a href="../../methods/inavidata-createelementlist/">CreateElementList</a> | <a href="../../objects/inavidata/">Data</a>.<a href="../../methods/inavidata-getchannelgroups/">GetChannelGroups</a> | <a href="../../objects/inavidata/">Data</a>.<a href="../../methods/inavidata-getchannels/">GetChannels</a> | <a href="../../objects/idropinformation/">DropInformation</a>.<a href="../../properties/idropinformation-diademelements/">DiademElements</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademElementList.HTM`*
