---
title: "ICalculation.RunParametrized"
description: "Executes the calculation without resolving the references of the inputs and outputs. Instead, the method uses the contents of the vectors that are specified as "
---

# ICalculation.RunParametrized

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: RunParametrized for Calculation

Executes the calculation without resolving the references of the inputs and outputs. Instead, the method uses the contents of the vectors that are specified as parameters. The vectors are assigned to the inputs or to the outputs via the name specified in Symbols when the index is the same. The Values vector can contain value-unit objects ( Value data type), channel objects ( Channel data type), and channel object collections ( Channel list data type). Ensure that the object type specified in Values matches the data type of the input or output that the data type Symbols references. Use the ValidateParametrized method to execute the configured validation script.

## Signature

```python
obj.RunParametrized(Symbols, Values)
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

*Source: `ICalculationSet/methods/FormulaCalc_method_RunParametrized_ICalculation.htm`*
