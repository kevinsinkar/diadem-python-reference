---
title: "IDiademChannels.AddCalculationChannelRef"
description: "Generates a new calculation channel with a reference to a calculation of the calculation manager in the script interface for internal data. Use the AddCalculati"
---

# IDiademChannels.AddCalculationChannelRef

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddCalculationChannelRef for Channels <Data>

Generates a new calculation channel with a reference to a calculation of the calculation manager in the script interface for internal data. Use the AddCalculationChannel method to create a new calculation channel using a simple one-line formula.

## Signature

```python
return_value = obj.AddCalculationChannelRef(CalculationReference, [DestIndex])
```

## Python example

```python
dd.CalculationSet.Load("Example.tca")
sMyCalculationReference = dd.CalculationSet.CalculationGroups(1).Calculations(1).GetReference()
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannelRef(sMyCalculationReference, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddCalculationChannelRef_IDiademChannels.htm`*
