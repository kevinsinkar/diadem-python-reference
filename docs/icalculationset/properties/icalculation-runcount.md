---
title: "ICalculation.RunCount"
description: "Specifies the number of cycles for a calculation. Instead of a number, you also can assign a variable name, such as Data.Root.ChannelGroups.Count , to this prop"
---

# ICalculation.RunCount

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: RunCount for Calculation

Specifies the number of cycles for a calculation. Instead of a number, you also can assign a variable name, such as Data.Root.ChannelGroups.Count , to this property. If you execute more than one cycle for a calculation, use expressions with @@ CCR @@ in the references of the inputs and/or outputs. This gives you variable inputs or variable outputs. If you define a calculation with two cycles and the reference "[1]/Cycle_@@CCR@@" for an input channel, for example, DIAdem adds the current increment number to the channel name during each calculation cycle. DIAdem executes the respective cycle when the corresponding channel is in the Data Portal. Otherwise, DIAdem skips this cycle. If the Data Portal does not contain a corresponding channel in any cycle, DIAdem displays an error message.

## Signature

```python
obj.RunCount
```

## Python example

```python
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyCalc.RunCount = 2
oMyCalc.Inputs(1).Reference.Channel = "[1]/Cycle_@@CCR@@"
oMyCalc.Run()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_RunCount_ICalculation.htm`*
