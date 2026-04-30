---
title: "ICalculation.GetPreCalculations"
description: "Returns a collection with the calculations that DIAdem executes in the specified order before executing the actual calculation. If DIAdem cannot clearly determi"
---

# ICalculation.GetPreCalculations

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: GetPreCalculations for Calculation

Returns a collection with the calculations that DIAdem executes in the specified order before executing the actual calculation. If DIAdem cannot clearly determine the calculation order, DIAdem displays an error message. The dependencies and the execution sequence of the calculations result from the dependent inputs.

## Signature

```python
return_value = obj.GetPreCalculations
```

## Python example

```python
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyCalcList = oMyCalc.GetPreCalculations()
for oMyPreCalc in oMyCalcList:
    dd.MsgBoxDisp(oMyPreCalc.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_GetPreCalculations_ICalculation.htm`*
