---
title: "ICalculation.ValidateParametrized"
description: "Checks the calculation without resolving the input and output references and executes the Validation script . Instead of the input and output references, the me"
---

# ICalculation.ValidateParametrized

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: ValidateParametrized for Calculation

Checks the calculation without resolving the input and output references and executes the Validation script . Instead of the input and output references, the method uses the vector contents that are specified as parameters. The vectors are assigned to the inputs or to the outputs via the name specified in Symbols when the index is the same. The Values vector can contain value-unit objects ( Value data type), channel objects ( Channel data type), and channel object collections ( Channel list data type). Ensure that the object type specified in Values matches the data type of the input or output that the data type Symbols references. Use the RunParametrized method to execute the configured calculation script.

## Signature

```python
bValidateParametrized = Object.ValidateParametrized(Symbols, Values)
```

## Python example

```python
oMySymbols = []
oMySymbols.append("A")
oMyValues = []
oMyValues.append(dd.CreateValueWithUnit(2,""))
oMySymbols = []
oMySymbols.append("B")
oMyValues = []
oMyValues.append(dd.CreateValueWithUnit(3,""))
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
if oMyCalc.ValidateParametrized(oMySymbols,oMyValues) :
    oMyCalc.RunParametrized(oMySymbols,oMyValues)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_ValidateParametrized_ICalculation.htm`*
