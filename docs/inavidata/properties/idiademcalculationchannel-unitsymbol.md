---
title: "IDiademCalculationChannel.UnitSymbol"
description: "Specifies the unit symbol of a calculation channel. The value of the UnitSymbol property for CalculationChannel is the same as the value of Value for Property <"
---

# IDiademCalculationChannel.UnitSymbol

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: UnitSymbol for CalculationChannel <Data>

Specifies the unit symbol of a calculation channel. The value of the UnitSymbol property for CalculationChannel is the same as the value of Value for Property <Data> with the property value unit_string . Use the DestUnit for CalculationChannel property to specify the unit symbol of a calculation channel at the next refresh of the channel values with the RunCalculation method.

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
print(oMyCalculationChn.UnitSymbol) # equivalent to oMyChn.Properties("unit_string").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_UnitSymbol_IDiademCalculationChannel.htm`*
