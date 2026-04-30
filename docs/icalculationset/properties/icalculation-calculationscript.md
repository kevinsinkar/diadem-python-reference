---
title: "ICalculation.CalculationScript"
description: "Specifies the calculation script of a calculation. If the calculation is encrypted ( IsCrypted = TRUE ), you can neither change nor read out the CalculationScri"
---

# ICalculation.CalculationScript

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: CalculationScript for Calculation

Specifies the calculation script of a calculation. If the calculation is encrypted ( IsCrypted = TRUE ), you can neither change nor read out the CalculationScript property. You can use the names of the inputs and outputs in the calculation to access these inputs and outputs in the calculation script. A Value data type input or output corresponds to a value-unit object. A Channel data type input or output corresponds to a channel object, and a Channel list data type input or output corresponds to a channel list object. In calculation scripts the following variables are also available: This Calculation object of the calculation CurrSymbols Vector with the names of the inputs and outputs ( Value or Channel data type) CurrValues Vector with the values of the inputs and outputs ( Value or Channel data type) Use the variables CurrSymbols and CurrValues to configure the Calculate command. Note The calculation script is the same as the contents of a VBS procedure. You cannot define functions or procedures in a calculation script. For example, do not use Exit Sub or an error output to finish the script so that DIAdem can create the outputs correctly.

## Signature

```python
obj.CalculationScript
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>The calculation script is the same as the contents of a VBS procedure. You cannot define functions or procedures in a calculation script. For example, do not use <span class="Monospace">Exit Sub</span> or an error output to finish the script so that DIAdem can create the outputs correctly.</td>
</tr>
</table>
</div>

## Python example

```python
import math
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyCalc.CalculationScript = "Call ChnSum(Y,Z)" + "\r\n" + "Call ChnLinScale(Z,math.e,2,P)"
oMyCalc.Run()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_CalculationScript_ICalculation.htm`*
