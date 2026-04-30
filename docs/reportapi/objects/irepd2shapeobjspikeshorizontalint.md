---
title: "IRepD2ShapeObjSpikesHorizontalInt"
description: "The 2DSpikesHorizontal object provides the curve properties of a 2D axis system in the Horizontal spikes display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpikesHorizontalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpikesHorizontal

The 2DSpikesHorizontal object provides the curve properties of a 2D axis system in the Horizontal spikes display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Report_EXPL","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpikesHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMyShape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyShape.Settings.Line.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspikeshorizontalint-settings/">Settings</a> | <a href="../../properties/irepd2shapeobjspikeshorizontalint-xchannel/">XChannel</a> | <a href="../../properties/irepd2shapeobjspikeshorizontalint-ychannel/">YChannel</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2curveint/">2DCurve</a>.<a href="../../properties/irepd2curveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpikesHorizontalInt.htm`*
