---
title: "ICalculationSet.Move"
description: "Changes the position of a calculation in a calculation group or the position of a calculation group in a calculation set. If the change causes a name conflict, "
---

# ICalculationSet.Move

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Move for CalculationSet

Changes the position of a calculation in a calculation group or the position of a calculation group in a calculation set. If the change causes a name conflict, DIAdem automatically changes the name of the calculation or of the calculation group.

## Signature

```python
obj.Move(Source, Destination, [DestIndex])
```

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups(1)
dd.CalculationSet.Move(oMyCalcTemp,dd.CalculationSet.CalculationGroups,3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Move_ICalculationSet.htm`*
