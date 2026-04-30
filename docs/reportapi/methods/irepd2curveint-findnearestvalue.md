---
title: "IRepD2CurveInt.FindNearestValue"
description: "Determines in a 2D axis system in DIAdem REPORT the curve point which is nearest to a given point ."
---

# IRepD2CurveInt.FindNearestValue

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: FindNearestValue for 2DCurve

Determines in a 2D axis system in DIAdem REPORT the curve point which is nearest to a given point .

## Signature

```python
return_value = obj.FindNearestValue(X, Y)
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_FindNearestValue_IRepD2CurveInt.htm`*
