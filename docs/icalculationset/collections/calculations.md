---
title: "Calculations"
description: "Collection of all Calculations of a calculation group. To access an individual calculation in a script use the Item method or enter the index or the name in par"
---

# Calculations

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: Calculations

Collection of all Calculations of a calculation group. To access an individual calculation in a script use the Item method or enter the index or the name in parentheses.

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups(1).Calculations
for oMyCalc in oMyCalcTemp:
    dd.MsgBoxDisp("Name of calculation: " + oMyCalc.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculationcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculationcollection-add/">Add</a> | <a href="../../methods/icalculationcollection-exists/">Exists</a> | <a href="../../methods/icalculationcollection-getindex/">GetIndex</a> | <a href="../../methods/icalculationcollection-item/">Item</a> | <a href="../../methods/icalculationcollection-remove/">Remove</a> | <a href="../../methods/icalculationcollection-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculationCollection.htm`*
