---
title: "IRepBoxWhiskerMarkerFillingInt"
description: "The 2DBoxWhiskerMarkerFilling object provides the curve marker filling of a 2D axis system in the Box-Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerFillingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBoxWhiskerMarkerFilling

The 2DBoxWhiskerMarkerFilling object provides the curve marker filling of a 2D axis system in the Box-Whisker display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\EXPL_Legend.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBoxWhisker, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyYChannels= oMyShape.YChannels
oMyYChannels.RemoveAll()
oMyYChannels.Add("[1]/X_Channel")
oMyYChannels.Add("[1]/Z_Channel_1")
oMyYChannels.Add("[1]/Z_Channel_2")
oMyYChannels.Add("[1]/Z_Channel_3")
oMyYChannels.Add("[1]/Z_Channel_4")
oMyYChannels.Add("[1]/Z_Channel_5")
oMyShape.Extensions.MarkerWhisker.Type = dd.eMarkerCircle
oMyShape.Extensions.MarkerWhisker.Filling.UseBorderColor = False
oMyShape.Extensions.MarkerWhisker.Filling.ColorIndex = dd.eColorIndexRed
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepboxwhiskermarkerfillingint-colorindex/">ColorIndex</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-gradientdirection/">GradientDirection</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-gradientmode/">GradientMode</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-rgb/">RGB</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-rgbfilling/">RGBFilling</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-transparency/">Transparency</a> | <a href="../../properties/irepboxwhiskermarkerfillingint-usebordercolor/">UseBorderColor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepboxwhiskermarkerfillingint-setfillingcolor/">SetFillingColor</a> | <a href="../../methods/irepboxwhiskermarkerfillingint-setpredefinedcolor/">SetPredefinedColor</a> | <a href="../../methods/irepboxwhiskermarkerfillingint-setrgbcolor/">SetRGBColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepboxwhiskermarkerint/">2DBoxWhiskerMarker</a>.<a href="../../properties/irepboxwhiskermarkerint-filling/">Filling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepBoxWhiskerMarkerFillingInt.htm`*
