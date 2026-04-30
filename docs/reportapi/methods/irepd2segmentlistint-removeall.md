---
title: "IRepD2SegmentListInt.RemoveAll"
description: "Deletes all background segments from a 2D axis system in DIAdem REPORT."
---

# IRepD2SegmentListInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for 2DBackgroundSegments

Deletes all background segments from a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMyReportObj.Settings.BackgroundSegments.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepD2SegmentListInt.htm`*
