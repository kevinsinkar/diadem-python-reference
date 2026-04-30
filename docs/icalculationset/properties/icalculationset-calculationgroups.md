---
title: "ICalculationSet.CalculationGroups"
description: "Returns a collection of all the calculation groups of a calculation set. To access a single calculation group in scripts, either use the Item method or enter th"
---

# ICalculationSet.CalculationGroups

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: CalculationGroups for CalculationSet

Returns a collection of all the calculation groups of a calculation set. To access a single calculation group in scripts, either use the Item method or enter the index or the name in parentheses.

## Signature

```python
return_value = obj.CalculationGroups
```

## Python example

```python
dd.MsgBoxDisp("Number of calculation sets: " + dd.CalculationSet.CalculationGroups.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_CalculationGroups_ICalculationSet.htm`*
