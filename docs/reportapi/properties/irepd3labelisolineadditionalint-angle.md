---
title: "IRepD3LabelIsolineAdditionalInt.Angle"
description: "Specifies the text direction of the isoline labels in a 3D axis system in DIAdem REPORT."
---

# IRepD3LabelIsolineAdditionalInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for 3DAdditionalIsolineLabel

Specifies the text direction of the isoline labels in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.Angle
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you assign the value NoValue to the <span class="Monospace">Angle</span> property, DIAdem adapts the text angle automatically to the slope of the curve at the point to which the text is assigned.</td></tr></table>
</div>

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMyLabel = oMyShape.Extensions.IsolineLabel
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.d"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionLength
oMyLabel.Repetition.PercentValue = 30
oMyLabel.Angle = 45
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepD3LabelIsolineAdditionalInt.htm`*
