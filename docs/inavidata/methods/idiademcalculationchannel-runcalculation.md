---
title: "IDiademCalculationChannel.RunCalculation"
description: "Runs a calculation in the script interface for internal data to determine the values of a calculation channel. When you create a calculation channel, DIAdem cal"
---

# IDiademCalculationChannel.RunCalculation

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RunCalculation for CalculationChannel <Data>

Runs a calculation in the script interface for internal data to determine the values of a calculation channel. When you create a calculation channel, DIAdem calculates the channel values automatically; you do not need to call the RunCalculation method. If the values of the channels in the calculation change, DIAdem updates the channel values when you restart the calculation using the RunCalculation method. If DIAdem cannot calculate the values of a calculation channel because, for example, an input channel is missing, DIAdem deletes all values and the unit of the calculation channel as soon as you update the values of this channel.

## Signature

```python
obj.RunCalculation()
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2",None , 1)
oMyCalculationChn.DestUnit = "m/s"
oMyCalculationChn.QuantityBased = True
#Changed input channel values or unit require a new calculation of the Calculation Channel
oMyCalculationChn.RunCalculation()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RunCalculation_IDiademCalculationChannel.htm`*
