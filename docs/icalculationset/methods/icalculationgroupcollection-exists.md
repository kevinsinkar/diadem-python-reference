---
title: "ICalculationGroupCollection.Exists"
description: "Checks whether a calculation group with a specific name exists."
---

# ICalculationGroupCollection.Exists

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Exists for CalculationGroups

Checks whether a calculation group with a specific name exists.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
if not dd.CalculationSet.CalculationGroups.Exists("Custom") :
    dd.CalculationSet.CalculationGroups.Add("Custom")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Exists_ICalculationGroupCollection.htm`*
