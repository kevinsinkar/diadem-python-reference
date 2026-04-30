---
title: "IRepD3IsolineLabelInt.Format"
description: "Specifies the Format definition for the isoline labels in a 3D axis system in the display modes Characteristic diagram or Surface in DIAdem REPORT."
---

# IRepD3IsolineLabelInt.Format

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Format for 3DIsolineLabel

Specifies the Format definition for the isoline labels in a 3D axis system in the display modes Characteristic diagram or Surface in DIAdem REPORT.

## Signature

```python
obj.Format
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMy3DAxisSystem.Settings
oMySettings.RotationAngleXY = 90
oMySettings.RotationAngleZ = 270
oMyLabel = oMyShape.Extensions.Isoline.Label
oMyLabel.Visible = True
oMyLabel.UseCurveColor = False
oMyLabel.RepetitionMode = dd.e3DLabelRepetitionSurfaceLength
oMyLabel.RepetitionPercent = 10
oMyLabel.Format = "d.de"
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Format_IRepD3IsolineLabelInt.htm`*
