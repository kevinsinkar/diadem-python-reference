---
title: "SelectedObjects"
description: "Collection of all ReportObject objects in DIAdem REPORT. Use the SelectedElements collection to access a selected element."
---

# SelectedObjects

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: SelectedObjects

Collection of all ReportObject objects in DIAdem REPORT. Use the SelectedElements collection to access a selected element.

## Python example

```python
oMyReportObj = dd.Report.SelectedObjects()
if dd.MsgBoxDisp("Number of selected object== " + oMyReportObj.Count + "\r\n" + "Do you want to remove selection?","MB_YesNo","MsgTypeNote") == "IDYes" :
    oMyReportObj.RemoveAll()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepselectedobjectslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepselectedobjectslistint-exists/">Exists</a> | <a href="../../methods/irepselectedobjectslistint-item/">Item</a> | <a href="../../methods/irepselectedobjectslistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepreportint/">Report</a>.<a href="../../properties/irepreportint-selectedobjects/">SelectedObjects</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSelectedObjectsListInt.htm`*
