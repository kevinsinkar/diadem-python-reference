---
title: "IRepD2ShapeObjFilledAreaSettingsInt"
description: "The 2DFilledAreaSettings object provides the curve parameter properties of a 2D axis system in the Filled area display mode in DIAdem REPORT."
---

# IRepD2ShapeObjFilledAreaSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DFilledAreaSettings

The 2DFilledAreaSettings object provides the curve parameter properties of a 2D axis system in the Filled area display mode in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMySettings.FillEffects.Pattern = dd.eFillPatternFilled
oMySettings.FillEffects.Color.SetPredefinedColor(dd.eColorIndexRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjfilledareasettingsint-connectnovalueneighbors/">ConnectNoValueNeighbors</a> | <a href="../../properties/irepd2shapeobjfilledareasettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepd2shapeobjfilledareasettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjfilledareasettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjfilledareasettingsint-usecurveexpansion/">UseCurveExpansion</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjfilledareaint/">2DFilledArea</a>.<a href="../../properties/irepd2shapeobjfilledareaint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjFilledAreaSettingsInt.htm`*
