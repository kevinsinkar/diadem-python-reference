---
title: "ICalculationSet.Copy"
description: "Copies a calculation or a calculation group within a calculation set. DIAdem assigns a new unique name to the copy. Note When copying, DIAdem also uses the inpu"
---

# ICalculationSet.Copy

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Copy for CalculationSet

Copies a calculation or a calculation group within a calculation set. DIAdem assigns a new unique name to the copy. Note When copying, DIAdem also uses the inputs and the outputs of the calculation. DIAdem copies an input including the dependencies of the input. If an output has dependent inputs, DIAdem creates a copy of the output without dependencies.

## Signature

```python
vCopy = Object.Copy(Source, Destination, [DestIndex])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  When copying, DIAdem also uses the inputs and the outputs of the calculation. DIAdem copies an input including the dependencies of the input. If an output has dependent inputs, DIAdem creates a copy of the output without dependencies.</td>
</tr>
</table>
</div>

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups(1).Calculations(1)
oMyNewCalc = dd.CalculationSet.Copy(oMyCalcTemp,dd.CalculationSet.CalculationGroups(3).Calculations,1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Copy_ICalculationSet.htm`*
