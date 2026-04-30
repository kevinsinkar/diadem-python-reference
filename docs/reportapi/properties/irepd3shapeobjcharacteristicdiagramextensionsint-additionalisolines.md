---
title: "IRepD3ShapeObjCharacteristicDiagramExtensionsInt.AdditionalIsolines"
description: "Returns a collection of all additional isolines in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT."
---

# IRepD3ShapeObjCharacteristicDiagramExtensionsInt.AdditionalIsolines

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AdditionalIsolines for 3DCharacteristicDiagramExtensions

Returns a collection of all additional isolines in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.AdditionalIsolines
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureMatrix
oMy3DAxisSystem.Settings.RotationAngleXY = 90
oMy3DAxisSystem.Settings.RotationAngleZ = 270
oMyAddIso = oMy3DCurve.Shape.Extensions.AdditionalIsolines
oMyAddIso.Visible = True
oMyAddIso.Count = 1
oMyAddIso.Item(1).Value = 0.6
oMyAddIsoLine = oMyAddIso.Item(1).Line
oMyAddIsoLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyAddIsoLine.LineType = dd.eLineTypeDashDot
oMyAddIsoLine.Width = dd.eLineWidth0050
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AdditionalIsolines_IRepD3ShapeObjCharacteristicDiagramExtensionsInt.htm`*
