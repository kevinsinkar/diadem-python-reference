---
title: "IRepD2BackgroundImageScalingInt.Enable"
description: "Specifies whether the background graphic of a 2D axis system in DIAdem REPORT can be scaled."
---

# IRepD2BackgroundImageScalingInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for 2DBackgroundImageScaling

Specifies whether the background graphic of a 2D axis system in DIAdem REPORT can be scaled.

## Signature

```python
obj.Enable
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\VIEW_MapDisplay.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[4]"
oMyShape.YChannel.Reference = "[1]/[3]"
oMyShape.Settings.Line.Width = dd.eLineWidth0100
oMySetting = oMy2DAxisSystem.Settings
oMyBackgroundImage = oMySetting.BackgroundImage
oMyBackgroundImage.FileName = dd.ProgramDrv + "Examples\\Documents\\Example_map.png"
oMyScaling = oMyBackgroundImage.Scaling
oMyScaling.Enable = True
oMyScaling.XBegin = 6.305216
oMyScaling.XEnd = 6.394826
oMyScaling.XUnit = "+deg;"
oMyScaling.YBegin = 50.582192
oMyScaling.YEnd = 50.62974
oMyScaling.YUnit = "+deg;"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepD2BackgroundImageScalingInt.htm`*
