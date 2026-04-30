---
title: "IRepD2SegmentListInt.Count"
description: "Changes the number of background segments in a 2D axis system in DIAdem REPORT or returns the number."
---

# IRepD2SegmentListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for 2DBackgroundSegments

Changes the number of background segments in a 2D axis system in DIAdem REPORT or returns the number.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of background segments: " + oMyReportObj.Settings.BackgroundSegments.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepD2SegmentListInt.htm`*
