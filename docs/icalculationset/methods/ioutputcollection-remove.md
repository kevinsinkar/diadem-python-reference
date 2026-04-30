---
title: "IOutputCollection.Remove"
description: "Deletes an output from the Outputs collection of a calculation. In the existing calculations, DIAdem automatically removes the dependencies of the inputs on the"
---

# IOutputCollection.Remove

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Remove for Outputs

Deletes an output from the Outputs collection of a calculation. In the existing calculations, DIAdem automatically removes the dependencies of the inputs on the deleted output.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyCalcOutputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs
if oMyCalcOutputs.Exists("R") :
    oMyCalcOutputs.Remove("R")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Remove_IOutputCollection.htm`*
