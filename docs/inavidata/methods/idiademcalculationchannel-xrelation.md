---
title: "IDiademCalculationChannel.XRelation"
description: "Specifies the x-channel for an xy-channel in the script interface for internal data. The x-channel must be in the same channel group as the y-channel."
---

# IDiademCalculationChannel.XRelation

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: XRelation for CalculationChannel <Data>

Specifies the x-channel for an xy-channel in the script interface for internal data. The x-channel must be in the same channel group as the y-channel.

## Signature

```python
return_value = obj.XRelation()
```

## Python example

```python
oMyChn = dd.Data.Root.ChannelGroups(1).Channels(2)
if (oMyChn.IsKindOf(dd.eDataCalculationChannel)) :
    oMyXChn = oMyChn.XRelation()
    print(oMyXChn.Name)
```

```python
oMyChnX = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyChnY = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyChnY.XRelation = oMyChnX
```

```python
oMyChnY = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyChnY.XRelation = None
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_XRelation_IDiademCalculationChannel.htm`*
