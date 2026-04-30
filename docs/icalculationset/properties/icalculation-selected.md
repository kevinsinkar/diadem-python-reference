---
title: "ICalculation.Selected"
description: "Specifies whether a calculation is selected. You can select the calculation with the Selected property, with the SelectAll method of the CalculationGroup object"
---

# ICalculation.Selected

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Selected for Calculation

Specifies whether a calculation is selected. You can select the calculation with the Selected property, with the SelectAll method of the CalculationGroup object, or with the SelectAll method of the CalculationSet object.

## Signature

```python
obj.Selected
```

## Python example

```python
dd.CalculationSet.CalculationGroups("Crash").SelectAll(False)
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

*Source: `ICalculationSet/properties/FormulaCalc_property_Selected_ICalculation.htm`*
