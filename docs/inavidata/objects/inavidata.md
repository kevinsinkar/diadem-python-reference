---
title: "INaviData"
description: "The Data object accesses the internal DIAdem data. You use the Data object to generate, to edit, and to delete channel groups and channels with the associated p"
---

# INaviData

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: Data

The Data object accesses the internal DIAdem data. You use the Data object to generate, to edit, and to delete channel groups and channels with the associated properties. The Data object is available as a global object in scripts and in dialog boxes. Only read access.

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the commands <a href="../../../comoff/commands/datafileload/">DataFileLoad</a>, <a href="../../../comoff/commands/datafileloadred/">DataFileLoadRed</a>, and <a href="../../../comoff/commands/datafileloadsel/">DataFileLoadSel</a>, to load files into the internal DIAdem data store. Use the <a href="../../../scriptnavi/objects/inavigator/">Navigator</a>.<a href="../../../scriptnavi/methods/inavigator-loaddata/">LoadData</a> method to load data elements from the search results or from the file browser in DIAdem NAVIGATOR, into DIAdem.</td></tr></table>
<table class="Borderless" id="table3"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="./">Data</a>.<a href="../../properties/inavidata-root/">Root</a>.<a href="../../methods/idiademroot-clear/">Clear</a> method to delete data from the internal data store.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp (dd.Data.Root.Properties.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/inavidata-root/">Root</a> | <a href="../../properties/inavidata-settings/">Settings</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavidata-createelementlist/">CreateElementList</a> | <a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../methods/inavidata-getchannelgroups/">GetChannelGroups</a> | <a href="../../methods/inavidata-getchannels/">GetChannels</a> | <a href="../../methods/inavidata-move/">Move</a> | <a href="../../methods/inavidata-remove/">Remove</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_INaviData.htm`*
