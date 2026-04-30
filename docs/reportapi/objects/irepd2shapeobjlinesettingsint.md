---
title: "IRepD2ShapeObjLineSettingsInt"
description: "The 2DLineSettings object provides the curve properties of a 2D axis system in the display mode Line display mode in DIAdem REPORT."
---

# IRepD2ShapeObjLineSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DLineSettings

The 2DLineSettings object provides the curve properties of a 2D axis system in the display mode Line display mode in DIAdem REPORT.

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
oMyCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve1")
oMyShape1 = oMyCurve1.Shape
oMyShape1.XChannel.Reference = ""
oMyShape1.YChannel.Reference = "[4]/[1]"
oMyCurve1.Shape.Settings.UseCurveSmoothing = False
oMyCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve2")
oMyShape2 = oMyCurve2.Shape
oMyShape2.XChannel.Reference = ""
oMyShape2.YChannel.Reference = "[4]/[1]"
oMyCurve2.Shape.Settings.UseCurveSmoothing = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjlinesettingsint-connectnovalueneighbors/">ConnectNoValueNeighbors</a> | <a href="../../properties/irepd2shapeobjlinesettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepd2shapeobjlinesettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjlinesettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjlinesettingsint-usecurveexpansion/">UseCurveExpansion</a> | <a href="../../properties/irepd2shapeobjlinesettingsint-usecurvesmoothing/">UseCurveSmoothing</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjlineint/">2DLine</a>.<a href="../../properties/irepd2shapeobjlineint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjLineSettingsInt.htm`*
