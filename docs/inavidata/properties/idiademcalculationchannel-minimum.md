---
title: "IDiademCalculationChannel.Minimum"
description: "Specifies the maximum of a calculation channel in the script interface for internal data. The value of the Minimum property for CalculationChannel is the same a"
---

# IDiademCalculationChannel.Minimum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Minimum for CalculationChannel <Data>

Specifies the maximum of a calculation channel in the script interface for internal data. The value of the Minimum property for CalculationChannel is the same as the value of Value for Property <Data> with the property value minimum .

## Signature

```python
obj.Minimum
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
print(oMyCalculationChn.Minimum)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Minimum_IDiademCalculationChannel.htm`*
