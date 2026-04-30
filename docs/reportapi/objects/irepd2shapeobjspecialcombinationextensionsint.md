---
title: "IRepD2ShapeObjSpecialCombinationExtensionsInt"
description: "The 2DSpecialCombinationExtensions object provides the extended properties of the curve parameters of a 2D axis system in the Special combination display mode i"
---

# IRepD2ShapeObjSpecialCombinationExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpecialCombinationExtensions

The 2DSpecialCombinationExtensions object provides the extended properties of the curve parameters of a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyExtension = oMyShape.Extensions
oMyExtension.Marker.Type = dd.eMarkerCircle
oMyExtension.Marker.Size = 3
oMyExtension.Marker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyExtension.Marker.Repetition.NValue = 20
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-additionalstyles/">AdditionalStyles</a> | <a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-endlabel/">EndLabel</a> | <a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-errorbars/">ErrorBars</a> | <a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-label/">Label</a> | <a href="../../properties/irepd2shapeobjspecialcombinationextensionsint-marker/">Marker</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjspecialcombinationint/">2DSpecialCombination</a>.<a href="../../properties/irepd2shapeobjspecialcombinationint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpecialCombinationExtensionsInt.htm`*
