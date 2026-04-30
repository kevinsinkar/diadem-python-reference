---
title: "ICalculation.QuantityBased"
description: "Specifies whether a calculation is Quantity-based . Note The setting of the QuantityBased property, not the setting in DIAdem ANALYSIS, specifies how the calcul"
---

# ICalculation.QuantityBased

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: QuantityBased for Calculation

Specifies whether a calculation is Quantity-based . Note The setting of the QuantityBased property, not the setting in DIAdem ANALYSIS, specifies how the calculation acts during execution.

## Signature

```python
obj.QuantityBased
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>The setting of the <span class="Monospace">QuantityBased</span> property, not the setting in DIAdem ANALYSIS, specifies how the calculation acts during execution.</td>
</tr>
</table>
</div>

## Python example

```python
dd.CalculationSet.CalculationGroups("Crash").Calculations(1).QuantityBased = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_QuantityBased_ICalculation.htm`*
