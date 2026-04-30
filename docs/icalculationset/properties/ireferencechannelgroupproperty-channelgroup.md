---
title: "IReferenceChannelGroupProperty.ChannelGroup"
description: "Specifies the channel group of the channel group property with which DIAdem replaces an input or an output when a calculation is executed. If you assign an empt"
---

# IReferenceChannelGroupProperty.ChannelGroup

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: ChannelGroup for ReferenceChannelGroupProperty

Specifies the channel group of the channel group property with which DIAdem replaces an input or an output when a calculation is executed. If you assign an empty string or the character combination [] to the ChannelGroup property, DIAdem uses the default channel group. If you assign the character combination [n] to the ChannelGroup property, DIAdem uses the channel groups with the index n . You can add the contents of a DIAdem variable or a calculator expression to the channel group property if you enclose the variable or the calculator expression in @@ characters. If the input of the calculation is dependent on an output from another calculation, you cannot change the ChannelGroup property.

## Signature

```python
obj.ChannelGroup
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeChannelGroupProperty
oMyInput.Reference.ChannelGroup = "Crash"
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

*Source: `ICalculationSet/properties/FormulaCalc_property_ChannelGroup_IReferenceChannelGroupProperty.htm`*
