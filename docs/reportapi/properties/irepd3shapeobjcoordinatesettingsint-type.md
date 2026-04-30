---
title: "IRepD3ShapeObjCoordinateSettingsInt.Type"
description: "Specifies the marker type in a 3D axis system in the Coordinate display mode in DIAdem REPORT."
---

# IRepD3ShapeObjCoordinateSettingsInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 3DCoordinateSettings

Specifies the marker type in a 3D axis system in the Coordinate display mode in DIAdem REPORT.

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
| `eMarkerShortDash` | 6 | short line |
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
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMy3DCoord = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCoordinate, "MyNew3DCoordinate")
oMyCoordShape = oMy3DCoord.Shape
oMyCoordShape.BoundingType = dd.eCoordinateChannelBounded
oMyCoordShape.DataStructure = dd.e3DDataStructureTriplet
oMyCoordShape.BoundingPosition = dd.e3DCoordinateBoundingNearestValue
oMyCoordShape.BoundingXChannel.Reference = "[2]/[1]"
oMyCoordShape.BoundingYChannel.Reference = "[2]/[2]"
oMyCoordShape.BoundingZChannel.Reference = "[2]/[3]"
oMyCoordShape.XCoordinate.Reference = 0.5
oMyCoordShape.YCoordinate.Reference = 0.5
oMyCoordShape.Settings.MarkerLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyCoordShape.Settings.Type = dd.eMarkerCircle
oMyCoordShape.Settings.MarkerLine.Width = dd.eLineWidth0100
oMyCoordShape.Extensions.CoordinateLabel.Type = dd.eEndLabelCoordinate
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepD3ShapeObjCoordinateSettingsInt.htm`*
