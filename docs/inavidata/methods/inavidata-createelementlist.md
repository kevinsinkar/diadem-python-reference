---
title: "INaviData.CreateElementList"
description: "Generates in the script interface for internal data a collection of elements. Every element from the generated collection is an Element and thus can be a root t"
---

# INaviData.CreateElementList

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: CreateElementList for Data

Generates in the script interface for internal data a collection of elements. Every element from the generated collection is an Element and thus can be a root type (eDataRoot), a channel group type (eDataChannelgroup), or a channel type (eDataChannel).

## Signature

```python
return_value = obj.CreateElementList()
```

## Python example

```python
oMyElementList = dd.Data.CreateElementList()
oMyChannelgroups = dd.Data.Root.ChannelGroups
for Channelgroup in oMyChannelgroups:
    oMyElementList.Add(Channelgroup)
    oMyChannels = Channelgroup.Channels
    for Channel in oMyChannels:
        oMyElementList.Add(Channel)
dd.MsgBoxDisp(oMyElementList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_CreateElementList_INaviData.htm`*
