---
title: "IRepMarkerFillingInt"
description: "The MarkerFilling object provides the properties of the curve marker filling of a 2D or a 3D axis system in DIAdem REPORT."
---

# IRepMarkerFillingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: MarkerFilling

The MarkerFilling object provides the properties of the curve marker filling of a 2D or a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
oMyMarkerFilling = oMyMarker.Filling
oMyMarkerFilling.UseCurveColor = False
oMyMarkerFilling.SetPredefinedColor(dd.eColorIndexRed)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepmarkerfillingint-colorindex/">ColorIndex</a> | <a href="../../properties/irepmarkerfillingint-gradientdirection/">GradientDirection</a> | <a href="../../properties/irepmarkerfillingint-gradientmode/">GradientMode</a> | <a href="../../properties/irepmarkerfillingint-rgb/">RGB</a> | <a href="../../properties/irepmarkerfillingint-rgbfilling/">RGBFilling</a> | <a href="../../properties/irepmarkerfillingint-transparency/">Transparency</a> | <a href="../../properties/irepmarkerfillingint-usecurvecolor/">UseCurveColor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepmarkerfillingint-setfillingcolor/">SetFillingColor</a> | <a href="../../methods/irepmarkerfillingint-setpredefinedcolor/">SetPredefinedColor</a> | <a href="../../methods/irepmarkerfillingint-setrgbcolor/">SetRGBColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2markeradditionalint/">2DAdditionalMarker</a>.<a href="../../properties/irepd2markeradditionalint-filling/">Filling</a> | <a href="../irepd3markeradditionalint/">3DAdditionalMarker</a>.<a href="../../properties/irepd3markeradditionalint-filling/">Filling</a> | <a href="../irepd3markeradditionalchannelsizeint/">3DAdditionalMarkerChannelSize</a>.<a href="../../properties/irepd3markeradditionalchannelsizeint-filling/">Filling</a> | <a href="../irepd3shapeobjcoordinatesettingsint/">3DCoordinateSettings</a>.<a href="../../properties/irepd3shapeobjcoordinatesettingsint-filling/">Filling</a> | <a href="../irepexpansionmarkerint/">CurveExpansionMarker</a>.<a href="../../properties/irepexpansionmarkerint-filling/">Filling</a> | <a href="../ireppolarmarkeradditionalint/">PolarAdditionalMarker</a>.<a href="../../properties/ireppolarmarkeradditionalint-filling/">Filling</a> | <a href="../irepspidermarkeradditionalint/">SpiderAdditionalMarker</a>.<a href="../../properties/irepspidermarkeradditionalint-filling/">Filling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepMarkerFillingInt.htm`*
