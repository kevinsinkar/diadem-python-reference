---
title: "IInput.Optional"
description: "Specifies whether the input is an optional input. If DIAdem cannot resolve the reference of an optional input, DIAdem assigns the Empty variable contents to thi"
---

# IInput.Optional

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Optional for Input

Specifies whether the input is an optional input. If DIAdem cannot resolve the reference of an optional input, DIAdem assigns the Empty variable contents to this input. This prevents an error occurring when DIAdem checks whether a calculation can be executed.

## Signature

```python
obj.Optional
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.Optional = True
oMyInput.ReferenceType = dd.eReferenceTypeValue
oMyInput.Reference.ValueExpression = "R1"
oMyInput.Reference.UnitSymbol = "mm"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Optional_IInput.htm`*
