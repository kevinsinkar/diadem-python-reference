---
title: "IRepD3IsolineLabelInt.RepetitionValue"
description: "Specifies that DIAdem REPORT displays the labels for additional isolines in a 3D display in the display modes Characteristic diagram or Surface at every nth poi"
---

# IRepD3IsolineLabelInt.RepetitionValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RepetitionValue for 3DIsolineLabel

Specifies that DIAdem REPORT displays the labels for additional isolines in a 3D display in the display modes Characteristic diagram or Surface at every nth point if you assign the value e3DLabelRepetitionSurfaceNthPoint to the property RepetitionMode .

## Signature

```python
obj.RepetitionValue
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
oMyLabel.RepetitionMode = dd.e3DLabelRepetitionSurfaceNthPoint
oMyLabel.RepetitionValue = 10
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

*Source: `ReportApi/properties/Report_property_RepetitionValue_IRepD3IsolineLabelInt.htm`*
