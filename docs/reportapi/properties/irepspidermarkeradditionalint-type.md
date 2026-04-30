---
title: "IRepSpiderMarkerAdditionalInt.Type"
description: "Specifies the symbol that DIAdem REPORT displays as the marker on a curve in a spider axis system."
---

# IRepSpiderMarkerAdditionalInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for SpiderAdditionalMarker

Specifies the symbol that DIAdem REPORT displays as the marker on a curve in a spider axis system.

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
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyMarker = oMyCurve.Shape.Extensions.Marker
oMyMarker.Type = dd.eMarkerSquare
oMyMarker.Size = 3
oMyMarker.Filling.UseCurveColor = True
oMyMarker.Line.Width = dd.eLineWidth0050
oMyMarker.Size = 3

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepSpiderMarkerAdditionalInt.htm`*
