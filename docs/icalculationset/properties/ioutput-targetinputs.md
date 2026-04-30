---
title: "IOutput.TargetInputs"
description: "Returns a collection of the Inputs that are dependent on a specific output of a calculation."
---

# IOutput.TargetInputs

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: TargetInputs for Output

Returns a collection of the Inputs that are dependent on a specific output of a calculation.

## Signature

```python
return_value = obj.TargetInputs
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs(1)
dd.MsgBoxDisp("No of inputs depending on output: " + oMyOutput.TargetInputs.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_TargetInputs_IOutput.htm`*
