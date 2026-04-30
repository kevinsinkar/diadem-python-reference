---
title: "IDiademCalculationChannel.CalculationReference"
description: "Specifies a reference string associated with a Calculation Manager calculation in the calculation group/calculation format, in the script interface for internal"
---

# IDiademCalculationChannel.CalculationReference

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: CalculationReference for CalculationChannel <Data>

Specifies a reference string associated with a Calculation Manager calculation in the calculation group/calculation format, in the script interface for internal data.

## Signature

```python
obj.CalculationReference
```

## Python example

```python
dd.CalculationSet.Load("Example.tca")
sMyCalculationReference = dd.CalculationSet.CalculationGroups(1).Calculations(1).GetReference()
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel(sMyCalculationReference, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_CalculationReference_IDiademCalculationChannel.htm`*
