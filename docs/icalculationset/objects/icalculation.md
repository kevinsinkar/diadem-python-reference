---
title: "ICalculation"
description: "The Calculation object provides a calculation. The Calculation object is an element of the Calculations collection."
---

# ICalculation

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: Calculation

The Calculation object provides a calculation. The Calculation object is an element of the Calculations collection.

## Python example

```python
oMyCalcTemp = dd.CalculationSet.CalculationGroups(1).Calculations.Add("Resultant")
oMyCalcTemp.Description = "Resultant of Head Acceleration"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculation-calculationgroup/">CalculationGroup</a> | <a href="../../properties/icalculation-calculationscript/">CalculationScript</a> | <a href="../../properties/icalculation-description/">Description</a> | <a href="../../properties/icalculation-inputs/">Inputs</a> | <a href="../../properties/icalculation-name/">Name</a> | <a href="../../properties/icalculation-outputs/">Outputs</a> | <a href="../../properties/icalculation-quantitybased/">QuantityBased</a> | <a href="../../properties/icalculation-runcount/">RunCount</a> | <a href="../../properties/icalculation-selected/">Selected</a> | <a href="../../properties/icalculation-tag/">Tag</a> | <a href="../../properties/icalculation-validationscript/">ValidationScript</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculation-getpostcalculations/">GetPostCalculations</a> | <a href="../../methods/icalculation-getprecalculations/">GetPreCalculations</a> | <a href="../../methods/icalculation-getvalidatemessage/">GetValidateMessage</a> | <a href="../../methods/icalculation-iscrypted/">IsCrypted</a> | <a href="../../methods/icalculation-run/">Run</a> | <a href="../../methods/icalculation-runparametrized/">RunParametrized</a> | <a href="../../methods/icalculation-validate/">Validate</a> | <a href="../../methods/icalculation-validateparametrized/">ValidateParametrized</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/calculationlist/">CalculationList</a>.<a href="../../methods/icalculationlist-item/">Item</a> | <a href="../../collections/calculations/">Calculations</a>.<a href="../../methods/icalculationcollection-add/">Add</a> | <a href="../../collections/calculations/">Calculations</a>.<a href="../../methods/icalculationcollection-item/">Item</a> | <a href="../iinput/">Input</a>.<a href="../../properties/iinput-calculation/">Calculation</a> | <a href="../ioutput/">Output</a>.<a href="../../properties/ioutput-calculation/">Calculation</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculation.htm`*
