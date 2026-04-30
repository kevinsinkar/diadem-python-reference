---
title: "IRepSpiderInt.Index"
description: "Returns the index of a curve in a spider axis system in DIAdem REPORT."
---

# IRepSpiderInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for Spider

Returns the index of a curve in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.Index
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectSpider :
        sOutput = sOutput + "Object " + oMyReportObj.Name + ": Index: "+ oMyReportObj.Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepSpiderInt.htm`*
