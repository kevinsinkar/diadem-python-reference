---
title: "IDiademCalculationChannel.ChannelGroup"
description: "Specifies the channel group which contains a specific calculation channel in the script interface for internal data."
---

# IDiademCalculationChannel.ChannelGroup

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelGroup for CalculationChannel <Data>

Specifies the channel group which contains a specific calculation channel in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelGroup
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel(sMyCalculationReference, 1)
print(oMyCalculationChn.ChannelGroup)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelGroup_IDiademCalculationChannel.htm`*
