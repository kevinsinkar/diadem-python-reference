---
title: "IRepD2BackgroundImageScalingInt"
description: "The 2DBackgroundImageScaling object provides the scaling properties of a background graphic in 2D axis system, in DIAdem REPORT."
---

# IRepD2BackgroundImageScalingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBackgroundImageScaling

The 2DBackgroundImageScaling object provides the scaling properties of a background graphic in 2D axis system, in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2backgroundimagescalingint-enable/">Enable</a> | <a href="../../properties/irepd2backgroundimagescalingint-xbegin/">XBegin</a> | <a href="../../properties/irepd2backgroundimagescalingint-xend/">XEnd</a> | <a href="../../properties/irepd2backgroundimagescalingint-xunit/">XUnit</a> | <a href="../../properties/irepd2backgroundimagescalingint-ybegin/">YBegin</a> | <a href="../../properties/irepd2backgroundimagescalingint-yend/">YEnd</a> | <a href="../../properties/irepd2backgroundimagescalingint-yunit/">YUnit</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2backgroundimageint/">2DBackgroundImage</a>.<a href="../../properties/irepd2backgroundimageint-scaling/">Scaling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2BackgroundImageScalingInt.htm`*
