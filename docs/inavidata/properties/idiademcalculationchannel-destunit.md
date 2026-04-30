---
title: "IDiademCalculationChannel.DestUnit"
description: "Specifies the unit symbol of a formula channel at the next refresh of the channel values with the RunCalculation method in the script interface for internal dat"
---

# IDiademCalculationChannel.DestUnit

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DestUnit for CalculationChannel <Data>

Specifies the unit symbol of a formula channel at the next refresh of the channel values with the RunCalculation method in the script interface for internal data. You can only use the DestUnit property in a formula channel that you create with the AddCalculationChannel method. If you specify the "Default" value, DIAdem uses the matching default unit of the active unit set for the result channel. If you specify a unit in the AddCalculationChannel for Channels <Data> method, DIAdem sets the QuantityBased for CalculationChannel <Data> to True and converts the unit to the specified unit. If you specify an empty string as unit symbol, DIAdem specifies the unit symbol. Use the UnitSymbol for CalculationChannel property to determine the current unit symbol of a calculation channel. Refer to the Help page Calculating Quantity-Based and Non-Quantity-Based in DIAdem for the conditions and rules for quantity-based calculations.

## Signature

```python
obj.DestUnit
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.Channelgroups(1).Channels.AddCalculationChannel("Result", "= Speed * 2","m/s", 1)
dd.LogFileWrite(oMyCalculationChn.DestUnit)
dd.LogFileWrite(oMyCalculationChn.QuantityBased)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DestUnit_IDiademCalculationChannel.htm`*
