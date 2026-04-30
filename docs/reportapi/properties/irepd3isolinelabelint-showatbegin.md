---
title: "IRepD3IsolineLabelInt.ShowAtBegin"
description: "Specifies whether DIAdem REPORT also displays the labels of additional isolines in 3D displays in the display type Characteristic Diagram or Surface at the curv"
---

# IRepD3IsolineLabelInt.ShowAtBegin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowAtBegin for 3DIsolineLabel

Specifies whether DIAdem REPORT also displays the labels of additional isolines in 3D displays in the display type Characteristic Diagram or Surface at the curve beginning.

## Signature

```python
obj.ShowAtBegin
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
oMyLabel.ShowAtEnd = True
oMyLabel.ShowAtBegin = True
oMyLabel.Font.Col()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowAtBegin_IRepD3IsolineLabelInt.htm`*
