---
title: "ICalculationSet.RunSelected"
description: "Executes selected calculations. The Selected property of a calculation specifies whether the calculation is selected. If a calculation requires an output from a"
---

# ICalculationSet.RunSelected

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: RunSelected for CalculationSet

Executes selected calculations. The Selected property of a calculation specifies whether the calculation is selected. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses this method to specify the sequence in which calculations are to be executed, and automatically expands the volume of calculations to be executed, if required. If DIAdem cannot clearly determine the calculation order, DIAdem displays an error message. DIAdem records the sequence of the executed calculations in the return value so that you can reproduce the calculation sequence. If an error occurs in a calculation during the calculation, the error message contains information about the incorrect calculation. The previously executed calculations remain. Use the Validate method of a calculation to execute the validation script of the respective calculation.

## Signature

```python
return_value = obj.RunSelected([FailedCalculations], [RunMode])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRunModeStopOnError` | 8 | DIAdem does not execute the subsequent calculations. The method aborts with an error message. |
| `eRunModeContinueOnError` | 16 | DIAdem executes the subsequent calculations. At the end the method outputs an error message that names all failed calculations. If you execute the method after On Error Resume Next , you can call the error status and obtain the list with failed calculations from the FailedCalculations parameter. |

## Python example

```python
oMyRunedCalculations = dd.CalculationSet.RunSelected
dd.MsgBoxDisp("First calculation: " + oMyRunedCalculations(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_RunSelected_ICalculationSet.htm`*
