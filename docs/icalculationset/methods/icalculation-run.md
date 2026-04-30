---
title: "ICalculation.Run"
description: "Executes a calculation. Use Validate to execute the validation script. If a calculation requires an output from an other calculation as an input, DIAdem first e"
---

# ICalculation.Run

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Run for Calculation

Executes a calculation. Use Validate to execute the validation script. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses this method to specify the sequence in which calculations are to be executed, and automatically expands the volume of calculations to be executed, if required. If DIAdem cannot clearly determine the calculation order, DIAdem displays an error message. DIAdem records the sequence of the executed calculations in the return value so that you can reproduce the calculation sequence. If an error occurs in a calculation during the calculation, the error message contains information about the incorrect calculation. The previously executed calculations remain.

## Signature

```python
return_value = obj.Run
```

## Python example

```python
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
if oMyCalc.Validate() :
    oMyCalc.Run()
else:
    dd.MsgBoxDisp("Error: "+oMyCalc.GetValidateMessage)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Run_ICalculation.htm`*
