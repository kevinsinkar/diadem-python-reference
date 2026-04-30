---
title: "IRepFormulaDisplayInt.SelectedElements"
description: "Returns a collection of all selected elements of a formula graphic in DIAdem REPORT."
---

# IRepFormulaDisplayInt.SelectedElements

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SelectedElements for FormulaDisplay

Returns a collection of all selected elements of a formula graphic in DIAdem REPORT.

## Signature

```python
return_value = obj.SelectedElements
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectFormulaDisplay :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for I in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SelectedElements_IRepFormulaDisplayInt.htm`*
