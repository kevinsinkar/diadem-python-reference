---
title: "IRepD3ShapeObjCoordinateInt.ZCoordinate"
description: "Specifies the z-channel of the curve in a 3D axis system with the display mode Coordinate in DIAdem REPORT."
---

# IRepD3ShapeObjCoordinateInt.ZCoordinate

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ZCoordinate for 3DCoordinate

Specifies the z-channel of the curve in a 3D axis system with the display mode Coordinate in DIAdem REPORT.

## Signature

```python
return_value = obj.ZCoordinate
```

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
oMyCoordShape.Settings.MarkerLine.Width = dd.eLineWidth0100
oMyCoordShape.Extensions.CoordinateLabel.Type = dd.eEndLabelCoordinate
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ZCoordinate_IRepD3ShapeObjCoordinateInt.htm`*
