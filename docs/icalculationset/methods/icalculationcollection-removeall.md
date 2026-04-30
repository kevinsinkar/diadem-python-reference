---
title: "ICalculationCollection.RemoveAll"
description: "Deletes all calculations from the Calculations collection. In the existing calculation groups, DIAdem automatically removes the dependencies on the deleted outp"
---

# ICalculationCollection.RemoveAll

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: RemoveAll for Calculations

Deletes all calculations from the Calculations collection. In the existing calculation groups, DIAdem automatically removes the dependencies on the deleted outputs.

## Signature

```python
obj.RemoveAll
```

## Python example

```python
dd.CalculationSet.CalculationGroups(1).Calculations.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_RemoveAll_ICalculationCollection.htm`*
