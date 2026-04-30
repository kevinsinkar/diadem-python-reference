---
title: "INaviData.GetChannel"
description: "Returns a channel in the script interface for internal data."
---

# INaviData.GetChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetChannel for Data

Returns a channel in the script interface for internal data.

## Signature

```python
return_value = obj.GetChannel(Reference)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <span class="Monospace">GetChannel</span> method to create data objects from channel references, for example, from layout configurations and then to continue processing the data using the script interface for internal data.</td></tr></table>
</div>

## Python example

```python
oMyChn = dd.Data.GetChannel("[1]/[1]")
dd.MsgBoxDisp (oMyChn.Name)
```

```python
oMyChn = dd.Data.GetChannel("Example/D*")
dd.MsgBoxDisp(oMyChn.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Related Functions</h2><p class="Body"><a href="../inavidata-getchannelgroups/">GetChannelGroups</a> | <a href="../inavidata-getchannels/">GetChannels</a></p>
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetChannel_INaviData.HTM`*
