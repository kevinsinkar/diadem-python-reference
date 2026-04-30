---
title: "IRepMarkerLineInt"
description: "The MarkerLine object provides the properties of the curve marker line of a 2D or a 3D axis system in DIAdem REPORT."
---

# IRepMarkerLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: MarkerLine

The MarkerLine object provides the properties of the curve marker line of a 2D or a 3D axis system in DIAdem REPORT.

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
oMyMarkerLine = oMyMarker.Line
oMyMarkerLine.UseCurveColor = False
oMyMarkerLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyMarkerLine.Width = dd.eLineWidth0100
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepmarkerlineint-color/">Color</a> | <a href="../../properties/irepmarkerlineint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepmarkerlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2markeradditionalint/">2DAdditionalMarker</a>.<a href="../../properties/irepd2markeradditionalint-line/">Line</a> | <a href="../irepd3markeradditionalint/">3DAdditionalMarker</a>.<a href="../../properties/irepd3markeradditionalint-line/">Line</a> | <a href="../irepd3markeradditionalchannelsizeint/">3DAdditionalMarkerChannelSize</a>.<a href="../../properties/irepd3markeradditionalchannelsizeint-line/">Line</a> | <a href="../irepd3shapeobjcoordinatesettingsint/">3DCoordinateSettings</a>.<a href="../../properties/irepd3shapeobjcoordinatesettingsint-markerline/">MarkerLine</a> | <a href="../irepexpansionmarkerint/">CurveExpansionMarker</a>.<a href="../../properties/irepexpansionmarkerint-line/">Line</a> | <a href="../ireppolarmarkeradditionalint/">PolarAdditionalMarker</a>.<a href="../../properties/ireppolarmarkeradditionalint-line/">Line</a> | <a href="../irepspidermarkeradditionalint/">SpiderAdditionalMarker</a>.<a href="../../properties/irepspidermarkeradditionalint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepMarkerLineInt.htm`*
