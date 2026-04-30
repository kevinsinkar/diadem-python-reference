---
title: "IReferenceChannelGroupProperty"
description: "The ReferenceChannelGroupProperty object provides a channel group property reference for an input or an output of a calculation. The channel group property refe"
---

# IReferenceChannelGroupProperty

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: ReferenceChannelGroupProperty

The ReferenceChannelGroupProperty object provides a channel group property reference for an input or an output of a calculation. The channel group property reference specifies which channel group property DIAdem uses for the execution of the calculation for the input or the output.

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeChannelGroupProperty
oMyInput.Reference.ChannelGroup = "Crash"
oMyInput.Reference.PropertyName = "Duration"
oMyInput.Reference.UnitSymbol = "ms"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireferencechannelgroupproperty-channelgroup/">ChannelGroup</a> | <a href="../../properties/ireferencechannelgroupproperty-parent/">Parent</a> | <a href="../../properties/ireferencechannelgroupproperty-propertyname/">PropertyName</a> | <a href="../../properties/ireferencechannelgroupproperty-unitpropertyname/">UnitPropertyName</a> | <a href="../../properties/ireferencechannelgroupproperty-unitsymbol/">UnitSymbol</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../iinput/">Input</a>.<a href="../../properties/iinput-reference/">Reference</a> | <a href="../ioutput/">Output</a>.<a href="../../properties/ioutput-reference/">Reference</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IReferenceChannelGroupProperty.htm`*
