---
title: "IRepPoint2DInt"
description: "The NearestValue2D object provides the coordinates and the index of a curve point that lie nearest to a specified point, in DIAdem REPORT."
---

# IRepPoint2DInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: NearestValue2D

The NearestValue2D object provides the coordinates and the index of a curve point that lie nearest to a specified point, in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyNearestValueObj = oMy2DCurve.FindNearestValue(20,30)
dd.Report.Refresh()
dd.MsgBoxDisp("x value: " + oMyNearestValueObj.X + "\r\n" + "y value: " + oMyNearestValueObj.Y + "\r\n" + "point index: " + oMyNearestValueObj.Index)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppoint2dint-index/">Index</a> | <a href="../../properties/ireppoint2dint-x/">X</a> | <a href="../../properties/ireppoint2dint-y/">Y</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../methods/irepd2curveint-findnearestvalue/">FindNearestValue</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPoint2DInt.htm`*
