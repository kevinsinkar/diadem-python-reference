---
title: "IReferenceDatasetProperty"
description: "The ReferenceDatasetProperty object provides a data set property reference for an input or an output of a calculation. The data set property reference specifies"
---

# IReferenceDatasetProperty

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: ReferenceDatasetProperty

The ReferenceDatasetProperty object provides a data set property reference for an input or an output of a calculation. The data set property reference specifies which data set property DIAdem uses for the execution of the calculation for the input or the output.

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeDatasetProperty
oMyInput.Reference.PropertyName = "Duration"
oMyInput.Reference.UnitSymbol = "s"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireferencedatasetproperty-parent/">Parent</a> | <a href="../../properties/ireferencedatasetproperty-propertyname/">PropertyName</a> | <a href="../../properties/ireferencedatasetproperty-unitpropertyname/">UnitPropertyName</a> | <a href="../../properties/ireferencedatasetproperty-unitsymbol/">UnitSymbol</a></p>
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

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IReferenceDatasetProperty.htm`*
