---
title: "IInputCollection.Count"
description: "Returns the number of inputs in a calculation."
---

# IInputCollection.Count

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Count for Inputs

Returns the number of inputs in a calculation.

## Signature

```python
obj.Count
```

## Python example

```python
dd.MsgBoxDisp("Number of inputs: " + dd.CalculationSet.CalculationGroups("Custom").Calculations(1).Inputs.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Count_IInputCollection.htm`*
