---
title: "IRepD3AdditionalIsolineListInt.Item"
description: "Returns the properties of the extended isolines in the display mode Characteristic diagram in a 3D axis system in DIAdem REPORT, which are associated with a spe"
---

# IRepD3AdditionalIsolineListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 3DAdditionalIsolines

Returns the properties of the extended isolines in the display mode Characteristic diagram in a 3D axis system in DIAdem REPORT, which are associated with a specific index. DIAdem only displays extended isolines in the xy-plane view.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

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

*Source: `ReportApi/methods/Report_method_Item_IRepD3AdditionalIsolineListInt.htm`*
