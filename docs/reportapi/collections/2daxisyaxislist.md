---
title: "2DAxisYAxisList"
description: "Collection of all 2DAxisY objects in DIAdem REPORT. Use the 2DAxisYAxisList collection to access an individual y-axis in a 2D axis system in DIAdem REPORT. The "
---

# 2DAxisYAxisList

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: 2DAxisYAxisList

Collection of all 2DAxisY objects in DIAdem REPORT. Use the 2DAxisYAxisList collection to access an individual y-axis in a 2D axis system in DIAdem REPORT. The first object of the 2DAxisYAxisList collection is identical with the 2DAxisY object.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMySubObjects = oMyReportObj.YAxisList
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Horizontal offset: " + oMySubObjects.Item(i).OffsetHorizontal + "\t" + "Axis name: " + oMySubObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisylistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2axisylistint-add/">Add</a> | <a href="../../methods/irepd2axisylistint-exists/">Exists</a> | <a href="../../methods/irepd2axisylistint-item/">Item</a> | <a href="../../methods/irepd2axisylistint-remove/">Remove</a> | <a href="../../methods/irepd2axisylistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-yaxislist/">YAxisList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisYListInt.htm`*
