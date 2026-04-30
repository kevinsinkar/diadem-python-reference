---
title: "IInput.Calculation"
description: "Returns the calculation to which the input is assigned."
---

# IInput.Calculation

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Calculation for Input

Returns the calculation to which the input is assigned.

## Signature

```python
return_value = obj.Calculation
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs(1)
for oMyInput in oMyOutput.TargetInputs:
    dd.MsgBoxDisp("Calculation = " + oMyInput.Calculation.Name + "/ Input = " + oMyInput.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Calculation_IInput.htm`*
