---
title: "IRepD2ShapeObjSpikesSettingsInt"
description: "The 2DSpikesSettings object provides the curve parameter properties of a 2D axis system in the Spikes display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpikesSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpikesSettings

The 2DSpikesSettings object provides the curve parameter properties of a 2D axis system in the Spikes display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpikes, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspikessettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjspikessettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjspikessettingsint-usecurveexpansion/">UseCurveExpansion</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjspikesint/">2DSpikes</a>.<a href="../../properties/irepd2shapeobjspikesint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpikesSettingsInt.htm`*
