---
title: "2DBackgroundSegments"
description: "Collection of all 2DBackgroundSegment objects in DIAdem REPORT. Use the 2DBackgroundSegments collection to access a single background element in DIAdem REPORT."
---

# 2DBackgroundSegments

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DBackgroundSegments

Collection of all 2DBackgroundSegment objects in DIAdem REPORT. Use the 2DBackgroundSegments collection to access a single background element in DIAdem REPORT.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        dd.MsgBoxDisp("Object name: " + oMyReportObj.Name + "\r\n" + "Number of background segments: " + oMyReportObj.Settings.BackgroundSegments.Count)
        for oMyBackgroundSegment in oMyReportObj.Settings.BackgroundSegments:
            sOutput = sOutput + "X-channel: " + oMyBackgroundSegment.XChannel.Reference + "\t" + "y-channel: " + oMyBackgroundSegment.YChannel.Reference + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2segmentlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2segmentlistint-add/">Add</a> | <a href="../../methods/irepd2segmentlistint-item/">Item</a> | <a href="../../methods/irepd2segmentlistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2axissettingsint/">2DAxisSettings</a>.<a href="../../properties/irepd2axissettingsint-backgroundsegments/">BackgroundSegments</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2SegmentListInt.htm`*
