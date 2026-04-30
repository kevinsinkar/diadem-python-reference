---
title: "IRepD3ShapeObjLineSettingsInt.ProjectToCoordinatePlaneXY"
description: "Specifies whether DIAdem projects the curve of a 3D axis system with the 3D curve display type in DIAdem REPORT to the XY-plane."
---

# IRepD3ShapeObjLineSettingsInt.ProjectToCoordinatePlaneXY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ProjectToCoordinatePlaneXY for 3DLineSettings

Specifies whether DIAdem projects the curve of a 3D axis system with the 3D curve display type in DIAdem REPORT to the XY-plane.

## Signature

```python
obj.ProjectToCoordinatePlaneXY
```

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeLine, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
#oMyShape.DataStructure = e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[3]/[1]"
oMyShape.YChannel.Reference = "[3]/[2]"
oMyShape.ZChannel.Reference = "[3]/[3]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyShape.Settings.ProjectToCoordinatePlaneXY = True
oMyShape.Settings.ProjectToCoordinatePlaneYZ = True
oMyShape.Settings.ProjectToCoordinatePlaneXZ = True
oMyShape.Settings.DisplayAs3DCurve = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ProjectToCoordinatePlaneXY_IRepD3ShapeObjLineSettingsInt.htm`*
