---
title: "IRepFormulaDisplayInt.IsSelected"
description: "Specifies whether a formula graphic is selected in DIAdem REPORT."
---

# IRepFormulaDisplayInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for FormulaDisplay

Specifies whether a formula graphic is selected in DIAdem REPORT.

## Signature

```python
obj.IsSelected
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectFormulaDisplay :
        sOutput = sOutput + "Object " + oMyReportObj.Name + " is selected: "+ oMyReportObj.IsSelected + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsSelected_IRepFormulaDisplayInt.htm`*
