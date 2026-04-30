---
title: "IInputCollection.Remove"
description: "Deletes an input from the Inputs collection of a calculation."
---

# IInputCollection.Remove

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Remove for Inputs

Deletes an input from the Inputs collection of a calculation.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyCalcInputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs
if oMyCalcInputs.Exists("X") :
    oMyCalcInputs.Remove("X")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Remove_IInputCollection.htm`*
