---
title: "ICalculationSet"
description: "The CalculationSet object enables access to a calculation set. Use the CalculationSet object to load and to save the calculation sets. In scripts the Calculatio"
---

# ICalculationSet

!!! abstract "Object &middot; `ICalculationSet.chm`"
    Object: CalculationSet

The CalculationSet object enables access to a calculation set. Use the CalculationSet object to load and to save the calculation sets. In scripts the CalculationSet object is available as a global object. Do not create an object or a variable with the name CalculationSet , because that overwrites the CalculationSet object.

## Python example

```python
for oMyCalcGroup in dd.CalculationSet.CalculationGroups:
    sText = "Calculation Group : " + oMyCalcGroup.Name + "\r\n"
    for oMyCalcTemp in oMyCalcGroup.Calculations:
        sText = sText + "Calculation: " + oMyCalcTemp.Name + "\r\n"
    dd.MsgBoxDisp(sText)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icalculationset-calculationgroups/">CalculationGroups</a> | <a href="../../properties/icalculationset-description/">Description</a> | <a href="../../properties/icalculationset-filename/">FileName</a> | <a href="../../properties/icalculationset-name/">Name</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icalculationset-append/">Append</a> | <a href="../../methods/icalculationset-clear/">Clear</a> | <a href="../../methods/icalculationset-copy/">Copy</a> | <a href="../../methods/icalculationset-export/">Export</a> | <a href="../../methods/icalculationset-ismodified/">IsModified</a> | <a href="../../methods/icalculationset-load/">Load</a> | <a href="../../methods/icalculationset-move/">Move</a> | <a href="../../methods/icalculationset-runselected/">RunSelected</a> | <a href="../../methods/icalculationset-save/">Save</a> | <a href="../../methods/icalculationset-saveas/">SaveAs</a> | <a href="../../methods/icalculationset-selectall/">SelectAll</a> | <a href="../../methods/icalculationset-showexecutiondlg/">ShowExecutionDlg</a> | <a href="../../methods/icalculationset-showsettingsdlg/">ShowSettingsDlg</a> | <a href="../../methods/icalculationset-validateselected/">ValidateSelected</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Connecting Channels and Values in Calculations</a> | <a href="#" data-unresolved="1">Creating a Calculation Script with Debug Option</a> | <a href="#" data-unresolved="1">Creating and Executing Calculations</a> | <a href="#" data-unresolved="1">Executing Calculations Multiple Times</a> | <a href="#" data-unresolved="1">Using Channel Lists in Calculations</a> | <a href="#" data-unresolved="1">Working with Dependent Inputs</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Calculating the Sound Pressure Level with Calculation Templates</a></p>
</div>
</div>

---

*Source: `ICalculationSet/objects/FormulaCalc_Objects_ICalculationSet.htm`*
