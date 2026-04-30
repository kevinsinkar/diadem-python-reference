---
title: "IRepPolarMarkerAdditionalInt.Type"
description: "Specifies the symbol that DIAdem REPORT displays as the marker of a polar curve."
---

# IRepPolarMarkerAdditionalInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for PolarAdditionalMarker

Specifies the symbol that DIAdem REPORT displays as the marker of a polar curve.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eMarkerNone` | 0 | None |
| `eMarkerSquare` | 1 | Square |
| `eMarkerRhombus` | 2 | Rhombus |
| `eMarkerTriangle` | 3 | Triangle |
| `eMarkerCross` | 4 | Cross |
| `eMarkerAsterisk` | 5 | Asterisk |
| `eMarkerShortDash` | 6 | Short dash |
| `eMarkerLongDash` | 7 | Long dash |
| `eMarkerPlus` | 8 | Plus |
| `eMarkerCircle` | 9 | Circle |
| `eMarkerTriangle_Bottom` | 10 | Triangle bottom |
| `eMarkerTriangle_Left` | 11 | Triangle left |
| `eMarkerTriangle_Right` | 12 | Triangle right |
| `eMarkerSquare_Top` | 13 | Square filled top |
| `eMarkerSquare_Bottom` | 14 | Square filled bottom |
| `eMarkerSquare_Left` | 15 | Square filled left |
| `eMarkerSquare_Right` | 16 | Square filled right |
| `eMarkerRhomb_Top` | 17 | Rhomb filled top |
| `eMarkerRhomb_Bottom` | 18 | Rhomb filled bottom |
| `eMarkerRhomb_Left` | 19 | Rhomb filled left |
| `eMarkerRhomb_Right` | 20 | Rhomb filled right |
| `eMarkerTriangle1_Left` | 21 | Triangle 1 filled left |
| `eMarkerTriangle1_Right` | 22 | Triangle 1 filled right |
| `eMarkerTriangle2_Left` | 23 | Triangle 2 filled left |
| `eMarkerTriangle2_Right` | 24 | Triangle 2 filled right |
| `eMarkerTriangle3_Top` | 25 | Triangle 3 filled top |
| `eMarkerTriangle3_Bottom` | 26 | Triangle 3 filled bottom |
| `eMarkerTriangle4_Top` | 27 | Triangle 4 filled top |
| `eMarkerTriangle4_Bottom` | 28 | Triangle 4 filled bottom |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionEveryNthPoint
oMyMarker.Repetition.NValue = 50
oMyMarker.Line.UseCurveColor = False
oMyMarker.Line.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMyMarker.Line.Width = dd.eLineWidth0280
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepPolarMarkerAdditionalInt.htm`*
