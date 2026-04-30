---
title: "IReferenceValue.ValueExpression"
description: "Specifies the expression with which DIAdem replaces an input or an output when a calculation is executed. You can use a numeric value or a variable name as the "
---

# IReferenceValue.ValueExpression

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: ValueExpression for ReferenceValue

Specifies the expression with which DIAdem replaces an input or an output when a calculation is executed. You can use a numeric value or a variable name as the expression. If the input of the calculation is dependent on an output from another calculation, you cannot change the ValueExpression property.

## Signature

```python
obj.ValueExpression
```

## Python example

```python
oMyInput = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Add("R",dd.eAdaptorTypeValue)
oMyInput.ReferenceType = dd.eReferenceTypeValue
oMyInput.Reference.ValueExpression = "1.23"
oMyInput.Reference.UnitSymbol = "mm"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_ValueExpression_IReferenceValue.htm`*
