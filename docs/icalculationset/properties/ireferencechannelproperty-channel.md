---
title: "IReferenceChannelProperty.Channel"
description: "Specifies the name of the Channel that contains the channel property with which DIAdem replaces an input or an output when a calculation is executed. You can ad"
---

# IReferenceChannelProperty.Channel

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Channel for ReferenceChannelProperty

Specifies the name of the Channel that contains the channel property with which DIAdem replaces an input or an output when a calculation is executed. You can add the contents of a DIAdem variable or a calculator expression to the channel name if you enclose the variable or the calculator expression in @@ characters. If the input of the calculation is dependent on an output from another calculation, you cannot change the Channel property.

## Signature

```python
obj.Channel
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs("R")
if oMyInput.ReferenceType == dd.eReferenceTypeChannelProperty :
    oMyInput.Reference.Channel = "Revs"
    oMyInput.Reference.PropertyName = "Maximum"
    oMyInput.Reference.UnitPropertyName = "unit_string"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Channel_IReferenceChannelProperty.htm`*
