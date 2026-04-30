---
title: "ICalculation.GetPostCalculations"
description: "Returns a collection with the calculations that DIAdem does not execute until DIAdem has executed the actual calculation. The dependencies and the execution seq"
---

# ICalculation.GetPostCalculations

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: GetPostCalculations for Calculation

Returns a collection with the calculations that DIAdem does not execute until DIAdem has executed the actual calculation. The dependencies and the execution sequence of the calculations result from the dependent inputs.

## Signature

```python
return_value = obj.GetPostCalculations
```

## Python example

```python
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyCalcList = oMyCalc.GetPreCalculations()
for oMyPostCalc in oMyCalcList:
    dd.MsgBoxDisp(oMyPostCalc.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_GetPostCalculations_ICalculation.htm`*
