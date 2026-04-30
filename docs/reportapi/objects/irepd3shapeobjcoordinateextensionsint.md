---
title: "IRepD3ShapeObjCoordinateExtensionsInt"
description: "The 3DCoordinateExtensions object provides the extended curve properties of a 3D axis system in the Coordinate display mode in DIAdem REPORT."
---

# IRepD3ShapeObjCoordinateExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DCoordinateExtensions

The 3DCoordinateExtensions object provides the extended curve properties of a 3D axis system in the Coordinate display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjcoordinateextensionsint-coordinatecomment/">CoordinateComment</a> | <a href="../../properties/irepd3shapeobjcoordinateextensionsint-coordinatelabel/">CoordinateLabel</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcoordinateint/">3DCoordinate</a>.<a href="../../properties/irepd3shapeobjcoordinateint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjCoordinateExtensionsInt.htm`*
