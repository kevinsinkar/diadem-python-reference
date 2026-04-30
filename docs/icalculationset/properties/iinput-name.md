---
title: "IInput.Name"
description: "Specifies the name of the input of a calculation. The name must conform to the naming conventions for calculations. If the name does not conform to the name con"
---

# IInput.Name

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Name for Input

Specifies the name of the input of a calculation. The name must conform to the naming conventions for calculations. If the name does not conform to the name conventions, DIAdem corrects the name.

## Signature

```python
obj.Name
```

## Python example

```python
oMyInputs = dd.CalculationSet.CalculationGroups("Custom").Calculations(1).Inputs
for I in range( 1, oMyInputs.Count+1):
    dd.MsgBoxDisp("Name: " + oMyInputs(i).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Name_IInput.htm`*
