---
title: "IReferenceDatasetProperty.UnitPropertyName"
description: "Specifies for the data set property reference that DIAdem uses to replace an input or an output when a calculation is executed, the name of an additional proper"
---

# IReferenceDatasetProperty.UnitPropertyName

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: UnitPropertyName for ReferenceDatasetProperty

Specifies for the data set property reference that DIAdem uses to replace an input or an output when a calculation is executed, the name of an additional property of the data set. DIAdem takes from this data set property the unit of the value that is to be calculated, if the data set property reference replaces an input of the calculation. If the data set property reference replaces an output of the calculation, DIAdem saves the unit of the calculated value to this data set property. You can add the contents of a DIAdem variable or a calculator expression to the data set property if you enclose the variable or the calculator expression in @@ characters. If you do not use a unit property, assign an empty string to the UnitPropertyName property. DIAdem specifies the unit via UnitSymbol . If the input of the calculation is dependent on an output from another calculation, you cannot change the UnitPropertyName property.

## Signature

```python
obj.UnitPropertyName
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs.Add("R",dd.eAdaptorTypeValue)
oMyOutput.ReferenceType = dd.eReferenceTypeDatasetProperty
oMyOutput.Reference.PropertyName = "Duration"
oMyOutput.Reference.UnitPropertyName = "Duration_unit"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_UnitPropertyName_IReferenceDatasetProperty.htm`*
