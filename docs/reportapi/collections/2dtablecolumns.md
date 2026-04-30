---
title: "2DTableColumns"
description: "Collection of all 2DTableColumn objects in DIAdem REPORT. Use the 2DTableColumns collection to access a single column in a 2D table in DIAdem REPORT."
---

# 2DTableColumns

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DTableColumns

Collection of all 2DTableColumn objects in DIAdem REPORT. Use the 2DTableColumns collection to access a single column in a 2D table in DIAdem REPORT.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySubObjects = oMyReportObj.Columns
        for oMySubObj in oMySubObjects:
            sOutput = sOutput + "Column type: " + oMySubObj.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable2dcolumnlistint-add/">Add</a> | <a href="../../methods/ireptable2dcolumnlistint-changetype/">ChangeType</a> | <a href="../../methods/ireptable2dcolumnlistint-copy/">Copy</a> | <a href="../../methods/ireptable2dcolumnlistint-item/">Item</a> | <a href="../../methods/ireptable2dcolumnlistint-move/">Move</a> | <a href="../../methods/ireptable2dcolumnlistint-remove/">Remove</a> | <a href="../../methods/ireptable2dcolumnlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ireptable2dint/">2DTable</a>.<a href="../../properties/ireptable2dint-columns/">Columns</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnListInt.htm`*
