---
title: "IRepD3ShapeObjPointsSettingsInt"
description: "The 3DPointsSettings object provides the curve properties of a 3D axis system in the Points display mode in DIAdem REPORT."
---

# IRepD3ShapeObjPointsSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DPointsSettings

The 3DPointsSettings object provides the curve properties of a 3D axis system in the Points display mode in DIAdem REPORT.

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
oMy3DSurface = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DSurface")
oMySurfaceShape = oMy3DSurface.Shape
oMySurfaceShape.DataStructure = dd.e3DDataStructureMatrix
oMySurfaceShape.XChannel.Reference = "[2]/[1]"
oMySurfaceShape.YChannel.Reference = "[2]/[2]"
oMySurfaceShape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapePoints, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMyShape.Settings.Marker.Type = dd.eMarkerAsterisk
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 6
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjpointssettingsint-marker/">Marker</a> | <a href="../../properties/irepd3shapeobjpointssettingsint-palette/">Palette</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjpointsint/">3DPoints</a>.<a href="../../properties/irepd3shapeobjpointsint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjPointsSettingsInt.htm`*
