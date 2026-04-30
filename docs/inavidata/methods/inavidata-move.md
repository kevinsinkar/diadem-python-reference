---
title: "INaviData.Move"
description: "Moves in the script interface for internal data a channel group or a channel to a different position in the Data Portal."
---

# INaviData.Move

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Move for Data

Moves in the script interface for internal data a channel group or a channel to a different position in the Data Portal.

## Signature

```python
obj.Move(Source, Destination, [DestIndex], [UseChnXRelations])
```

## Python example

```python
oMyChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyChannels = dd.Data.Root.ChannelGroups(2).Channels
dd.Data.Move(oMyChannel, oMyChannels, 2)
```

```python
oMyChannel1 = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyChannel2 = dd.Data.Root.ChannelGroups(2).Channels(1)
dd.Data.Move(oMyChannel1, oMyChannel2,None , True)
```

```python
oMyChannels = dd.Data.Root.ChannelGroups(1).Channels
oMyGroup    = dd.Data.Root.ChannelGroups(2)
oMyChnList  = dd.Data.CreateElementList()
for oMyChannel in oMyChannels:
    oMyChnList.Add(oMyChannel)
dd.Data.Move(oMyChnList, oMyGroup.Channels,None , True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Move_INaviData.htm`*
