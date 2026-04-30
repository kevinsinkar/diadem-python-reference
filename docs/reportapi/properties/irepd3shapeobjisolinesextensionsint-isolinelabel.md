---
title: "IRepD3ShapeObjIsolinesExtensionsInt.IsolineLabel"
description: "Specifies the properties of the isoline labels in a 3D display in DIAdem REPORT."
---

# IRepD3ShapeObjIsolinesExtensionsInt.IsolineLabel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsolineLabel for 3DIsolinesExtensions

Specifies the properties of the isoline labels in a 3D display in DIAdem REPORT.

## Signature

```python
return_value = obj.IsolineLabel
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsolineLabel_IRepD3ShapeObjIsolinesExtensionsInt.htm`*
