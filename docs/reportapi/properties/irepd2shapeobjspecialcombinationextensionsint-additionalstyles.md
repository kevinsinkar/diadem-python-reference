---
title: "IRepD2ShapeObjSpecialCombinationExtensionsInt.AdditionalStyles"
description: "Specifies the properties of the special forms of a curve in a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationExtensionsInt.AdditionalStyles

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AdditionalStyles for 2DSpecialCombinationExtensions

Specifies the properties of the special forms of a curve in a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.AdditionalStyles
```

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
oMyAdditionalStyle = oMyExtension.AdditionalStyles
oMyAdditionalStyle.Type = dd.e2DAdditionalStyleStairs
oMyAdditionalStyle.Line.LineType = dd.eLineTypeDashed1
oMyAdditionalStyle.Line.Interval = 5
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AdditionalStyles_IRepD2ShapeObjSpecialCombinationExtensionsInt.htm`*
