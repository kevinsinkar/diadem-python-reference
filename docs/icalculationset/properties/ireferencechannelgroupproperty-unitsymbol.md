---
title: "IReferenceChannelGroupProperty.UnitSymbol"
description: "Specifies the unit symbol of the channel group property with which DIAdem replaces an output or input when DIAdem executes a calculation, when the UnitPropertyN"
---

# IReferenceChannelGroupProperty.UnitSymbol

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: UnitSymbol for ReferenceChannelGroupProperty

Specifies the unit symbol of the channel group property with which DIAdem replaces an output or input when DIAdem executes a calculation, when the UnitPropertyName property contains an empty string. At an input DIAdem assigns the default unit symbol to the numeric value and assigns it to a unit. At an output DIAdem converts the value into the default unit and uses the resulting numeric value. If you assign an empty string to the UnitSymbol property, the unit of the input is undefined. At an output DIAdem uses the numeric value unchanged. You can add the contents of a DIAdem variable or a calculator expression to the unit symbol if you enclose the variable or the calculator expression in @@ characters. If the input of the calculation is dependent on an output from another calculation, you cannot change the UnitSymbol property.

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeChannelGroupProperty
oMyInput.Reference.ChannelGroup = "Crash"
oMyInput.Reference.PropertyName = "Duration"
oMyInput.Reference.UnitPropertyName = ""
oMyInput.Reference.UnitSymbol = "ms"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_UnitSymbol_IReferenceChannelGroupProperty.htm`*
