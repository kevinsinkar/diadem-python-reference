---
title: "IRepCoordinateMarkerFillingInt"
description: "The CoordinateMarkerFilling object provides the marker filling for an additional comment in the 2D and 3D display mode Coordinate in DIAdem REPORT."
---

# IRepCoordinateMarkerFillingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CoordinateMarkerFilling

The CoordinateMarkerFilling object provides the marker filling for an additional comment in the 2D and 3D display mode Coordinate in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurveLine")
oMyCurveShape = oMyCurveLine.Shape
oMyCurveShape.XChannel.Reference = "[1]/[1]"
oMyCurveShape.YChannel.Reference = "[1]/[2]"

oMyCurveCoord = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeCoordinate,"My2DCurveCoord")
oMyCoordShape = oMyCurveCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateFree
oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordShape.Settings.Size = 2
oMyCoordShape.Settings.MarkerFilling.UseMarkerColor = False
oMyCoordShape.Settings.MarkerFilling.SetPredefinedColor(dd.eColorIndexDarkBlue)

MaxValY = dd.Data.GetChannel("[1]/[2]").Properties("maximum").Value
MaxValX = dd.Data.GetChannel("[1]/[1]").Values(dd.PNo("[1]/[2]", MaxValY))
oMyCoordShape.XCoordinate.Reference = MaxValX
oMyCoordShape.YCoordinate.Reference = MaxValY
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcoordinatemarkerfillingint-colorindex/">ColorIndex</a> | <a href="../../properties/irepcoordinatemarkerfillingint-gradientdirection/">GradientDirection</a> | <a href="../../properties/irepcoordinatemarkerfillingint-gradientmode/">GradientMode</a> | <a href="../../properties/irepcoordinatemarkerfillingint-rgb/">RGB</a> | <a href="../../properties/irepcoordinatemarkerfillingint-rgbfilling/">RGBFilling</a> | <a href="../../properties/irepcoordinatemarkerfillingint-transparency/">Transparency</a> | <a href="../../properties/irepcoordinatemarkerfillingint-usemarkercolor/">UseMarkerColor</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepcoordinatemarkerfillingint-setfillingcolor/">SetFillingColor</a> | <a href="../../methods/irepcoordinatemarkerfillingint-setpredefinedcolor/">SetPredefinedColor</a> | <a href="../../methods/irepcoordinatemarkerfillingint-setrgbcolor/">SetRGBColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjcoordinatesettingsint/">2DCoordinateSettings</a>.<a href="../../properties/irepd2shapeobjcoordinatesettingsint-markerfilling/">MarkerFilling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCoordinateMarkerFillingInt.htm`*
