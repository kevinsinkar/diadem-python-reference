---
title: "CalculationGroups"
description: "Collection of all Calculation groups in a calculation set. To access a single calculation group in scripts, either use the Item method or enter the index or the"
---

# CalculationGroups

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: CalculationGroups

Collection of all Calculation groups in a calculation set. To access a single calculation group in scripts, either use the Item method or enter the index or the name in parentheses.

## Python example

```python
for oMyCalcGroup in dd.CalculationSet.CalculationGroups:
    sText = sText + "Calculation Group : " + oMyCalcGroup.Name + "\r\n"
dd.MsgBoxDisp(sText)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculationgroupcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculationgroupcollection-add/">Add</a> | <a href="../../methods/icalculationgroupcollection-exists/">Exists</a> | <a href="../../methods/icalculationgroupcollection-getindex/">GetIndex</a> | <a href="../../methods/icalculationgroupcollection-item/">Item</a> | <a href="../../methods/icalculationgroupcollection-remove/">Remove</a> | <a href="../../methods/icalculationgroupcollection-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculationGroupCollection.htm`*
