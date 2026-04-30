---
title: "ICalculationList.Count"
description: "Returns the number of calculations that are executed during a calculation sequence, or are put before or after a calculation sequence. If a calculation requires"
---

# ICalculationList.Count

!!! abstract "Property &middot; `ICalculationSet.chm`"
    Property: Count for CalculationList

Returns the number of calculations that are executed during a calculation sequence, or are put before or after a calculation sequence. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses this method to specify the sequence in which calculations are to be executed, and automatically expands the volume of calculations to be executed, if required.

## Signature

```python
obj.Count
```

## Python example

```python
dd.CalculationSet.SelectAll(False)
dd.CalculationSet.CalculationGroups("Custom").Calculations(1).Selected = True
dd.CalculationSet.CalculationGroups("Custom").Calculations(2).Selected = True
oMyRunedCalculations = dd.CalculationSet.RunSelected
dd.MsgBoxDisp("No of calculations: " + oMyRunedCalculations.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/properties/FormulaCalc_property_Count_ICalculationList.htm`*
