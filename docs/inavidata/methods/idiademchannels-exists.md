---
title: "IDiademChannels.Exists"
description: "Checks whether a Channel object with a specific name already exists in the Channels <Data> collection in the script interface for internal data. The Channels <D"
---

# IDiademChannels.Exists

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Exists for Channels <Data>

Checks whether a Channel object with a specific name already exists in the Channels <Data> collection in the script interface for internal data. The Channels <Data> collection contains all channels of a channel group.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oGrp = dd.Data.Root.ChannelGroups(1)
if oGrp.Channels.Exists("FirstChannel") :
    oGrp.Channels.Add("SecondChannel", dd.DataTypeFloat64)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Exists_IDiademChannels.HTM`*
