---
title: "ICalculation.Validate"
description: "Checks whether DIAdem can execute the calculation. DIAdem checks whether the input references and the output references of the calculation can be resolved. DIAd"
---

# ICalculation.Validate

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Validate for Calculation

Checks whether DIAdem can execute the calculation. DIAdem checks whether the input references and the output references of the calculation can be resolved. DIAdem also executes the Validation script , in which you can specify further conditions for the execution of the calculation. If the calculation expects input from the output of another calculation, DIAdem also checks this calculation. DIAdem checks in the required order of the execution. If DIAdem cannot determine the execution sequence, the calculation cannot be executed. If the calculation is incorrect, DIAdem neither outputs an error message nor aborts the executing script. If the test fails, the GetValidateMessage method contains the information about the error cause. Use the ValidateSelected method of the calculation set to execute the validation scripts of all selected calculations.

## Signature

```python
bValidate = Object.Validate
```

## Python example

```python
bNoErr = dd.CalculationSet.CalculationGroups(1).Calculations(1).Validate()
if not bNoErr :
    dd.MsgBoxDisp("Error: " + dd.CalculationSet.CalculationGroups(1).Calculations(1).GetValidateMessage())
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Validate_ICalculation.htm`*
