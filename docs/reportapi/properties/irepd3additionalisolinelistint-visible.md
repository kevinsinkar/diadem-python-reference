---
title: "IRepD3AdditionalIsolineListInt.Visible"
description: "Specifies whether DIAdem REPORT plots extended isolines in the Characteristic diagram display mode in a 3D axis system. DIAdem only displays extended isolines i"
---

# IRepD3AdditionalIsolineListInt.Visible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Visible for 3DAdditionalIsolines

Specifies whether DIAdem REPORT plots extended isolines in the Characteristic diagram display mode in a 3D axis system. DIAdem only displays extended isolines in the xy-plane view.

## Signature

```python
obj.Visible
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Visible_IRepD3AdditionalIsolineListInt.htm`*
