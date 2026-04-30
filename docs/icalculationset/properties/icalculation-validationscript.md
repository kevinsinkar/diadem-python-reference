---
title: "ICalculation.ValidationScript"
description: "Specifies the validation script of a calculation. If the calculation is encrypted ( IsCrypted = TRUE ), you can neither change nor read out the ValidationScript"
---

# ICalculation.ValidationScript

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: ValidationScript for Calculation

Specifies the validation script of a calculation. If the calculation is encrypted ( IsCrypted = TRUE ), you can neither change nor read out the ValidationScript property. You can use the names of the non-dependent inputs in the calculation to access these inputs in the validation script. In validation scripts the following variables are also available: This Calculation object of the calculation Failed Return value that contains a message if the test failed. Note The validation script is the same as the contents of a VBS procedure. You cannot define functions or procedures in a validation script. Do not use Exit Sub or an error output to finish the script so that DIAdem can process the test correctly.

## Signature

```python
obj.ValidationScript
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>The validation script is the same as the contents of a VBS procedure. You cannot define functions or procedures in a validation script. Do not use <span class="Monospace">Exit Sub</span> or an error output to finish the script so that DIAdem can process the test correctly.</td>
</tr>
</table>
</div>

## Python example

```python
oMyCalc = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyCalc.ValidationScript = "If N.Size>0 Then" + "\r\n" + " Failed = \"Channel not None\"" + "\r\n" + "End If"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_ValidationScript_ICalculation.htm`*
