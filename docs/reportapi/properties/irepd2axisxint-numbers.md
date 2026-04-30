---
title: "IRepD2AxisXInt.Numbers"
description: "Specifies the properties of the scale labels of the x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXInt.Numbers

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Numbers for 2DAxisX

Specifies the properties of the scale labels of the x-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Numbers
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DXAxis = oMy2DAxisSystem.XAxis
oMy2DXAxis.Scaling.AutoScalingType = dd.eAxisAutoScalingBeginEndManual
oMy2DXAxis.Scaling.Begin = 0
oMy2DXAxis.Scaling.End = 65
oMy2DXAxis.DisableCurveClipping = True
oMyXAxisNumbers = oMy2DXAxis.Numbers
oMyXAxisNumbers.Angle = 45
oMyXAxisNumbers.RelativePosition = dd.eRelativePositionLeft
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Numbers_IRepD2AxisXInt.htm`*
