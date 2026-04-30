---
title: "IRepD2AxisYListInt.Add"
description: "Adds a y-axis to a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for 2DAxisYAxisList

Adds a y-axis to a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(Name)
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
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[3]"
oMyAxis = oMy2DaxisSystem.YAxisList.Add("SecondAxis")
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

*Source: `ReportApi/methods/Report_method_Add_IRepD2AxisYListInt.htm`*
