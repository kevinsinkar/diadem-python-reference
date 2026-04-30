---
title: "IRepPolarInt.ConvertPolarCoordinateToPageYPosition"
description: "Converts in a polar axis system in DIAdem REPORT an angle and a radius into a y-page coordinate."
---

# IRepPolarInt.ConvertPolarCoordinateToPageYPosition

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ConvertPolarCoordinateToPageYPosition for PolarSystem

Converts in a polar axis system in DIAdem REPORT an angle and a radius into a y-page coordinate.

## Signature

```python
iConvertPolarCoordinateToPageYPosition = Object.ConvertPolarCoordinateToPageYPosition(Angle, Length)
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")

oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPos = oMyPolarSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[4]"

dd.Report.Refresh()
oMyArrow = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectArrow, "MyArrow")
oMyArrowPosition = oMyArrow.Position.ByCoordinate
oMyChnGroupChannels = dd.Data.Root.ChannelGroups(5).Channels
MaxValLength = oMyChnGroupChannels(4).Properties("maximum").Value
MaxValAngle  = oMyChnGroupChannels(1).Values(dd.PNo("[5]/[4]", MaxValLength))
oMyArrowPosition.X1 = oMyPolarSystem.ConvertPolarCoordinateToPageXPosition (MaxValAngle, MaxValLength) + 10
oMyArrowPosition.Y1 = oMyPolarSystem.ConvertPolarCoordinateToPageYPosition (MaxValAngle, MaxValLength) + 10
oMyArrowPosition.X2 = oMyPolarSystem.ConvertPolarCoordinateToPageXPosition (MaxValAngle, MaxValLength)
oMyArrowPosition.Y2 = oMyPolarSystem.ConvertPolarCoordinateToPageYPosition (MaxValAngle, MaxValLength)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ConvertPolarCoordinateToPageYPosition_IRepPolarInt.htm`*
