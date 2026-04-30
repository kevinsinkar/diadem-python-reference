---
title: "IInput.SourceOutput"
description: "Returns the Output object on which the input of a calculation is dependent."
---

# IInput.SourceOutput

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: SourceOutput for Input

Returns the Output object on which the input of a calculation is dependent.

## Signature

```python
return_value = obj.SourceOutput
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(2).Inputs(1)
if oMyInput.IsOutputConnected :
    dd.MsgBoxDisp("Output connected: " + oMyInput.SourceOutput.Calculation.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_SourceOutput_IInput.htm`*
