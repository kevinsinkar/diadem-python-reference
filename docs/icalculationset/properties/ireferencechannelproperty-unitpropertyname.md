---
title: "IReferenceChannelProperty.UnitPropertyName"
description: "Specifies the name of an additional property of the channel for the channel group property reference that DIAdem uses to replace an input or an output when a ca"
---

# IReferenceChannelProperty.UnitPropertyName

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: UnitPropertyName for ReferenceChannelProperty

Specifies the name of an additional property of the channel for the channel group property reference that DIAdem uses to replace an input or an output when a calculation is executed. DIAdem takes from this channel property the unit of the value that is to be calculated, if the channel property reference replaces an input of the calculation. If the channel property reference replaces an output of the calculation, DIAdem saves the unit of the calculated value to this channel property. If you assign the UnitPropertyName property to the text "unit_string" , DIAdem converts the output value into the channel unit. You can add the contents of a DIAdem variable or a calculator expression to the channel property if you enclose the variable or the calculator expression in @@ characters. If you do not use a unit property, assign an empty string to the UnitPropertyName property. DIAdem specifies the unit via UnitSymbol . If the input of the calculation is dependent on an output from another calculation, you cannot change the UnitPropertyName property.

## Signature

```python
obj.UnitPropertyName
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs.Add("R",dd.eAdaptorTypeValue)
oMyOutput.ReferenceType = dd.eReferenceTypeChannelProperty
oMyOutput.Reference.Channel = "Revs"
oMyOutput.Reference.PropertyName = "Optimum"
oMyOutput.Reference.UnitPropertyName = "Optimum_unit"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_UnitPropertyName_IReferenceChannelProperty.htm`*
