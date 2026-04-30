---
title: "IRepD2CurveInt.YAxisReference"
description: "Specifies the y-axis of a 2D axis system in DIAdem REPORT. Use this property to assign a curve to an axis from the 2DAxisYAxisList collection. You can use the n"
---

# IRepD2CurveInt.YAxisReference

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YAxisReference for 2DCurve

Specifies the y-axis of a 2D axis system in DIAdem REPORT. Use this property to assign a curve to an axis from the 2DAxisYAxisList collection. You can use the name or index to specify the y-axis.

## Signature

```python
obj.YAxisReference
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyFirstCurve")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MySecondCurve")
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[3]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[4]"
oMyAxis = oMy2DaxisSystem.YAxisList.Add("SecondAxis")
oMy2DCurve1.YAxisReference = 1
oMy2DCurve2.YAxisReference = "SecondAxis"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YAxisReference_IRepD2CurveInt.htm`*
