---
title: "IOutputCollection.Exists"
description: "Checks whether a calculation contains an output with a specific name."
---

# IOutputCollection.Exists

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Exists for Outputs

Checks whether a calculation contains an output with a specific name.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups("Custom").Calculations(1)
if not oMyCalcTemp.Outputs.Exists("R") :
    oMyCalcTemp.Outputs.Add("R", dd.eAdaptorTypeChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Exists_IOutputCollection.htm`*
