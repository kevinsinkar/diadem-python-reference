---
title: "InputList"
description: "Collection of all the Inputs that are dependent on an output of a calculation. This collection is not name oriented so that the collection can contain objects w"
---

# InputList

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: InputList

Collection of all the Inputs that are dependent on an output of a calculation. This collection is not name oriented so that the collection can contain objects with the same name. Use the Item method or specify the index in parenthesis to access an individual input in this collection in scripts. You cannot change the collection elements.

## Python example

```python
oMyDepInputs = dd.CalculationSet.CalculationGroups(1).Calculations(1).Outputs(1).TargetInputs
dd.MsgBoxDisp("No of inputs depending on output: " + oMyDepInputs.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iinputlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iinputlist-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ioutput/">Output</a>.<a href="../../properties/ioutput-targetinputs/">TargetInputs</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_IInputList.htm`*
