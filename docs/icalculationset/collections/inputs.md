---
title: "Inputs"
description: "Collection of all Inputs of a calculation. To access an individual input in scripts, use the Item method, or enter the index or the name in parentheses."
---

# Inputs

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: Inputs

Collection of all Inputs of a calculation. To access an individual input in scripts, use the Item method, or enter the index or the name in parentheses.

## Python example

```python
oMyCalcInputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs
for oMyInput in oMyCalcInputs:
    dd.MsgBoxDisp("Name of input: " + oMyInput.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iinputcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iinputcollection-add/">Add</a> | <a href="../../methods/iinputcollection-addbyoutput/">AddByOutput</a> | <a href="../../methods/iinputcollection-exists/">Exists</a> | <a href="../../methods/iinputcollection-item/">Item</a> | <a href="../../methods/iinputcollection-move/">Move</a> | <a href="../../methods/iinputcollection-remove/">Remove</a> | <a href="../../methods/iinputcollection-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IInputCollection.htm`*
