---
title: "Outputs"
description: "Collection of all Outputs of a calculation. To access an individual output in scripts, use the Item method, or enter the index or the name in parentheses."
---

# Outputs

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: Outputs

Collection of all Outputs of a calculation. To access an individual output in scripts, use the Item method, or enter the index or the name in parentheses.

## Python example

```python
oMyCalcOutputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs
for oMyOutput in oMyCalcOutputs:
    dd.MsgBoxDisp("Name of output: " + oMyOutput.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ioutputcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ioutputcollection-add/">Add</a> | <a href="../../methods/ioutputcollection-exists/">Exists</a> | <a href="../../methods/ioutputcollection-item/">Item</a> | <a href="../../methods/ioutputcollection-move/">Move</a> | <a href="../../methods/ioutputcollection-remove/">Remove</a> | <a href="../../methods/ioutputcollection-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IOutputCollection.htm`*
