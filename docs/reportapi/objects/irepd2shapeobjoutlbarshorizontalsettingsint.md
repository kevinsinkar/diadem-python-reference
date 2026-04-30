---
title: "IRepD2ShapeObjOutlBarsHorizontalSettingsInt"
description: "The 2DOutlineBarsHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Horizontal outlined bars display mode in DIAdem RE"
---

# IRepD2ShapeObjOutlBarsHorizontalSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DOutlineBarsHorizontalSettings

The 2DOutlineBarsHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Horizontal outlined bars display mode in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBarsHorizontal, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.Line.Width = dd.eLineWidth0200
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-type/">Type</a> | <a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-usecurveexpansion/">UseCurveExpansion</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjoutlinebarshorizontalint/">2DOutlineBarsHorizontal</a>.<a href="../../properties/irepd2shapeobjoutlinebarshorizontalint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjOutlBarsHorizontalSettingsInt.htm`*
