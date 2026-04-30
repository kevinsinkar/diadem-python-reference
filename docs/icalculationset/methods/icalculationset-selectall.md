---
title: "ICalculationSet.SelectAll"
description: "Selects or deselects all calculations."
---

# ICalculationSet.SelectAll

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: SelectAll for CalculationSet

Selects or deselects all calculations.

## Signature

```python
obj.SelectAll(SelectValue)
```

## Python example

```python
dd.CalculationSet.SelectAll(False)
dd.CalculationSet.CalculationGroups("Crash").Calculations(1).Selected = True
dd.CalculationSet.CalculationGroups("Crash").Calculations(2).Selected = True
oMyRunedCalculations = dd.CalculationSet.RunSelected
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_SelectAll_ICalculationSet.htm`*
