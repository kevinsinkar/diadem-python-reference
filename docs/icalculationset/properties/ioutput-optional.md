---
title: "IOutput.Optional"
description: "Specifies whether the output is an optional output. The channel that an optional output references only displays in the Data Portal if channel values are assign"
---

# IOutput.Optional

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Optional for Output

Specifies whether the output is an optional output. The channel that an optional output references only displays in the Data Portal if channel values are assigned to the channel during the calculation. If the optional channel references a non-existent channel in the Data Portal, DIAdem only generates this channel if you assign channel values to this channel during the calculation. If you only change the properties of the channel during the calculation, DIAdem does not generate this channel.

## Signature

```python
obj.Optional
```

## Python example

```python
oMyOutput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs.Add("R",dd.eAdaptorTypeChannel)
oMyOutput.Optional = True
oMyOutput.ReferenceType = dd.eReferenceTypeChannel
oMyOutput.Reference.Channel = "Revs"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Optional_IOutput.htm`*
