---
title: "ICalculationSet.Append"
description: "Adds a calculation set file ( *.tca ) to the current calculation set. When name conflicts arise, DIAdem changes the names of the added calculation and calculati"
---

# ICalculationSet.Append

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Append for CalculationSet

Adds a calculation set file ( *.tca ) to the current calculation set. When name conflicts arise, DIAdem changes the names of the added calculation and calculation groups.

## Signature

```python
obj.Append(FileName)
```

## Python example

```python
dd.CalculationSet.Append("MyCalculationSet.tca")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Append_ICalculationSet.htm`*
