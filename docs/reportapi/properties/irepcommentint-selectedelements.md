---
title: "IRepCommentInt.SelectedElements"
description: "Returns a collection of all selected elements of a comment in DIAdem REPORT. The only element from a comment that you can select is the comment arrow. Use the p"
---

# IRepCommentInt.SelectedElements

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SelectedElements for Comment

Returns a collection of all selected elements of a comment in DIAdem REPORT. The only element from a comment that you can select is the comment arrow. Use the property SelectedObjects to access the main object you have selected.

## Signature

```python
return_value = obj.SelectedElements
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectComment :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMyReportObj.SelectedElements.Count)
        for oMySelection in oMyReportObj.SelectedElements:
            sOutput = sOutput + "Element type: " + oMySelection.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SelectedElements_IRepCommentInt.htm`*
