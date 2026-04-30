---
title: "IRepD3IsoValueTableListInt.Item"
description: "Returns the isoline associated with a specific index in the contour table for the 3D display mode Characteristic diagram in DIAdem REPORT."
---

# IRepD3IsoValueTableListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for 3DIsoValueTable

Returns the isoline associated with a specific index in the contour table for the 3D display mode Characteristic diagram in DIAdem REPORT.

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
iChannelMax = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("minimum").Value
oMyIsoValTable = oMyShape.Settings.IsoValueTable
oMyIsoValTable.Count = 5
oMy3DCurve.Shape.Extensions.Isoline.Type = dd.e3DCharacteristicIsoValueFromIsoValueTable
oMy3DCurve.Shape.Extensions.Isoline.Color.ColorIndex = dd.eColorIndexPalette
for i in range( 1, oMyIsoValTable.Count+1):
    oMyIsoValTable.Item(i).Color.SetPredefinedColor(i)
    oMyIsoValTable.Item(i).Interval = 20
    oMyIsoValTable.Item(i).LineType = dd.eLineTypeDotted
    oMyIsoValTable.Item(i).UpperLimit = iChannelMin + (iChannelMax - iChannelMin) / oMyIsoValTable.Count * i
    oMyIsoValTable.Item(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepD3IsoValueTableListInt.htm`*
