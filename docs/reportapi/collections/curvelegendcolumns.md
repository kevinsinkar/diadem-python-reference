---
title: "CurveLegendColumns"
description: "Collection of all CurveLegendColumn objects in DIAdem REPORT. Use the CurveLegendColumns collection to delete or to create new columns in curve legends."
---

# CurveLegendColumns

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: CurveLegendColumns

Collection of all CurveLegendColumn objects in DIAdem REPORT. Use the CurveLegendColumns collection to delete or to create new columns in curve legends.

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.CurveLegend.Columns.RemoveAll()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendcontentcolumnslistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepcurvelegendcontentcolumnslistint-add/">Add</a> | <a href="../../methods/irepcurvelegendcontentcolumnslistint-item/">Item</a> | <a href="../../methods/irepcurvelegendcontentcolumnslistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepcurvelegendint/">CurveLegend</a>.<a href="../../properties/irepcurvelegendint-columns/">Columns</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurvelegendContentColumnsListInt.htm`*
