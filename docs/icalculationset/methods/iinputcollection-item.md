---
title: "IInputCollection.Item"
description: "Returns the Input object associated with a specific name or with a specific index."
---

# IInputCollection.Item

!!! abstract "Method &middot; `ICalculationSet.chm`"
    Method: Item for Inputs

Returns the Input object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp("Name of first input: " + dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs.Item(1).Name)
dd.MsgBoxDisp("Name of first input: " + dd.CalculationSet.CalculationGroups(1).Calculations(1).Inputs(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/methods/FormulaCalc_method_Item_IInputCollection.htm`*
