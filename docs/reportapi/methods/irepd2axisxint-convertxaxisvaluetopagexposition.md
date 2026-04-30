---
title: "IRepD2AxisXInt.ConvertXAxisValueToPageXPosition"
description: "Converts the x-coordinates of a 2D axis system in DIAdem REPORT into page coordinates."
---

# IRepD2AxisXInt.ConvertXAxisValueToPageXPosition

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ConvertXAxisValueToPageXPosition for 2DAxisX

Converts the x-coordinates of a 2D axis system in DIAdem REPORT into page coordinates.

## Signature

```python
iConvertXAxisValueToPageXPosition = Object.ConvertXAxisValueToPageXPosition(Value)
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
dd.Report.Refresh()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow, "MyArrow")
oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyChnGroupChannels = dd.Data.Root.ChannelGroups(1).Channels
MaxValY = oMyChnGroupChannels(2).Properties("maximum").Value
MaxValX = oMyChnGroupChannels(1).Values(dd.PNo("[1]/[2]", MaxValY))
oMyArrowPosition.X1 = oMy2DaxisSystem.XAxis.ConvertXAxisValueToPageXPosition(MaxValX) + 10
oMyArrowPosition.Y1 = oMy2DaxisSystem.YAxis.ConvertYAxisValueToPageYPosition(MaxValY) + 10
oMyArrowPosition.X2 = oMy2DaxisSystem.XAxis.ConvertXAxisValueToPageXPosition(MaxValX)
oMyArrowPosition.Y2 = oMy2DaxisSystem.YAxis.ConvertYAxisValueToPageYPosition(MaxValY)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ConvertXAxisValueToPageXPosition_IRepD2AxisXInt.htm`*
