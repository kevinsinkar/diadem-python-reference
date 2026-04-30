---
title: "ICalculation.Outputs"
description: "Provides the collection of all outputs of a calculation."
---

# ICalculation.Outputs

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Outputs for Calculation

Provides the collection of all outputs of a calculation.

## Signature

```python
return_value = obj.Outputs
```

## Python example

```python
oMyCalcOutputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs
for i in range( 1, oMyCalcOutputs.Count+1):
    dd.MsgBoxDisp("Name of output: " + oMyCalcOutputs(i).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Outputs_ICalculation.htm`*
