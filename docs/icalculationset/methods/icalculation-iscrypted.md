---
title: "ICalculation.IsCrypted"
description: "Specifies whether the calculation is encrypted. If the calculation is encrypted, you cannot view or edit formulas and scripts. However, you can execute the calc"
---

# ICalculation.IsCrypted

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: IsCrypted for Calculation

Specifies whether the calculation is encrypted. If the calculation is encrypted, you cannot view or edit formulas and scripts. However, you can execute the calculation.

## Signature

```python
bIsCrypted = Object.IsCrypted
```

## Python example

```python
if dd.CalculationSet.CalculationGroups(1).Calculations(1).IsCrypted :
    dd.MsgBoxDisp("Calculation has been crypted")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_IsCrypted_ICalculation.htm`*
