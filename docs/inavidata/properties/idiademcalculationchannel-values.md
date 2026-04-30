---
title: "IDiademCalculationChannel.Values"
description: "Specifies the single value of a calculation channel at a specific channel position in the script interface for internal data. You can only read the Values prope"
---

# IDiademCalculationChannel.Values

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Values for CalculationChannel <Data>

Specifies the single value of a calculation channel at a specific channel position in the script interface for internal data. You can only read the Values property.

## Signature

```python
obj.Values(Index)
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
print("First channel value: " , oMyCalculationChn.Values(1) , "\r\n" , "Second channel value: " , oMyCalculationChn.Values(2))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Values_IDiademCalculationChannel.htm`*
