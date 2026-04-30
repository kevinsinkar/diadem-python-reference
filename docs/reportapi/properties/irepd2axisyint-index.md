---
title: "IRepD2AxisYInt.Index"
description: "Specifies the index of a y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.Index

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Index for 2DAxisY

Specifies the index of a y-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Index
```

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMySubObjects = oMyReportObj.YAxisList
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Horizontal offset: " + oMySubObjects.Item(i).OffsetHorizontal + "\t" + "Axis index: " + oMySubObjects.Item(i).Index + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Index_IRepD2AxisYInt.htm`*
