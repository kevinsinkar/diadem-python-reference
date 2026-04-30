---
title: "IDiademCalculationChannel.QuantityBased"
description: "Specifies whether DIAdem calculates the calculation channel quantity-based in the script interface for internal data. You can only use the DestUnit property in "
---

# IDiademCalculationChannel.QuantityBased

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: QuantityBased for CalculationChannel <Data>

Specifies whether DIAdem calculates the calculation channel quantity-based in the script interface for internal data. You can only use the DestUnit property in a formula channel that you create with the AddCalculationChannel method. If you specify the "Default" value, DIAdem uses the default unit of the unit set of the result channel. If you specify a unit in the AddCalculationChannel for Channels <Data> method, DIAdem sets the QuantityBased for CalculationChannel <Data> to True and converts the unit to the specified unit. Refer to the Help page Calculating Quantity-Based and Non-Quantity-Based in DIAdem for the conditions and rules for quantity-based calculations.

## Signature

```python
obj.QuantityBased
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

*Source: `Inavidata/properties/DiaCmpnt_property_QuantityBased_IDiademCalculationChannel.htm`*
