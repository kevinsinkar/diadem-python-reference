---
title: "IRepD2AxisYInt"
description: "The 2DAxisY object provides the y-axis for a 2D axis system in DIAdem REPORT. The 2DAxisY object is identical with the first element of the 2DAxisYAxisList coll"
---

# IRepD2AxisYInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisY

The 2DAxisY object provides the y-axis for a 2D axis system in DIAdem REPORT. The 2DAxisY object is identical with the first element of the 2DAxisYAxisList collection.

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DAxisSystem :
        oMySubObjects = oMyReportObj.YAxisList
        for i in range( 1, oMySubObjects.Count+1):
            sOutput = sOutput + "Horizontal offset: " + dd.Str(oMySubObjects.Item(i).OffsetHorizontal) + "\t" + "Axis name: " + oMySubObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisyint-disablecurveclipping/">DisableCurveClipping</a> | <a href="../../properties/irepd2axisyint-height/">Height</a> | <a href="../../properties/irepd2axisyint-index/">Index</a> | <a href="../../properties/irepd2axisyint-label/">Label</a> | <a href="../../properties/irepd2axisyint-line/">Line</a> | <a href="../../properties/irepd2axisyint-name/">Name</a> | <a href="../../properties/irepd2axisyint-numbers/">Numbers</a> | <a href="../../properties/irepd2axisyint-offsethorizontal/">OffsetHorizontal</a> | <a href="../../properties/irepd2axisyint-offsetorigin/">OffsetOrigin</a> | <a href="../../properties/irepd2axisyint-offsetvertical/">OffsetVertical</a> | <a href="../../properties/irepd2axisyint-scaling/">Scaling</a> | <a href="../../properties/irepd2axisyint-tagstored/">TagStored</a> | <a href="../../properties/irepd2axisyint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepd2axisyint-targetunit/">TargetUnit</a> | <a href="../../properties/irepd2axisyint-tickdisplay/">TickDisplay</a> | <a href="../../properties/irepd2axisyint-visible/">Visible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepd2axisyint-convertpageypositiontoyaxisvalue/">ConvertPageYPositionToYAxisValue</a> | <a href="../../methods/irepd2axisyint-convertyaxisvaluetopageyposition/">ConvertYAxisValueToPageYPosition</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-yaxis/">YAxis</a> | <a href="../../collections/2daxisyaxislist/">2DAxisYAxisList</a>.<a href="../../methods/irepd2axisylistint-add/">Add</a> | <a href="../../collections/2daxisyaxislist/">2DAxisYAxisList</a>.<a href="../../methods/irepd2axisylistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisYInt.htm`*
