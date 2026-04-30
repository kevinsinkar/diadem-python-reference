---
title: "IReferenceDatasetProperty.PropertyName"
description: "Specifies the name of the data set property with which DIAdem replaces an input or an output when a calculation is executed. You can add the contents of a DIAde"
---

# IReferenceDatasetProperty.PropertyName

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: PropertyName for ReferenceDatasetProperty

Specifies the name of the data set property with which DIAdem replaces an input or an output when a calculation is executed. You can add the contents of a DIAdem variable or a calculator expression to the channel group property if you enclose the variable or the calculator expression in @@ characters. If the input of the calculation is dependent on an output from another calculation, you cannot change the PropertyName property.

## Signature

```python
obj.PropertyName
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeDatasetProperty
oMyInput.Reference.PropertyName = "Duration"
oMyInput.Reference.UnitSymbol = "ms"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_PropertyName_IReferenceDatasetProperty.htm`*
