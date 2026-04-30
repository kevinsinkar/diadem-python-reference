---
title: "ICalculationSet.ValidateSelected"
description: "Checks whether DIAdem can execute the selected calculations. The Selected property of a calculation specifies whether the calculation is selected. DIAdem checks"
---

# ICalculationSet.ValidateSelected

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: ValidateSelected for CalculationSet

Checks whether DIAdem can execute the selected calculations. The Selected property of a calculation specifies whether the calculation is selected. DIAdem checks whether the input references and the output references of each calculation can be removed. DIAdem also executes the Validation script in which you can specify further conditions for the execution of each calculation. If a calculation expects input from the output of another calculation, DIAdem also checks this calculation. DIAdem checks in the required order of the execution. If DIAdem cannot determine the execution sequence, the calculation cannot run. If the inspection fails, DIAdem writes the list of incorrect calculations in the FailedCalculations parameter. Use the Validate method of a calculation to execute the validation script of each calculation.

## Signature

```python
bValidateSelected = Object.ValidateSelected([FailedCalculations])
```

## Python example

```python
dd.CalculationSet.SelectAll(True)
if not dd.CalculationSet.ValidateSelected(oMyValidatedCalculations) :
    dd.MsgBoxDisp("Invalid calculation: " + oMyValidatedCalculations(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_ValidateSelected_ICalculationSet.htm`*
