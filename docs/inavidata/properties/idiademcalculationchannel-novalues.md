---
title: "IDiademCalculationChannel.NoValues"
description: "Specifies whether a calculation channel contains NoValues. The value of the NoValues property for CalculationChannel is the same as the value of Value for Prope"
---

# IDiademCalculationChannel.NoValues

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: NoValues for CalculationChannel <Data>

Specifies whether a calculation channel contains NoValues. The value of the NoValues property for CalculationChannel is the same as the value of Value for Property <Data> with the property value noValuekey .

## Signature

```python
obj.NoValues
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTriStateFalse` | 0 | Does not contain NoValues |
| `eTriStateUnknown` | 1 | Unknown |

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
print(oMyCalculationChn.NoValues)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_NoValues_IDiademCalculationChannel.htm`*
