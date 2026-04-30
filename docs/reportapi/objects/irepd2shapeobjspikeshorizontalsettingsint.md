---
title: "IRepD2ShapeObjSpikesHorizontalSettingsInt"
description: "The 2DSpikesHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Horizontal spikes display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpikesHorizontalSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpikesHorizontalSettings

The 2DSpikesHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Horizontal spikes display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpikesHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[2]"
oMyShape.YChannel.Reference = "[1]/[1]"
oMyShape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShape.Settings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspikeshorizontalsettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjspikeshorizontalsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjspikeshorizontalsettingsint-usecurveexpansion/">UseCurveExpansion</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjspikeshorizontalint/">2DSpikesHorizontal</a>.<a href="../../properties/irepd2shapeobjspikeshorizontalint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpikesHorizontalSettingsInt.htm`*
