---
title: "ICalculationGroup"
description: "The CalculationGroup object provides a calculation group. The CalculationGroup object is an element of the CalculationGroups collection."
---

# ICalculationGroup

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: CalculationGroup

The CalculationGroup object provides a calculation group. The CalculationGroup object is an element of the CalculationGroups collection.

## Python example

```python
oMyCalcGroup = dd.CalculationSet.CalculationGroups.Add("Head_EuroNCAP")
oMyCalcGroup.Description = "Head Criterion - European Car Assessment Program"()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculationgroup-calculations/">Calculations</a> | <a href="../../properties/icalculationgroup-description/">Description</a> | <a href="../../properties/icalculationgroup-name/">Name</a> | <a href="../../properties/icalculationgroup-tag/">Tag</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculationgroup-selectall/">SelectAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../icalculation/">Calculation</a>.<a href="../../properties/icalculation-calculationgroup/">CalculationGroup</a> | <a href="../../collections/calculationgroups/">CalculationGroups</a>.<a href="../../methods/icalculationgroupcollection-add/">Add</a> | <a href="../../collections/calculationgroups/">CalculationGroups</a>.<a href="../../methods/icalculationgroupcollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculationGroup.htm`*
