---
title: "ReportObjects"
description: "Collection of all ReportObject objects in DIAdem REPORT. Use the ReportObjects collection to delete or to create new objects for the graphical display."
---

# ReportObjects

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: ReportObjects

Collection of all ReportObject objects in DIAdem REPORT. Use the ReportObjects collection to delete or to create new objects for the graphical display.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    sOutput = sOutput + "Object type: " + oMyReportObj.ObjectType + "\t" + "Object name: " + oMyReportObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepctrllistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../methods/irepctrllistint-exists/">Exists</a> | <a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../methods/irepctrllistint-remove/">Remove</a> | <a href="../../methods/irepctrllistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepsheetint/">Sheet</a>.<a href="../../properties/irepsheetint-objects/">Objects</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCtrlListInt.htm`*
