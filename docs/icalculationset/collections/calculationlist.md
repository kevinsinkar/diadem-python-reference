---
title: "CalculationList"
description: "Calculations collection. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses thi"
---

# CalculationList

!!! abstract "Collection &middot; `ICalculationSet.chm`"
    Collection: CalculationList

Calculations collection. If a calculation requires an output from an other calculation as an input, DIAdem first executes the other calculation. DIAdem uses this method to specify the sequence in which calculations are to be executed, and automatically expands the volume of calculations to be executed, if required. This collection is not name oriented so that the collection can contain objects with the same name. Use the Item method or specify the index in parenthesis to access an individual input in this collection in scripts. You cannot change the collection elements.

## Python example

```python
dd.CalculationSet.SelectAll(True)
oMyRunedCalculations = dd.CalculationSet.RunSelected()
dd.MsgBoxDisp("No of calculations: " + oMyRunedCalculations.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculationlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculationlist-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/icalculation/">Calculation</a>.<a href="../../methods/icalculation-getpostcalculations/">GetPostCalculations</a> | <a href="../../objects/icalculation/">Calculation</a>.<a href="../../methods/icalculation-getprecalculations/">GetPreCalculations</a> | <a href="../../objects/icalculation/">Calculation</a>.<a href="../../methods/icalculation-run/">Run</a> | <a href="../../objects/icalculationset/">CalculationSet</a>.<a href="../../methods/icalculationset-runselected/">RunSelected</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculationList.htm`*
