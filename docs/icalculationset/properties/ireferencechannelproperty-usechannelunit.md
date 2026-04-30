---
title: "IReferenceChannelProperty.UseChannelUnit"
description: "Specifies whether DIAdem uses the unit of the channel or uses any unit, for the channel property with which DIAdem replaces an input or an output when DIAdem ex"
---

# IReferenceChannelProperty.UseChannelUnit

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: UseChannelUnit for ReferenceChannelProperty

Specifies whether DIAdem uses the unit of the channel or uses any unit, for the channel property with which DIAdem replaces an input or an output when DIAdem executes a calculation. If the input of the calculation is dependent on an output from another calculation, you cannot change the UseChannelUnit property.

## Signature

```python
obj.UseChannelUnit
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs("R")
if oMyInput.ReferenceType == dd.eReferenceTypeChannelProperty :
    oMyInput.Reference.Channel = "Revs"
    oMyInput.Reference.PropertyName = "Maximum"
    oMyInput.Reference.UseChannelUnit = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_UseChannelUnit_IReferenceChannelProperty.HTM`*
