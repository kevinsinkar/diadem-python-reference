---
title: "IRepFormulaDisplaySelectedSubObjectsListInt.Count"
description: "Specifies the number of selected elements of a formula graphic in DIAdem REPORT."
---

# IRepFormulaDisplaySelectedSubObjectsListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for FormulaDisplaySelectedElements

Specifies the number of selected elements of a formula graphic in DIAdem REPORT.

## Signature

```python
obj.Count
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

*Source: `ReportApi/properties/Report_property_Count_IRepFormulaDisplaySelectedSubObjectsListInt.htm`*
