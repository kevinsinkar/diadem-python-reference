---
title: "IRepSpiderCurveListInt.Count"
description: "Returns the number of curves in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for SpiderCurves

Returns the number of curves in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of curves: " + oMyReportObj.CurvesSpider.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepSpiderCurveListInt.htm`*
